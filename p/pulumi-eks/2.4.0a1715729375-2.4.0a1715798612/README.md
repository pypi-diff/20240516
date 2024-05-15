# Comparing `tmp/pulumi_eks-2.4.0a1715729375.tar.gz` & `tmp/pulumi_eks-2.4.0a1715798612.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_eks-2.4.0a1715729375.tar", last modified: Tue May 14 23:34:03 2024, max compression
+gzip compressed data, was "pulumi_eks-2.4.0a1715798612.tar", last modified: Wed May 15 18:48:46 2024, max compression
```

## Comparing `pulumi_eks-2.4.0a1715729375.tar` & `pulumi_eks-2.4.0a1715798612.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:34:02.997788 pulumi_eks-2.4.0a1715729375/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-14 23:34:02.997788 pulumi_eks-2.4.0a1715729375/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:34:02.997788 pulumi_eks-2.4.0a1715729375/pulumi_eks/
--rw-------   0 runner    (1001) docker     (127)     1150 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/__init__.py
--rw-------   0 runner    (1001) docker     (127)    88001 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     9222 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/_utilities.py
--rw-------   0 runner    (1001) docker     (127)    95529 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/cluster.py
--rw-------   0 runner    (1001) docker     (127)     4860 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/cluster_creation_role_provider.py
--rw-------   0 runner    (1001) docker     (127)    30218 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/managed_node_group.py
--rw-------   0 runner    (1001) docker     (127)    46243 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/node_group.py
--rw-------   0 runner    (1001) docker     (127)     8405 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/node_group_security_group.py
--rw-------   0 runner    (1001) docker     (127)    49155 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/node_group_v2.py
--rw-------   0 runner    (1001) docker     (127)    40852 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2715 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/provider.py
--rw-------   0 runner    (1001) docker     (127)       40 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/py.typed
--rw-------   0 runner    (1001) docker     (127)    39043 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/vpc_cni.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:34:02.997788 pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-14 23:34:02.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-14 23:34:02.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 23:34:02.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 23:34:02.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 23:34:02.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      720 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 23:34:02.997788 pulumi_eks-2.4.0a1715729375/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:48:46.622979 pulumi_eks-2.4.0a1715798612/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-15 18:48:46.622979 pulumi_eks-2.4.0a1715798612/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:48:46.618980 pulumi_eks-2.4.0a1715798612/pulumi_eks/
+-rw-------   0 runner    (1001) docker     (127)     1150 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/__init__.py
+-rw-------   0 runner    (1001) docker     (127)    89785 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     9222 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/_utilities.py
+-rw-------   0 runner    (1001) docker     (127)    95529 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/cluster.py
+-rw-------   0 runner    (1001) docker     (127)     4860 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/cluster_creation_role_provider.py
+-rw-------   0 runner    (1001) docker     (127)    30218 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/managed_node_group.py
+-rw-------   0 runner    (1001) docker     (127)    48913 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/node_group.py
+-rw-------   0 runner    (1001) docker     (127)     8405 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/node_group_security_group.py
+-rw-------   0 runner    (1001) docker     (127)    51825 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/node_group_v2.py
+-rw-------   0 runner    (1001) docker     (127)    42512 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2715 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/provider.py
+-rw-------   0 runner    (1001) docker     (127)       40 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/py.typed
+-rw-------   0 runner    (1001) docker     (127)    39043 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/vpc_cni.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:48:46.622979 pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-15 18:48:46.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-15 18:48:46.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:48:46.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 18:48:46.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 18:48:46.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      720 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 18:48:46.622979 pulumi_eks-2.4.0a1715798612/setup.cfg
```

### Comparing `pulumi_eks-2.4.0a1715729375/PKG-INFO` & `pulumi_eks-2.4.0a1715798612/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_eks
-Version: 2.4.0a1715729375
+Version: 2.4.0a1715798612
 Summary: Pulumi Amazon Web Services (AWS) EKS Components.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-eks
 Keywords: pulumi,aws,eks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_eks Version: 2.4.0a1715729375 Summary:
+Metadata-Version: 2.1 Name: pulumi_eks Version: 2.4.0a1715798612 Summary:
 Pulumi Amazon Web Services (AWS) EKS Components. License: Apache-2.0 Project-
 URL: Homepage, https://pulumi.com Project-URL: Repository, https://github.com/
 pulumi/pulumi-eks Keywords: pulumi,aws,eks Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Requires-Dist: parver>=0.2.1 Requires-Dist:
 pulumi<4.0.0,>=3.0.0 Requires-Dist: pulumi-aws<7.0.0,>=6.0.0 Requires-Dist:
 pulumi-kubernetes<5.0.0,>=4.0.0 Requires-Dist: semver>=2.8.1 [![Build Status]
 (https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml/badge.svg)]
```

### Comparing `pulumi_eks-2.4.0a1715729375/README.md` & `pulumi_eks-2.4.0a1715798612/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715729375/pulumi_eks/__init__.py` & `pulumi_eks-2.4.0a1715798612/pulumi_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715729375/pulumi_eks/_inputs.py` & `pulumi_eks-2.4.0a1715798612/pulumi_eks/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
                  ami_id: Optional[pulumi.Input[str]] = None,
                  ami_type: Optional[pulumi.Input[str]] = None,
                  auto_scaling_group_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  bootstrap_extra_args: Optional[str] = None,
                  cloud_formation_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  cluster_ingress_rule: Optional[pulumi.Input['pulumi_aws.ec2.SecurityGroupRule']] = None,
                  desired_capacity: Optional[pulumi.Input[int]] = None,
+                 enable_detailed_monitoring: Optional[pulumi.Input[bool]] = None,
                  encrypt_root_block_device: Optional[pulumi.Input[bool]] = None,
                  extra_node_security_groups: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroup']]]] = None,
                  gpu: Optional[pulumi.Input[bool]] = None,
                  instance_profile: Optional['pulumi_aws.iam.InstanceProfile'] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
                  key_name: Optional[pulumi.Input[str]] = None,
                  kubelet_extra_args: Optional[str] = None,
@@ -77,14 +78,21 @@
                Note: Given the inheritance of auto-generated CF tags and `cloudFormationTags`, you should either supply the tag in `autoScalingGroupTags` or `cloudFormationTags`, but not both.
         :param str bootstrap_extra_args: Additional args to pass directly to `/etc/eks/bootstrap.sh`. For details on available options, see: https://github.com/awslabs/amazon-eks-ami/blob/master/files/bootstrap.sh. Note that the `--apiserver-endpoint`, `--b64-cluster-ca` and `--kubelet-extra-args` flags are included automatically based on other configuration parameters.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] cloud_formation_tags: The tags to apply to the CloudFormation Stack of the Worker NodeGroup.
                
                Note: Given the inheritance of auto-generated CF tags and `cloudFormationTags`, you should either supply the tag in `autoScalingGroupTags` or `cloudFormationTags`, but not both.
         :param pulumi.Input['pulumi_aws.ec2.SecurityGroupRule'] cluster_ingress_rule: The ingress rule that gives node group access.
         :param pulumi.Input[int] desired_capacity: The number of worker nodes that should be running in the cluster. Defaults to 2.
+        :param pulumi.Input[bool] enable_detailed_monitoring: Enables/disables detailed monitoring of the EC2 instances.
+               
+               With detailed monitoring, all metrics, including status check metrics, are available in 1-minute intervals.
+               When enabled, you can also get aggregated data across groups of similar instances.
+               
+               Note: You are charged per metric that is sent to CloudWatch. You are not charged for data storage.
+               For more information, see "Paid tier" and "Example 1 - EC2 Detailed Monitoring" here https://aws.amazon.com/cloudwatch/pricing/.
         :param pulumi.Input[bool] encrypt_root_block_device: Encrypt the root block device of the nodes in the node group.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroup']]] extra_node_security_groups: Extra security groups to attach on all nodes in this worker node group.
                
                This additional set of security groups captures any user application rules that will be needed for the nodes.
         :param pulumi.Input[bool] gpu: Use the latest recommended EKS Optimized Linux AMI with GPU support for the worker nodes from the AWS Systems Manager Parameter Store.
                
                Defaults to false.
@@ -135,14 +143,16 @@
             pulumi.set(__self__, "bootstrap_extra_args", bootstrap_extra_args)
         if cloud_formation_tags is not None:
             pulumi.set(__self__, "cloud_formation_tags", cloud_formation_tags)
         if cluster_ingress_rule is not None:
             pulumi.set(__self__, "cluster_ingress_rule", cluster_ingress_rule)
         if desired_capacity is not None:
             pulumi.set(__self__, "desired_capacity", desired_capacity)
+        if enable_detailed_monitoring is not None:
+            pulumi.set(__self__, "enable_detailed_monitoring", enable_detailed_monitoring)
         if encrypt_root_block_device is not None:
             pulumi.set(__self__, "encrypt_root_block_device", encrypt_root_block_device)
         if extra_node_security_groups is not None:
             pulumi.set(__self__, "extra_node_security_groups", extra_node_security_groups)
         if gpu is not None:
             pulumi.set(__self__, "gpu", gpu)
         if instance_profile is not None:
@@ -278,14 +288,32 @@
         return pulumi.get(self, "desired_capacity")
 
     @desired_capacity.setter
     def desired_capacity(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "desired_capacity", value)
 
     @property
+    @pulumi.getter(name="enableDetailedMonitoring")
+    def enable_detailed_monitoring(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Enables/disables detailed monitoring of the EC2 instances.
+
+        With detailed monitoring, all metrics, including status check metrics, are available in 1-minute intervals.
+        When enabled, you can also get aggregated data across groups of similar instances.
+
+        Note: You are charged per metric that is sent to CloudWatch. You are not charged for data storage.
+        For more information, see "Paid tier" and "Example 1 - EC2 Detailed Monitoring" here https://aws.amazon.com/cloudwatch/pricing/.
+        """
+        return pulumi.get(self, "enable_detailed_monitoring")
+
+    @enable_detailed_monitoring.setter
+    def enable_detailed_monitoring(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enable_detailed_monitoring", value)
+
+    @property
     @pulumi.getter(name="encryptRootBlockDevice")
     def encrypt_root_block_device(self) -> Optional[pulumi.Input[bool]]:
         """
         Encrypt the root block device of the nodes in the node group.
         """
         return pulumi.get(self, "encrypt_root_block_device")
```

### Comparing `pulumi_eks-2.4.0a1715729375/pulumi_eks/_utilities.py` & `pulumi_eks-2.4.0a1715798612/pulumi_eks/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715729375/pulumi_eks/cluster.py` & `pulumi_eks-2.4.0a1715798612/pulumi_eks/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715729375/pulumi_eks/cluster_creation_role_provider.py` & `pulumi_eks-2.4.0a1715798612/pulumi_eks/cluster_creation_role_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715729375/pulumi_eks/managed_node_group.py` & `pulumi_eks-2.4.0a1715798612/pulumi_eks/managed_node_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715729375/pulumi_eks/node_group.py` & `pulumi_eks-2.4.0a1715798612/pulumi_eks/node_group_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,49 +10,52 @@
 from . import _utilities
 from ._inputs import *
 from .cluster import Cluster
 from .vpc_cni import VpcCni
 import pulumi_aws
 import pulumi_kubernetes
 
-__all__ = ['NodeGroupArgs', 'NodeGroup']
+__all__ = ['NodeGroupV2Args', 'NodeGroupV2']
 
 @pulumi.input_type
-class NodeGroupArgs:
+class NodeGroupV2Args:
     def __init__(__self__, *,
                  cluster: pulumi.Input[Union['Cluster', 'CoreDataArgs']],
                  ami_id: Optional[pulumi.Input[str]] = None,
                  ami_type: Optional[pulumi.Input[str]] = None,
                  auto_scaling_group_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  bootstrap_extra_args: Optional[str] = None,
                  cloud_formation_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  cluster_ingress_rule: Optional[pulumi.Input['pulumi_aws.ec2.SecurityGroupRule']] = None,
                  desired_capacity: Optional[pulumi.Input[int]] = None,
+                 enable_detailed_monitoring: Optional[pulumi.Input[bool]] = None,
                  encrypt_root_block_device: Optional[pulumi.Input[bool]] = None,
                  extra_node_security_groups: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroup']]]] = None,
                  gpu: Optional[pulumi.Input[bool]] = None,
                  instance_profile: Optional['pulumi_aws.iam.InstanceProfile'] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
                  key_name: Optional[pulumi.Input[str]] = None,
                  kubelet_extra_args: Optional[str] = None,
                  labels: Optional[Mapping[str, str]] = None,
+                 launch_template_tag_specifications: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.LaunchTemplateTagSpecificationArgs']]]] = None,
                  max_size: Optional[pulumi.Input[int]] = None,
+                 min_refresh_percentage: Optional[pulumi.Input[int]] = None,
                  min_size: Optional[pulumi.Input[int]] = None,
                  node_associate_public_ip_address: Optional[bool] = None,
                  node_public_key: Optional[pulumi.Input[str]] = None,
                  node_root_volume_size: Optional[pulumi.Input[int]] = None,
                  node_security_group: Optional[pulumi.Input['pulumi_aws.ec2.SecurityGroup']] = None,
                  node_subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  node_user_data: Optional[pulumi.Input[str]] = None,
                  node_user_data_override: Optional[pulumi.Input[str]] = None,
                  spot_price: Optional[pulumi.Input[str]] = None,
                  taints: Optional[Mapping[str, 'TaintArgs']] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a NodeGroup resource.
+        The set of arguments for constructing a NodeGroupV2 resource.
         :param pulumi.Input[Union['Cluster', 'CoreDataArgs']] cluster: The target EKS cluster.
         :param pulumi.Input[str] ami_id: The AMI ID to use for the worker nodes.
                
                Defaults to the latest recommended EKS Optimized Linux AMI from the AWS Systems Manager Parameter Store.
                
                Note: `amiId` and `gpu` are mutually exclusive.
                
@@ -70,14 +73,21 @@
                Note: Given the inheritance of auto-generated CF tags and `cloudFormationTags`, you should either supply the tag in `autoScalingGroupTags` or `cloudFormationTags`, but not both.
         :param str bootstrap_extra_args: Additional args to pass directly to `/etc/eks/bootstrap.sh`. For details on available options, see: https://github.com/awslabs/amazon-eks-ami/blob/master/files/bootstrap.sh. Note that the `--apiserver-endpoint`, `--b64-cluster-ca` and `--kubelet-extra-args` flags are included automatically based on other configuration parameters.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] cloud_formation_tags: The tags to apply to the CloudFormation Stack of the Worker NodeGroup.
                
                Note: Given the inheritance of auto-generated CF tags and `cloudFormationTags`, you should either supply the tag in `autoScalingGroupTags` or `cloudFormationTags`, but not both.
         :param pulumi.Input['pulumi_aws.ec2.SecurityGroupRule'] cluster_ingress_rule: The ingress rule that gives node group access.
         :param pulumi.Input[int] desired_capacity: The number of worker nodes that should be running in the cluster. Defaults to 2.
+        :param pulumi.Input[bool] enable_detailed_monitoring: Enables/disables detailed monitoring of the EC2 instances.
+               
+               With detailed monitoring, all metrics, including status check metrics, are available in 1-minute intervals.
+               When enabled, you can also get aggregated data across groups of similar instances.
+               
+               Note: You are charged per metric that is sent to CloudWatch. You are not charged for data storage.
+               For more information, see "Paid tier" and "Example 1 - EC2 Detailed Monitoring" here https://aws.amazon.com/cloudwatch/pricing/.
         :param pulumi.Input[bool] encrypt_root_block_device: Encrypt the root block device of the nodes in the node group.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroup']]] extra_node_security_groups: Extra security groups to attach on all nodes in this worker node group.
                
                This additional set of security groups captures any user application rules that will be needed for the nodes.
         :param pulumi.Input[bool] gpu: Use the latest recommended EKS Optimized Linux AMI with GPU support for the worker nodes from the AWS Systems Manager Parameter Store.
                
                Defaults to false.
@@ -88,15 +98,17 @@
                - https://docs.aws.amazon.com/eks/latest/userguide/eks-optimized-ami.html
                - https://docs.aws.amazon.com/eks/latest/userguide/retrieve-ami-id.html
         :param 'pulumi_aws.iam.InstanceProfile' instance_profile: The ingress rule that gives node group access.
         :param pulumi.Input[str] instance_type: The instance type to use for the cluster's nodes. Defaults to "t2.medium".
         :param pulumi.Input[str] key_name: Name of the key pair to use for SSH access to worker nodes.
         :param str kubelet_extra_args: Extra args to pass to the Kubelet. Corresponds to the options passed in the `--kubeletExtraArgs` flag to `/etc/eks/bootstrap.sh`. For example, '--port=10251 --address=0.0.0.0'. Note that the `labels` and `taints` properties will be applied to this list (using `--node-labels` and `--register-with-taints` respectively) after to the explicit `kubeletExtraArgs`.
         :param Mapping[str, str] labels: Custom k8s node labels to be attached to each worker node. Adds the given key/value pairs to the `--node-labels` kubelet argument.
+        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.LaunchTemplateTagSpecificationArgs']]] launch_template_tag_specifications: The tag specifications to apply to the launch template.
         :param pulumi.Input[int] max_size: The maximum number of worker nodes running in the cluster. Defaults to 2.
+        :param pulumi.Input[int] min_refresh_percentage: The minimum amount of instances that should remain available during an instance refresh, expressed as a percentage. Defaults to 50.
         :param pulumi.Input[int] min_size: The minimum number of worker nodes running in the cluster. Defaults to 1.
         :param bool node_associate_public_ip_address: Whether or not to auto-assign public IP addresses on the EKS worker nodes. If this toggle is set to true, the EKS workers will be auto-assigned public IPs. If false, they will not be auto-assigned public IPs.
         :param pulumi.Input[str] node_public_key: Public key material for SSH access to worker nodes. See allowed formats at:
                https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html
                If not provided, no SSH access is enabled on VMs.
         :param pulumi.Input[int] node_root_volume_size: The size in GiB of a cluster node's root volume. Defaults to 20.
         :param pulumi.Input['pulumi_aws.ec2.SecurityGroup'] node_security_group: The security group for the worker node group to communicate with the cluster.
@@ -129,14 +141,16 @@
             pulumi.set(__self__, "bootstrap_extra_args", bootstrap_extra_args)
         if cloud_formation_tags is not None:
             pulumi.set(__self__, "cloud_formation_tags", cloud_formation_tags)
         if cluster_ingress_rule is not None:
             pulumi.set(__self__, "cluster_ingress_rule", cluster_ingress_rule)
         if desired_capacity is not None:
             pulumi.set(__self__, "desired_capacity", desired_capacity)
+        if enable_detailed_monitoring is not None:
+            pulumi.set(__self__, "enable_detailed_monitoring", enable_detailed_monitoring)
         if encrypt_root_block_device is not None:
             pulumi.set(__self__, "encrypt_root_block_device", encrypt_root_block_device)
         if extra_node_security_groups is not None:
             pulumi.set(__self__, "extra_node_security_groups", extra_node_security_groups)
         if gpu is not None:
             pulumi.set(__self__, "gpu", gpu)
         if instance_profile is not None:
@@ -145,16 +159,20 @@
             pulumi.set(__self__, "instance_type", instance_type)
         if key_name is not None:
             pulumi.set(__self__, "key_name", key_name)
         if kubelet_extra_args is not None:
             pulumi.set(__self__, "kubelet_extra_args", kubelet_extra_args)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
+        if launch_template_tag_specifications is not None:
+            pulumi.set(__self__, "launch_template_tag_specifications", launch_template_tag_specifications)
         if max_size is not None:
             pulumi.set(__self__, "max_size", max_size)
+        if min_refresh_percentage is not None:
+            pulumi.set(__self__, "min_refresh_percentage", min_refresh_percentage)
         if min_size is not None:
             pulumi.set(__self__, "min_size", min_size)
         if node_associate_public_ip_address is not None:
             pulumi.set(__self__, "node_associate_public_ip_address", node_associate_public_ip_address)
         if node_public_key is not None:
             pulumi.set(__self__, "node_public_key", node_public_key)
         if node_root_volume_size is not None:
@@ -284,14 +302,32 @@
         return pulumi.get(self, "desired_capacity")
 
     @desired_capacity.setter
     def desired_capacity(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "desired_capacity", value)
 
     @property
+    @pulumi.getter(name="enableDetailedMonitoring")
+    def enable_detailed_monitoring(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Enables/disables detailed monitoring of the EC2 instances.
+
+        With detailed monitoring, all metrics, including status check metrics, are available in 1-minute intervals.
+        When enabled, you can also get aggregated data across groups of similar instances.
+
+        Note: You are charged per metric that is sent to CloudWatch. You are not charged for data storage.
+        For more information, see "Paid tier" and "Example 1 - EC2 Detailed Monitoring" here https://aws.amazon.com/cloudwatch/pricing/.
+        """
+        return pulumi.get(self, "enable_detailed_monitoring")
+
+    @enable_detailed_monitoring.setter
+    def enable_detailed_monitoring(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enable_detailed_monitoring", value)
+
+    @property
     @pulumi.getter(name="encryptRootBlockDevice")
     def encrypt_root_block_device(self) -> Optional[pulumi.Input[bool]]:
         """
         Encrypt the root block device of the nodes in the node group.
         """
         return pulumi.get(self, "encrypt_root_block_device")
 
@@ -390,26 +426,50 @@
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[Mapping[str, str]]):
         pulumi.set(self, "labels", value)
 
     @property
+    @pulumi.getter(name="launchTemplateTagSpecifications")
+    def launch_template_tag_specifications(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.LaunchTemplateTagSpecificationArgs']]]]:
+        """
+        The tag specifications to apply to the launch template.
+        """
+        return pulumi.get(self, "launch_template_tag_specifications")
+
+    @launch_template_tag_specifications.setter
+    def launch_template_tag_specifications(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.LaunchTemplateTagSpecificationArgs']]]]):
+        pulumi.set(self, "launch_template_tag_specifications", value)
+
+    @property
     @pulumi.getter(name="maxSize")
     def max_size(self) -> Optional[pulumi.Input[int]]:
         """
         The maximum number of worker nodes running in the cluster. Defaults to 2.
         """
         return pulumi.get(self, "max_size")
 
     @max_size.setter
     def max_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_size", value)
 
     @property
+    @pulumi.getter(name="minRefreshPercentage")
+    def min_refresh_percentage(self) -> Optional[pulumi.Input[int]]:
+        """
+        The minimum amount of instances that should remain available during an instance refresh, expressed as a percentage. Defaults to 50.
+        """
+        return pulumi.get(self, "min_refresh_percentage")
+
+    @min_refresh_percentage.setter
+    def min_refresh_percentage(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "min_refresh_percentage", value)
+
+    @property
     @pulumi.getter(name="minSize")
     def min_size(self) -> Optional[pulumi.Input[int]]:
         """
         The minimum number of worker nodes running in the cluster. Defaults to 1.
         """
         return pulumi.get(self, "min_size")
 
@@ -547,36 +607,39 @@
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
 
-class NodeGroup(pulumi.ComponentResource):
+class NodeGroupV2(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  ami_id: Optional[pulumi.Input[str]] = None,
                  ami_type: Optional[pulumi.Input[str]] = None,
                  auto_scaling_group_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  bootstrap_extra_args: Optional[str] = None,
                  cloud_formation_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  cluster: Optional[pulumi.Input[Union['Cluster', pulumi.InputType['CoreDataArgs']]]] = None,
                  cluster_ingress_rule: Optional[pulumi.Input['pulumi_aws.ec2.SecurityGroupRule']] = None,
                  desired_capacity: Optional[pulumi.Input[int]] = None,
+                 enable_detailed_monitoring: Optional[pulumi.Input[bool]] = None,
                  encrypt_root_block_device: Optional[pulumi.Input[bool]] = None,
                  extra_node_security_groups: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroup']]]] = None,
                  gpu: Optional[pulumi.Input[bool]] = None,
                  instance_profile: Optional['pulumi_aws.iam.InstanceProfile'] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
                  key_name: Optional[pulumi.Input[str]] = None,
                  kubelet_extra_args: Optional[str] = None,
                  labels: Optional[Mapping[str, str]] = None,
+                 launch_template_tag_specifications: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ec2.LaunchTemplateTagSpecificationArgs']]]]] = None,
                  max_size: Optional[pulumi.Input[int]] = None,
+                 min_refresh_percentage: Optional[pulumi.Input[int]] = None,
                  min_size: Optional[pulumi.Input[int]] = None,
                  node_associate_public_ip_address: Optional[bool] = None,
                  node_public_key: Optional[pulumi.Input[str]] = None,
                  node_root_volume_size: Optional[pulumi.Input[int]] = None,
                  node_security_group: Optional[pulumi.Input['pulumi_aws.ec2.SecurityGroup']] = None,
                  node_subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  node_user_data: Optional[pulumi.Input[str]] = None,
@@ -611,14 +674,21 @@
         :param str bootstrap_extra_args: Additional args to pass directly to `/etc/eks/bootstrap.sh`. For details on available options, see: https://github.com/awslabs/amazon-eks-ami/blob/master/files/bootstrap.sh. Note that the `--apiserver-endpoint`, `--b64-cluster-ca` and `--kubelet-extra-args` flags are included automatically based on other configuration parameters.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] cloud_formation_tags: The tags to apply to the CloudFormation Stack of the Worker NodeGroup.
                
                Note: Given the inheritance of auto-generated CF tags and `cloudFormationTags`, you should either supply the tag in `autoScalingGroupTags` or `cloudFormationTags`, but not both.
         :param pulumi.Input[Union['Cluster', pulumi.InputType['CoreDataArgs']]] cluster: The target EKS cluster.
         :param pulumi.Input['pulumi_aws.ec2.SecurityGroupRule'] cluster_ingress_rule: The ingress rule that gives node group access.
         :param pulumi.Input[int] desired_capacity: The number of worker nodes that should be running in the cluster. Defaults to 2.
+        :param pulumi.Input[bool] enable_detailed_monitoring: Enables/disables detailed monitoring of the EC2 instances.
+               
+               With detailed monitoring, all metrics, including status check metrics, are available in 1-minute intervals.
+               When enabled, you can also get aggregated data across groups of similar instances.
+               
+               Note: You are charged per metric that is sent to CloudWatch. You are not charged for data storage.
+               For more information, see "Paid tier" and "Example 1 - EC2 Detailed Monitoring" here https://aws.amazon.com/cloudwatch/pricing/.
         :param pulumi.Input[bool] encrypt_root_block_device: Encrypt the root block device of the nodes in the node group.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroup']]] extra_node_security_groups: Extra security groups to attach on all nodes in this worker node group.
                
                This additional set of security groups captures any user application rules that will be needed for the nodes.
         :param pulumi.Input[bool] gpu: Use the latest recommended EKS Optimized Linux AMI with GPU support for the worker nodes from the AWS Systems Manager Parameter Store.
                
                Defaults to false.
@@ -629,15 +699,17 @@
                - https://docs.aws.amazon.com/eks/latest/userguide/eks-optimized-ami.html
                - https://docs.aws.amazon.com/eks/latest/userguide/retrieve-ami-id.html
         :param 'pulumi_aws.iam.InstanceProfile' instance_profile: The ingress rule that gives node group access.
         :param pulumi.Input[str] instance_type: The instance type to use for the cluster's nodes. Defaults to "t2.medium".
         :param pulumi.Input[str] key_name: Name of the key pair to use for SSH access to worker nodes.
         :param str kubelet_extra_args: Extra args to pass to the Kubelet. Corresponds to the options passed in the `--kubeletExtraArgs` flag to `/etc/eks/bootstrap.sh`. For example, '--port=10251 --address=0.0.0.0'. Note that the `labels` and `taints` properties will be applied to this list (using `--node-labels` and `--register-with-taints` respectively) after to the explicit `kubeletExtraArgs`.
         :param Mapping[str, str] labels: Custom k8s node labels to be attached to each worker node. Adds the given key/value pairs to the `--node-labels` kubelet argument.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ec2.LaunchTemplateTagSpecificationArgs']]]] launch_template_tag_specifications: The tag specifications to apply to the launch template.
         :param pulumi.Input[int] max_size: The maximum number of worker nodes running in the cluster. Defaults to 2.
+        :param pulumi.Input[int] min_refresh_percentage: The minimum amount of instances that should remain available during an instance refresh, expressed as a percentage. Defaults to 50.
         :param pulumi.Input[int] min_size: The minimum number of worker nodes running in the cluster. Defaults to 1.
         :param bool node_associate_public_ip_address: Whether or not to auto-assign public IP addresses on the EKS worker nodes. If this toggle is set to true, the EKS workers will be auto-assigned public IPs. If false, they will not be auto-assigned public IPs.
         :param pulumi.Input[str] node_public_key: Public key material for SSH access to worker nodes. See allowed formats at:
                https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html
                If not provided, no SSH access is enabled on VMs.
         :param pulumi.Input[int] node_root_volume_size: The size in GiB of a cluster node's root volume. Defaults to 20.
         :param pulumi.Input['pulumi_aws.ec2.SecurityGroup'] node_security_group: The security group for the worker node group to communicate with the cluster.
@@ -659,26 +731,26 @@
         :param Mapping[str, pulumi.InputType['TaintArgs']] taints: Custom k8s node taints to be attached to each worker node. Adds the given taints to the `--register-with-taints` kubelet argument
         :param pulumi.Input[str] version: Desired Kubernetes master / control plane version. If you do not specify a value, the latest available version is used.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: NodeGroupArgs,
+                 args: NodeGroupV2Args,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         NodeGroup is a component that wraps the AWS EC2 instances that provide compute capacity for an EKS cluster.
 
         :param str resource_name: The name of the resource.
-        :param NodeGroupArgs args: The arguments to use to populate this resource's properties.
+        :param NodeGroupV2Args args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(NodeGroupArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(NodeGroupV2Args, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -687,23 +759,26 @@
                  ami_type: Optional[pulumi.Input[str]] = None,
                  auto_scaling_group_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  bootstrap_extra_args: Optional[str] = None,
                  cloud_formation_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  cluster: Optional[pulumi.Input[Union['Cluster', pulumi.InputType['CoreDataArgs']]]] = None,
                  cluster_ingress_rule: Optional[pulumi.Input['pulumi_aws.ec2.SecurityGroupRule']] = None,
                  desired_capacity: Optional[pulumi.Input[int]] = None,
+                 enable_detailed_monitoring: Optional[pulumi.Input[bool]] = None,
                  encrypt_root_block_device: Optional[pulumi.Input[bool]] = None,
                  extra_node_security_groups: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroup']]]] = None,
                  gpu: Optional[pulumi.Input[bool]] = None,
                  instance_profile: Optional['pulumi_aws.iam.InstanceProfile'] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
                  key_name: Optional[pulumi.Input[str]] = None,
                  kubelet_extra_args: Optional[str] = None,
                  labels: Optional[Mapping[str, str]] = None,
+                 launch_template_tag_specifications: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ec2.LaunchTemplateTagSpecificationArgs']]]]] = None,
                  max_size: Optional[pulumi.Input[int]] = None,
+                 min_refresh_percentage: Optional[pulumi.Input[int]] = None,
                  min_size: Optional[pulumi.Input[int]] = None,
                  node_associate_public_ip_address: Optional[bool] = None,
                  node_public_key: Optional[pulumi.Input[str]] = None,
                  node_root_volume_size: Optional[pulumi.Input[int]] = None,
                  node_security_group: Optional[pulumi.Input['pulumi_aws.ec2.SecurityGroup']] = None,
                  node_subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  node_user_data: Optional[pulumi.Input[str]] = None,
@@ -716,70 +791,64 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = NodeGroupArgs.__new__(NodeGroupArgs)
+            __props__ = NodeGroupV2Args.__new__(NodeGroupV2Args)
 
             __props__.__dict__["ami_id"] = ami_id
             __props__.__dict__["ami_type"] = ami_type
             __props__.__dict__["auto_scaling_group_tags"] = auto_scaling_group_tags
             __props__.__dict__["bootstrap_extra_args"] = bootstrap_extra_args
             __props__.__dict__["cloud_formation_tags"] = cloud_formation_tags
             if cluster is None and not opts.urn:
                 raise TypeError("Missing required property 'cluster'")
             __props__.__dict__["cluster"] = cluster
             __props__.__dict__["cluster_ingress_rule"] = cluster_ingress_rule
             __props__.__dict__["desired_capacity"] = desired_capacity
+            __props__.__dict__["enable_detailed_monitoring"] = enable_detailed_monitoring
             __props__.__dict__["encrypt_root_block_device"] = encrypt_root_block_device
             __props__.__dict__["extra_node_security_groups"] = extra_node_security_groups
             __props__.__dict__["gpu"] = gpu
             __props__.__dict__["instance_profile"] = instance_profile
             __props__.__dict__["instance_type"] = instance_type
             __props__.__dict__["key_name"] = key_name
             __props__.__dict__["kubelet_extra_args"] = kubelet_extra_args
             __props__.__dict__["labels"] = labels
+            __props__.__dict__["launch_template_tag_specifications"] = launch_template_tag_specifications
             __props__.__dict__["max_size"] = max_size
+            __props__.__dict__["min_refresh_percentage"] = min_refresh_percentage
             __props__.__dict__["min_size"] = min_size
             __props__.__dict__["node_associate_public_ip_address"] = node_associate_public_ip_address
             __props__.__dict__["node_public_key"] = node_public_key
             __props__.__dict__["node_root_volume_size"] = node_root_volume_size
             __props__.__dict__["node_security_group"] = node_security_group
             __props__.__dict__["node_subnet_ids"] = node_subnet_ids
             __props__.__dict__["node_user_data"] = node_user_data
             __props__.__dict__["node_user_data_override"] = node_user_data_override
             __props__.__dict__["spot_price"] = spot_price
             __props__.__dict__["taints"] = taints
             __props__.__dict__["version"] = version
-            __props__.__dict__["auto_scaling_group_name"] = None
-            __props__.__dict__["cfn_stack"] = None
-        super(NodeGroup, __self__).__init__(
-            'eks:index:NodeGroup',
+            __props__.__dict__["auto_scaling_group"] = None
+        super(NodeGroupV2, __self__).__init__(
+            'eks:index:NodeGroupV2',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
-    @pulumi.getter(name="autoScalingGroupName")
-    def auto_scaling_group_name(self) -> pulumi.Output[str]:
-        """
-        The AutoScalingGroup name for the Node group.
-        """
-        return pulumi.get(self, "auto_scaling_group_name")
-
-    @property
-    @pulumi.getter(name="cfnStack")
-    def cfn_stack(self) -> pulumi.Output['pulumi_aws.cloudformation.Stack']:
+    @pulumi.getter(name="autoScalingGroup")
+    def auto_scaling_group(self) -> pulumi.Output['pulumi_aws.autoscaling.Group']:
         """
-        The CloudFormation Stack which defines the Node AutoScalingGroup.
+        The AutoScalingGroup for the Node group.
         """
-        return pulumi.get(self, "cfn_stack")
+        return pulumi.get(self, "auto_scaling_group")
 
     @property
     @pulumi.getter(name="extraNodeSecurityGroups")
     def extra_node_security_groups(self) -> pulumi.Output[Sequence['pulumi_aws.ec2.SecurityGroup']]:
         """
         The additional security groups for the node group that captures user-specific rules.
         """
```

### Comparing `pulumi_eks-2.4.0a1715729375/pulumi_eks/node_group_security_group.py` & `pulumi_eks-2.4.0a1715798612/pulumi_eks/node_group_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715729375/pulumi_eks/node_group_v2.py` & `pulumi_eks-2.4.0a1715798612/pulumi_eks/node_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,51 +10,50 @@
 from . import _utilities
 from ._inputs import *
 from .cluster import Cluster
 from .vpc_cni import VpcCni
 import pulumi_aws
 import pulumi_kubernetes
 
-__all__ = ['NodeGroupV2Args', 'NodeGroupV2']
+__all__ = ['NodeGroupArgs', 'NodeGroup']
 
 @pulumi.input_type
-class NodeGroupV2Args:
+class NodeGroupArgs:
     def __init__(__self__, *,
                  cluster: pulumi.Input[Union['Cluster', 'CoreDataArgs']],
                  ami_id: Optional[pulumi.Input[str]] = None,
                  ami_type: Optional[pulumi.Input[str]] = None,
                  auto_scaling_group_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  bootstrap_extra_args: Optional[str] = None,
                  cloud_formation_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  cluster_ingress_rule: Optional[pulumi.Input['pulumi_aws.ec2.SecurityGroupRule']] = None,
                  desired_capacity: Optional[pulumi.Input[int]] = None,
+                 enable_detailed_monitoring: Optional[pulumi.Input[bool]] = None,
                  encrypt_root_block_device: Optional[pulumi.Input[bool]] = None,
                  extra_node_security_groups: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroup']]]] = None,
                  gpu: Optional[pulumi.Input[bool]] = None,
                  instance_profile: Optional['pulumi_aws.iam.InstanceProfile'] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
                  key_name: Optional[pulumi.Input[str]] = None,
                  kubelet_extra_args: Optional[str] = None,
                  labels: Optional[Mapping[str, str]] = None,
-                 launch_template_tag_specifications: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.LaunchTemplateTagSpecificationArgs']]]] = None,
                  max_size: Optional[pulumi.Input[int]] = None,
-                 min_refresh_percentage: Optional[pulumi.Input[int]] = None,
                  min_size: Optional[pulumi.Input[int]] = None,
                  node_associate_public_ip_address: Optional[bool] = None,
                  node_public_key: Optional[pulumi.Input[str]] = None,
                  node_root_volume_size: Optional[pulumi.Input[int]] = None,
                  node_security_group: Optional[pulumi.Input['pulumi_aws.ec2.SecurityGroup']] = None,
                  node_subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  node_user_data: Optional[pulumi.Input[str]] = None,
                  node_user_data_override: Optional[pulumi.Input[str]] = None,
                  spot_price: Optional[pulumi.Input[str]] = None,
                  taints: Optional[Mapping[str, 'TaintArgs']] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a NodeGroupV2 resource.
+        The set of arguments for constructing a NodeGroup resource.
         :param pulumi.Input[Union['Cluster', 'CoreDataArgs']] cluster: The target EKS cluster.
         :param pulumi.Input[str] ami_id: The AMI ID to use for the worker nodes.
                
                Defaults to the latest recommended EKS Optimized Linux AMI from the AWS Systems Manager Parameter Store.
                
                Note: `amiId` and `gpu` are mutually exclusive.
                
@@ -72,14 +71,21 @@
                Note: Given the inheritance of auto-generated CF tags and `cloudFormationTags`, you should either supply the tag in `autoScalingGroupTags` or `cloudFormationTags`, but not both.
         :param str bootstrap_extra_args: Additional args to pass directly to `/etc/eks/bootstrap.sh`. For details on available options, see: https://github.com/awslabs/amazon-eks-ami/blob/master/files/bootstrap.sh. Note that the `--apiserver-endpoint`, `--b64-cluster-ca` and `--kubelet-extra-args` flags are included automatically based on other configuration parameters.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] cloud_formation_tags: The tags to apply to the CloudFormation Stack of the Worker NodeGroup.
                
                Note: Given the inheritance of auto-generated CF tags and `cloudFormationTags`, you should either supply the tag in `autoScalingGroupTags` or `cloudFormationTags`, but not both.
         :param pulumi.Input['pulumi_aws.ec2.SecurityGroupRule'] cluster_ingress_rule: The ingress rule that gives node group access.
         :param pulumi.Input[int] desired_capacity: The number of worker nodes that should be running in the cluster. Defaults to 2.
+        :param pulumi.Input[bool] enable_detailed_monitoring: Enables/disables detailed monitoring of the EC2 instances.
+               
+               With detailed monitoring, all metrics, including status check metrics, are available in 1-minute intervals.
+               When enabled, you can also get aggregated data across groups of similar instances.
+               
+               Note: You are charged per metric that is sent to CloudWatch. You are not charged for data storage.
+               For more information, see "Paid tier" and "Example 1 - EC2 Detailed Monitoring" here https://aws.amazon.com/cloudwatch/pricing/.
         :param pulumi.Input[bool] encrypt_root_block_device: Encrypt the root block device of the nodes in the node group.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroup']]] extra_node_security_groups: Extra security groups to attach on all nodes in this worker node group.
                
                This additional set of security groups captures any user application rules that will be needed for the nodes.
         :param pulumi.Input[bool] gpu: Use the latest recommended EKS Optimized Linux AMI with GPU support for the worker nodes from the AWS Systems Manager Parameter Store.
                
                Defaults to false.
@@ -90,17 +96,15 @@
                - https://docs.aws.amazon.com/eks/latest/userguide/eks-optimized-ami.html
                - https://docs.aws.amazon.com/eks/latest/userguide/retrieve-ami-id.html
         :param 'pulumi_aws.iam.InstanceProfile' instance_profile: The ingress rule that gives node group access.
         :param pulumi.Input[str] instance_type: The instance type to use for the cluster's nodes. Defaults to "t2.medium".
         :param pulumi.Input[str] key_name: Name of the key pair to use for SSH access to worker nodes.
         :param str kubelet_extra_args: Extra args to pass to the Kubelet. Corresponds to the options passed in the `--kubeletExtraArgs` flag to `/etc/eks/bootstrap.sh`. For example, '--port=10251 --address=0.0.0.0'. Note that the `labels` and `taints` properties will be applied to this list (using `--node-labels` and `--register-with-taints` respectively) after to the explicit `kubeletExtraArgs`.
         :param Mapping[str, str] labels: Custom k8s node labels to be attached to each worker node. Adds the given key/value pairs to the `--node-labels` kubelet argument.
-        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.LaunchTemplateTagSpecificationArgs']]] launch_template_tag_specifications: The tag specifications to apply to the launch template.
         :param pulumi.Input[int] max_size: The maximum number of worker nodes running in the cluster. Defaults to 2.
-        :param pulumi.Input[int] min_refresh_percentage: The minimum amount of instances that should remain available during an instance refresh, expressed as a percentage. Defaults to 50.
         :param pulumi.Input[int] min_size: The minimum number of worker nodes running in the cluster. Defaults to 1.
         :param bool node_associate_public_ip_address: Whether or not to auto-assign public IP addresses on the EKS worker nodes. If this toggle is set to true, the EKS workers will be auto-assigned public IPs. If false, they will not be auto-assigned public IPs.
         :param pulumi.Input[str] node_public_key: Public key material for SSH access to worker nodes. See allowed formats at:
                https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html
                If not provided, no SSH access is enabled on VMs.
         :param pulumi.Input[int] node_root_volume_size: The size in GiB of a cluster node's root volume. Defaults to 20.
         :param pulumi.Input['pulumi_aws.ec2.SecurityGroup'] node_security_group: The security group for the worker node group to communicate with the cluster.
@@ -133,14 +137,16 @@
             pulumi.set(__self__, "bootstrap_extra_args", bootstrap_extra_args)
         if cloud_formation_tags is not None:
             pulumi.set(__self__, "cloud_formation_tags", cloud_formation_tags)
         if cluster_ingress_rule is not None:
             pulumi.set(__self__, "cluster_ingress_rule", cluster_ingress_rule)
         if desired_capacity is not None:
             pulumi.set(__self__, "desired_capacity", desired_capacity)
+        if enable_detailed_monitoring is not None:
+            pulumi.set(__self__, "enable_detailed_monitoring", enable_detailed_monitoring)
         if encrypt_root_block_device is not None:
             pulumi.set(__self__, "encrypt_root_block_device", encrypt_root_block_device)
         if extra_node_security_groups is not None:
             pulumi.set(__self__, "extra_node_security_groups", extra_node_security_groups)
         if gpu is not None:
             pulumi.set(__self__, "gpu", gpu)
         if instance_profile is not None:
@@ -149,20 +155,16 @@
             pulumi.set(__self__, "instance_type", instance_type)
         if key_name is not None:
             pulumi.set(__self__, "key_name", key_name)
         if kubelet_extra_args is not None:
             pulumi.set(__self__, "kubelet_extra_args", kubelet_extra_args)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
-        if launch_template_tag_specifications is not None:
-            pulumi.set(__self__, "launch_template_tag_specifications", launch_template_tag_specifications)
         if max_size is not None:
             pulumi.set(__self__, "max_size", max_size)
-        if min_refresh_percentage is not None:
-            pulumi.set(__self__, "min_refresh_percentage", min_refresh_percentage)
         if min_size is not None:
             pulumi.set(__self__, "min_size", min_size)
         if node_associate_public_ip_address is not None:
             pulumi.set(__self__, "node_associate_public_ip_address", node_associate_public_ip_address)
         if node_public_key is not None:
             pulumi.set(__self__, "node_public_key", node_public_key)
         if node_root_volume_size is not None:
@@ -292,14 +294,32 @@
         return pulumi.get(self, "desired_capacity")
 
     @desired_capacity.setter
     def desired_capacity(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "desired_capacity", value)
 
     @property
+    @pulumi.getter(name="enableDetailedMonitoring")
+    def enable_detailed_monitoring(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Enables/disables detailed monitoring of the EC2 instances.
+
+        With detailed monitoring, all metrics, including status check metrics, are available in 1-minute intervals.
+        When enabled, you can also get aggregated data across groups of similar instances.
+
+        Note: You are charged per metric that is sent to CloudWatch. You are not charged for data storage.
+        For more information, see "Paid tier" and "Example 1 - EC2 Detailed Monitoring" here https://aws.amazon.com/cloudwatch/pricing/.
+        """
+        return pulumi.get(self, "enable_detailed_monitoring")
+
+    @enable_detailed_monitoring.setter
+    def enable_detailed_monitoring(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enable_detailed_monitoring", value)
+
+    @property
     @pulumi.getter(name="encryptRootBlockDevice")
     def encrypt_root_block_device(self) -> Optional[pulumi.Input[bool]]:
         """
         Encrypt the root block device of the nodes in the node group.
         """
         return pulumi.get(self, "encrypt_root_block_device")
 
@@ -398,50 +418,26 @@
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[Mapping[str, str]]):
         pulumi.set(self, "labels", value)
 
     @property
-    @pulumi.getter(name="launchTemplateTagSpecifications")
-    def launch_template_tag_specifications(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.LaunchTemplateTagSpecificationArgs']]]]:
-        """
-        The tag specifications to apply to the launch template.
-        """
-        return pulumi.get(self, "launch_template_tag_specifications")
-
-    @launch_template_tag_specifications.setter
-    def launch_template_tag_specifications(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.LaunchTemplateTagSpecificationArgs']]]]):
-        pulumi.set(self, "launch_template_tag_specifications", value)
-
-    @property
     @pulumi.getter(name="maxSize")
     def max_size(self) -> Optional[pulumi.Input[int]]:
         """
         The maximum number of worker nodes running in the cluster. Defaults to 2.
         """
         return pulumi.get(self, "max_size")
 
     @max_size.setter
     def max_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_size", value)
 
     @property
-    @pulumi.getter(name="minRefreshPercentage")
-    def min_refresh_percentage(self) -> Optional[pulumi.Input[int]]:
-        """
-        The minimum amount of instances that should remain available during an instance refresh, expressed as a percentage. Defaults to 50.
-        """
-        return pulumi.get(self, "min_refresh_percentage")
-
-    @min_refresh_percentage.setter
-    def min_refresh_percentage(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "min_refresh_percentage", value)
-
-    @property
     @pulumi.getter(name="minSize")
     def min_size(self) -> Optional[pulumi.Input[int]]:
         """
         The minimum number of worker nodes running in the cluster. Defaults to 1.
         """
         return pulumi.get(self, "min_size")
 
@@ -579,38 +575,37 @@
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
 
-class NodeGroupV2(pulumi.ComponentResource):
+class NodeGroup(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  ami_id: Optional[pulumi.Input[str]] = None,
                  ami_type: Optional[pulumi.Input[str]] = None,
                  auto_scaling_group_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  bootstrap_extra_args: Optional[str] = None,
                  cloud_formation_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  cluster: Optional[pulumi.Input[Union['Cluster', pulumi.InputType['CoreDataArgs']]]] = None,
                  cluster_ingress_rule: Optional[pulumi.Input['pulumi_aws.ec2.SecurityGroupRule']] = None,
                  desired_capacity: Optional[pulumi.Input[int]] = None,
+                 enable_detailed_monitoring: Optional[pulumi.Input[bool]] = None,
                  encrypt_root_block_device: Optional[pulumi.Input[bool]] = None,
                  extra_node_security_groups: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroup']]]] = None,
                  gpu: Optional[pulumi.Input[bool]] = None,
                  instance_profile: Optional['pulumi_aws.iam.InstanceProfile'] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
                  key_name: Optional[pulumi.Input[str]] = None,
                  kubelet_extra_args: Optional[str] = None,
                  labels: Optional[Mapping[str, str]] = None,
-                 launch_template_tag_specifications: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ec2.LaunchTemplateTagSpecificationArgs']]]]] = None,
                  max_size: Optional[pulumi.Input[int]] = None,
-                 min_refresh_percentage: Optional[pulumi.Input[int]] = None,
                  min_size: Optional[pulumi.Input[int]] = None,
                  node_associate_public_ip_address: Optional[bool] = None,
                  node_public_key: Optional[pulumi.Input[str]] = None,
                  node_root_volume_size: Optional[pulumi.Input[int]] = None,
                  node_security_group: Optional[pulumi.Input['pulumi_aws.ec2.SecurityGroup']] = None,
                  node_subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  node_user_data: Optional[pulumi.Input[str]] = None,
@@ -645,14 +640,21 @@
         :param str bootstrap_extra_args: Additional args to pass directly to `/etc/eks/bootstrap.sh`. For details on available options, see: https://github.com/awslabs/amazon-eks-ami/blob/master/files/bootstrap.sh. Note that the `--apiserver-endpoint`, `--b64-cluster-ca` and `--kubelet-extra-args` flags are included automatically based on other configuration parameters.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] cloud_formation_tags: The tags to apply to the CloudFormation Stack of the Worker NodeGroup.
                
                Note: Given the inheritance of auto-generated CF tags and `cloudFormationTags`, you should either supply the tag in `autoScalingGroupTags` or `cloudFormationTags`, but not both.
         :param pulumi.Input[Union['Cluster', pulumi.InputType['CoreDataArgs']]] cluster: The target EKS cluster.
         :param pulumi.Input['pulumi_aws.ec2.SecurityGroupRule'] cluster_ingress_rule: The ingress rule that gives node group access.
         :param pulumi.Input[int] desired_capacity: The number of worker nodes that should be running in the cluster. Defaults to 2.
+        :param pulumi.Input[bool] enable_detailed_monitoring: Enables/disables detailed monitoring of the EC2 instances.
+               
+               With detailed monitoring, all metrics, including status check metrics, are available in 1-minute intervals.
+               When enabled, you can also get aggregated data across groups of similar instances.
+               
+               Note: You are charged per metric that is sent to CloudWatch. You are not charged for data storage.
+               For more information, see "Paid tier" and "Example 1 - EC2 Detailed Monitoring" here https://aws.amazon.com/cloudwatch/pricing/.
         :param pulumi.Input[bool] encrypt_root_block_device: Encrypt the root block device of the nodes in the node group.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroup']]] extra_node_security_groups: Extra security groups to attach on all nodes in this worker node group.
                
                This additional set of security groups captures any user application rules that will be needed for the nodes.
         :param pulumi.Input[bool] gpu: Use the latest recommended EKS Optimized Linux AMI with GPU support for the worker nodes from the AWS Systems Manager Parameter Store.
                
                Defaults to false.
@@ -663,17 +665,15 @@
                - https://docs.aws.amazon.com/eks/latest/userguide/eks-optimized-ami.html
                - https://docs.aws.amazon.com/eks/latest/userguide/retrieve-ami-id.html
         :param 'pulumi_aws.iam.InstanceProfile' instance_profile: The ingress rule that gives node group access.
         :param pulumi.Input[str] instance_type: The instance type to use for the cluster's nodes. Defaults to "t2.medium".
         :param pulumi.Input[str] key_name: Name of the key pair to use for SSH access to worker nodes.
         :param str kubelet_extra_args: Extra args to pass to the Kubelet. Corresponds to the options passed in the `--kubeletExtraArgs` flag to `/etc/eks/bootstrap.sh`. For example, '--port=10251 --address=0.0.0.0'. Note that the `labels` and `taints` properties will be applied to this list (using `--node-labels` and `--register-with-taints` respectively) after to the explicit `kubeletExtraArgs`.
         :param Mapping[str, str] labels: Custom k8s node labels to be attached to each worker node. Adds the given key/value pairs to the `--node-labels` kubelet argument.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ec2.LaunchTemplateTagSpecificationArgs']]]] launch_template_tag_specifications: The tag specifications to apply to the launch template.
         :param pulumi.Input[int] max_size: The maximum number of worker nodes running in the cluster. Defaults to 2.
-        :param pulumi.Input[int] min_refresh_percentage: The minimum amount of instances that should remain available during an instance refresh, expressed as a percentage. Defaults to 50.
         :param pulumi.Input[int] min_size: The minimum number of worker nodes running in the cluster. Defaults to 1.
         :param bool node_associate_public_ip_address: Whether or not to auto-assign public IP addresses on the EKS worker nodes. If this toggle is set to true, the EKS workers will be auto-assigned public IPs. If false, they will not be auto-assigned public IPs.
         :param pulumi.Input[str] node_public_key: Public key material for SSH access to worker nodes. See allowed formats at:
                https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html
                If not provided, no SSH access is enabled on VMs.
         :param pulumi.Input[int] node_root_volume_size: The size in GiB of a cluster node's root volume. Defaults to 20.
         :param pulumi.Input['pulumi_aws.ec2.SecurityGroup'] node_security_group: The security group for the worker node group to communicate with the cluster.
@@ -695,26 +695,26 @@
         :param Mapping[str, pulumi.InputType['TaintArgs']] taints: Custom k8s node taints to be attached to each worker node. Adds the given taints to the `--register-with-taints` kubelet argument
         :param pulumi.Input[str] version: Desired Kubernetes master / control plane version. If you do not specify a value, the latest available version is used.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: NodeGroupV2Args,
+                 args: NodeGroupArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         NodeGroup is a component that wraps the AWS EC2 instances that provide compute capacity for an EKS cluster.
 
         :param str resource_name: The name of the resource.
-        :param NodeGroupV2Args args: The arguments to use to populate this resource's properties.
+        :param NodeGroupArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(NodeGroupV2Args, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(NodeGroupArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -723,25 +723,24 @@
                  ami_type: Optional[pulumi.Input[str]] = None,
                  auto_scaling_group_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  bootstrap_extra_args: Optional[str] = None,
                  cloud_formation_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  cluster: Optional[pulumi.Input[Union['Cluster', pulumi.InputType['CoreDataArgs']]]] = None,
                  cluster_ingress_rule: Optional[pulumi.Input['pulumi_aws.ec2.SecurityGroupRule']] = None,
                  desired_capacity: Optional[pulumi.Input[int]] = None,
+                 enable_detailed_monitoring: Optional[pulumi.Input[bool]] = None,
                  encrypt_root_block_device: Optional[pulumi.Input[bool]] = None,
                  extra_node_security_groups: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroup']]]] = None,
                  gpu: Optional[pulumi.Input[bool]] = None,
                  instance_profile: Optional['pulumi_aws.iam.InstanceProfile'] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
                  key_name: Optional[pulumi.Input[str]] = None,
                  kubelet_extra_args: Optional[str] = None,
                  labels: Optional[Mapping[str, str]] = None,
-                 launch_template_tag_specifications: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ec2.LaunchTemplateTagSpecificationArgs']]]]] = None,
                  max_size: Optional[pulumi.Input[int]] = None,
-                 min_refresh_percentage: Optional[pulumi.Input[int]] = None,
                  min_size: Optional[pulumi.Input[int]] = None,
                  node_associate_public_ip_address: Optional[bool] = None,
                  node_public_key: Optional[pulumi.Input[str]] = None,
                  node_root_volume_size: Optional[pulumi.Input[int]] = None,
                  node_security_group: Optional[pulumi.Input['pulumi_aws.ec2.SecurityGroup']] = None,
                  node_subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  node_user_data: Optional[pulumi.Input[str]] = None,
@@ -754,63 +753,71 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = NodeGroupV2Args.__new__(NodeGroupV2Args)
+            __props__ = NodeGroupArgs.__new__(NodeGroupArgs)
 
             __props__.__dict__["ami_id"] = ami_id
             __props__.__dict__["ami_type"] = ami_type
             __props__.__dict__["auto_scaling_group_tags"] = auto_scaling_group_tags
             __props__.__dict__["bootstrap_extra_args"] = bootstrap_extra_args
             __props__.__dict__["cloud_formation_tags"] = cloud_formation_tags
             if cluster is None and not opts.urn:
                 raise TypeError("Missing required property 'cluster'")
             __props__.__dict__["cluster"] = cluster
             __props__.__dict__["cluster_ingress_rule"] = cluster_ingress_rule
             __props__.__dict__["desired_capacity"] = desired_capacity
+            __props__.__dict__["enable_detailed_monitoring"] = enable_detailed_monitoring
             __props__.__dict__["encrypt_root_block_device"] = encrypt_root_block_device
             __props__.__dict__["extra_node_security_groups"] = extra_node_security_groups
             __props__.__dict__["gpu"] = gpu
             __props__.__dict__["instance_profile"] = instance_profile
             __props__.__dict__["instance_type"] = instance_type
             __props__.__dict__["key_name"] = key_name
             __props__.__dict__["kubelet_extra_args"] = kubelet_extra_args
             __props__.__dict__["labels"] = labels
-            __props__.__dict__["launch_template_tag_specifications"] = launch_template_tag_specifications
             __props__.__dict__["max_size"] = max_size
-            __props__.__dict__["min_refresh_percentage"] = min_refresh_percentage
             __props__.__dict__["min_size"] = min_size
             __props__.__dict__["node_associate_public_ip_address"] = node_associate_public_ip_address
             __props__.__dict__["node_public_key"] = node_public_key
             __props__.__dict__["node_root_volume_size"] = node_root_volume_size
             __props__.__dict__["node_security_group"] = node_security_group
             __props__.__dict__["node_subnet_ids"] = node_subnet_ids
             __props__.__dict__["node_user_data"] = node_user_data
             __props__.__dict__["node_user_data_override"] = node_user_data_override
             __props__.__dict__["spot_price"] = spot_price
             __props__.__dict__["taints"] = taints
             __props__.__dict__["version"] = version
-            __props__.__dict__["auto_scaling_group"] = None
-        super(NodeGroupV2, __self__).__init__(
-            'eks:index:NodeGroupV2',
+            __props__.__dict__["auto_scaling_group_name"] = None
+            __props__.__dict__["cfn_stack"] = None
+        super(NodeGroup, __self__).__init__(
+            'eks:index:NodeGroup',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
-    @pulumi.getter(name="autoScalingGroup")
-    def auto_scaling_group(self) -> pulumi.Output['pulumi_aws.autoscaling.Group']:
+    @pulumi.getter(name="autoScalingGroupName")
+    def auto_scaling_group_name(self) -> pulumi.Output[str]:
+        """
+        The AutoScalingGroup name for the Node group.
+        """
+        return pulumi.get(self, "auto_scaling_group_name")
+
+    @property
+    @pulumi.getter(name="cfnStack")
+    def cfn_stack(self) -> pulumi.Output['pulumi_aws.cloudformation.Stack']:
         """
-        The AutoScalingGroup for the Node group.
+        The CloudFormation Stack which defines the Node AutoScalingGroup.
         """
-        return pulumi.get(self, "auto_scaling_group")
+        return pulumi.get(self, "cfn_stack")
 
     @property
     @pulumi.getter(name="extraNodeSecurityGroups")
     def extra_node_security_groups(self) -> pulumi.Output[Sequence['pulumi_aws.ec2.SecurityGroup']]:
         """
         The additional security groups for the node group that captures user-specific rules.
         """
```

### Comparing `pulumi_eks-2.4.0a1715729375/pulumi_eks/outputs.py` & `pulumi_eks-2.4.0a1715798612/pulumi_eks/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,16 @@
             suggest = "bootstrap_extra_args"
         elif key == "cloudFormationTags":
             suggest = "cloud_formation_tags"
         elif key == "clusterIngressRule":
             suggest = "cluster_ingress_rule"
         elif key == "desiredCapacity":
             suggest = "desired_capacity"
+        elif key == "enableDetailedMonitoring":
+            suggest = "enable_detailed_monitoring"
         elif key == "encryptRootBlockDevice":
             suggest = "encrypt_root_block_device"
         elif key == "extraNodeSecurityGroups":
             suggest = "extra_node_security_groups"
         elif key == "instanceProfile":
             suggest = "instance_profile"
         elif key == "instanceType":
@@ -90,14 +92,15 @@
                  ami_id: Optional[str] = None,
                  ami_type: Optional[str] = None,
                  auto_scaling_group_tags: Optional[Mapping[str, str]] = None,
                  bootstrap_extra_args: Optional[str] = None,
                  cloud_formation_tags: Optional[Mapping[str, str]] = None,
                  cluster_ingress_rule: Optional['pulumi_aws.ec2.SecurityGroupRule'] = None,
                  desired_capacity: Optional[int] = None,
+                 enable_detailed_monitoring: Optional[bool] = None,
                  encrypt_root_block_device: Optional[bool] = None,
                  extra_node_security_groups: Optional[Sequence['pulumi_aws.ec2.SecurityGroup']] = None,
                  gpu: Optional[bool] = None,
                  instance_profile: Optional['pulumi_aws.iam.InstanceProfile'] = None,
                  instance_type: Optional[str] = None,
                  key_name: Optional[str] = None,
                  kubelet_extra_args: Optional[str] = None,
@@ -136,14 +139,21 @@
                Note: Given the inheritance of auto-generated CF tags and `cloudFormationTags`, you should either supply the tag in `autoScalingGroupTags` or `cloudFormationTags`, but not both.
         :param str bootstrap_extra_args: Additional args to pass directly to `/etc/eks/bootstrap.sh`. For details on available options, see: https://github.com/awslabs/amazon-eks-ami/blob/master/files/bootstrap.sh. Note that the `--apiserver-endpoint`, `--b64-cluster-ca` and `--kubelet-extra-args` flags are included automatically based on other configuration parameters.
         :param Mapping[str, str] cloud_formation_tags: The tags to apply to the CloudFormation Stack of the Worker NodeGroup.
                
                Note: Given the inheritance of auto-generated CF tags and `cloudFormationTags`, you should either supply the tag in `autoScalingGroupTags` or `cloudFormationTags`, but not both.
         :param 'pulumi_aws.ec2.SecurityGroupRule' cluster_ingress_rule: The ingress rule that gives node group access.
         :param int desired_capacity: The number of worker nodes that should be running in the cluster. Defaults to 2.
+        :param bool enable_detailed_monitoring: Enables/disables detailed monitoring of the EC2 instances.
+               
+               With detailed monitoring, all metrics, including status check metrics, are available in 1-minute intervals.
+               When enabled, you can also get aggregated data across groups of similar instances.
+               
+               Note: You are charged per metric that is sent to CloudWatch. You are not charged for data storage.
+               For more information, see "Paid tier" and "Example 1 - EC2 Detailed Monitoring" here https://aws.amazon.com/cloudwatch/pricing/.
         :param bool encrypt_root_block_device: Encrypt the root block device of the nodes in the node group.
         :param Sequence['pulumi_aws.ec2.SecurityGroup'] extra_node_security_groups: Extra security groups to attach on all nodes in this worker node group.
                
                This additional set of security groups captures any user application rules that will be needed for the nodes.
         :param bool gpu: Use the latest recommended EKS Optimized Linux AMI with GPU support for the worker nodes from the AWS Systems Manager Parameter Store.
                
                Defaults to false.
@@ -194,14 +204,16 @@
             pulumi.set(__self__, "bootstrap_extra_args", bootstrap_extra_args)
         if cloud_formation_tags is not None:
             pulumi.set(__self__, "cloud_formation_tags", cloud_formation_tags)
         if cluster_ingress_rule is not None:
             pulumi.set(__self__, "cluster_ingress_rule", cluster_ingress_rule)
         if desired_capacity is not None:
             pulumi.set(__self__, "desired_capacity", desired_capacity)
+        if enable_detailed_monitoring is not None:
+            pulumi.set(__self__, "enable_detailed_monitoring", enable_detailed_monitoring)
         if encrypt_root_block_device is not None:
             pulumi.set(__self__, "encrypt_root_block_device", encrypt_root_block_device)
         if extra_node_security_groups is not None:
             pulumi.set(__self__, "extra_node_security_groups", extra_node_security_groups)
         if gpu is not None:
             pulumi.set(__self__, "gpu", gpu)
         if instance_profile is not None:
@@ -309,14 +321,28 @@
     def desired_capacity(self) -> Optional[int]:
         """
         The number of worker nodes that should be running in the cluster. Defaults to 2.
         """
         return pulumi.get(self, "desired_capacity")
 
     @property
+    @pulumi.getter(name="enableDetailedMonitoring")
+    def enable_detailed_monitoring(self) -> Optional[bool]:
+        """
+        Enables/disables detailed monitoring of the EC2 instances.
+
+        With detailed monitoring, all metrics, including status check metrics, are available in 1-minute intervals.
+        When enabled, you can also get aggregated data across groups of similar instances.
+
+        Note: You are charged per metric that is sent to CloudWatch. You are not charged for data storage.
+        For more information, see "Paid tier" and "Example 1 - EC2 Detailed Monitoring" here https://aws.amazon.com/cloudwatch/pricing/.
+        """
+        return pulumi.get(self, "enable_detailed_monitoring")
+
+    @property
     @pulumi.getter(name="encryptRootBlockDevice")
     def encrypt_root_block_device(self) -> Optional[bool]:
         """
         Encrypt the root block device of the nodes in the node group.
         """
         return pulumi.get(self, "encrypt_root_block_device")
```

### Comparing `pulumi_eks-2.4.0a1715729375/pulumi_eks/provider.py` & `pulumi_eks-2.4.0a1715798612/pulumi_eks/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715729375/pulumi_eks/vpc_cni.py` & `pulumi_eks-2.4.0a1715798612/pulumi_eks/vpc_cni.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/PKG-INFO` & `pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_eks
-Version: 2.4.0a1715729375
+Version: 2.4.0a1715798612
 Summary: Pulumi Amazon Web Services (AWS) EKS Components.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-eks
 Keywords: pulumi,aws,eks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_eks Version: 2.4.0a1715729375 Summary:
+Metadata-Version: 2.1 Name: pulumi_eks Version: 2.4.0a1715798612 Summary:
 Pulumi Amazon Web Services (AWS) EKS Components. License: Apache-2.0 Project-
 URL: Homepage, https://pulumi.com Project-URL: Repository, https://github.com/
 pulumi/pulumi-eks Keywords: pulumi,aws,eks Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Requires-Dist: parver>=0.2.1 Requires-Dist:
 pulumi<4.0.0,>=3.0.0 Requires-Dist: pulumi-aws<7.0.0,>=6.0.0 Requires-Dist:
 pulumi-kubernetes<5.0.0,>=4.0.0 Requires-Dist: semver>=2.8.1 [![Build Status]
 (https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml/badge.svg)]
```

### Comparing `pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/SOURCES.txt` & `pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715729375/pyproject.toml` & `pulumi_eks-2.4.0a1715798612/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_eks"
   description = "Pulumi Amazon Web Services (AWS) EKS Components."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "pulumi-aws>=6.0.0,<7.0.0", "pulumi-kubernetes>=4.0.0,<5.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "aws", "eks"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "2.4.0a1715729375"
+  version = "2.4.0a1715798612"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-eks"
 
 [build-system]
```

