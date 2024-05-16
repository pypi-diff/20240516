# Comparing `tmp/alibabacloud_alikafka20190916-2.6.6.tar.gz` & `tmp/alibabacloud_alikafka20190916-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alikafka20190916-2.6.6.tar", last modified: Tue Apr 23 17:13:02 2024, max compression
+gzip compressed data, was "dist/alibabacloud_alikafka20190916-2.7.0.tar", last modified: Thu May 16 17:19:44 2024, max compression
```

## Comparing `alibabacloud_alikafka20190916-2.6.6.tar` & `alibabacloud_alikafka20190916-2.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/
--rw-r--r--   0 root         (0) root         (0)     6781 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2440 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916/__init__.py
--rw-r--r--   0 root         (0) root         (0)   184296 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916/client.py
--rw-r--r--   0 root         (0) root         (0)   401503 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2440 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2640 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/
+-rw-r--r--   0 root         (0) root         (0)     7147 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/alibabacloud_alikafka20190916/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/alibabacloud_alikafka20190916/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   243066 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/alibabacloud_alikafka20190916/client.py
+-rw-r--r--   0 root         (0) root         (0)   453450 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/alibabacloud_alikafka20190916/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/alibabacloud_alikafka20190916.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/alibabacloud_alikafka20190916.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/alibabacloud_alikafka20190916.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/alibabacloud_alikafka20190916.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/alibabacloud_alikafka20190916.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/alibabacloud_alikafka20190916.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2640 2024-05-16 17:19:44.000000 alibabacloud_alikafka20190916-2.7.0/setup.py
```

### Comparing `alibabacloud_alikafka20190916-2.6.6/ChangeLog.md` & `alibabacloud_alikafka20190916-2.7.0/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+2024-04-23 Version: 2.6.6
+- Update API CreatePostPayOrder: update param DiskSize.
+- Update API CreatePostPayOrder: update param DiskType.
+- Update API CreatePrePayOrder: update param ConfluentConfig.
+- Update API GetInstanceList: add param Series.
+- Update API GetInstanceList: update response param.
+- Update API UpgradePrePayOrder: update param ConfluentConfig.
+
+
 2024-04-11 Version: 2.6.5
 - Update API CreatePostPayOrder: add param PaidType.
 - Update API CreatePostPayOrder: add param ServerlessConfig.
 - Update API CreatePostPayOrder: update param DiskSize.
 - Update API CreatePostPayOrder: update param DiskType.
 - Update API GetInstanceList: update response param.
```

### Comparing `alibabacloud_alikafka20190916-2.6.6/LICENSE` & `alibabacloud_alikafka20190916-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916-2.6.6/PKG-INFO` & `alibabacloud_alikafka20190916-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alikafka20190916
-Version: 2.6.6
+Version: 2.7.0
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916-2.6.6/README-CN.md` & `alibabacloud_alikafka20190916-2.7.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916-2.6.6/README.md` & `alibabacloud_alikafka20190916-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916/client.py` & `alibabacloud_alikafka20190916-2.7.0/alibabacloud_alikafka20190916/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,14 +42,21 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def change_resource_group_with_options(
         self,
         request: alikafka_20190916_models.ChangeResourceGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ChangeResourceGroupResponse:
+        """
+        @summary Changes the resource group of an ApsaraMQ for Kafka instance.
+        
+        @param request: ChangeResourceGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ChangeResourceGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.new_resource_group_id):
             query['NewResourceGroupId'] = request.new_resource_group_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_id):
@@ -74,14 +81,21 @@
         )
 
     async def change_resource_group_with_options_async(
         self,
         request: alikafka_20190916_models.ChangeResourceGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ChangeResourceGroupResponse:
+        """
+        @summary Changes the resource group of an ApsaraMQ for Kafka instance.
+        
+        @param request: ChangeResourceGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ChangeResourceGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.new_resource_group_id):
             query['NewResourceGroupId'] = request.new_resource_group_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_id):
@@ -105,29 +119,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def change_resource_group(
         self,
         request: alikafka_20190916_models.ChangeResourceGroupRequest,
     ) -> alikafka_20190916_models.ChangeResourceGroupResponse:
+        """
+        @summary Changes the resource group of an ApsaraMQ for Kafka instance.
+        
+        @param request: ChangeResourceGroupRequest
+        @return: ChangeResourceGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.change_resource_group_with_options(request, runtime)
 
     async def change_resource_group_async(
         self,
         request: alikafka_20190916_models.ChangeResourceGroupRequest,
     ) -> alikafka_20190916_models.ChangeResourceGroupResponse:
+        """
+        @summary Changes the resource group of an ApsaraMQ for Kafka instance.
+        
+        @param request: ChangeResourceGroupRequest
+        @return: ChangeResourceGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.change_resource_group_with_options_async(request, runtime)
 
     def convert_post_pay_order_with_options(
         self,
         request: alikafka_20190916_models.ConvertPostPayOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ConvertPostPayOrderResponse:
+        """
+        @summary Changes the billing method of a Message Queue for Apache Kafka instance from pay-as-you-go to subscription.
+        
+        @param request: ConvertPostPayOrderRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConvertPostPayOrderResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.duration):
             query['Duration'] = request.duration
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -152,14 +185,21 @@
         )
 
     async def convert_post_pay_order_with_options_async(
         self,
         request: alikafka_20190916_models.ConvertPostPayOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ConvertPostPayOrderResponse:
+        """
+        @summary Changes the billing method of a Message Queue for Apache Kafka instance from pay-as-you-go to subscription.
+        
+        @param request: ConvertPostPayOrderRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConvertPostPayOrderResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.duration):
             query['Duration'] = request.duration
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -183,29 +223,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def convert_post_pay_order(
         self,
         request: alikafka_20190916_models.ConvertPostPayOrderRequest,
     ) -> alikafka_20190916_models.ConvertPostPayOrderResponse:
+        """
+        @summary Changes the billing method of a Message Queue for Apache Kafka instance from pay-as-you-go to subscription.
+        
+        @param request: ConvertPostPayOrderRequest
+        @return: ConvertPostPayOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.convert_post_pay_order_with_options(request, runtime)
 
     async def convert_post_pay_order_async(
         self,
         request: alikafka_20190916_models.ConvertPostPayOrderRequest,
     ) -> alikafka_20190916_models.ConvertPostPayOrderResponse:
+        """
+        @summary Changes the billing method of a Message Queue for Apache Kafka instance from pay-as-you-go to subscription.
+        
+        @param request: ConvertPostPayOrderRequest
+        @return: ConvertPostPayOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.convert_post_pay_order_with_options_async(request, runtime)
 
     def create_acl_with_options(
         self,
         request: alikafka_20190916_models.CreateAclRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreateAclResponse:
+        """
+        @summary Creates an access control list (ACL).
+        
+        @param request: CreateAclRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAclResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_operation_type):
             query['AclOperationType'] = request.acl_operation_type
         if not UtilClient.is_unset(request.acl_operation_types):
             query['AclOperationTypes'] = request.acl_operation_types
         if not UtilClient.is_unset(request.acl_permission_type):
@@ -244,14 +303,21 @@
         )
 
     async def create_acl_with_options_async(
         self,
         request: alikafka_20190916_models.CreateAclRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreateAclResponse:
+        """
+        @summary Creates an access control list (ACL).
+        
+        @param request: CreateAclRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAclResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_operation_type):
             query['AclOperationType'] = request.acl_operation_type
         if not UtilClient.is_unset(request.acl_operation_types):
             query['AclOperationTypes'] = request.acl_operation_types
         if not UtilClient.is_unset(request.acl_permission_type):
@@ -289,29 +355,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_acl(
         self,
         request: alikafka_20190916_models.CreateAclRequest,
     ) -> alikafka_20190916_models.CreateAclResponse:
+        """
+        @summary Creates an access control list (ACL).
+        
+        @param request: CreateAclRequest
+        @return: CreateAclResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_acl_with_options(request, runtime)
 
     async def create_acl_async(
         self,
         request: alikafka_20190916_models.CreateAclRequest,
     ) -> alikafka_20190916_models.CreateAclResponse:
+        """
+        @summary Creates an access control list (ACL).
+        
+        @param request: CreateAclRequest
+        @return: CreateAclResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_acl_with_options_async(request, runtime)
 
     def create_consumer_group_with_options(
         self,
         request: alikafka_20190916_models.CreateConsumerGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreateConsumerGroupResponse:
+        """
+        @summary Creates a consumer group.
+        
+        @param request: CreateConsumerGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateConsumerGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.consumer_id):
             query['ConsumerId'] = request.consumer_id
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -340,14 +425,21 @@
         )
 
     async def create_consumer_group_with_options_async(
         self,
         request: alikafka_20190916_models.CreateConsumerGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreateConsumerGroupResponse:
+        """
+        @summary Creates a consumer group.
+        
+        @param request: CreateConsumerGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateConsumerGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.consumer_id):
             query['ConsumerId'] = request.consumer_id
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -375,31 +467,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_consumer_group(
         self,
         request: alikafka_20190916_models.CreateConsumerGroupRequest,
     ) -> alikafka_20190916_models.CreateConsumerGroupResponse:
+        """
+        @summary Creates a consumer group.
+        
+        @param request: CreateConsumerGroupRequest
+        @return: CreateConsumerGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_consumer_group_with_options(request, runtime)
 
     async def create_consumer_group_async(
         self,
         request: alikafka_20190916_models.CreateConsumerGroupRequest,
     ) -> alikafka_20190916_models.CreateConsumerGroupResponse:
+        """
+        @summary Creates a consumer group.
+        
+        @param request: CreateConsumerGroupRequest
+        @return: CreateConsumerGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_consumer_group_with_options_async(request, runtime)
 
     def create_post_pay_order_with_options(
         self,
         tmp_req: alikafka_20190916_models.CreatePostPayOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreatePostPayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](~~84737~~).
+        @summary Creates a pay-as-you-go ApsaraMQ for Kafka instance. Pay-as-you-go instances allow you to pay after you use the resources. You are charged for pay-as-you-go instances based on the actual resource usage. You can use pay-as-you-go instances in test scenarios or scenarios in which the peak traffic is uncertain.
+        
+        @description Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         
         @param tmp_req: CreatePostPayOrderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreatePostPayOrderResponse
         """
         UtilClient.validate_model(tmp_req)
         request = alikafka_20190916_models.CreatePostPayOrderShrinkRequest()
@@ -456,15 +562,17 @@
 
     async def create_post_pay_order_with_options_async(
         self,
         tmp_req: alikafka_20190916_models.CreatePostPayOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreatePostPayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](~~84737~~).
+        @summary Creates a pay-as-you-go ApsaraMQ for Kafka instance. Pay-as-you-go instances allow you to pay after you use the resources. You are charged for pay-as-you-go instances based on the actual resource usage. You can use pay-as-you-go instances in test scenarios or scenarios in which the peak traffic is uncertain.
+        
+        @description Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         
         @param tmp_req: CreatePostPayOrderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreatePostPayOrderResponse
         """
         UtilClient.validate_model(tmp_req)
         request = alikafka_20190916_models.CreatePostPayOrderShrinkRequest()
@@ -520,43 +628,49 @@
         )
 
     def create_post_pay_order(
         self,
         request: alikafka_20190916_models.CreatePostPayOrderRequest,
     ) -> alikafka_20190916_models.CreatePostPayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](~~84737~~).
+        @summary Creates a pay-as-you-go ApsaraMQ for Kafka instance. Pay-as-you-go instances allow you to pay after you use the resources. You are charged for pay-as-you-go instances based on the actual resource usage. You can use pay-as-you-go instances in test scenarios or scenarios in which the peak traffic is uncertain.
+        
+        @description Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         
         @param request: CreatePostPayOrderRequest
         @return: CreatePostPayOrderResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_post_pay_order_with_options(request, runtime)
 
     async def create_post_pay_order_async(
         self,
         request: alikafka_20190916_models.CreatePostPayOrderRequest,
     ) -> alikafka_20190916_models.CreatePostPayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](~~84737~~).
+        @summary Creates a pay-as-you-go ApsaraMQ for Kafka instance. Pay-as-you-go instances allow you to pay after you use the resources. You are charged for pay-as-you-go instances based on the actual resource usage. You can use pay-as-you-go instances in test scenarios or scenarios in which the peak traffic is uncertain.
+        
+        @description Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         
         @param request: CreatePostPayOrderRequest
         @return: CreatePostPayOrderResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_post_pay_order_with_options_async(request, runtime)
 
     def create_pre_pay_order_with_options(
         self,
         tmp_req: alikafka_20190916_models.CreatePrePayOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreatePrePayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing methods and pricing of subscription ApsaraMQ for Kafka instances. For more information, see [Billing](~~84737~~).
-        *   If you create an ApsaraMQ for Kafka instance by calling this operation, the subscription duration is one month and the auto-renewal feature is enabled by default. The auto-renewal cycle is also one month. If you want to change the auto-renewal cycle or disable the auto-renewal feature, you can go to the [Renewal](https://renew.console.aliyun.com/#/ecs) page in the Alibaba Cloud Management Console.
+        @summary Creates a subscription ApsaraMQ for Kafka instance. You can use subscription instances only after you pay for them. Subscription instances are suitable for long-term and stable business scenarios.
+        
+        @description    Before you call this operation, make sure that you understand the billing methods and pricing of subscription ApsaraMQ for Kafka instances. For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
+        If you create an ApsaraMQ for Kafka instance by calling this operation, the subscription duration is one month and the auto-renewal feature is enabled by default. The auto-renewal cycle is also one month. If you want to change the auto-renewal cycle or disable the auto-renewal feature, you can go to the [Renewal](https://renew.console.aliyun.com/#/ecs) page in the Alibaba Cloud Management Console.
         
         @param tmp_req: CreatePrePayOrderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreatePrePayOrderResponse
         """
         UtilClient.validate_model(tmp_req)
         request = alikafka_20190916_models.CreatePrePayOrderShrinkRequest()
@@ -615,16 +729,18 @@
 
     async def create_pre_pay_order_with_options_async(
         self,
         tmp_req: alikafka_20190916_models.CreatePrePayOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreatePrePayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing methods and pricing of subscription ApsaraMQ for Kafka instances. For more information, see [Billing](~~84737~~).
-        *   If you create an ApsaraMQ for Kafka instance by calling this operation, the subscription duration is one month and the auto-renewal feature is enabled by default. The auto-renewal cycle is also one month. If you want to change the auto-renewal cycle or disable the auto-renewal feature, you can go to the [Renewal](https://renew.console.aliyun.com/#/ecs) page in the Alibaba Cloud Management Console.
+        @summary Creates a subscription ApsaraMQ for Kafka instance. You can use subscription instances only after you pay for them. Subscription instances are suitable for long-term and stable business scenarios.
+        
+        @description    Before you call this operation, make sure that you understand the billing methods and pricing of subscription ApsaraMQ for Kafka instances. For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
+        If you create an ApsaraMQ for Kafka instance by calling this operation, the subscription duration is one month and the auto-renewal feature is enabled by default. The auto-renewal cycle is also one month. If you want to change the auto-renewal cycle or disable the auto-renewal feature, you can go to the [Renewal](https://renew.console.aliyun.com/#/ecs) page in the Alibaba Cloud Management Console.
         
         @param tmp_req: CreatePrePayOrderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreatePrePayOrderResponse
         """
         UtilClient.validate_model(tmp_req)
         request = alikafka_20190916_models.CreatePrePayOrderShrinkRequest()
@@ -682,42 +798,53 @@
         )
 
     def create_pre_pay_order(
         self,
         request: alikafka_20190916_models.CreatePrePayOrderRequest,
     ) -> alikafka_20190916_models.CreatePrePayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing methods and pricing of subscription ApsaraMQ for Kafka instances. For more information, see [Billing](~~84737~~).
-        *   If you create an ApsaraMQ for Kafka instance by calling this operation, the subscription duration is one month and the auto-renewal feature is enabled by default. The auto-renewal cycle is also one month. If you want to change the auto-renewal cycle or disable the auto-renewal feature, you can go to the [Renewal](https://renew.console.aliyun.com/#/ecs) page in the Alibaba Cloud Management Console.
+        @summary Creates a subscription ApsaraMQ for Kafka instance. You can use subscription instances only after you pay for them. Subscription instances are suitable for long-term and stable business scenarios.
+        
+        @description    Before you call this operation, make sure that you understand the billing methods and pricing of subscription ApsaraMQ for Kafka instances. For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
+        If you create an ApsaraMQ for Kafka instance by calling this operation, the subscription duration is one month and the auto-renewal feature is enabled by default. The auto-renewal cycle is also one month. If you want to change the auto-renewal cycle or disable the auto-renewal feature, you can go to the [Renewal](https://renew.console.aliyun.com/#/ecs) page in the Alibaba Cloud Management Console.
         
         @param request: CreatePrePayOrderRequest
         @return: CreatePrePayOrderResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_pre_pay_order_with_options(request, runtime)
 
     async def create_pre_pay_order_async(
         self,
         request: alikafka_20190916_models.CreatePrePayOrderRequest,
     ) -> alikafka_20190916_models.CreatePrePayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing methods and pricing of subscription ApsaraMQ for Kafka instances. For more information, see [Billing](~~84737~~).
-        *   If you create an ApsaraMQ for Kafka instance by calling this operation, the subscription duration is one month and the auto-renewal feature is enabled by default. The auto-renewal cycle is also one month. If you want to change the auto-renewal cycle or disable the auto-renewal feature, you can go to the [Renewal](https://renew.console.aliyun.com/#/ecs) page in the Alibaba Cloud Management Console.
+        @summary Creates a subscription ApsaraMQ for Kafka instance. You can use subscription instances only after you pay for them. Subscription instances are suitable for long-term and stable business scenarios.
+        
+        @description    Before you call this operation, make sure that you understand the billing methods and pricing of subscription ApsaraMQ for Kafka instances. For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
+        If you create an ApsaraMQ for Kafka instance by calling this operation, the subscription duration is one month and the auto-renewal feature is enabled by default. The auto-renewal cycle is also one month. If you want to change the auto-renewal cycle or disable the auto-renewal feature, you can go to the [Renewal](https://renew.console.aliyun.com/#/ecs) page in the Alibaba Cloud Management Console.
         
         @param request: CreatePrePayOrderRequest
         @return: CreatePrePayOrderResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_pre_pay_order_with_options_async(request, runtime)
 
     def create_sasl_user_with_options(
         self,
         request: alikafka_20190916_models.CreateSaslUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreateSaslUserResponse:
+        """
+        @summary Creates a Simple Authentication and Security Layer (SASL) user.
+        
+        @param request: CreateSaslUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateSaslUserResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.mechanism):
             query['Mechanism'] = request.mechanism
         if not UtilClient.is_unset(request.password):
@@ -748,14 +875,21 @@
         )
 
     async def create_sasl_user_with_options_async(
         self,
         request: alikafka_20190916_models.CreateSaslUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreateSaslUserResponse:
+        """
+        @summary Creates a Simple Authentication and Security Layer (SASL) user.
+        
+        @param request: CreateSaslUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateSaslUserResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.mechanism):
             query['Mechanism'] = request.mechanism
         if not UtilClient.is_unset(request.password):
@@ -785,32 +919,194 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_sasl_user(
         self,
         request: alikafka_20190916_models.CreateSaslUserRequest,
     ) -> alikafka_20190916_models.CreateSaslUserResponse:
+        """
+        @summary Creates a Simple Authentication and Security Layer (SASL) user.
+        
+        @param request: CreateSaslUserRequest
+        @return: CreateSaslUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_sasl_user_with_options(request, runtime)
 
     async def create_sasl_user_async(
         self,
         request: alikafka_20190916_models.CreateSaslUserRequest,
     ) -> alikafka_20190916_models.CreateSaslUserResponse:
+        """
+        @summary Creates a Simple Authentication and Security Layer (SASL) user.
+        
+        @param request: CreateSaslUserRequest
+        @return: CreateSaslUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_sasl_user_with_options_async(request, runtime)
 
+    def create_scheduled_scaling_rule_with_options(
+        self,
+        tmp_req: alikafka_20190916_models.CreateScheduledScalingRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> alikafka_20190916_models.CreateScheduledScalingRuleResponse:
+        """
+        @summary 创建定时伸缩配置
+        
+        @param tmp_req: CreateScheduledScalingRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateScheduledScalingRuleResponse
+        """
+        UtilClient.validate_model(tmp_req)
+        request = alikafka_20190916_models.CreateScheduledScalingRuleShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.weekly_types):
+            request.weekly_types_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.weekly_types, 'WeeklyTypes', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.duration_minutes):
+            query['DurationMinutes'] = request.duration_minutes
+        if not UtilClient.is_unset(request.enable):
+            query['Enable'] = request.enable
+        if not UtilClient.is_unset(request.first_scheduled_time):
+            query['FirstScheduledTime'] = request.first_scheduled_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.repeat_type):
+            query['RepeatType'] = request.repeat_type
+        if not UtilClient.is_unset(request.reserved_pub_flow):
+            query['ReservedPubFlow'] = request.reserved_pub_flow
+        if not UtilClient.is_unset(request.reserved_sub_flow):
+            query['ReservedSubFlow'] = request.reserved_sub_flow
+        if not UtilClient.is_unset(request.rule_name):
+            query['RuleName'] = request.rule_name
+        if not UtilClient.is_unset(request.schedule_type):
+            query['ScheduleType'] = request.schedule_type
+        if not UtilClient.is_unset(request.time_zone):
+            query['TimeZone'] = request.time_zone
+        if not UtilClient.is_unset(request.weekly_types_shrink):
+            query['WeeklyTypes'] = request.weekly_types_shrink
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateScheduledScalingRule',
+            version='2019-09-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            alikafka_20190916_models.CreateScheduledScalingRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_scheduled_scaling_rule_with_options_async(
+        self,
+        tmp_req: alikafka_20190916_models.CreateScheduledScalingRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> alikafka_20190916_models.CreateScheduledScalingRuleResponse:
+        """
+        @summary 创建定时伸缩配置
+        
+        @param tmp_req: CreateScheduledScalingRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateScheduledScalingRuleResponse
+        """
+        UtilClient.validate_model(tmp_req)
+        request = alikafka_20190916_models.CreateScheduledScalingRuleShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.weekly_types):
+            request.weekly_types_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.weekly_types, 'WeeklyTypes', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.duration_minutes):
+            query['DurationMinutes'] = request.duration_minutes
+        if not UtilClient.is_unset(request.enable):
+            query['Enable'] = request.enable
+        if not UtilClient.is_unset(request.first_scheduled_time):
+            query['FirstScheduledTime'] = request.first_scheduled_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.repeat_type):
+            query['RepeatType'] = request.repeat_type
+        if not UtilClient.is_unset(request.reserved_pub_flow):
+            query['ReservedPubFlow'] = request.reserved_pub_flow
+        if not UtilClient.is_unset(request.reserved_sub_flow):
+            query['ReservedSubFlow'] = request.reserved_sub_flow
+        if not UtilClient.is_unset(request.rule_name):
+            query['RuleName'] = request.rule_name
+        if not UtilClient.is_unset(request.schedule_type):
+            query['ScheduleType'] = request.schedule_type
+        if not UtilClient.is_unset(request.time_zone):
+            query['TimeZone'] = request.time_zone
+        if not UtilClient.is_unset(request.weekly_types_shrink):
+            query['WeeklyTypes'] = request.weekly_types_shrink
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateScheduledScalingRule',
+            version='2019-09-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            alikafka_20190916_models.CreateScheduledScalingRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_scheduled_scaling_rule(
+        self,
+        request: alikafka_20190916_models.CreateScheduledScalingRuleRequest,
+    ) -> alikafka_20190916_models.CreateScheduledScalingRuleResponse:
+        """
+        @summary 创建定时伸缩配置
+        
+        @param request: CreateScheduledScalingRuleRequest
+        @return: CreateScheduledScalingRuleResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.create_scheduled_scaling_rule_with_options(request, runtime)
+
+    async def create_scheduled_scaling_rule_async(
+        self,
+        request: alikafka_20190916_models.CreateScheduledScalingRuleRequest,
+    ) -> alikafka_20190916_models.CreateScheduledScalingRuleResponse:
+        """
+        @summary 创建定时伸缩配置
+        
+        @param request: CreateScheduledScalingRuleRequest
+        @return: CreateScheduledScalingRuleResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.create_scheduled_scaling_rule_with_options_async(request, runtime)
+
     def create_topic_with_options(
         self,
         request: alikafka_20190916_models.CreateTopicRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreateTopicResponse:
         """
-        Each Alibaba Cloud account can call this operation up to once per second.
-        *   The maximum number of topics that you can create in an instance is determined by the specification of the instance.
+        @summary Creates a topic.
+        
+        @description    Each Alibaba Cloud account can call this operation up to once per second.
+        The maximum number of topics that you can create in an instance is determined by the specification of the instance.
         
         @param request: CreateTopicRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateTopicResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -857,16 +1153,18 @@
 
     async def create_topic_with_options_async(
         self,
         request: alikafka_20190916_models.CreateTopicRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreateTopicResponse:
         """
-        Each Alibaba Cloud account can call this operation up to once per second.
-        *   The maximum number of topics that you can create in an instance is determined by the specification of the instance.
+        @summary Creates a topic.
+        
+        @description    Each Alibaba Cloud account can call this operation up to once per second.
+        The maximum number of topics that you can create in an instance is determined by the specification of the instance.
         
         @param request: CreateTopicRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateTopicResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -912,42 +1210,53 @@
         )
 
     def create_topic(
         self,
         request: alikafka_20190916_models.CreateTopicRequest,
     ) -> alikafka_20190916_models.CreateTopicResponse:
         """
-        Each Alibaba Cloud account can call this operation up to once per second.
-        *   The maximum number of topics that you can create in an instance is determined by the specification of the instance.
+        @summary Creates a topic.
+        
+        @description    Each Alibaba Cloud account can call this operation up to once per second.
+        The maximum number of topics that you can create in an instance is determined by the specification of the instance.
         
         @param request: CreateTopicRequest
         @return: CreateTopicResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_topic_with_options(request, runtime)
 
     async def create_topic_async(
         self,
         request: alikafka_20190916_models.CreateTopicRequest,
     ) -> alikafka_20190916_models.CreateTopicResponse:
         """
-        Each Alibaba Cloud account can call this operation up to once per second.
-        *   The maximum number of topics that you can create in an instance is determined by the specification of the instance.
+        @summary Creates a topic.
+        
+        @description    Each Alibaba Cloud account can call this operation up to once per second.
+        The maximum number of topics that you can create in an instance is determined by the specification of the instance.
         
         @param request: CreateTopicRequest
         @return: CreateTopicResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_topic_with_options_async(request, runtime)
 
     def delete_acl_with_options(
         self,
         request: alikafka_20190916_models.DeleteAclRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DeleteAclResponse:
+        """
+        @summary Deletes an access control list (ACL).
+        
+        @param request: DeleteAclRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAclResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_operation_type):
             query['AclOperationType'] = request.acl_operation_type
         if not UtilClient.is_unset(request.acl_operation_types):
             query['AclOperationTypes'] = request.acl_operation_types
         if not UtilClient.is_unset(request.acl_permission_type):
@@ -986,14 +1295,21 @@
         )
 
     async def delete_acl_with_options_async(
         self,
         request: alikafka_20190916_models.DeleteAclRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DeleteAclResponse:
+        """
+        @summary Deletes an access control list (ACL).
+        
+        @param request: DeleteAclRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAclResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_operation_type):
             query['AclOperationType'] = request.acl_operation_type
         if not UtilClient.is_unset(request.acl_operation_types):
             query['AclOperationTypes'] = request.acl_operation_types
         if not UtilClient.is_unset(request.acl_permission_type):
@@ -1031,29 +1347,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_acl(
         self,
         request: alikafka_20190916_models.DeleteAclRequest,
     ) -> alikafka_20190916_models.DeleteAclResponse:
+        """
+        @summary Deletes an access control list (ACL).
+        
+        @param request: DeleteAclRequest
+        @return: DeleteAclResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_acl_with_options(request, runtime)
 
     async def delete_acl_async(
         self,
         request: alikafka_20190916_models.DeleteAclRequest,
     ) -> alikafka_20190916_models.DeleteAclResponse:
+        """
+        @summary Deletes an access control list (ACL).
+        
+        @param request: DeleteAclRequest
+        @return: DeleteAclResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_acl_with_options_async(request, runtime)
 
     def delete_consumer_group_with_options(
         self,
         request: alikafka_20190916_models.DeleteConsumerGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DeleteConsumerGroupResponse:
+        """
+        @summary Deletes a consumer group from a specified Message Queue for Apache Kafka instance.
+        
+        @param request: DeleteConsumerGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteConsumerGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.consumer_id):
             query['ConsumerId'] = request.consumer_id
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -1078,14 +1413,21 @@
         )
 
     async def delete_consumer_group_with_options_async(
         self,
         request: alikafka_20190916_models.DeleteConsumerGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DeleteConsumerGroupResponse:
+        """
+        @summary Deletes a consumer group from a specified Message Queue for Apache Kafka instance.
+        
+        @param request: DeleteConsumerGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteConsumerGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.consumer_id):
             query['ConsumerId'] = request.consumer_id
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -1109,29 +1451,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_consumer_group(
         self,
         request: alikafka_20190916_models.DeleteConsumerGroupRequest,
     ) -> alikafka_20190916_models.DeleteConsumerGroupResponse:
+        """
+        @summary Deletes a consumer group from a specified Message Queue for Apache Kafka instance.
+        
+        @param request: DeleteConsumerGroupRequest
+        @return: DeleteConsumerGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_consumer_group_with_options(request, runtime)
 
     async def delete_consumer_group_async(
         self,
         request: alikafka_20190916_models.DeleteConsumerGroupRequest,
     ) -> alikafka_20190916_models.DeleteConsumerGroupResponse:
+        """
+        @summary Deletes a consumer group from a specified Message Queue for Apache Kafka instance.
+        
+        @param request: DeleteConsumerGroupRequest
+        @return: DeleteConsumerGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_consumer_group_with_options_async(request, runtime)
 
     def delete_instance_with_options(
         self,
         request: alikafka_20190916_models.DeleteInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DeleteInstanceResponse:
+        """
+        @summary Deletes an instance. You can delete subscription and pay-as-you-go instances after you release them.
+        
+        @param request: DeleteInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -1154,14 +1515,21 @@
         )
 
     async def delete_instance_with_options_async(
         self,
         request: alikafka_20190916_models.DeleteInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DeleteInstanceResponse:
+        """
+        @summary Deletes an instance. You can delete subscription and pay-as-you-go instances after you release them.
+        
+        @param request: DeleteInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -1183,29 +1551,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_instance(
         self,
         request: alikafka_20190916_models.DeleteInstanceRequest,
     ) -> alikafka_20190916_models.DeleteInstanceResponse:
+        """
+        @summary Deletes an instance. You can delete subscription and pay-as-you-go instances after you release them.
+        
+        @param request: DeleteInstanceRequest
+        @return: DeleteInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_instance_with_options(request, runtime)
 
     async def delete_instance_async(
         self,
         request: alikafka_20190916_models.DeleteInstanceRequest,
     ) -> alikafka_20190916_models.DeleteInstanceResponse:
+        """
+        @summary Deletes an instance. You can delete subscription and pay-as-you-go instances after you release them.
+        
+        @param request: DeleteInstanceRequest
+        @return: DeleteInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_instance_with_options_async(request, runtime)
 
     def delete_sasl_user_with_options(
         self,
         request: alikafka_20190916_models.DeleteSaslUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DeleteSaslUserResponse:
+        """
+        @summary Deletes a Simple Authentication and Security Layer (SASL) user.
+        
+        @param request: DeleteSaslUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteSaslUserResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.mechanism):
             query['Mechanism'] = request.mechanism
         if not UtilClient.is_unset(request.region_id):
@@ -1234,14 +1621,21 @@
         )
 
     async def delete_sasl_user_with_options_async(
         self,
         request: alikafka_20190916_models.DeleteSaslUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DeleteSaslUserResponse:
+        """
+        @summary Deletes a Simple Authentication and Security Layer (SASL) user.
+        
+        @param request: DeleteSaslUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteSaslUserResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.mechanism):
             query['Mechanism'] = request.mechanism
         if not UtilClient.is_unset(request.region_id):
@@ -1269,29 +1663,152 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_sasl_user(
         self,
         request: alikafka_20190916_models.DeleteSaslUserRequest,
     ) -> alikafka_20190916_models.DeleteSaslUserResponse:
+        """
+        @summary Deletes a Simple Authentication and Security Layer (SASL) user.
+        
+        @param request: DeleteSaslUserRequest
+        @return: DeleteSaslUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_sasl_user_with_options(request, runtime)
 
     async def delete_sasl_user_async(
         self,
         request: alikafka_20190916_models.DeleteSaslUserRequest,
     ) -> alikafka_20190916_models.DeleteSaslUserResponse:
+        """
+        @summary Deletes a Simple Authentication and Security Layer (SASL) user.
+        
+        @param request: DeleteSaslUserRequest
+        @return: DeleteSaslUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_sasl_user_with_options_async(request, runtime)
 
+    def delete_scheduled_scaling_rule_with_options(
+        self,
+        request: alikafka_20190916_models.DeleteScheduledScalingRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> alikafka_20190916_models.DeleteScheduledScalingRuleResponse:
+        """
+        @summary 删除定时伸缩规则
+        
+        @param request: DeleteScheduledScalingRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteScheduledScalingRuleResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_name):
+            query['RuleName'] = request.rule_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteScheduledScalingRule',
+            version='2019-09-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            alikafka_20190916_models.DeleteScheduledScalingRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_scheduled_scaling_rule_with_options_async(
+        self,
+        request: alikafka_20190916_models.DeleteScheduledScalingRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> alikafka_20190916_models.DeleteScheduledScalingRuleResponse:
+        """
+        @summary 删除定时伸缩规则
+        
+        @param request: DeleteScheduledScalingRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteScheduledScalingRuleResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_name):
+            query['RuleName'] = request.rule_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteScheduledScalingRule',
+            version='2019-09-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            alikafka_20190916_models.DeleteScheduledScalingRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_scheduled_scaling_rule(
+        self,
+        request: alikafka_20190916_models.DeleteScheduledScalingRuleRequest,
+    ) -> alikafka_20190916_models.DeleteScheduledScalingRuleResponse:
+        """
+        @summary 删除定时伸缩规则
+        
+        @param request: DeleteScheduledScalingRuleRequest
+        @return: DeleteScheduledScalingRuleResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.delete_scheduled_scaling_rule_with_options(request, runtime)
+
+    async def delete_scheduled_scaling_rule_async(
+        self,
+        request: alikafka_20190916_models.DeleteScheduledScalingRuleRequest,
+    ) -> alikafka_20190916_models.DeleteScheduledScalingRuleResponse:
+        """
+        @summary 删除定时伸缩规则
+        
+        @param request: DeleteScheduledScalingRuleRequest
+        @return: DeleteScheduledScalingRuleResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_scheduled_scaling_rule_with_options_async(request, runtime)
+
     def delete_topic_with_options(
         self,
         request: alikafka_20190916_models.DeleteTopicRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DeleteTopicResponse:
+        """
+        @summary Deletes a topic.
+        
+        @param request: DeleteTopicRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTopicResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.topic):
@@ -1316,14 +1833,21 @@
         )
 
     async def delete_topic_with_options_async(
         self,
         request: alikafka_20190916_models.DeleteTopicRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DeleteTopicResponse:
+        """
+        @summary Deletes a topic.
+        
+        @param request: DeleteTopicRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTopicResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.topic):
@@ -1347,29 +1871,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_topic(
         self,
         request: alikafka_20190916_models.DeleteTopicRequest,
     ) -> alikafka_20190916_models.DeleteTopicResponse:
+        """
+        @summary Deletes a topic.
+        
+        @param request: DeleteTopicRequest
+        @return: DeleteTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_topic_with_options(request, runtime)
 
     async def delete_topic_async(
         self,
         request: alikafka_20190916_models.DeleteTopicRequest,
     ) -> alikafka_20190916_models.DeleteTopicResponse:
+        """
+        @summary Deletes a topic.
+        
+        @param request: DeleteTopicRequest
+        @return: DeleteTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_topic_with_options_async(request, runtime)
 
     def describe_acls_with_options(
         self,
         request: alikafka_20190916_models.DescribeAclsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DescribeAclsResponse:
+        """
+        @summary Queries access control lists (ACLs).
+        
+        @param request: DescribeAclsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAclsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_operation_type):
             query['AclOperationType'] = request.acl_operation_type
         if not UtilClient.is_unset(request.acl_permission_type):
             query['AclPermissionType'] = request.acl_permission_type
         if not UtilClient.is_unset(request.acl_resource_name):
@@ -1406,14 +1949,21 @@
         )
 
     async def describe_acls_with_options_async(
         self,
         request: alikafka_20190916_models.DescribeAclsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DescribeAclsResponse:
+        """
+        @summary Queries access control lists (ACLs).
+        
+        @param request: DescribeAclsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAclsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_operation_type):
             query['AclOperationType'] = request.acl_operation_type
         if not UtilClient.is_unset(request.acl_permission_type):
             query['AclPermissionType'] = request.acl_permission_type
         if not UtilClient.is_unset(request.acl_resource_name):
@@ -1449,29 +1999,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_acls(
         self,
         request: alikafka_20190916_models.DescribeAclsRequest,
     ) -> alikafka_20190916_models.DescribeAclsResponse:
+        """
+        @summary Queries access control lists (ACLs).
+        
+        @param request: DescribeAclsRequest
+        @return: DescribeAclsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_acls_with_options(request, runtime)
 
     async def describe_acls_async(
         self,
         request: alikafka_20190916_models.DescribeAclsRequest,
     ) -> alikafka_20190916_models.DescribeAclsResponse:
+        """
+        @summary Queries access control lists (ACLs).
+        
+        @param request: DescribeAclsRequest
+        @return: DescribeAclsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_acls_with_options_async(request, runtime)
 
     def describe_sasl_users_with_options(
         self,
         request: alikafka_20190916_models.DescribeSaslUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DescribeSaslUsersResponse:
+        """
+        @summary Queries Simple Authentication and Security Layer (SASL) users.
+        
+        @param request: DescribeSaslUsersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSaslUsersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -1494,14 +2063,21 @@
         )
 
     async def describe_sasl_users_with_options_async(
         self,
         request: alikafka_20190916_models.DescribeSaslUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DescribeSaslUsersResponse:
+        """
+        @summary Queries Simple Authentication and Security Layer (SASL) users.
+        
+        @param request: DescribeSaslUsersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSaslUsersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -1523,29 +2099,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_sasl_users(
         self,
         request: alikafka_20190916_models.DescribeSaslUsersRequest,
     ) -> alikafka_20190916_models.DescribeSaslUsersResponse:
+        """
+        @summary Queries Simple Authentication and Security Layer (SASL) users.
+        
+        @param request: DescribeSaslUsersRequest
+        @return: DescribeSaslUsersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_sasl_users_with_options(request, runtime)
 
     async def describe_sasl_users_async(
         self,
         request: alikafka_20190916_models.DescribeSaslUsersRequest,
     ) -> alikafka_20190916_models.DescribeSaslUsersResponse:
+        """
+        @summary Queries Simple Authentication and Security Layer (SASL) users.
+        
+        @param request: DescribeSaslUsersRequest
+        @return: DescribeSaslUsersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_sasl_users_with_options_async(request, runtime)
 
     def enable_auto_group_creation_with_options(
         self,
         request: alikafka_20190916_models.EnableAutoGroupCreationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.EnableAutoGroupCreationResponse:
+        """
+        @summary Enables and disables the flexible group creation feature.
+        
+        @param request: EnableAutoGroupCreationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableAutoGroupCreationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.enable):
             query['Enable'] = request.enable
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -1570,14 +2165,21 @@
         )
 
     async def enable_auto_group_creation_with_options_async(
         self,
         request: alikafka_20190916_models.EnableAutoGroupCreationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.EnableAutoGroupCreationResponse:
+        """
+        @summary Enables and disables the flexible group creation feature.
+        
+        @param request: EnableAutoGroupCreationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableAutoGroupCreationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.enable):
             query['Enable'] = request.enable
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -1601,29 +2203,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def enable_auto_group_creation(
         self,
         request: alikafka_20190916_models.EnableAutoGroupCreationRequest,
     ) -> alikafka_20190916_models.EnableAutoGroupCreationResponse:
+        """
+        @summary Enables and disables the flexible group creation feature.
+        
+        @param request: EnableAutoGroupCreationRequest
+        @return: EnableAutoGroupCreationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.enable_auto_group_creation_with_options(request, runtime)
 
     async def enable_auto_group_creation_async(
         self,
         request: alikafka_20190916_models.EnableAutoGroupCreationRequest,
     ) -> alikafka_20190916_models.EnableAutoGroupCreationResponse:
+        """
+        @summary Enables and disables the flexible group creation feature.
+        
+        @param request: EnableAutoGroupCreationRequest
+        @return: EnableAutoGroupCreationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.enable_auto_group_creation_with_options_async(request, runtime)
 
     def enable_auto_topic_creation_with_options(
         self,
         request: alikafka_20190916_models.EnableAutoTopicCreationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.EnableAutoTopicCreationResponse:
+        """
+        @summary Enables or disables the automatic topic creation feature, or changes the number of partitions in topics that are automatically created.
+        
+        @param request: EnableAutoTopicCreationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableAutoTopicCreationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.operate):
             query['Operate'] = request.operate
         if not UtilClient.is_unset(request.partition_num):
@@ -1650,14 +2271,21 @@
         )
 
     async def enable_auto_topic_creation_with_options_async(
         self,
         request: alikafka_20190916_models.EnableAutoTopicCreationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.EnableAutoTopicCreationResponse:
+        """
+        @summary Enables or disables the automatic topic creation feature, or changes the number of partitions in topics that are automatically created.
+        
+        @param request: EnableAutoTopicCreationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableAutoTopicCreationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.operate):
             query['Operate'] = request.operate
         if not UtilClient.is_unset(request.partition_num):
@@ -1683,29 +2311,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def enable_auto_topic_creation(
         self,
         request: alikafka_20190916_models.EnableAutoTopicCreationRequest,
     ) -> alikafka_20190916_models.EnableAutoTopicCreationResponse:
+        """
+        @summary Enables or disables the automatic topic creation feature, or changes the number of partitions in topics that are automatically created.
+        
+        @param request: EnableAutoTopicCreationRequest
+        @return: EnableAutoTopicCreationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.enable_auto_topic_creation_with_options(request, runtime)
 
     async def enable_auto_topic_creation_async(
         self,
         request: alikafka_20190916_models.EnableAutoTopicCreationRequest,
     ) -> alikafka_20190916_models.EnableAutoTopicCreationResponse:
+        """
+        @summary Enables or disables the automatic topic creation feature, or changes the number of partitions in topics that are automatically created.
+        
+        @param request: EnableAutoTopicCreationRequest
+        @return: EnableAutoTopicCreationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.enable_auto_topic_creation_with_options_async(request, runtime)
 
     def get_all_instance_id_list_with_options(
         self,
         request: alikafka_20190916_models.GetAllInstanceIdListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetAllInstanceIdListResponse:
+        """
+        @summary Queries the IDs of all instances in the current account.
+        
+        @param request: GetAllInstanceIdListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAllInstanceIdListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1726,14 +2373,21 @@
         )
 
     async def get_all_instance_id_list_with_options_async(
         self,
         request: alikafka_20190916_models.GetAllInstanceIdListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetAllInstanceIdListResponse:
+        """
+        @summary Queries the IDs of all instances in the current account.
+        
+        @param request: GetAllInstanceIdListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAllInstanceIdListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1753,29 +2407,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_all_instance_id_list(
         self,
         request: alikafka_20190916_models.GetAllInstanceIdListRequest,
     ) -> alikafka_20190916_models.GetAllInstanceIdListResponse:
+        """
+        @summary Queries the IDs of all instances in the current account.
+        
+        @param request: GetAllInstanceIdListRequest
+        @return: GetAllInstanceIdListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_all_instance_id_list_with_options(request, runtime)
 
     async def get_all_instance_id_list_async(
         self,
         request: alikafka_20190916_models.GetAllInstanceIdListRequest,
     ) -> alikafka_20190916_models.GetAllInstanceIdListResponse:
+        """
+        @summary Queries the IDs of all instances in the current account.
+        
+        @param request: GetAllInstanceIdListRequest
+        @return: GetAllInstanceIdListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_all_instance_id_list_with_options_async(request, runtime)
 
     def get_allowed_ip_list_with_options(
         self,
         request: alikafka_20190916_models.GetAllowedIpListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetAllowedIpListResponse:
+        """
+        @summary Queries the IP address whitelist.
+        
+        @param request: GetAllowedIpListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAllowedIpListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -1798,14 +2471,21 @@
         )
 
     async def get_allowed_ip_list_with_options_async(
         self,
         request: alikafka_20190916_models.GetAllowedIpListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetAllowedIpListResponse:
+        """
+        @summary Queries the IP address whitelist.
+        
+        @param request: GetAllowedIpListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAllowedIpListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -1827,29 +2507,148 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_allowed_ip_list(
         self,
         request: alikafka_20190916_models.GetAllowedIpListRequest,
     ) -> alikafka_20190916_models.GetAllowedIpListResponse:
+        """
+        @summary Queries the IP address whitelist.
+        
+        @param request: GetAllowedIpListRequest
+        @return: GetAllowedIpListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_allowed_ip_list_with_options(request, runtime)
 
     async def get_allowed_ip_list_async(
         self,
         request: alikafka_20190916_models.GetAllowedIpListRequest,
     ) -> alikafka_20190916_models.GetAllowedIpListResponse:
+        """
+        @summary Queries the IP address whitelist.
+        
+        @param request: GetAllowedIpListRequest
+        @return: GetAllowedIpListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_allowed_ip_list_with_options_async(request, runtime)
 
+    def get_auto_scaling_configuration_with_options(
+        self,
+        request: alikafka_20190916_models.GetAutoScalingConfigurationRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> alikafka_20190916_models.GetAutoScalingConfigurationResponse:
+        """
+        @summary 查询自动伸缩配置
+        
+        @param request: GetAutoScalingConfigurationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAutoScalingConfigurationResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAutoScalingConfiguration',
+            version='2019-09-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            alikafka_20190916_models.GetAutoScalingConfigurationResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_auto_scaling_configuration_with_options_async(
+        self,
+        request: alikafka_20190916_models.GetAutoScalingConfigurationRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> alikafka_20190916_models.GetAutoScalingConfigurationResponse:
+        """
+        @summary 查询自动伸缩配置
+        
+        @param request: GetAutoScalingConfigurationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAutoScalingConfigurationResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAutoScalingConfiguration',
+            version='2019-09-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            alikafka_20190916_models.GetAutoScalingConfigurationResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_auto_scaling_configuration(
+        self,
+        request: alikafka_20190916_models.GetAutoScalingConfigurationRequest,
+    ) -> alikafka_20190916_models.GetAutoScalingConfigurationResponse:
+        """
+        @summary 查询自动伸缩配置
+        
+        @param request: GetAutoScalingConfigurationRequest
+        @return: GetAutoScalingConfigurationResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.get_auto_scaling_configuration_with_options(request, runtime)
+
+    async def get_auto_scaling_configuration_async(
+        self,
+        request: alikafka_20190916_models.GetAutoScalingConfigurationRequest,
+    ) -> alikafka_20190916_models.GetAutoScalingConfigurationResponse:
+        """
+        @summary 查询自动伸缩配置
+        
+        @param request: GetAutoScalingConfigurationRequest
+        @return: GetAutoScalingConfigurationResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.get_auto_scaling_configuration_with_options_async(request, runtime)
+
     def get_consumer_list_with_options(
         self,
         request: alikafka_20190916_models.GetConsumerListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetConsumerListResponse:
+        """
+        @summary Queries one or more consumer groups in a specified Message Queue for Apache Kafka instance.
+        
+        @param request: GetConsumerListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetConsumerListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.consumer_id):
             query['ConsumerId'] = request.consumer_id
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.instance_id):
@@ -1878,14 +2677,21 @@
         )
 
     async def get_consumer_list_with_options_async(
         self,
         request: alikafka_20190916_models.GetConsumerListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetConsumerListResponse:
+        """
+        @summary Queries one or more consumer groups in a specified Message Queue for Apache Kafka instance.
+        
+        @param request: GetConsumerListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetConsumerListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.consumer_id):
             query['ConsumerId'] = request.consumer_id
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.instance_id):
@@ -1913,29 +2719,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_consumer_list(
         self,
         request: alikafka_20190916_models.GetConsumerListRequest,
     ) -> alikafka_20190916_models.GetConsumerListResponse:
+        """
+        @summary Queries one or more consumer groups in a specified Message Queue for Apache Kafka instance.
+        
+        @param request: GetConsumerListRequest
+        @return: GetConsumerListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_consumer_list_with_options(request, runtime)
 
     async def get_consumer_list_async(
         self,
         request: alikafka_20190916_models.GetConsumerListRequest,
     ) -> alikafka_20190916_models.GetConsumerListResponse:
+        """
+        @summary Queries one or more consumer groups in a specified Message Queue for Apache Kafka instance.
+        
+        @param request: GetConsumerListRequest
+        @return: GetConsumerListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_consumer_list_with_options_async(request, runtime)
 
     def get_consumer_progress_with_options(
         self,
         request: alikafka_20190916_models.GetConsumerProgressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetConsumerProgressResponse:
+        """
+        @summary Queries the consumer progress of a consumer group.
+        
+        @param request: GetConsumerProgressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetConsumerProgressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.consumer_id):
             query['ConsumerId'] = request.consumer_id
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -1960,14 +2785,21 @@
         )
 
     async def get_consumer_progress_with_options_async(
         self,
         request: alikafka_20190916_models.GetConsumerProgressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetConsumerProgressResponse:
+        """
+        @summary Queries the consumer progress of a consumer group.
+        
+        @param request: GetConsumerProgressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetConsumerProgressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.consumer_id):
             query['ConsumerId'] = request.consumer_id
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -1991,29 +2823,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_consumer_progress(
         self,
         request: alikafka_20190916_models.GetConsumerProgressRequest,
     ) -> alikafka_20190916_models.GetConsumerProgressResponse:
+        """
+        @summary Queries the consumer progress of a consumer group.
+        
+        @param request: GetConsumerProgressRequest
+        @return: GetConsumerProgressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_consumer_progress_with_options(request, runtime)
 
     async def get_consumer_progress_async(
         self,
         request: alikafka_20190916_models.GetConsumerProgressRequest,
     ) -> alikafka_20190916_models.GetConsumerProgressResponse:
+        """
+        @summary Queries the consumer progress of a consumer group.
+        
+        @param request: GetConsumerProgressRequest
+        @return: GetConsumerProgressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_consumer_progress_with_options_async(request, runtime)
 
     def get_instance_list_with_options(
         self,
         request: alikafka_20190916_models.GetInstanceListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetInstanceListResponse:
+        """
+        @summary Queries the information about instances in a specified region.
+        
+        @param request: GetInstanceListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetInstanceListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.order_id):
             query['OrderId'] = request.order_id
         if not UtilClient.is_unset(request.region_id):
@@ -2044,14 +2895,21 @@
         )
 
     async def get_instance_list_with_options_async(
         self,
         request: alikafka_20190916_models.GetInstanceListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetInstanceListResponse:
+        """
+        @summary Queries the information about instances in a specified region.
+        
+        @param request: GetInstanceListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetInstanceListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.order_id):
             query['OrderId'] = request.order_id
         if not UtilClient.is_unset(request.region_id):
@@ -2081,29 +2939,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_instance_list(
         self,
         request: alikafka_20190916_models.GetInstanceListRequest,
     ) -> alikafka_20190916_models.GetInstanceListResponse:
+        """
+        @summary Queries the information about instances in a specified region.
+        
+        @param request: GetInstanceListRequest
+        @return: GetInstanceListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_instance_list_with_options(request, runtime)
 
     async def get_instance_list_async(
         self,
         request: alikafka_20190916_models.GetInstanceListRequest,
     ) -> alikafka_20190916_models.GetInstanceListResponse:
+        """
+        @summary Queries the information about instances in a specified region.
+        
+        @param request: GetInstanceListRequest
+        @return: GetInstanceListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_instance_list_with_options_async(request, runtime)
 
     def get_quota_tip_with_options(
         self,
         request: alikafka_20190916_models.GetQuotaTipRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetQuotaTipResponse:
+        """
+        @summary Queries the used quota of topics and partitions.
+        
+        @param request: GetQuotaTipRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetQuotaTipResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -2126,14 +3003,21 @@
         )
 
     async def get_quota_tip_with_options_async(
         self,
         request: alikafka_20190916_models.GetQuotaTipRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetQuotaTipResponse:
+        """
+        @summary Queries the used quota of topics and partitions.
+        
+        @param request: GetQuotaTipRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetQuotaTipResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -2155,29 +3039,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_quota_tip(
         self,
         request: alikafka_20190916_models.GetQuotaTipRequest,
     ) -> alikafka_20190916_models.GetQuotaTipResponse:
+        """
+        @summary Queries the used quota of topics and partitions.
+        
+        @param request: GetQuotaTipRequest
+        @return: GetQuotaTipResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_quota_tip_with_options(request, runtime)
 
     async def get_quota_tip_async(
         self,
         request: alikafka_20190916_models.GetQuotaTipRequest,
     ) -> alikafka_20190916_models.GetQuotaTipResponse:
+        """
+        @summary Queries the used quota of topics and partitions.
+        
+        @param request: GetQuotaTipRequest
+        @return: GetQuotaTipResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_quota_tip_with_options_async(request, runtime)
 
     def get_topic_list_with_options(
         self,
         request: alikafka_20190916_models.GetTopicListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetTopicListResponse:
+        """
+        @summary Queries the information about a topic.
+        
+        @param request: GetTopicListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTopicListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.page_size):
@@ -2206,14 +3109,21 @@
         )
 
     async def get_topic_list_with_options_async(
         self,
         request: alikafka_20190916_models.GetTopicListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetTopicListResponse:
+        """
+        @summary Queries the information about a topic.
+        
+        @param request: GetTopicListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTopicListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.page_size):
@@ -2241,29 +3151,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_topic_list(
         self,
         request: alikafka_20190916_models.GetTopicListRequest,
     ) -> alikafka_20190916_models.GetTopicListResponse:
+        """
+        @summary Queries the information about a topic.
+        
+        @param request: GetTopicListRequest
+        @return: GetTopicListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_topic_list_with_options(request, runtime)
 
     async def get_topic_list_async(
         self,
         request: alikafka_20190916_models.GetTopicListRequest,
     ) -> alikafka_20190916_models.GetTopicListResponse:
+        """
+        @summary Queries the information about a topic.
+        
+        @param request: GetTopicListRequest
+        @return: GetTopicListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_topic_list_with_options_async(request, runtime)
 
     def get_topic_status_with_options(
         self,
         request: alikafka_20190916_models.GetTopicStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetTopicStatusResponse:
+        """
+        @summary Queries the status information about messages in a specified topic.
+        
+        @param request: GetTopicStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTopicStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.topic):
@@ -2288,14 +3217,21 @@
         )
 
     async def get_topic_status_with_options_async(
         self,
         request: alikafka_20190916_models.GetTopicStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetTopicStatusResponse:
+        """
+        @summary Queries the status information about messages in a specified topic.
+        
+        @param request: GetTopicStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTopicStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.topic):
@@ -2319,29 +3255,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_topic_status(
         self,
         request: alikafka_20190916_models.GetTopicStatusRequest,
     ) -> alikafka_20190916_models.GetTopicStatusResponse:
+        """
+        @summary Queries the status information about messages in a specified topic.
+        
+        @param request: GetTopicStatusRequest
+        @return: GetTopicStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_topic_status_with_options(request, runtime)
 
     async def get_topic_status_async(
         self,
         request: alikafka_20190916_models.GetTopicStatusRequest,
     ) -> alikafka_20190916_models.GetTopicStatusResponse:
+        """
+        @summary Queries the status information about messages in a specified topic.
+        
+        @param request: GetTopicStatusRequest
+        @return: GetTopicStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_topic_status_with_options_async(request, runtime)
 
     def get_topic_subscribe_status_with_options(
         self,
         request: alikafka_20190916_models.GetTopicSubscribeStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetTopicSubscribeStatusResponse:
+        """
+        @summary Obtains the information about a group that subscribes to a topic.
+        
+        @param request: GetTopicSubscribeStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTopicSubscribeStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.topic):
@@ -2366,14 +3321,21 @@
         )
 
     async def get_topic_subscribe_status_with_options_async(
         self,
         request: alikafka_20190916_models.GetTopicSubscribeStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetTopicSubscribeStatusResponse:
+        """
+        @summary Obtains the information about a group that subscribes to a topic.
+        
+        @param request: GetTopicSubscribeStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTopicSubscribeStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.topic):
@@ -2397,29 +3359,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_topic_subscribe_status(
         self,
         request: alikafka_20190916_models.GetTopicSubscribeStatusRequest,
     ) -> alikafka_20190916_models.GetTopicSubscribeStatusResponse:
+        """
+        @summary Obtains the information about a group that subscribes to a topic.
+        
+        @param request: GetTopicSubscribeStatusRequest
+        @return: GetTopicSubscribeStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_topic_subscribe_status_with_options(request, runtime)
 
     async def get_topic_subscribe_status_async(
         self,
         request: alikafka_20190916_models.GetTopicSubscribeStatusRequest,
     ) -> alikafka_20190916_models.GetTopicSubscribeStatusResponse:
+        """
+        @summary Obtains the information about a group that subscribes to a topic.
+        
+        @param request: GetTopicSubscribeStatusRequest
+        @return: GetTopicSubscribeStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_topic_subscribe_status_with_options_async(request, runtime)
 
     def list_tag_resources_with_options(
         self,
         request: alikafka_20190916_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ListTagResourcesResponse:
+        """
+        @summary Queries the tags that are attached to a specified resource.
+        
+        @param request: ListTagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_id):
@@ -2448,14 +3429,21 @@
         )
 
     async def list_tag_resources_with_options_async(
         self,
         request: alikafka_20190916_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ListTagResourcesResponse:
+        """
+        @summary Queries the tags that are attached to a specified resource.
+        
+        @param request: ListTagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_id):
@@ -2483,29 +3471,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_tag_resources(
         self,
         request: alikafka_20190916_models.ListTagResourcesRequest,
     ) -> alikafka_20190916_models.ListTagResourcesResponse:
+        """
+        @summary Queries the tags that are attached to a specified resource.
+        
+        @param request: ListTagResourcesRequest
+        @return: ListTagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_tag_resources_with_options(request, runtime)
 
     async def list_tag_resources_async(
         self,
         request: alikafka_20190916_models.ListTagResourcesRequest,
     ) -> alikafka_20190916_models.ListTagResourcesResponse:
+        """
+        @summary Queries the tags that are attached to a specified resource.
+        
+        @param request: ListTagResourcesRequest
+        @return: ListTagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_tag_resources_with_options_async(request, runtime)
 
     def modify_instance_name_with_options(
         self,
         request: alikafka_20190916_models.ModifyInstanceNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ModifyInstanceNameResponse:
+        """
+        @summary Changes the name of an ApsaraMQ for Kafka instance. After you deploy an instance, you can call this operation to change the name of the instance.
+        
+        @param request: ModifyInstanceNameRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyInstanceNameResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.instance_name):
             query['InstanceName'] = request.instance_name
         if not UtilClient.is_unset(request.region_id):
@@ -2530,14 +3537,21 @@
         )
 
     async def modify_instance_name_with_options_async(
         self,
         request: alikafka_20190916_models.ModifyInstanceNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ModifyInstanceNameResponse:
+        """
+        @summary Changes the name of an ApsaraMQ for Kafka instance. After you deploy an instance, you can call this operation to change the name of the instance.
+        
+        @param request: ModifyInstanceNameRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyInstanceNameResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.instance_name):
             query['InstanceName'] = request.instance_name
         if not UtilClient.is_unset(request.region_id):
@@ -2561,29 +3575,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_instance_name(
         self,
         request: alikafka_20190916_models.ModifyInstanceNameRequest,
     ) -> alikafka_20190916_models.ModifyInstanceNameResponse:
+        """
+        @summary Changes the name of an ApsaraMQ for Kafka instance. After you deploy an instance, you can call this operation to change the name of the instance.
+        
+        @param request: ModifyInstanceNameRequest
+        @return: ModifyInstanceNameResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_instance_name_with_options(request, runtime)
 
     async def modify_instance_name_async(
         self,
         request: alikafka_20190916_models.ModifyInstanceNameRequest,
     ) -> alikafka_20190916_models.ModifyInstanceNameResponse:
+        """
+        @summary Changes the name of an ApsaraMQ for Kafka instance. After you deploy an instance, you can call this operation to change the name of the instance.
+        
+        @param request: ModifyInstanceNameRequest
+        @return: ModifyInstanceNameResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_instance_name_with_options_async(request, runtime)
 
     def modify_partition_num_with_options(
         self,
         request: alikafka_20190916_models.ModifyPartitionNumRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ModifyPartitionNumResponse:
+        """
+        @summary Changes the number of partitions in a specified topic.
+        
+        @param request: ModifyPartitionNumRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyPartitionNumResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.add_partition_num):
             query['AddPartitionNum'] = request.add_partition_num
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -2610,14 +3643,21 @@
         )
 
     async def modify_partition_num_with_options_async(
         self,
         request: alikafka_20190916_models.ModifyPartitionNumRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ModifyPartitionNumResponse:
+        """
+        @summary Changes the number of partitions in a specified topic.
+        
+        @param request: ModifyPartitionNumRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyPartitionNumResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.add_partition_num):
             query['AddPartitionNum'] = request.add_partition_num
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -2643,29 +3683,156 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_partition_num(
         self,
         request: alikafka_20190916_models.ModifyPartitionNumRequest,
     ) -> alikafka_20190916_models.ModifyPartitionNumResponse:
+        """
+        @summary Changes the number of partitions in a specified topic.
+        
+        @param request: ModifyPartitionNumRequest
+        @return: ModifyPartitionNumResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_partition_num_with_options(request, runtime)
 
     async def modify_partition_num_async(
         self,
         request: alikafka_20190916_models.ModifyPartitionNumRequest,
     ) -> alikafka_20190916_models.ModifyPartitionNumResponse:
+        """
+        @summary Changes the number of partitions in a specified topic.
+        
+        @param request: ModifyPartitionNumRequest
+        @return: ModifyPartitionNumResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_partition_num_with_options_async(request, runtime)
 
+    def modify_scheduled_scaling_rule_with_options(
+        self,
+        request: alikafka_20190916_models.ModifyScheduledScalingRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> alikafka_20190916_models.ModifyScheduledScalingRuleResponse:
+        """
+        @summary 修改定时伸缩规则
+        
+        @param request: ModifyScheduledScalingRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyScheduledScalingRuleResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.enable):
+            query['Enable'] = request.enable
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_name):
+            query['RuleName'] = request.rule_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyScheduledScalingRule',
+            version='2019-09-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            alikafka_20190916_models.ModifyScheduledScalingRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_scheduled_scaling_rule_with_options_async(
+        self,
+        request: alikafka_20190916_models.ModifyScheduledScalingRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> alikafka_20190916_models.ModifyScheduledScalingRuleResponse:
+        """
+        @summary 修改定时伸缩规则
+        
+        @param request: ModifyScheduledScalingRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyScheduledScalingRuleResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.enable):
+            query['Enable'] = request.enable
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_name):
+            query['RuleName'] = request.rule_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyScheduledScalingRule',
+            version='2019-09-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            alikafka_20190916_models.ModifyScheduledScalingRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_scheduled_scaling_rule(
+        self,
+        request: alikafka_20190916_models.ModifyScheduledScalingRuleRequest,
+    ) -> alikafka_20190916_models.ModifyScheduledScalingRuleResponse:
+        """
+        @summary 修改定时伸缩规则
+        
+        @param request: ModifyScheduledScalingRuleRequest
+        @return: ModifyScheduledScalingRuleResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.modify_scheduled_scaling_rule_with_options(request, runtime)
+
+    async def modify_scheduled_scaling_rule_async(
+        self,
+        request: alikafka_20190916_models.ModifyScheduledScalingRuleRequest,
+    ) -> alikafka_20190916_models.ModifyScheduledScalingRuleResponse:
+        """
+        @summary 修改定时伸缩规则
+        
+        @param request: ModifyScheduledScalingRuleRequest
+        @return: ModifyScheduledScalingRuleResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_scheduled_scaling_rule_with_options_async(request, runtime)
+
     def modify_topic_remark_with_options(
         self,
         request: alikafka_20190916_models.ModifyTopicRemarkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ModifyTopicRemarkResponse:
+        """
+        @summary Modifies the description of a topic.
+        
+        @param request: ModifyTopicRemarkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyTopicRemarkResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.remark):
@@ -2692,14 +3859,21 @@
         )
 
     async def modify_topic_remark_with_options_async(
         self,
         request: alikafka_20190916_models.ModifyTopicRemarkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ModifyTopicRemarkResponse:
+        """
+        @summary Modifies the description of a topic.
+        
+        @param request: ModifyTopicRemarkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyTopicRemarkResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.remark):
@@ -2725,29 +3899,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_topic_remark(
         self,
         request: alikafka_20190916_models.ModifyTopicRemarkRequest,
     ) -> alikafka_20190916_models.ModifyTopicRemarkResponse:
+        """
+        @summary Modifies the description of a topic.
+        
+        @param request: ModifyTopicRemarkRequest
+        @return: ModifyTopicRemarkResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_topic_remark_with_options(request, runtime)
 
     async def modify_topic_remark_async(
         self,
         request: alikafka_20190916_models.ModifyTopicRemarkRequest,
     ) -> alikafka_20190916_models.ModifyTopicRemarkResponse:
+        """
+        @summary Modifies the description of a topic.
+        
+        @param request: ModifyTopicRemarkRequest
+        @return: ModifyTopicRemarkResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_topic_remark_with_options_async(request, runtime)
 
     def query_message_with_options(
         self,
         request: alikafka_20190916_models.QueryMessageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.QueryMessageResponse:
+        """
+        @summary Queries messages stored in a topic. You can query messages by creation time or offset.
+        
+        @param request: QueryMessageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMessageResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='QueryMessage',
@@ -2766,14 +3959,21 @@
         )
 
     async def query_message_with_options_async(
         self,
         request: alikafka_20190916_models.QueryMessageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.QueryMessageResponse:
+        """
+        @summary Queries messages stored in a topic. You can query messages by creation time or offset.
+        
+        @param request: QueryMessageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMessageResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='QueryMessage',
@@ -2791,31 +3991,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_message(
         self,
         request: alikafka_20190916_models.QueryMessageRequest,
     ) -> alikafka_20190916_models.QueryMessageResponse:
+        """
+        @summary Queries messages stored in a topic. You can query messages by creation time or offset.
+        
+        @param request: QueryMessageRequest
+        @return: QueryMessageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_message_with_options(request, runtime)
 
     async def query_message_async(
         self,
         request: alikafka_20190916_models.QueryMessageRequest,
     ) -> alikafka_20190916_models.QueryMessageResponse:
+        """
+        @summary Queries messages stored in a topic. You can query messages by creation time or offset.
+        
+        @param request: QueryMessageRequest
+        @return: QueryMessageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_message_with_options_async(request, runtime)
 
     def release_instance_with_options(
         self,
         request: alikafka_20190916_models.ReleaseInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ReleaseInstanceResponse:
         """
-        You cannot call this operation to release a subscription Message Queue for Apache Kafka instance.
+        @summary Releases a pay-as-you-go Message Queue for Apache Kafka instance.
+        
+        @description You cannot call this operation to release a subscription Message Queue for Apache Kafka instance.
         
         @param request: ReleaseInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ReleaseInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2846,15 +4060,17 @@
 
     async def release_instance_with_options_async(
         self,
         request: alikafka_20190916_models.ReleaseInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ReleaseInstanceResponse:
         """
-        You cannot call this operation to release a subscription Message Queue for Apache Kafka instance.
+        @summary Releases a pay-as-you-go Message Queue for Apache Kafka instance.
+        
+        @description You cannot call this operation to release a subscription Message Queue for Apache Kafka instance.
         
         @param request: ReleaseInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ReleaseInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2884,42 +4100,48 @@
         )
 
     def release_instance(
         self,
         request: alikafka_20190916_models.ReleaseInstanceRequest,
     ) -> alikafka_20190916_models.ReleaseInstanceResponse:
         """
-        You cannot call this operation to release a subscription Message Queue for Apache Kafka instance.
+        @summary Releases a pay-as-you-go Message Queue for Apache Kafka instance.
+        
+        @description You cannot call this operation to release a subscription Message Queue for Apache Kafka instance.
         
         @param request: ReleaseInstanceRequest
         @return: ReleaseInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.release_instance_with_options(request, runtime)
 
     async def release_instance_async(
         self,
         request: alikafka_20190916_models.ReleaseInstanceRequest,
     ) -> alikafka_20190916_models.ReleaseInstanceResponse:
         """
-        You cannot call this operation to release a subscription Message Queue for Apache Kafka instance.
+        @summary Releases a pay-as-you-go Message Queue for Apache Kafka instance.
+        
+        @description You cannot call this operation to release a subscription Message Queue for Apache Kafka instance.
         
         @param request: ReleaseInstanceRequest
         @return: ReleaseInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.release_instance_with_options_async(request, runtime)
 
     def reopen_instance_with_options(
         self,
         request: alikafka_20190916_models.ReopenInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ReopenInstanceResponse:
         """
-        You can call this operation only if your instance is in the Stopped state.
+        @summary Enables an ApsaraMQ for Kafka instance.
+        
+        @description You can call this operation only if your instance is in the Stopped state.
         
         @param request: ReopenInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ReopenInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2948,15 +4170,17 @@
 
     async def reopen_instance_with_options_async(
         self,
         request: alikafka_20190916_models.ReopenInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ReopenInstanceResponse:
         """
-        You can call this operation only if your instance is in the Stopped state.
+        @summary Enables an ApsaraMQ for Kafka instance.
+        
+        @description You can call this operation only if your instance is in the Stopped state.
         
         @param request: ReopenInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ReopenInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2984,42 +4208,48 @@
         )
 
     def reopen_instance(
         self,
         request: alikafka_20190916_models.ReopenInstanceRequest,
     ) -> alikafka_20190916_models.ReopenInstanceResponse:
         """
-        You can call this operation only if your instance is in the Stopped state.
+        @summary Enables an ApsaraMQ for Kafka instance.
+        
+        @description You can call this operation only if your instance is in the Stopped state.
         
         @param request: ReopenInstanceRequest
         @return: ReopenInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.reopen_instance_with_options(request, runtime)
 
     async def reopen_instance_async(
         self,
         request: alikafka_20190916_models.ReopenInstanceRequest,
     ) -> alikafka_20190916_models.ReopenInstanceResponse:
         """
-        You can call this operation only if your instance is in the Stopped state.
+        @summary Enables an ApsaraMQ for Kafka instance.
+        
+        @description You can call this operation only if your instance is in the Stopped state.
         
         @param request: ReopenInstanceRequest
         @return: ReopenInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.reopen_instance_with_options_async(request, runtime)
 
     def start_instance_with_options(
         self,
         request: alikafka_20190916_models.StartInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.StartInstanceResponse:
         """
-        >  You can call this operation up to twice per second.
+        @summary Deploys an ApsaraMQ for Kafka instance. You must purchase and deploy an ApsaraMQ for Kafka instance before you can use the instance to send and receive messages.
+        
+        @description >  You can call this operation up to twice per second.
         
         @param request: StartInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3086,15 +4316,17 @@
 
     async def start_instance_with_options_async(
         self,
         request: alikafka_20190916_models.StartInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.StartInstanceResponse:
         """
-        >  You can call this operation up to twice per second.
+        @summary Deploys an ApsaraMQ for Kafka instance. You must purchase and deploy an ApsaraMQ for Kafka instance before you can use the instance to send and receive messages.
+        
+        @description >  You can call this operation up to twice per second.
         
         @param request: StartInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3160,42 +4392,48 @@
         )
 
     def start_instance(
         self,
         request: alikafka_20190916_models.StartInstanceRequest,
     ) -> alikafka_20190916_models.StartInstanceResponse:
         """
-        >  You can call this operation up to twice per second.
+        @summary Deploys an ApsaraMQ for Kafka instance. You must purchase and deploy an ApsaraMQ for Kafka instance before you can use the instance to send and receive messages.
+        
+        @description >  You can call this operation up to twice per second.
         
         @param request: StartInstanceRequest
         @return: StartInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.start_instance_with_options(request, runtime)
 
     async def start_instance_async(
         self,
         request: alikafka_20190916_models.StartInstanceRequest,
     ) -> alikafka_20190916_models.StartInstanceResponse:
         """
-        >  You can call this operation up to twice per second.
+        @summary Deploys an ApsaraMQ for Kafka instance. You must purchase and deploy an ApsaraMQ for Kafka instance before you can use the instance to send and receive messages.
+        
+        @description >  You can call this operation up to twice per second.
         
         @param request: StartInstanceRequest
         @return: StartInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.start_instance_with_options_async(request, runtime)
 
     def stop_instance_with_options(
         self,
         request: alikafka_20190916_models.StopInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.StopInstanceResponse:
         """
-        You cannot stop a subscription ApsaraMQ for Kafka instance. If you want to stop a subscription ApsaraMQ for Kafka instance, submit a ticket.
+        @summary Stops an ApsaraMQ for Kafka instance.
+        
+        @description You cannot stop a subscription ApsaraMQ for Kafka instance. If you want to stop a subscription ApsaraMQ for Kafka instance, submit a ticket.
         
         @param request: StopInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StopInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3224,15 +4462,17 @@
 
     async def stop_instance_with_options_async(
         self,
         request: alikafka_20190916_models.StopInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.StopInstanceResponse:
         """
-        You cannot stop a subscription ApsaraMQ for Kafka instance. If you want to stop a subscription ApsaraMQ for Kafka instance, submit a ticket.
+        @summary Stops an ApsaraMQ for Kafka instance.
+        
+        @description You cannot stop a subscription ApsaraMQ for Kafka instance. If you want to stop a subscription ApsaraMQ for Kafka instance, submit a ticket.
         
         @param request: StopInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StopInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3260,40 +4500,51 @@
         )
 
     def stop_instance(
         self,
         request: alikafka_20190916_models.StopInstanceRequest,
     ) -> alikafka_20190916_models.StopInstanceResponse:
         """
-        You cannot stop a subscription ApsaraMQ for Kafka instance. If you want to stop a subscription ApsaraMQ for Kafka instance, submit a ticket.
+        @summary Stops an ApsaraMQ for Kafka instance.
+        
+        @description You cannot stop a subscription ApsaraMQ for Kafka instance. If you want to stop a subscription ApsaraMQ for Kafka instance, submit a ticket.
         
         @param request: StopInstanceRequest
         @return: StopInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.stop_instance_with_options(request, runtime)
 
     async def stop_instance_async(
         self,
         request: alikafka_20190916_models.StopInstanceRequest,
     ) -> alikafka_20190916_models.StopInstanceResponse:
         """
-        You cannot stop a subscription ApsaraMQ for Kafka instance. If you want to stop a subscription ApsaraMQ for Kafka instance, submit a ticket.
+        @summary Stops an ApsaraMQ for Kafka instance.
+        
+        @description You cannot stop a subscription ApsaraMQ for Kafka instance. If you want to stop a subscription ApsaraMQ for Kafka instance, submit a ticket.
         
         @param request: StopInstanceRequest
         @return: StopInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.stop_instance_with_options_async(request, runtime)
 
     def tag_resources_with_options(
         self,
         request: alikafka_20190916_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.TagResourcesResponse:
+        """
+        @summary Attaches a tag to a resource.
+        
+        @param request: TagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_id):
@@ -3322,14 +4573,21 @@
         )
 
     async def tag_resources_with_options_async(
         self,
         request: alikafka_20190916_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.TagResourcesResponse:
+        """
+        @summary Attaches a tag to a resource.
+        
+        @param request: TagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_id):
@@ -3357,29 +4615,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def tag_resources(
         self,
         request: alikafka_20190916_models.TagResourcesRequest,
     ) -> alikafka_20190916_models.TagResourcesResponse:
+        """
+        @summary Attaches a tag to a resource.
+        
+        @param request: TagResourcesRequest
+        @return: TagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.tag_resources_with_options(request, runtime)
 
     async def tag_resources_async(
         self,
         request: alikafka_20190916_models.TagResourcesRequest,
     ) -> alikafka_20190916_models.TagResourcesResponse:
+        """
+        @summary Attaches a tag to a resource.
+        
+        @param request: TagResourcesRequest
+        @return: TagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.tag_resources_with_options_async(request, runtime)
 
     def untag_resources_with_options(
         self,
         request: alikafka_20190916_models.UntagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UntagResourcesResponse:
+        """
+        @summary Detaches tags from a specified resource.
+        
+        @param request: UntagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UntagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.all):
             query['All'] = request.all
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_id):
@@ -3408,14 +4685,21 @@
         )
 
     async def untag_resources_with_options_async(
         self,
         request: alikafka_20190916_models.UntagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UntagResourcesResponse:
+        """
+        @summary Detaches tags from a specified resource.
+        
+        @param request: UntagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UntagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.all):
             query['All'] = request.all
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_id):
@@ -3443,29 +4727,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def untag_resources(
         self,
         request: alikafka_20190916_models.UntagResourcesRequest,
     ) -> alikafka_20190916_models.UntagResourcesResponse:
+        """
+        @summary Detaches tags from a specified resource.
+        
+        @param request: UntagResourcesRequest
+        @return: UntagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.untag_resources_with_options(request, runtime)
 
     async def untag_resources_async(
         self,
         request: alikafka_20190916_models.UntagResourcesRequest,
     ) -> alikafka_20190916_models.UntagResourcesResponse:
+        """
+        @summary Detaches tags from a specified resource.
+        
+        @param request: UntagResourcesRequest
+        @return: UntagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.untag_resources_with_options_async(request, runtime)
 
     def update_allowed_ip_with_options(
         self,
         request: alikafka_20190916_models.UpdateAllowedIpRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UpdateAllowedIpResponse:
+        """
+        @summary Updates the IP address whitelist of an ApsaraMQ for Kafka instance. Only IP addresses and ports that are configured in the IP address whitelist of an instance can access the instance.
+        
+        @param request: UpdateAllowedIpRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAllowedIpResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.allowed_list_ip):
             query['AllowedListIp'] = request.allowed_list_ip
         if not UtilClient.is_unset(request.allowed_list_type):
             query['AllowedListType'] = request.allowed_list_type
         if not UtilClient.is_unset(request.description):
@@ -3498,14 +4801,21 @@
         )
 
     async def update_allowed_ip_with_options_async(
         self,
         request: alikafka_20190916_models.UpdateAllowedIpRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UpdateAllowedIpResponse:
+        """
+        @summary Updates the IP address whitelist of an ApsaraMQ for Kafka instance. Only IP addresses and ports that are configured in the IP address whitelist of an instance can access the instance.
+        
+        @param request: UpdateAllowedIpRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAllowedIpResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.allowed_list_ip):
             query['AllowedListIp'] = request.allowed_list_ip
         if not UtilClient.is_unset(request.allowed_list_type):
             query['AllowedListType'] = request.allowed_list_type
         if not UtilClient.is_unset(request.description):
@@ -3537,34 +4847,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_allowed_ip(
         self,
         request: alikafka_20190916_models.UpdateAllowedIpRequest,
     ) -> alikafka_20190916_models.UpdateAllowedIpResponse:
+        """
+        @summary Updates the IP address whitelist of an ApsaraMQ for Kafka instance. Only IP addresses and ports that are configured in the IP address whitelist of an instance can access the instance.
+        
+        @param request: UpdateAllowedIpRequest
+        @return: UpdateAllowedIpResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_allowed_ip_with_options(request, runtime)
 
     async def update_allowed_ip_async(
         self,
         request: alikafka_20190916_models.UpdateAllowedIpRequest,
     ) -> alikafka_20190916_models.UpdateAllowedIpResponse:
+        """
+        @summary Updates the IP address whitelist of an ApsaraMQ for Kafka instance. Only IP addresses and ports that are configured in the IP address whitelist of an instance can access the instance.
+        
+        @param request: UpdateAllowedIpRequest
+        @return: UpdateAllowedIpResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_allowed_ip_with_options_async(request, runtime)
 
     def update_consumer_offset_with_options(
         self,
         tmp_req: alikafka_20190916_models.UpdateConsumerOffsetRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UpdateConsumerOffsetResponse:
         """
-        You can call this operation to reset the consumer offset of a specific consumer group. You can use the timestamp or offset parameter to reset the consumer offset of a consumer group. You can implement the following features by configuring a combination of different parameters:
-        *   Reset the consumer offsets of one or all subscribed topics of a consumer group to the latest offset. This way, you can consume messages in the topics from the latest offset.
-        *   Reset the consumer offsets of one or all subscribed topics of a consumer group to a specific point in time. This way, you can consume messages in the topics from the specified point in time.
-        *   Reset the consumer offset of one subscribed topic of a consumer group to a specific offset in a specific partition. This way, you can consume messages from the specified offset in the specified partition.
+        @summary Resets the consumer offsets of the subscribed topics of a consumer group.
+        
+        @description You can call this operation to reset the consumer offset of a specific consumer group. You can use the timestamp or offset parameter to reset the consumer offset of a consumer group. You can implement the following features by configuring a combination of different parameters:
+        Reset the consumer offsets of one or all subscribed topics of a consumer group to the latest offset. This way, you can consume messages in the topics from the latest offset.
+        Reset the consumer offsets of one or all subscribed topics of a consumer group to a specific point in time. This way, you can consume messages in the topics from the specified point in time.
+        Reset the consumer offset of one subscribed topic of a consumer group to a specific offset in a specific partition. This way, you can consume messages from the specified offset in the specified partition.
         
         @param tmp_req: UpdateConsumerOffsetRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateConsumerOffsetResponse
         """
         UtilClient.validate_model(tmp_req)
         request = alikafka_20190916_models.UpdateConsumerOffsetShrinkRequest()
@@ -3607,18 +4931,20 @@
 
     async def update_consumer_offset_with_options_async(
         self,
         tmp_req: alikafka_20190916_models.UpdateConsumerOffsetRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UpdateConsumerOffsetResponse:
         """
-        You can call this operation to reset the consumer offset of a specific consumer group. You can use the timestamp or offset parameter to reset the consumer offset of a consumer group. You can implement the following features by configuring a combination of different parameters:
-        *   Reset the consumer offsets of one or all subscribed topics of a consumer group to the latest offset. This way, you can consume messages in the topics from the latest offset.
-        *   Reset the consumer offsets of one or all subscribed topics of a consumer group to a specific point in time. This way, you can consume messages in the topics from the specified point in time.
-        *   Reset the consumer offset of one subscribed topic of a consumer group to a specific offset in a specific partition. This way, you can consume messages from the specified offset in the specified partition.
+        @summary Resets the consumer offsets of the subscribed topics of a consumer group.
+        
+        @description You can call this operation to reset the consumer offset of a specific consumer group. You can use the timestamp or offset parameter to reset the consumer offset of a consumer group. You can implement the following features by configuring a combination of different parameters:
+        Reset the consumer offsets of one or all subscribed topics of a consumer group to the latest offset. This way, you can consume messages in the topics from the latest offset.
+        Reset the consumer offsets of one or all subscribed topics of a consumer group to a specific point in time. This way, you can consume messages in the topics from the specified point in time.
+        Reset the consumer offset of one subscribed topic of a consumer group to a specific offset in a specific partition. This way, you can consume messages from the specified offset in the specified partition.
         
         @param tmp_req: UpdateConsumerOffsetRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateConsumerOffsetResponse
         """
         UtilClient.validate_model(tmp_req)
         request = alikafka_20190916_models.UpdateConsumerOffsetShrinkRequest()
@@ -3660,52 +4986,58 @@
         )
 
     def update_consumer_offset(
         self,
         request: alikafka_20190916_models.UpdateConsumerOffsetRequest,
     ) -> alikafka_20190916_models.UpdateConsumerOffsetResponse:
         """
-        You can call this operation to reset the consumer offset of a specific consumer group. You can use the timestamp or offset parameter to reset the consumer offset of a consumer group. You can implement the following features by configuring a combination of different parameters:
-        *   Reset the consumer offsets of one or all subscribed topics of a consumer group to the latest offset. This way, you can consume messages in the topics from the latest offset.
-        *   Reset the consumer offsets of one or all subscribed topics of a consumer group to a specific point in time. This way, you can consume messages in the topics from the specified point in time.
-        *   Reset the consumer offset of one subscribed topic of a consumer group to a specific offset in a specific partition. This way, you can consume messages from the specified offset in the specified partition.
+        @summary Resets the consumer offsets of the subscribed topics of a consumer group.
+        
+        @description You can call this operation to reset the consumer offset of a specific consumer group. You can use the timestamp or offset parameter to reset the consumer offset of a consumer group. You can implement the following features by configuring a combination of different parameters:
+        Reset the consumer offsets of one or all subscribed topics of a consumer group to the latest offset. This way, you can consume messages in the topics from the latest offset.
+        Reset the consumer offsets of one or all subscribed topics of a consumer group to a specific point in time. This way, you can consume messages in the topics from the specified point in time.
+        Reset the consumer offset of one subscribed topic of a consumer group to a specific offset in a specific partition. This way, you can consume messages from the specified offset in the specified partition.
         
         @param request: UpdateConsumerOffsetRequest
         @return: UpdateConsumerOffsetResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_consumer_offset_with_options(request, runtime)
 
     async def update_consumer_offset_async(
         self,
         request: alikafka_20190916_models.UpdateConsumerOffsetRequest,
     ) -> alikafka_20190916_models.UpdateConsumerOffsetResponse:
         """
-        You can call this operation to reset the consumer offset of a specific consumer group. You can use the timestamp or offset parameter to reset the consumer offset of a consumer group. You can implement the following features by configuring a combination of different parameters:
-        *   Reset the consumer offsets of one or all subscribed topics of a consumer group to the latest offset. This way, you can consume messages in the topics from the latest offset.
-        *   Reset the consumer offsets of one or all subscribed topics of a consumer group to a specific point in time. This way, you can consume messages in the topics from the specified point in time.
-        *   Reset the consumer offset of one subscribed topic of a consumer group to a specific offset in a specific partition. This way, you can consume messages from the specified offset in the specified partition.
+        @summary Resets the consumer offsets of the subscribed topics of a consumer group.
+        
+        @description You can call this operation to reset the consumer offset of a specific consumer group. You can use the timestamp or offset parameter to reset the consumer offset of a consumer group. You can implement the following features by configuring a combination of different parameters:
+        Reset the consumer offsets of one or all subscribed topics of a consumer group to the latest offset. This way, you can consume messages in the topics from the latest offset.
+        Reset the consumer offsets of one or all subscribed topics of a consumer group to a specific point in time. This way, you can consume messages in the topics from the specified point in time.
+        Reset the consumer offset of one subscribed topic of a consumer group to a specific offset in a specific partition. This way, you can consume messages from the specified offset in the specified partition.
         
         @param request: UpdateConsumerOffsetRequest
         @return: UpdateConsumerOffsetResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_consumer_offset_with_options_async(request, runtime)
 
     def update_instance_config_with_options(
         self,
         request: alikafka_20190916_models.UpdateInstanceConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UpdateInstanceConfigResponse:
         """
-        ## *Permissions**\
-        If a RAM user wants to call the **UpdateInstanceConfig** operation, the RAM user must be granted the required permissions. For more information about how to grant permissions, see [RAM policies](~~185815~~).
+        @summary Modifies the configurations of an ApsaraMQ for Kafka instance. ApsaraMQ for Kafka allows you to modify the configurations of an instance, including the access control list (ACL) feature, the Secure Sockets Layer (SSL) feature, the message retention period, and the maximum message size.
+        
+        @description ## *Permissions**\
+        If a RAM user wants to call the *UpdateInstanceConfig** operation, the RAM user must be granted the required permissions. For more information about how to grant permissions, see [RAM policies](https://help.aliyun.com/document_detail/185815.html).
         |API|Action|Resource|
         |---|---|---|
-        |UpdateInstanceConfig|alikafka: UpdateInstance|acs:alikafka:*:*:{instanceId}|
+        |UpdateInstanceConfig|alikafka: UpdateInstance|acs:alikafka::*:{instanceId}|
         
         @param request: UpdateInstanceConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateInstanceConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3736,19 +5068,21 @@
 
     async def update_instance_config_with_options_async(
         self,
         request: alikafka_20190916_models.UpdateInstanceConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UpdateInstanceConfigResponse:
         """
-        ## *Permissions**\
-        If a RAM user wants to call the **UpdateInstanceConfig** operation, the RAM user must be granted the required permissions. For more information about how to grant permissions, see [RAM policies](~~185815~~).
+        @summary Modifies the configurations of an ApsaraMQ for Kafka instance. ApsaraMQ for Kafka allows you to modify the configurations of an instance, including the access control list (ACL) feature, the Secure Sockets Layer (SSL) feature, the message retention period, and the maximum message size.
+        
+        @description ## *Permissions**\
+        If a RAM user wants to call the *UpdateInstanceConfig** operation, the RAM user must be granted the required permissions. For more information about how to grant permissions, see [RAM policies](https://help.aliyun.com/document_detail/185815.html).
         |API|Action|Resource|
         |---|---|---|
-        |UpdateInstanceConfig|alikafka: UpdateInstance|acs:alikafka:*:*:{instanceId}|
+        |UpdateInstanceConfig|alikafka: UpdateInstance|acs:alikafka::*:{instanceId}|
         
         @param request: UpdateInstanceConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateInstanceConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3778,48 +5112,59 @@
         )
 
     def update_instance_config(
         self,
         request: alikafka_20190916_models.UpdateInstanceConfigRequest,
     ) -> alikafka_20190916_models.UpdateInstanceConfigResponse:
         """
-        ## *Permissions**\
-        If a RAM user wants to call the **UpdateInstanceConfig** operation, the RAM user must be granted the required permissions. For more information about how to grant permissions, see [RAM policies](~~185815~~).
+        @summary Modifies the configurations of an ApsaraMQ for Kafka instance. ApsaraMQ for Kafka allows you to modify the configurations of an instance, including the access control list (ACL) feature, the Secure Sockets Layer (SSL) feature, the message retention period, and the maximum message size.
+        
+        @description ## *Permissions**\
+        If a RAM user wants to call the *UpdateInstanceConfig** operation, the RAM user must be granted the required permissions. For more information about how to grant permissions, see [RAM policies](https://help.aliyun.com/document_detail/185815.html).
         |API|Action|Resource|
         |---|---|---|
-        |UpdateInstanceConfig|alikafka: UpdateInstance|acs:alikafka:*:*:{instanceId}|
+        |UpdateInstanceConfig|alikafka: UpdateInstance|acs:alikafka::*:{instanceId}|
         
         @param request: UpdateInstanceConfigRequest
         @return: UpdateInstanceConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_instance_config_with_options(request, runtime)
 
     async def update_instance_config_async(
         self,
         request: alikafka_20190916_models.UpdateInstanceConfigRequest,
     ) -> alikafka_20190916_models.UpdateInstanceConfigResponse:
         """
-        ## *Permissions**\
-        If a RAM user wants to call the **UpdateInstanceConfig** operation, the RAM user must be granted the required permissions. For more information about how to grant permissions, see [RAM policies](~~185815~~).
+        @summary Modifies the configurations of an ApsaraMQ for Kafka instance. ApsaraMQ for Kafka allows you to modify the configurations of an instance, including the access control list (ACL) feature, the Secure Sockets Layer (SSL) feature, the message retention period, and the maximum message size.
+        
+        @description ## *Permissions**\
+        If a RAM user wants to call the *UpdateInstanceConfig** operation, the RAM user must be granted the required permissions. For more information about how to grant permissions, see [RAM policies](https://help.aliyun.com/document_detail/185815.html).
         |API|Action|Resource|
         |---|---|---|
-        |UpdateInstanceConfig|alikafka: UpdateInstance|acs:alikafka:*:*:{instanceId}|
+        |UpdateInstanceConfig|alikafka: UpdateInstance|acs:alikafka::*:{instanceId}|
         
         @param request: UpdateInstanceConfigRequest
         @return: UpdateInstanceConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_instance_config_with_options_async(request, runtime)
 
     def update_topic_config_with_options(
         self,
         request: alikafka_20190916_models.UpdateTopicConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UpdateTopicConfigResponse:
+        """
+        @summary Modifies the configurations of a topic. After you create a topic, you can modify the message retention period and maximum message size of the topic.
+        
+        @param request: UpdateTopicConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateTopicConfigResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config):
             query['Config'] = request.config
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -3848,14 +5193,21 @@
         )
 
     async def update_topic_config_with_options_async(
         self,
         request: alikafka_20190916_models.UpdateTopicConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UpdateTopicConfigResponse:
+        """
+        @summary Modifies the configurations of a topic. After you create a topic, you can modify the message retention period and maximum message size of the topic.
+        
+        @param request: UpdateTopicConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateTopicConfigResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config):
             query['Config'] = request.config
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -3883,36 +5235,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_topic_config(
         self,
         request: alikafka_20190916_models.UpdateTopicConfigRequest,
     ) -> alikafka_20190916_models.UpdateTopicConfigResponse:
+        """
+        @summary Modifies the configurations of a topic. After you create a topic, you can modify the message retention period and maximum message size of the topic.
+        
+        @param request: UpdateTopicConfigRequest
+        @return: UpdateTopicConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_topic_config_with_options(request, runtime)
 
     async def update_topic_config_async(
         self,
         request: alikafka_20190916_models.UpdateTopicConfigRequest,
     ) -> alikafka_20190916_models.UpdateTopicConfigResponse:
+        """
+        @summary Modifies the configurations of a topic. After you create a topic, you can modify the message retention period and maximum message size of the topic.
+        
+        @param request: UpdateTopicConfigRequest
+        @return: UpdateTopicConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_topic_config_with_options_async(request, runtime)
 
     def upgrade_instance_version_with_options(
         self,
         request: alikafka_20190916_models.UpgradeInstanceVersionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UpgradeInstanceVersionResponse:
         """
-        ## *Permissions**\
-        A RAM user must be granted the required permissions before the RAM user calls the **UpgradeInstanceVersion** operation. For information about how to grant permissions, see [RAM policies](~~185815~~).
+        @summary Updates the version of an instance.
+        
+        @description ## *Permissions**\
+        A RAM user must be granted the required permissions before the RAM user calls the *UpgradeInstanceVersion** operation. For information about how to grant permissions, see [RAM policies](https://help.aliyun.com/document_detail/185815.html).
         |API|Action|Resource|
         |---|---|---|
-        |UpgradeInstanceVersion|UpdateInstance|acs:alikafka:*:*:{instanceId}|
-        ## **QPS limits**\
+        |UpgradeInstanceVersion|UpdateInstance|acs:alikafka::*:{instanceId}|
+        ## *QPS limits**\
         You can send a maximum of two queries per second (QPS).
         
         @param request: UpgradeInstanceVersionRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpgradeInstanceVersionResponse
         """
         UtilClient.validate_model(request)
@@ -3944,20 +5310,22 @@
 
     async def upgrade_instance_version_with_options_async(
         self,
         request: alikafka_20190916_models.UpgradeInstanceVersionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UpgradeInstanceVersionResponse:
         """
-        ## *Permissions**\
-        A RAM user must be granted the required permissions before the RAM user calls the **UpgradeInstanceVersion** operation. For information about how to grant permissions, see [RAM policies](~~185815~~).
+        @summary Updates the version of an instance.
+        
+        @description ## *Permissions**\
+        A RAM user must be granted the required permissions before the RAM user calls the *UpgradeInstanceVersion** operation. For information about how to grant permissions, see [RAM policies](https://help.aliyun.com/document_detail/185815.html).
         |API|Action|Resource|
         |---|---|---|
-        |UpgradeInstanceVersion|UpdateInstance|acs:alikafka:*:*:{instanceId}|
-        ## **QPS limits**\
+        |UpgradeInstanceVersion|UpdateInstance|acs:alikafka::*:{instanceId}|
+        ## *QPS limits**\
         You can send a maximum of two queries per second (QPS).
         
         @param request: UpgradeInstanceVersionRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpgradeInstanceVersionResponse
         """
         UtilClient.validate_model(request)
@@ -3988,54 +5356,60 @@
         )
 
     def upgrade_instance_version(
         self,
         request: alikafka_20190916_models.UpgradeInstanceVersionRequest,
     ) -> alikafka_20190916_models.UpgradeInstanceVersionResponse:
         """
-        ## *Permissions**\
-        A RAM user must be granted the required permissions before the RAM user calls the **UpgradeInstanceVersion** operation. For information about how to grant permissions, see [RAM policies](~~185815~~).
+        @summary Updates the version of an instance.
+        
+        @description ## *Permissions**\
+        A RAM user must be granted the required permissions before the RAM user calls the *UpgradeInstanceVersion** operation. For information about how to grant permissions, see [RAM policies](https://help.aliyun.com/document_detail/185815.html).
         |API|Action|Resource|
         |---|---|---|
-        |UpgradeInstanceVersion|UpdateInstance|acs:alikafka:*:*:{instanceId}|
-        ## **QPS limits**\
+        |UpgradeInstanceVersion|UpdateInstance|acs:alikafka::*:{instanceId}|
+        ## *QPS limits**\
         You can send a maximum of two queries per second (QPS).
         
         @param request: UpgradeInstanceVersionRequest
         @return: UpgradeInstanceVersionResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.upgrade_instance_version_with_options(request, runtime)
 
     async def upgrade_instance_version_async(
         self,
         request: alikafka_20190916_models.UpgradeInstanceVersionRequest,
     ) -> alikafka_20190916_models.UpgradeInstanceVersionResponse:
         """
-        ## *Permissions**\
-        A RAM user must be granted the required permissions before the RAM user calls the **UpgradeInstanceVersion** operation. For information about how to grant permissions, see [RAM policies](~~185815~~).
+        @summary Updates the version of an instance.
+        
+        @description ## *Permissions**\
+        A RAM user must be granted the required permissions before the RAM user calls the *UpgradeInstanceVersion** operation. For information about how to grant permissions, see [RAM policies](https://help.aliyun.com/document_detail/185815.html).
         |API|Action|Resource|
         |---|---|---|
-        |UpgradeInstanceVersion|UpdateInstance|acs:alikafka:*:*:{instanceId}|
-        ## **QPS limits**\
+        |UpgradeInstanceVersion|UpdateInstance|acs:alikafka::*:{instanceId}|
+        ## *QPS limits**\
         You can send a maximum of two queries per second (QPS).
         
         @param request: UpgradeInstanceVersionRequest
         @return: UpgradeInstanceVersionResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.upgrade_instance_version_with_options_async(request, runtime)
 
     def upgrade_post_pay_order_with_options(
         self,
         tmp_req: alikafka_20190916_models.UpgradePostPayOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UpgradePostPayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](~~84737~~).
+        @summary Upgrades a pay-as-you-go ApsaraMQ for Kafka instance.
+        
+        @description Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         
         @param tmp_req: UpgradePostPayOrderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpgradePostPayOrderResponse
         """
         UtilClient.validate_model(tmp_req)
         request = alikafka_20190916_models.UpgradePostPayOrderShrinkRequest()
@@ -4086,15 +5460,17 @@
 
     async def upgrade_post_pay_order_with_options_async(
         self,
         tmp_req: alikafka_20190916_models.UpgradePostPayOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UpgradePostPayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](~~84737~~).
+        @summary Upgrades a pay-as-you-go ApsaraMQ for Kafka instance.
+        
+        @description Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         
         @param tmp_req: UpgradePostPayOrderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpgradePostPayOrderResponse
         """
         UtilClient.validate_model(tmp_req)
         request = alikafka_20190916_models.UpgradePostPayOrderShrinkRequest()
@@ -4144,42 +5520,48 @@
         )
 
     def upgrade_post_pay_order(
         self,
         request: alikafka_20190916_models.UpgradePostPayOrderRequest,
     ) -> alikafka_20190916_models.UpgradePostPayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](~~84737~~).
+        @summary Upgrades a pay-as-you-go ApsaraMQ for Kafka instance.
+        
+        @description Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         
         @param request: UpgradePostPayOrderRequest
         @return: UpgradePostPayOrderResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.upgrade_post_pay_order_with_options(request, runtime)
 
     async def upgrade_post_pay_order_async(
         self,
         request: alikafka_20190916_models.UpgradePostPayOrderRequest,
     ) -> alikafka_20190916_models.UpgradePostPayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](~~84737~~).
+        @summary Upgrades a pay-as-you-go ApsaraMQ for Kafka instance.
+        
+        @description Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         
         @param request: UpgradePostPayOrderRequest
         @return: UpgradePostPayOrderResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.upgrade_post_pay_order_with_options_async(request, runtime)
 
     def upgrade_pre_pay_order_with_options(
         self,
         tmp_req: alikafka_20190916_models.UpgradePrePayOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UpgradePrePayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing method and pricing of subscription Message Queue for Apache Kafka instances. For more information, see [Billing overview](~~84737~~).
+        @summary Upgrades a Message Queue for Apache Kafka instance that uses the subscription billing method.
+        
+        @description Before you call this operation, make sure that you understand the billing method and pricing of subscription Message Queue for Apache Kafka instances. For more information, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         
         @param tmp_req: UpgradePrePayOrderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpgradePrePayOrderResponse
         """
         UtilClient.validate_model(tmp_req)
         request = alikafka_20190916_models.UpgradePrePayOrderShrinkRequest()
@@ -4232,15 +5614,17 @@
 
     async def upgrade_pre_pay_order_with_options_async(
         self,
         tmp_req: alikafka_20190916_models.UpgradePrePayOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.UpgradePrePayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing method and pricing of subscription Message Queue for Apache Kafka instances. For more information, see [Billing overview](~~84737~~).
+        @summary Upgrades a Message Queue for Apache Kafka instance that uses the subscription billing method.
+        
+        @description Before you call this operation, make sure that you understand the billing method and pricing of subscription Message Queue for Apache Kafka instances. For more information, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         
         @param tmp_req: UpgradePrePayOrderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpgradePrePayOrderResponse
         """
         UtilClient.validate_model(tmp_req)
         request = alikafka_20190916_models.UpgradePrePayOrderShrinkRequest()
@@ -4292,27 +5676,31 @@
         )
 
     def upgrade_pre_pay_order(
         self,
         request: alikafka_20190916_models.UpgradePrePayOrderRequest,
     ) -> alikafka_20190916_models.UpgradePrePayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing method and pricing of subscription Message Queue for Apache Kafka instances. For more information, see [Billing overview](~~84737~~).
+        @summary Upgrades a Message Queue for Apache Kafka instance that uses the subscription billing method.
+        
+        @description Before you call this operation, make sure that you understand the billing method and pricing of subscription Message Queue for Apache Kafka instances. For more information, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         
         @param request: UpgradePrePayOrderRequest
         @return: UpgradePrePayOrderResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.upgrade_pre_pay_order_with_options(request, runtime)
 
     async def upgrade_pre_pay_order_async(
         self,
         request: alikafka_20190916_models.UpgradePrePayOrderRequest,
     ) -> alikafka_20190916_models.UpgradePrePayOrderResponse:
         """
-        Before you call this operation, make sure that you understand the billing method and pricing of subscription Message Queue for Apache Kafka instances. For more information, see [Billing overview](~~84737~~).
+        @summary Upgrades a Message Queue for Apache Kafka instance that uses the subscription billing method.
+        
+        @description Before you call this operation, make sure that you understand the billing method and pricing of subscription Message Queue for Apache Kafka instances. For more information, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         
         @param request: UpgradePrePayOrderRequest
         @return: UpgradePrePayOrderResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.upgrade_pre_pay_order_with_options_async(request, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916/models.py` & `alibabacloud_alikafka20190916-2.7.0/alibabacloud_alikafka20190916/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,21 +9,27 @@
         self,
         new_resource_group_id: str = None,
         region_id: str = None,
         resource_id: str = None,
     ):
         # The ID of the resource group to which you want to transfer the cloud resource.
         # 
-        # >  You can use resource groups to manage resources owned by your Alibaba Cloud account. Resource groups simplify the resource and permission management of your Alibaba Cloud account. For more information, see [What is resource management?](~~94475~~)
+        # >  You can use resource groups to manage resources owned by your Alibaba Cloud account. Resource groups simplify the resource and permission management of your Alibaba Cloud account. For more information, see [What is resource management?](https://help.aliyun.com/document_detail/94475.html)
+        # 
+        # This parameter is required.
         self.new_resource_group_id = new_resource_group_id
         # The region ID of the resource.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource to which you want to attach a tag. Only the ID of a Message Queue for Apache Kafka instance is supported.
         # 
         # For example, if the ID of the instance is alikafka_post-cn-v0h1fgs2xxxx, the resource ID is alikafka_post-cn-v0h1fgs2xxxx.
+        # 
+        # This parameter is required.
         self.resource_id = resource_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -157,16 +163,20 @@
         # The subscription duration. Unit: months. Valid values:
         # 
         # *   **1~12**\
         # *   **24**\
         # *   **36**\
         self.duration = duration
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -300,48 +310,89 @@
         acl_resource_pattern_type: str = None,
         acl_resource_type: str = None,
         host: str = None,
         instance_id: str = None,
         region_id: str = None,
         username: str = None,
     ):
-        # The operation type. Valid values:
+        # The type of the operation allowed by the access control list (ACL). Valid values:
         # 
-        # *   **Write**: data writes
-        # *   **Read**: data reads
-        # *   **Describe**: reads of transaction IDs****\
-        # *   **IdempotentWrite**: idempotent data writes to clusters****\
+        # *   **Write**\
+        # *   **Read**\
+        # *   **Describe**: reads of transactional IDs.
+        # *   **IdempotentWrite**: idempotent data writes to clusters.
+        # *   **IDEMPOTENT_WRITE**: idempotent data writes to clusters. This value is available only for ApsaraMQ for Kafka V3 instances.
+        # *   **DESCRIBE_CONFIGS**: queries of configurations. This value is available only for ApsaraMQ for Kafka V3 instances.
+        # 
+        # This parameter is required.
         self.acl_operation_type = acl_operation_type
+        # The types of operations allowed by the ACL. Separate multiple operation types with commas (,).
+        # 
+        # Valid values:
+        # 
+        # *   **Write**\
+        # *   **Read**\
+        # *   **Describe**: reads of transactional IDs.
+        # *   **IdempotentWrite**: idempotent data writes to clusters.
+        # *   **IDEMPOTENT_WRITE**: idempotent data writes to clusters. This value is available only for ApsaraMQ for Kafka V3 instances.
+        # *   **DESCRIBE_CONFIGS**: queries of configurations. This value is available only for ApsaraMQ for Kafka V3 instances.
+        # 
+        # >  This parameter is available only for ApsaraMQ for Kafka V3 serverless instances.
         self.acl_operation_types = acl_operation_types
+        # The authorization method. Valid values:
+        # 
+        # *   **DENY**\
+        # *   **ALLOW**\
+        # 
+        # >  This parameter is available only for ApsaraMQ for Kafka V3 serverless instances.
         self.acl_permission_type = acl_permission_type
         # The name or ID of the resource.
         # 
         # *   The value can be the name of a topic, consumer group, or cluster, or the ID of a transaction.
-        # *   You can use an asterisk (\*) to represent the names or IDs of all relevant resources.
+        # *   You can use an asterisk (\\*) to represent the names or IDs of all relevant resources.
+        # 
+        # This parameter is required.
         self.acl_resource_name = acl_resource_name
         # The matching mode. Valid values:
         # 
         # *   **LITERAL**: exact match
         # *   **PREFIXED**: prefix match
+        # 
+        # This parameter is required.
         self.acl_resource_pattern_type = acl_resource_pattern_type
         # The resource type. Valid values:
         # 
         # *   **Topic**\
         # *   **Group**\
         # *   **Cluster**\
-        # *   **TransactionalId**: transaction
+        # *   **TransactionalId**: transactional ID
+        # 
+        # This parameter is required.
         self.acl_resource_type = acl_resource_type
+        # The source IP address.
+        # 
+        # > 
+        # 
+        # *   You can specify only a specific IP address or use the asterisk (\\*) wildcard character to specify all IP addresses. CIDR blocks are not supported.
+        # 
+        # *   This parameter is available only for ApsaraMQ for Kafka V3 serverless instances.
         self.host = host
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The region ID.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The username.
         # 
-        # You can use an asterisk (\*) to represent all usernames.
+        # You can use an asterisk (\\*) to represent all usernames.
+        # 
+        # This parameter is required.
         self.username = username
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -492,14 +543,16 @@
         key: str = None,
         value: str = None,
     ):
         # The tag key.
         # 
         # *   You must specify this parameter.
         # *   The tag key can be up to 128 characters in length and cannot start with acs: or aliyun. It cannot contain `http://` or `https://`.
+        # 
+        # This parameter is required.
         self.key = key
         # The tag value.
         # 
         # *   You can leave this parameter empty.
         # *   The tag value can be up to 128 characters in length and cannot start with acs: or aliyun. It cannot contain `http://` or `https://`.
         self.value = value
 
@@ -534,21 +587,27 @@
         instance_id: str = None,
         region_id: str = None,
         remark: str = None,
         tag: List[CreateConsumerGroupRequestTag] = None,
     ):
         # The name of the consumer group.
         # 
-        # *   The value can contain only letters, digits, hyphens (-), and underscores (\_), and the value must contain at least one letter or digit.
+        # *   The value can contain only letters, digits, hyphens (-), and underscores (_), and the value must contain at least one letter or digit.
         # *   The value must be 3 to 128 characters in length. If the value that you specify contains more than 128 characters, the system automatically truncates the value to 128 characters.
         # *   After a consumer group is created, you cannot change the name of the consumer group.
+        # 
+        # This parameter is required.
         self.consumer_id = consumer_id
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The description of the consumer group.
         self.remark = remark
         # The tags.
         self.tag = tag
 
     def validate(self):
@@ -687,15 +746,21 @@
 
 class CreatePostPayOrderRequestServerlessConfig(TeaModel):
     def __init__(
         self,
         reserved_publish_capacity: int = None,
         reserved_subscribe_capacity: int = None,
     ):
+        # The reserved capacity for publishing messages. You can specify only an integer for this parameter. Minimum value: 60.
+        # 
+        # >  The actual maximum reserved capacity for publishing messages varies based on available resources in the region. The actual range displayed on the buy page shall prevail.
         self.reserved_publish_capacity = reserved_publish_capacity
+        # The reserved capacity for subscribing to messages. You can specify only an integer for this parameter. Minimum value: 20.
+        # 
+        # >  The actual maximum reserved capacity for subscribing to messages varies based on available resources in the region. The actual range displayed on the buy page shall prevail.
         self.reserved_subscribe_capacity = reserved_subscribe_capacity
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -725,14 +790,16 @@
         value: str = None,
     ):
         # The key of tag N.
         # 
         # *   Valid values of N: 1 to 20.
         # *   If this parameter is left empty, the keys of all tags are matched.
         # *   The tag key must be up to 128 characters in length. It cannot start with acs: or aliyun or contain [http:// or https://.](http://https://。)
+        # 
+        # This parameter is required.
         self.key = key
         # The value of tag N.
         # 
         # *   Valid values of N: 1 to 20.
         # *   If you do not specify a tag key, you cannot specify a tag value. If this parameter is not configured, all tag values are matched.
         # *   The tag value must be 1 to 128 characters in length. It cannot start with acs: or aliyun or contain [http:// or https://.](http://https://。)
         self.value = value
@@ -779,69 +846,99 @@
         tag: List[CreatePostPayOrderRequestTag] = None,
         topic_quota: int = None,
     ):
         # The deployment mode of the instance. Valid values:
         # 
         # *   **4**: deploys the instance that allows access from the Internet and a VPC.
         # *   **5**: deploys the instance that allows access only from a VPC.
+        # 
+        # This parameter is required.
         self.deploy_type = deploy_type
         # The disk size.
         # 
-        # For more information about the valid values, see [Billing](~~84737~~).
+        # For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
+        # 
+        # >  If you create a serverless ApsaraMQ for Kafka V3 instance, you do not need to configure this parameter.
         self.disk_size = disk_size
         # The disk type. Valid values:
         # 
         # *   **0**: ultra disk
         # *   **1**: standard SSD
+        # 
+        # >  If you create a serverless ApsaraMQ for Kafka V3 instance, you do not need to configure this parameter.
         self.disk_type = disk_type
-        # The Internet traffic for the instance.
+        # The maximum Internet traffic in the instance.
         # 
-        # *   This parameter is required if the **DeployType** parameter is set to **4**.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   If you set **DeployType** to **4**, you must configure this parameter.
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
+        # 
+        # >  If you create a serverless ApsaraMQ for Kafka V3 instance, you do not need to configure this parameter.
         self.eip_max = eip_max
-        # The maximum traffic for the instance. We recommend that you do not configure this parameter.
+        # The maximum traffic in the instance. We recommend that you do not configure this parameter.
+        # 
+        # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         # 
-        # *   You must specify at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # >  If you create a serverless ApsaraMQ for Kafka V3 instance, you do not need to configure this parameter.
         self.io_max = io_max
         # The traffic specification of the instance. We recommend that you configure this parameter.
         # 
-        # *   You must specify at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
+        # 
+        # >  If you create a serverless ApsaraMQ for Kafka V3 instance, you do not need to configure this parameter.
         self.io_max_spec = io_max_spec
+        # The billing method of the instance. Valid values:
+        # 
+        # *   1: the pay-as-you-go billing method for ApsaraMQ for Kafka V2 instances.
+        # *   3: the pay-as-you-go billing method for serverless ApsaraMQ for Kafka V3 instances.
         self.paid_type = paid_type
         # The number of partitions. We recommend that you configure this parameter.
         # 
-        # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
-        # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure one of PartitionNum and TopicQuota. We recommend that you configure only ParittionNum.
+        # *   If you configure PartitionNum and TopicQuota at the same time, the system verifies whether the price of the partitions equals the price of the topics based on the previous topic-based selling mode. If the price of the partitions does not equal the price of the topics, an error is returned. If the price of the partitions equals the price of the topics, the instance is purchased based on the partition number.
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
+        # 
+        # >  If you create a serverless ApsaraMQ for Kafka V3 instance, you do not need to configure this parameter.
         self.partition_num = partition_num
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         # 
         # If this parameter is left empty, the default resource group is used. You can view the resource group ID on the Resource Group page in the Resource Management console.
         self.resource_group_id = resource_group_id
+        # The parameters configured for the serverless ApsaraMQ for Kafka V3 instance. When you create a Serverless ApsaraMQ for Kafka V3 serverless instance, you must configure these parameters.
         self.serverless_config = serverless_config
-        # The edition of the instance. Valid values:
+        # The instance edition.
         # 
-        # *   **normal**: Standard Edition (High Write)
-        # *   **professional**: Professional Edition (High Write)
-        # *   **professionalForHighRead**: Professional Edition (High Read)
+        # Valid values if you set PaidType to 1:
+        # 
+        # *   normal: Standard Edition (High Write)
+        # *   professional: Professional Edition (High Write)
+        # *   professionalForHighRead: Professional Edition (High Read)
+        # 
+        # Valid values if you set PaidType to 3:
+        # 
+        # *   normal: Serverless Standard Edition
+        # *   professional: Serverless Professional Edition
         # 
-        # For more information about these instance editions, see [Billing](~~84737~~).
+        # For more information about the instance editions, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.spec_type = spec_type
         # The tags.
         self.tag = tag
         # The number of topics. We recommend that you do not configure this parameter.
         # 
-        # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
-        # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
-        # *   The default value of the TopicQuota parameter varies based on the value of the IoMaxSpec parameter. If the number of topics that you consume exceeds the default value, you are charged additional fees.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure one of PartitionNum and TopicQuota. We recommend that you configure only ParittionNum.
+        # *   If you configure PartitionNum and TopicQuota at the same time, the system verifies whether the price of the partitions equals the price of the topics based on the previous topic-based selling mode. If the price of the partitions does not equal the price of the topics, an error is returned. If the price of the partitions equals the price of the topics, the instance is purchased based on the partition number.
+        # *   The default value of TopicQuota varies based on the value of IoMaxSpec. If the number of topics that you consume exceeds the default value, you are charged additional fees.
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
+        # 
+        # >  If you create a serverless ApsaraMQ for Kafka V3 instance, you do not need to configure this parameter.
         self.topic_quota = topic_quota
 
     def validate(self):
         if self.serverless_config:
             self.serverless_config.validate()
         if self.tag:
             for k in self.tag:
@@ -930,14 +1027,16 @@
         value: str = None,
     ):
         # The key of tag N.
         # 
         # *   Valid values of N: 1 to 20.
         # *   If this parameter is left empty, the keys of all tags are matched.
         # *   The tag key must be up to 128 characters in length. It cannot start with acs: or aliyun or contain [http:// or https://.](http://https://。)
+        # 
+        # This parameter is required.
         self.key = key
         # The value of tag N.
         # 
         # *   Valid values of N: 1 to 20.
         # *   If you do not specify a tag key, you cannot specify a tag value. If this parameter is not configured, all tag values are matched.
         # *   The tag value must be 1 to 128 characters in length. It cannot start with acs: or aliyun or contain [http:// or https://.](http://https://。)
         self.value = value
@@ -984,69 +1083,99 @@
         tag: List[CreatePostPayOrderShrinkRequestTag] = None,
         topic_quota: int = None,
     ):
         # The deployment mode of the instance. Valid values:
         # 
         # *   **4**: deploys the instance that allows access from the Internet and a VPC.
         # *   **5**: deploys the instance that allows access only from a VPC.
+        # 
+        # This parameter is required.
         self.deploy_type = deploy_type
         # The disk size.
         # 
-        # For more information about the valid values, see [Billing](~~84737~~).
+        # For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
+        # 
+        # >  If you create a serverless ApsaraMQ for Kafka V3 instance, you do not need to configure this parameter.
         self.disk_size = disk_size
         # The disk type. Valid values:
         # 
         # *   **0**: ultra disk
         # *   **1**: standard SSD
+        # 
+        # >  If you create a serverless ApsaraMQ for Kafka V3 instance, you do not need to configure this parameter.
         self.disk_type = disk_type
-        # The Internet traffic for the instance.
+        # The maximum Internet traffic in the instance.
         # 
-        # *   This parameter is required if the **DeployType** parameter is set to **4**.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   If you set **DeployType** to **4**, you must configure this parameter.
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
+        # 
+        # >  If you create a serverless ApsaraMQ for Kafka V3 instance, you do not need to configure this parameter.
         self.eip_max = eip_max
-        # The maximum traffic for the instance. We recommend that you do not configure this parameter.
+        # The maximum traffic in the instance. We recommend that you do not configure this parameter.
         # 
-        # *   You must specify at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
+        # 
+        # >  If you create a serverless ApsaraMQ for Kafka V3 instance, you do not need to configure this parameter.
         self.io_max = io_max
         # The traffic specification of the instance. We recommend that you configure this parameter.
         # 
-        # *   You must specify at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
+        # 
+        # >  If you create a serverless ApsaraMQ for Kafka V3 instance, you do not need to configure this parameter.
         self.io_max_spec = io_max_spec
+        # The billing method of the instance. Valid values:
+        # 
+        # *   1: the pay-as-you-go billing method for ApsaraMQ for Kafka V2 instances.
+        # *   3: the pay-as-you-go billing method for serverless ApsaraMQ for Kafka V3 instances.
         self.paid_type = paid_type
         # The number of partitions. We recommend that you configure this parameter.
         # 
-        # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
-        # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure one of PartitionNum and TopicQuota. We recommend that you configure only ParittionNum.
+        # *   If you configure PartitionNum and TopicQuota at the same time, the system verifies whether the price of the partitions equals the price of the topics based on the previous topic-based selling mode. If the price of the partitions does not equal the price of the topics, an error is returned. If the price of the partitions equals the price of the topics, the instance is purchased based on the partition number.
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
+        # 
+        # >  If you create a serverless ApsaraMQ for Kafka V3 instance, you do not need to configure this parameter.
         self.partition_num = partition_num
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         # 
         # If this parameter is left empty, the default resource group is used. You can view the resource group ID on the Resource Group page in the Resource Management console.
         self.resource_group_id = resource_group_id
+        # The parameters configured for the serverless ApsaraMQ for Kafka V3 instance. When you create a Serverless ApsaraMQ for Kafka V3 serverless instance, you must configure these parameters.
         self.serverless_config_shrink = serverless_config_shrink
-        # The edition of the instance. Valid values:
+        # The instance edition.
         # 
-        # *   **normal**: Standard Edition (High Write)
-        # *   **professional**: Professional Edition (High Write)
-        # *   **professionalForHighRead**: Professional Edition (High Read)
+        # Valid values if you set PaidType to 1:
+        # 
+        # *   normal: Standard Edition (High Write)
+        # *   professional: Professional Edition (High Write)
+        # *   professionalForHighRead: Professional Edition (High Read)
+        # 
+        # Valid values if you set PaidType to 3:
+        # 
+        # *   normal: Serverless Standard Edition
+        # *   professional: Serverless Professional Edition
         # 
-        # For more information about these instance editions, see [Billing](~~84737~~).
+        # For more information about the instance editions, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.spec_type = spec_type
         # The tags.
         self.tag = tag
         # The number of topics. We recommend that you do not configure this parameter.
         # 
-        # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
-        # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
-        # *   The default value of the TopicQuota parameter varies based on the value of the IoMaxSpec parameter. If the number of topics that you consume exceeds the default value, you are charged additional fees.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure one of PartitionNum and TopicQuota. We recommend that you configure only ParittionNum.
+        # *   If you configure PartitionNum and TopicQuota at the same time, the system verifies whether the price of the partitions equals the price of the topics based on the previous topic-based selling mode. If the price of the partitions does not equal the price of the topics, an error is returned. If the price of the partitions equals the price of the topics, the instance is purchased based on the partition number.
+        # *   The default value of TopicQuota varies based on the value of IoMaxSpec. If the number of topics that you consume exceeds the default value, you are charged additional fees.
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
+        # 
+        # >  If you create a serverless ApsaraMQ for Kafka V3 instance, you do not need to configure this parameter.
         self.topic_quota = topic_quota
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -1240,31 +1369,49 @@
         ksql_storage: int = None,
         schema_registry_cu: int = None,
         schema_registry_replica: int = None,
         zoo_keeper_cu: int = None,
         zoo_keeper_replica: int = None,
         zoo_keeper_storage: int = None,
     ):
+        # The number of CPU cores of Connect.
         self.connect_cu = connect_cu
+        # The number of replicas of Connect.
         self.connect_replica = connect_replica
+        # The number of CPU cores of Control Center.
         self.control_center_cu = control_center_cu
+        # The number of replicas of Control Center.
         self.control_center_replica = control_center_replica
+        # The disk capacity of Control Center. Unit: GB
         self.control_center_storage = control_center_storage
+        # The number of CPU cores of the Kafka broker.
         self.kafka_cu = kafka_cu
+        # The number of replicas of the Kafka broker.
         self.kafka_replica = kafka_replica
+        # The number of CPU cores of Kafka Rest Proxy.
         self.kafka_rest_proxy_cu = kafka_rest_proxy_cu
+        # The number of replicas of Kafka Rest Proxy.
         self.kafka_rest_proxy_replica = kafka_rest_proxy_replica
+        # The disk capacity of the Kafka broker. Unit: GB
         self.kafka_storage = kafka_storage
+        # The number of CPU cores of ksqIDB.
         self.ksql_cu = ksql_cu
+        # The number of replicas of ksqlDB.
         self.ksql_replica = ksql_replica
+        # The disk capacity of ksqlDB. Unit: GB
         self.ksql_storage = ksql_storage
+        # The number of CPU cores of Schema Registry.
         self.schema_registry_cu = schema_registry_cu
+        # The number of replicas of Schema Registry.
         self.schema_registry_replica = schema_registry_replica
+        # The number of CPU cores of ZooKeeper.
         self.zoo_keeper_cu = zoo_keeper_cu
+        # The number of replicas of ZooKeeper.
         self.zoo_keeper_replica = zoo_keeper_replica
+        # The disk capacity of ZooKeeper. Unit: GB
         self.zoo_keeper_storage = zoo_keeper_storage
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1358,14 +1505,16 @@
         value: str = None,
     ):
         # The key of tag N.
         # 
         # *   Valid values of N: 1 to 20.
         # *   If this parameter is left empty, the keys of all tags are matched.
         # *   The tag key can be up to 128 characters in length and cannot start with acs: or aliyun or contain [http:// or https://.](http://https://。)
+        # 
+        # This parameter is required.
         self.key = key
         # The value of tag N.
         # 
         # *   Valid values of N: 1 to 20.
         # *   This parameter can be left empty.
         # *   The tag value can be 1 to 128 characters in length and cannot start with acs: or aliyun or contain [http:// or https://.](http://https://。)
         self.value = value
@@ -1409,74 +1558,84 @@
         partition_num: int = None,
         region_id: str = None,
         resource_group_id: str = None,
         spec_type: str = None,
         tag: List[CreatePrePayOrderRequestTag] = None,
         topic_quota: int = None,
     ):
+        # The configurations of ApsaraMQ for Confluent components.
         self.confluent_config = confluent_config
         # The deployment mode of the instance. Valid values:
         # 
         # *   **4**: deploys the instance that allows access from the Internet and a VPC.
         # *   **5**: deploys the instance that allows access only from a VPC.
         self.deploy_type = deploy_type
         # The disk size. Unit: GB.
         # 
-        # For more information about the valid values, see [Billing](~~84737~~).
+        # For more information about the valid values, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.disk_size = disk_size
         # The disk type. Valid values:
         # 
         # *   **0**: ultra disk
         # *   **1**: standard SSD
         self.disk_type = disk_type
+        # The subscription duration. Unit: months. Default value: 1. Valid values:
+        # 
+        # *   **1 to 12**\
         self.duration = duration
         # The Internet traffic for the instance.
         # 
         # *   This parameter is required if the **DeployType** parameter is set to **4**.
-        # *   For more information about the valid values, see [Pay-as-you-go](~~72142~~).
+        # *   For more information about the valid values, see [Pay-as-you-go](https://help.aliyun.com/document_detail/72142.html).
         self.eip_max = eip_max
         # The maximum traffic for the instance. We recommend that you do not configure this parameter.
         # 
         # *   You must configure at least one of the **IoMax** and **IoMaxSpec** parameters. If both parameters are configured, the value of the **IoMaxSpec** parameter takes effect. We recommend that you configure only the **IoMaxSpec** parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   For more information about the valid values, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.io_max = io_max
         # The traffic specification of the instance. We recommend that you configure this parameter.
         # 
         # *   You must configure at least one of the **IoMax** and **IoMaxSpec** parameters. If both parameters are configured, the value of the **IoMaxSpec** parameter takes effect. We recommend that you configure only the **IoMaxSpec** parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   For more information about the valid values, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.io_max_spec = io_max_spec
+        # The billing method of the instance. Valid values:
+        # 
+        # *   **0**: the subscription billing method
+        # *   **4**: the subscription billing method for ApsaraMQ for Confluent instances
         self.paid_type = paid_type
         # The number of partitions. We recommend that you configure this parameter.
         # 
         # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
         # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   For more information about the valid values, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.partition_num = partition_num
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         # 
         # If this parameter is left empty, the default resource group is used. You can view the resource group ID on the Resource Group page in the Resource Management console.
         self.resource_group_id = resource_group_id
         # The edition of the instance. Valid values:
         # 
         # *   **normal**: Standard Edition (High Write)
         # *   **professional**: Professional Edition (High Write)
         # *   **professionalForHighRead**: Professional Edition (High Read)
         # 
-        # For more information, see [Billing](~~84737~~).
+        # For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.spec_type = spec_type
         # The tags.
         self.tag = tag
         # The number of topics. We recommend that you do not configure this parameter.
         # 
         # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
         # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
         # *   The default value of the TopicQuota parameter varies based on the value of the IoMaxSpec parameter. If the number of topics that you consume exceeds the default value, you are charged additional fees.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   For more information about the valid values, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.topic_quota = topic_quota
 
     def validate(self):
         if self.confluent_config:
             self.confluent_config.validate()
         if self.tag:
             for k in self.tag:
@@ -1569,14 +1728,16 @@
         value: str = None,
     ):
         # The key of tag N.
         # 
         # *   Valid values of N: 1 to 20.
         # *   If this parameter is left empty, the keys of all tags are matched.
         # *   The tag key can be up to 128 characters in length and cannot start with acs: or aliyun or contain [http:// or https://.](http://https://。)
+        # 
+        # This parameter is required.
         self.key = key
         # The value of tag N.
         # 
         # *   Valid values of N: 1 to 20.
         # *   This parameter can be left empty.
         # *   The tag value can be 1 to 128 characters in length and cannot start with acs: or aliyun or contain [http:// or https://.](http://https://。)
         self.value = value
@@ -1620,74 +1781,84 @@
         partition_num: int = None,
         region_id: str = None,
         resource_group_id: str = None,
         spec_type: str = None,
         tag: List[CreatePrePayOrderShrinkRequestTag] = None,
         topic_quota: int = None,
     ):
+        # The configurations of ApsaraMQ for Confluent components.
         self.confluent_config_shrink = confluent_config_shrink
         # The deployment mode of the instance. Valid values:
         # 
         # *   **4**: deploys the instance that allows access from the Internet and a VPC.
         # *   **5**: deploys the instance that allows access only from a VPC.
         self.deploy_type = deploy_type
         # The disk size. Unit: GB.
         # 
-        # For more information about the valid values, see [Billing](~~84737~~).
+        # For more information about the valid values, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.disk_size = disk_size
         # The disk type. Valid values:
         # 
         # *   **0**: ultra disk
         # *   **1**: standard SSD
         self.disk_type = disk_type
+        # The subscription duration. Unit: months. Default value: 1. Valid values:
+        # 
+        # *   **1 to 12**\
         self.duration = duration
         # The Internet traffic for the instance.
         # 
         # *   This parameter is required if the **DeployType** parameter is set to **4**.
-        # *   For more information about the valid values, see [Pay-as-you-go](~~72142~~).
+        # *   For more information about the valid values, see [Pay-as-you-go](https://help.aliyun.com/document_detail/72142.html).
         self.eip_max = eip_max
         # The maximum traffic for the instance. We recommend that you do not configure this parameter.
         # 
         # *   You must configure at least one of the **IoMax** and **IoMaxSpec** parameters. If both parameters are configured, the value of the **IoMaxSpec** parameter takes effect. We recommend that you configure only the **IoMaxSpec** parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   For more information about the valid values, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.io_max = io_max
         # The traffic specification of the instance. We recommend that you configure this parameter.
         # 
         # *   You must configure at least one of the **IoMax** and **IoMaxSpec** parameters. If both parameters are configured, the value of the **IoMaxSpec** parameter takes effect. We recommend that you configure only the **IoMaxSpec** parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   For more information about the valid values, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.io_max_spec = io_max_spec
+        # The billing method of the instance. Valid values:
+        # 
+        # *   **0**: the subscription billing method
+        # *   **4**: the subscription billing method for ApsaraMQ for Confluent instances
         self.paid_type = paid_type
         # The number of partitions. We recommend that you configure this parameter.
         # 
         # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
         # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   For more information about the valid values, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.partition_num = partition_num
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         # 
         # If this parameter is left empty, the default resource group is used. You can view the resource group ID on the Resource Group page in the Resource Management console.
         self.resource_group_id = resource_group_id
         # The edition of the instance. Valid values:
         # 
         # *   **normal**: Standard Edition (High Write)
         # *   **professional**: Professional Edition (High Write)
         # *   **professionalForHighRead**: Professional Edition (High Read)
         # 
-        # For more information, see [Billing](~~84737~~).
+        # For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.spec_type = spec_type
         # The tags.
         self.tag = tag
         # The number of topics. We recommend that you do not configure this parameter.
         # 
         # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
         # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
         # *   The default value of the TopicQuota parameter varies based on the value of the IoMaxSpec parameter. If the number of topics that you consume exceeds the default value, you are charged additional fees.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   For more information about the valid values, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.topic_quota = topic_quota
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -1874,36 +2045,44 @@
         mechanism: str = None,
         password: str = None,
         region_id: str = None,
         type: str = None,
         username: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The encryption method. Valid values:
         # 
         # *   SCRAM-SHA-512 (default)
         # *   SCRAM-SHA-256
         # 
         # > 
         # 
         # *   This parameter is available only for ApsaraMQ for Kafka V3 serverless instances.
         self.mechanism = mechanism
         # The password of the SASL user.
+        # 
+        # This parameter is required.
         self.password = password
         # The region ID.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The SASL mechanism. Valid values:
         # 
         # *   **plain**: a simple mechanism that uses usernames and passwords to verify user identities. Message Queue for Apache Kafka provides an optimized PLAIN mechanism that allows you to dynamically create SASL users for an instance without the need to restart the instance.
         # *   **scram**: a mechanism that uses usernames and passwords to verify user identities. This mechanism provides better security protection than the PLAIN mechanism. Message Queue for Apache Kafka uses SCRAM-SHA-256.
         # 
         # Default value: **plain**.
         self.type = type
         # The name of the SASL user.
+        # 
+        # This parameter is required.
         self.username = username
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2028,24 +2207,317 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateSaslUserResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateScheduledScalingRuleRequest(TeaModel):
+    def __init__(
+        self,
+        duration_minutes: int = None,
+        enable: bool = None,
+        first_scheduled_time: int = None,
+        instance_id: str = None,
+        region_id: str = None,
+        repeat_type: str = None,
+        reserved_pub_flow: int = None,
+        reserved_sub_flow: int = None,
+        rule_name: str = None,
+        schedule_type: str = None,
+        time_zone: str = None,
+        weekly_types: List[str] = None,
+    ):
+        # This parameter is required.
+        self.duration_minutes = duration_minutes
+        self.enable = enable
+        # This parameter is required.
+        self.first_scheduled_time = first_scheduled_time
+        # This parameter is required.
+        self.instance_id = instance_id
+        # This parameter is required.
+        self.region_id = region_id
+        self.repeat_type = repeat_type
+        # This parameter is required.
+        self.reserved_pub_flow = reserved_pub_flow
+        # This parameter is required.
+        self.reserved_sub_flow = reserved_sub_flow
+        # This parameter is required.
+        self.rule_name = rule_name
+        # This parameter is required.
+        self.schedule_type = schedule_type
+        # This parameter is required.
+        self.time_zone = time_zone
+        self.weekly_types = weekly_types
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.duration_minutes is not None:
+            result['DurationMinutes'] = self.duration_minutes
+        if self.enable is not None:
+            result['Enable'] = self.enable
+        if self.first_scheduled_time is not None:
+            result['FirstScheduledTime'] = self.first_scheduled_time
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.repeat_type is not None:
+            result['RepeatType'] = self.repeat_type
+        if self.reserved_pub_flow is not None:
+            result['ReservedPubFlow'] = self.reserved_pub_flow
+        if self.reserved_sub_flow is not None:
+            result['ReservedSubFlow'] = self.reserved_sub_flow
+        if self.rule_name is not None:
+            result['RuleName'] = self.rule_name
+        if self.schedule_type is not None:
+            result['ScheduleType'] = self.schedule_type
+        if self.time_zone is not None:
+            result['TimeZone'] = self.time_zone
+        if self.weekly_types is not None:
+            result['WeeklyTypes'] = self.weekly_types
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DurationMinutes') is not None:
+            self.duration_minutes = m.get('DurationMinutes')
+        if m.get('Enable') is not None:
+            self.enable = m.get('Enable')
+        if m.get('FirstScheduledTime') is not None:
+            self.first_scheduled_time = m.get('FirstScheduledTime')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RepeatType') is not None:
+            self.repeat_type = m.get('RepeatType')
+        if m.get('ReservedPubFlow') is not None:
+            self.reserved_pub_flow = m.get('ReservedPubFlow')
+        if m.get('ReservedSubFlow') is not None:
+            self.reserved_sub_flow = m.get('ReservedSubFlow')
+        if m.get('RuleName') is not None:
+            self.rule_name = m.get('RuleName')
+        if m.get('ScheduleType') is not None:
+            self.schedule_type = m.get('ScheduleType')
+        if m.get('TimeZone') is not None:
+            self.time_zone = m.get('TimeZone')
+        if m.get('WeeklyTypes') is not None:
+            self.weekly_types = m.get('WeeklyTypes')
+        return self
+
+
+class CreateScheduledScalingRuleShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        duration_minutes: int = None,
+        enable: bool = None,
+        first_scheduled_time: int = None,
+        instance_id: str = None,
+        region_id: str = None,
+        repeat_type: str = None,
+        reserved_pub_flow: int = None,
+        reserved_sub_flow: int = None,
+        rule_name: str = None,
+        schedule_type: str = None,
+        time_zone: str = None,
+        weekly_types_shrink: str = None,
+    ):
+        # This parameter is required.
+        self.duration_minutes = duration_minutes
+        self.enable = enable
+        # This parameter is required.
+        self.first_scheduled_time = first_scheduled_time
+        # This parameter is required.
+        self.instance_id = instance_id
+        # This parameter is required.
+        self.region_id = region_id
+        self.repeat_type = repeat_type
+        # This parameter is required.
+        self.reserved_pub_flow = reserved_pub_flow
+        # This parameter is required.
+        self.reserved_sub_flow = reserved_sub_flow
+        # This parameter is required.
+        self.rule_name = rule_name
+        # This parameter is required.
+        self.schedule_type = schedule_type
+        # This parameter is required.
+        self.time_zone = time_zone
+        self.weekly_types_shrink = weekly_types_shrink
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.duration_minutes is not None:
+            result['DurationMinutes'] = self.duration_minutes
+        if self.enable is not None:
+            result['Enable'] = self.enable
+        if self.first_scheduled_time is not None:
+            result['FirstScheduledTime'] = self.first_scheduled_time
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.repeat_type is not None:
+            result['RepeatType'] = self.repeat_type
+        if self.reserved_pub_flow is not None:
+            result['ReservedPubFlow'] = self.reserved_pub_flow
+        if self.reserved_sub_flow is not None:
+            result['ReservedSubFlow'] = self.reserved_sub_flow
+        if self.rule_name is not None:
+            result['RuleName'] = self.rule_name
+        if self.schedule_type is not None:
+            result['ScheduleType'] = self.schedule_type
+        if self.time_zone is not None:
+            result['TimeZone'] = self.time_zone
+        if self.weekly_types_shrink is not None:
+            result['WeeklyTypes'] = self.weekly_types_shrink
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DurationMinutes') is not None:
+            self.duration_minutes = m.get('DurationMinutes')
+        if m.get('Enable') is not None:
+            self.enable = m.get('Enable')
+        if m.get('FirstScheduledTime') is not None:
+            self.first_scheduled_time = m.get('FirstScheduledTime')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RepeatType') is not None:
+            self.repeat_type = m.get('RepeatType')
+        if m.get('ReservedPubFlow') is not None:
+            self.reserved_pub_flow = m.get('ReservedPubFlow')
+        if m.get('ReservedSubFlow') is not None:
+            self.reserved_sub_flow = m.get('ReservedSubFlow')
+        if m.get('RuleName') is not None:
+            self.rule_name = m.get('RuleName')
+        if m.get('ScheduleType') is not None:
+            self.schedule_type = m.get('ScheduleType')
+        if m.get('TimeZone') is not None:
+            self.time_zone = m.get('TimeZone')
+        if m.get('WeeklyTypes') is not None:
+            self.weekly_types_shrink = m.get('WeeklyTypes')
+        return self
+
+
+class CreateScheduledScalingRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        # Id of the request
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class CreateScheduledScalingRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateScheduledScalingRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateScheduledScalingRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateTopicRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
         # The tag key.
         # 
         # *   If you do not specify this parameter, the keys of all tags are matched.
         # *   The tag key must be 1 to 128 characters in length and cannot contain `http://` or `https://`. The tag key cannot start with `aliyun` or `acs:`.
+        # 
+        # This parameter is required.
         self.key = key
         # The tag value.
         # 
         # *   You can leave this parameter empty.
         # *   The tag value must be 1 to 128 characters in length and cannot contain http:// or https://. The tag value cannot start with aliyun or acs:.
         self.value = value
 
@@ -2098,14 +2570,16 @@
         # *   The value of this parameter must be in JSON format.
         # *   The key must be **replications**. The value indicates the number of replicas for the topic. The value must be an integer that ranges from 1 to 3.
         # *   This parameter is available only when **LocalTopic** is set to **true**, or the instance is of the **Open Source Edition (Local Disk)**.****\
         # 
         # > If you specify this parameter, **ReplicationFactor** does not take effect.
         self.config = config
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The type of storage that the topic uses. Valid values:
         # 
         # *   false: The topic uses cloud storage.
         # *   true: The topic uses local storage.
         self.local_topic = local_topic
         # The minimum number of in-sync replicas (ISRs).
@@ -2113,37 +2587,48 @@
         # *   This parameter is available only when **LocalTopic** is set to **true**, or the instance is of the **Open Source Edition (Local Disk)**.****\
         # *   The value of this parameter must be smaller than the value of ReplicationFactor.
         # *   Valid values: 1 to 3.
         self.min_insync_replicas = min_insync_replicas
         # The number of partitions in the topic.
         # 
         # *   Valid values: 1 to 360.
-        # *   The system recommends the number of partitions based on the specification of the instance. You can view the recommended number in the Message Queue for Apache Kafka console. We recommend that you specify the number that is recommended by the system as the value of this parameter to reduce the risk of data skew.
+        # *   In the ApsaraMQ for Kafka console, you can view the number of partitions that the system recommends based on the specifications of the instance. We recommend that you specify the number that is recommended by the system as the value of this parameter to reduce the risk of data skew.
+        # 
+        # Default values:
+        # 
+        # *   ApsaraMQ for Kafka V2 instance: 12
+        # *   ApsaraMQ for Kafka V3 instance: 3
         self.partition_num = partition_num
         # The region ID of the instance in which you want to create a topic.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The description of the topic.
         # 
-        # *   The description can contain only letters, digits, hyphens (-), and underscores (\_).
+        # *   The description can contain only letters, digits, hyphens (-), and underscores (_).
         # *   The description must be 3 to 64 characters in length.
+        # 
+        # This parameter is required.
         self.remark = remark
         # The number of replicas for the topic.
         # 
         # *   This parameter is available only when **LocalTopic** is set to **true**, or the instance is of the **Open Source Edition (Local Disk)**.****\
         # *   Valid values: 1 to 3.
         # 
         # > If you set this parameter to **1**, data loss may occur. Exercise caution when you configure this parameter.
         self.replication_factor = replication_factor
         # The tags that you want to add to the topic.
         self.tag = tag
         # The topic name.
         # 
-        # *   The name can contain only letters, digits, hyphens (-), and underscores (\_).
+        # *   The name can contain only letters, digits, hyphens (-), and underscores (_).
         # *   The name must be 3 to 64 characters in length. If the name that you specify contains more than 64 characters, the system automatically truncates the name.
         # *   After a topic is created, you cannot change the name of the topic.
+        # 
+        # This parameter is required.
         self.topic = topic
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -2316,14 +2801,16 @@
     ):
         # The operation allowed by the access control list (ACL). Valid values:
         # 
         # *   **Write**: data writes
         # *   **Read**: data reads
         # *   **Describe**: reads of transactional IDs
         # *   **IdempotentWrite**: idempotent data writes to clusters
+        # 
+        # This parameter is required.
         self.acl_operation_type = acl_operation_type
         # The operations allowed by the ACL. Separate multiple operations with commas (,).
         # 
         # Valid values:
         # 
         # *   **Write**: data writes
         # *   **Read**: data reads
@@ -2338,35 +2825,47 @@
         # *   ALLOW
         # 
         # >  This parameter is available only for ApsaraMQ for Kafka V3 serverless instances.
         self.acl_permission_type = acl_permission_type
         # The name of the resource.
         # 
         # *   The value can be the name of a topic or consumer group.
-        # *   You can use an asterisk (\*) to indicate the names of all topics or consumer groups.
+        # *   You can use an asterisk (\\*) to indicate the names of all topics or consumer groups.
+        # 
+        # This parameter is required.
         self.acl_resource_name = acl_resource_name
         # The mode that is used to match resources. Valid values:
         # 
         # *   **LITERAL:** full match
         # *   **PREFIXED**: prefix match
+        # 
+        # This parameter is required.
         self.acl_resource_pattern_type = acl_resource_pattern_type
         # The resource type. Valid values:
         # 
         # *   **Topic**: topic
         # *   **Group**: consumer group
         # *   **Cluster**: cluster
         # *   **TransactionalId**: transactional ID
+        # 
+        # This parameter is required.
         self.acl_resource_type = acl_resource_type
         # The IP address of the source.
         self.host = host
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the region.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The name of the user.
+        # 
+        # This parameter is required.
         self.username = username
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2515,18 +3014,24 @@
     def __init__(
         self,
         consumer_id: str = None,
         instance_id: str = None,
         region_id: str = None,
     ):
         # The name of the consumer group.
+        # 
+        # This parameter is required.
         self.consumer_id = consumer_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2646,16 +3151,20 @@
 class DeleteInstanceRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2774,26 +3283,38 @@
         instance_id: str = None,
         mechanism: str = None,
         region_id: str = None,
         type: str = None,
         username: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
+        # The encryption method. Valid values:
+        # 
+        # *   SCRAM-SHA-512. This is the default value.
+        # *   SCRAM-SHA-256
+        # 
+        # >  This parameter is available only for ApsaraMQ for Kafka V3 serverless instances.
         self.mechanism = mechanism
         # The ID of the region.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The SASL mechanism. Valid values:
         # 
         # *   **plain**: a simple mechanism that uses usernames and passwords to verify user identities. Message Queue for Apache Kafka provides an optimized PLAIN mechanism that allows you to dynamically create SASL users for an instance without the need to restart the instance.
         # *   **scram**: a mechanism that uses usernames and passwords to verify user identities. This mechanism provides better security protection than the PLAIN mechanism. Message Queue for Apache Kafka uses SCRAM-SHA-256.
         # 
         # Default value: **plain**.
         self.type = type
         # The name of the user.
+        # 
+        # This parameter is required.
         self.username = username
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2832,19 +3353,19 @@
     def __init__(
         self,
         code: int = None,
         message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
-        # The HTTP status code returned. The HTTP status code 200 indicates that the request is successful.
+        # The HTTP status code. If the request is successful, 200 is returned.
         self.code = code
         # The returned message.
         self.message = message
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
         # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         pass
 
@@ -2914,26 +3435,161 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteSaslUserResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteScheduledScalingRuleRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        region_id: str = None,
+        rule_name: str = None,
+    ):
+        # This parameter is required.
+        self.instance_id = instance_id
+        # This parameter is required.
+        self.region_id = region_id
+        # This parameter is required.
+        self.rule_name = rule_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.rule_name is not None:
+            result['RuleName'] = self.rule_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RuleName') is not None:
+            self.rule_name = m.get('RuleName')
+        return self
+
+
+class DeleteScheduledScalingRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        # Id of the request
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class DeleteScheduledScalingRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteScheduledScalingRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteScheduledScalingRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteTopicRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
         topic: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The name of the topic.
+        # 
+        # This parameter is required.
         self.topic = topic
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3064,32 +3720,42 @@
         username: str = None,
     ):
         self.acl_operation_type = acl_operation_type
         self.acl_permission_type = acl_permission_type
         # The name or ID of the resource.
         # 
         # *   The value can be the name of a topic or a consumer group.
-        # *   You can use an asterisk (\*) to represent the names of all topics or consumer groups.
+        # *   You can use an asterisk (\\*) to represent the names of all topics or consumer groups.
+        # 
+        # This parameter is required.
         self.acl_resource_name = acl_resource_name
         # The match mode. Valid values:
         # 
         # *   LITERAL: full-name match
         # *   PREFIXED: prefix match
         self.acl_resource_pattern_type = acl_resource_pattern_type
         # The resource type. Valid values:
         # 
         # *   **Topic**\
         # *   **Group**\
+        # 
+        # This parameter is required.
         self.acl_resource_type = acl_resource_type
         self.host = host
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the region.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The name of the user.
+        # 
+        # This parameter is required.
         self.username = username
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3147,38 +3813,38 @@
         acl_permission_type: str = None,
         acl_resource_name: str = None,
         acl_resource_pattern_type: str = None,
         acl_resource_type: str = None,
         host: str = None,
         username: str = None,
     ):
-        # The type of the operation. Valid values:
+        # The operation type. Valid values:
         # 
         # *   **Write**\
         # *   **Read**\
         self.acl_operation_type = acl_operation_type
         self.acl_permission_type = acl_permission_type
-        # The name of the resource.
+        # The resource name.
         # 
-        # *   The value can be the name of a topic or a consumer group.
-        # *   An asterisk (\*) represents the names of all topics or consumer groups.
+        # *   The value can be the name of a topic or consumer group.
+        # *   You can use the asterisk (\\*) wildcard character to specify the names of all topics or consumer groups.
         self.acl_resource_name = acl_resource_name
-        # The match mode. Valid values:
+        # The matching mode. Valid values:
         # 
-        # *   **LITERAL**: full-name match
+        # *   **LITERAL:** full-name match
         # *   **PREFIXED**: prefix match
         self.acl_resource_pattern_type = acl_resource_pattern_type
-        # The type of the resources to which you want to attach tags. Valid values:
+        # The resource type. Valid values:
         # 
         # *   **Topic**\
         # *   **Group**\
         self.acl_resource_type = acl_resource_type
         # The host.
         self.host = host
-        # The name of the user.
+        # The username.
         self.username = username
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3263,15 +3929,15 @@
         kafka_acl_list: DescribeAclsResponseBodyKafkaAclList = None,
         message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
         # The HTTP status code returned. The HTTP status code 200 indicates that the request is successful.
         self.code = code
-        # The ACLs.
+        # The access control lists (ACLs).
         self.kafka_acl_list = kafka_acl_list
         # The returned message.
         self.message = message
         # The ID of the request.
         self.request_id = request_id
         # Indicates whether the request is successful.
         self.success = success
@@ -3358,16 +4024,20 @@
 class DescribeSaslUsersRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the region.
+        # 
+        # This parameter is required.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3394,25 +4064,28 @@
     def __init__(
         self,
         mechanism: str = None,
         password: str = None,
         type: str = None,
         username: str = None,
     ):
+        # The encryption method.
+        # 
+        # >  This field is available only for ApsaraMQ for Kafka V3 Serverless instances.
         self.mechanism = mechanism
-        # The password that is used to access the Elasticsearch cluster.
+        # The password.
         self.password = password
-        # The request type. Valid values:
+        # The type. Valid values:
         # 
-        # *   **plain**: a simple mechanism that uses usernames and passwords to verify user identities. Message Queue for Apache Kafka provides an optimized PLAIN mechanism that allows you to dynamically create SASL users for an instance without the need to restart the instance.
-        # *   **scram**: a mechanism that uses usernames and passwords to verify user identities. This mechanism provides better security protection than the PLAIN mechanism. Message Queue for Apache Kafka uses SCRAM-SHA-256.
+        # *   **plain**: a simple mechanism that uses usernames and passwords to verify user identities. ApsaraMQ for Kafka provides an improved PLAIN mechanism that allows you to dynamically add SASL users without the need to restart an instance.
+        # *   **SCRAM**: a mechanism that uses usernames and passwords to verify user identities. Compared with the PLAIN mechanism, this mechanism provides better security protection. ApsaraMQ for Kafka uses the SCRAM-SHA-256 algorithm.
         # 
         # Default value: **plain**.
         self.type = type
-        # The name of the user.
+        # The username.
         self.username = username
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3489,15 +4162,15 @@
     ):
         # The HTTP status code returned. The HTTP status code 200 indicates that the request is successful.
         self.code = code
         # The returned message.
         self.message = message
         # The ID of the request.
         self.request_id = request_id
-        # The SASL users.
+        # The Simple Authentication and Security Layer (SASL) users.
         self.sasl_user_list = sasl_user_list
         # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         if self.sasl_user_list:
             self.sasl_user_list.validate()
@@ -3584,20 +4257,26 @@
         instance_id: str = None,
         region_id: str = None,
     ):
         # Specify whether to enable the flexible group creation feature. Valid values:
         # 
         # *   **true**: enables the flexible group creation feature.
         # *   **false**: disabled the flexible group creation feature.
+        # 
+        # This parameter is required.
         self.enable = enable
         # The instance ID.
         # 
-        # You can call the [GetInstanceList](~~437663~~) operation to query instances.
+        # You can call the [GetInstanceList](https://help.aliyun.com/document_detail/437663.html) operation to query instances.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The region ID.
+        # 
+        # This parameter is required.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3721,26 +4400,32 @@
         self,
         instance_id: str = None,
         operate: str = None,
         partition_num: int = None,
         region_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The operation that you want to perform. Valid values:
         # 
         # *   enable: enables the automatic topic creation feature.
         # *   disable: disables the automatic topic creation feature.
         # *   updatePartition: changes the number of partitions in topics that are automatically created.
+        # 
+        # This parameter is required.
         self.operate = operate
         # The changed number of partitions in topics that are automatically created.
         # 
         # This parameter takes effect only if you set Operate to updatePartition.
         self.partition_num = partition_num
         # The region ID.
+        # 
+        # This parameter is required.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3989,16 +4674,20 @@
 class GetAllowedIpListRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The region ID.
+        # 
+        # This parameter is required.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4268,32 +4957,358 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetAllowedIpListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetAutoScalingConfigurationRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        region_id: str = None,
+    ):
+        # This parameter is required.
+        self.instance_id = instance_id
+        # This parameter is required.
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class GetAutoScalingConfigurationResponseBodyDataScheduledScalingRulesScheduledScalingRulesWeeklyTypes(TeaModel):
+    def __init__(
+        self,
+        weekly_types: List[str] = None,
+    ):
+        self.weekly_types = weekly_types
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.weekly_types is not None:
+            result['WeeklyTypes'] = self.weekly_types
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('WeeklyTypes') is not None:
+            self.weekly_types = m.get('WeeklyTypes')
+        return self
+
+
+class GetAutoScalingConfigurationResponseBodyDataScheduledScalingRulesScheduledScalingRules(TeaModel):
+    def __init__(
+        self,
+        duration_minutes: int = None,
+        enable: bool = None,
+        estimated_elastic_scaling_down_time_secs: int = None,
+        estimated_elastic_scaling_up_time_secs: int = None,
+        first_scheduled_time: int = None,
+        repeat_type: str = None,
+        reserved_pub_flow: int = None,
+        reserved_sub_flow: int = None,
+        rule_id: int = None,
+        rule_name: str = None,
+        schedule_type: str = None,
+        time_zone: str = None,
+        weekly_types: GetAutoScalingConfigurationResponseBodyDataScheduledScalingRulesScheduledScalingRulesWeeklyTypes = None,
+    ):
+        self.duration_minutes = duration_minutes
+        self.enable = enable
+        self.estimated_elastic_scaling_down_time_secs = estimated_elastic_scaling_down_time_secs
+        self.estimated_elastic_scaling_up_time_secs = estimated_elastic_scaling_up_time_secs
+        self.first_scheduled_time = first_scheduled_time
+        self.repeat_type = repeat_type
+        self.reserved_pub_flow = reserved_pub_flow
+        self.reserved_sub_flow = reserved_sub_flow
+        self.rule_id = rule_id
+        self.rule_name = rule_name
+        self.schedule_type = schedule_type
+        self.time_zone = time_zone
+        self.weekly_types = weekly_types
+
+    def validate(self):
+        if self.weekly_types:
+            self.weekly_types.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.duration_minutes is not None:
+            result['DurationMinutes'] = self.duration_minutes
+        if self.enable is not None:
+            result['Enable'] = self.enable
+        if self.estimated_elastic_scaling_down_time_secs is not None:
+            result['EstimatedElasticScalingDownTimeSecs'] = self.estimated_elastic_scaling_down_time_secs
+        if self.estimated_elastic_scaling_up_time_secs is not None:
+            result['EstimatedElasticScalingUpTimeSecs'] = self.estimated_elastic_scaling_up_time_secs
+        if self.first_scheduled_time is not None:
+            result['FirstScheduledTime'] = self.first_scheduled_time
+        if self.repeat_type is not None:
+            result['RepeatType'] = self.repeat_type
+        if self.reserved_pub_flow is not None:
+            result['ReservedPubFlow'] = self.reserved_pub_flow
+        if self.reserved_sub_flow is not None:
+            result['ReservedSubFlow'] = self.reserved_sub_flow
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        if self.rule_name is not None:
+            result['RuleName'] = self.rule_name
+        if self.schedule_type is not None:
+            result['ScheduleType'] = self.schedule_type
+        if self.time_zone is not None:
+            result['TimeZone'] = self.time_zone
+        if self.weekly_types is not None:
+            result['WeeklyTypes'] = self.weekly_types.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DurationMinutes') is not None:
+            self.duration_minutes = m.get('DurationMinutes')
+        if m.get('Enable') is not None:
+            self.enable = m.get('Enable')
+        if m.get('EstimatedElasticScalingDownTimeSecs') is not None:
+            self.estimated_elastic_scaling_down_time_secs = m.get('EstimatedElasticScalingDownTimeSecs')
+        if m.get('EstimatedElasticScalingUpTimeSecs') is not None:
+            self.estimated_elastic_scaling_up_time_secs = m.get('EstimatedElasticScalingUpTimeSecs')
+        if m.get('FirstScheduledTime') is not None:
+            self.first_scheduled_time = m.get('FirstScheduledTime')
+        if m.get('RepeatType') is not None:
+            self.repeat_type = m.get('RepeatType')
+        if m.get('ReservedPubFlow') is not None:
+            self.reserved_pub_flow = m.get('ReservedPubFlow')
+        if m.get('ReservedSubFlow') is not None:
+            self.reserved_sub_flow = m.get('ReservedSubFlow')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        if m.get('RuleName') is not None:
+            self.rule_name = m.get('RuleName')
+        if m.get('ScheduleType') is not None:
+            self.schedule_type = m.get('ScheduleType')
+        if m.get('TimeZone') is not None:
+            self.time_zone = m.get('TimeZone')
+        if m.get('WeeklyTypes') is not None:
+            temp_model = GetAutoScalingConfigurationResponseBodyDataScheduledScalingRulesScheduledScalingRulesWeeklyTypes()
+            self.weekly_types = temp_model.from_map(m['WeeklyTypes'])
+        return self
+
+
+class GetAutoScalingConfigurationResponseBodyDataScheduledScalingRules(TeaModel):
+    def __init__(
+        self,
+        scheduled_scaling_rules: List[GetAutoScalingConfigurationResponseBodyDataScheduledScalingRulesScheduledScalingRules] = None,
+    ):
+        self.scheduled_scaling_rules = scheduled_scaling_rules
+
+    def validate(self):
+        if self.scheduled_scaling_rules:
+            for k in self.scheduled_scaling_rules:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['ScheduledScalingRules'] = []
+        if self.scheduled_scaling_rules is not None:
+            for k in self.scheduled_scaling_rules:
+                result['ScheduledScalingRules'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.scheduled_scaling_rules = []
+        if m.get('ScheduledScalingRules') is not None:
+            for k in m.get('ScheduledScalingRules'):
+                temp_model = GetAutoScalingConfigurationResponseBodyDataScheduledScalingRulesScheduledScalingRules()
+                self.scheduled_scaling_rules.append(temp_model.from_map(k))
+        return self
+
+
+class GetAutoScalingConfigurationResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        scheduled_scaling_rules: GetAutoScalingConfigurationResponseBodyDataScheduledScalingRules = None,
+    ):
+        self.scheduled_scaling_rules = scheduled_scaling_rules
+
+    def validate(self):
+        if self.scheduled_scaling_rules:
+            self.scheduled_scaling_rules.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.scheduled_scaling_rules is not None:
+            result['ScheduledScalingRules'] = self.scheduled_scaling_rules.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ScheduledScalingRules') is not None:
+            temp_model = GetAutoScalingConfigurationResponseBodyDataScheduledScalingRules()
+            self.scheduled_scaling_rules = temp_model.from_map(m['ScheduledScalingRules'])
+        return self
+
+
+class GetAutoScalingConfigurationResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        data: GetAutoScalingConfigurationResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        # Id of the request
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = GetAutoScalingConfigurationResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetAutoScalingConfigurationResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetAutoScalingConfigurationResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetAutoScalingConfigurationResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetConsumerListRequest(TeaModel):
     def __init__(
         self,
         consumer_id: str = None,
         current_page: int = None,
         instance_id: str = None,
         page_size: int = None,
         region_id: str = None,
     ):
         # The name of the consumer group. If you do not configure this parameter, all consumer groups are queried.
         self.consumer_id = consumer_id
         # The page number.
         self.current_page = current_page
         # The ID of the instance to which the consumer group belongs.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The number of entries to be returned per page.
         self.page_size = page_size
         # The region ID of the instance to which the consumer group belongs.
+        # 
+        # This parameter is required.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4622,18 +5637,24 @@
     def __init__(
         self,
         consumer_id: str = None,
         instance_id: str = None,
         region_id: str = None,
     ):
         # The name of the consumer group.
+        # 
+        # This parameter is required.
         self.consumer_id = consumer_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5130,20 +6151,26 @@
         region_id: str = None,
         resource_group_id: str = None,
         series: str = None,
         tag: List[GetInstanceListRequestTag] = None,
     ):
         # The IDs of instances.
         self.instance_id = instance_id
-        # The ID of the order. You can obtain the order ID on the [Orders](https://usercenter2-intl.aliyun.com/order/list?pageIndex=1\&pageSize=20\&spm=5176.12818093.top-nav.ditem-ord.36f016d0OQFmJa) page in Alibaba Cloud User Center.
+        # The ID of the order. You can obtain the order ID on the [Orders](https://usercenter2-intl.aliyun.com/order/list?pageIndex=1\\&pageSize=20\\&spm=5176.12818093.top-nav.ditem-ord.36f016d0OQFmJa) page in Alibaba Cloud User Center.
         self.order_id = order_id
         # The ID of the region where the instance resides.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group. You can obtain this ID on the Resource Group page in the Resource Management console.
         self.resource_group_id = resource_group_id
+        # 实例系列标识，可根据系列号来过滤不同系列的实例。取值如下：
+        # - v2
+        # - v3
+        # - confluent
         self.series = series
         # The tags.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
@@ -5210,31 +6237,49 @@
         ksql_storage: int = None,
         schema_registry_cu: int = None,
         schema_registry_replica: int = None,
         zoo_keeper_cu: int = None,
         zoo_keeper_replica: int = None,
         zoo_keeper_storage: int = None,
     ):
+        # The number of CPU cores of Connect.
         self.connect_cu = connect_cu
+        # The number of replicas of Connect.
         self.connect_replica = connect_replica
+        # The number of CPU cores of Control Center.
         self.control_center_cu = control_center_cu
+        # The number of replicas of Control Center.
         self.control_center_replica = control_center_replica
+        # The disk capacity of Control Center. Unit: GB.
         self.control_center_storage = control_center_storage
+        # The number of CPU cores of the Kafka broker.
         self.kafka_cu = kafka_cu
+        # The number of replicas of the Kafka broker.
         self.kafka_replica = kafka_replica
+        # The number of CPU cores of Kafka Rest Proxy.
         self.kafka_rest_proxy_cu = kafka_rest_proxy_cu
+        # The number of replicas of Kafka Rest Proxy.
         self.kafka_rest_proxy_replica = kafka_rest_proxy_replica
+        # The disk capacity of the Kafka broker. Unit: GB.
         self.kafka_storage = kafka_storage
+        # The number of CPU cores of ksqlDB.
         self.ksql_cu = ksql_cu
+        # The number of replicas of ksqlDB.
         self.ksql_replica = ksql_replica
+        # The disk capacity of ksqlDB. Unit: GB.
         self.ksql_storage = ksql_storage
+        # The number of CPU cores of Schema Registry.
         self.schema_registry_cu = schema_registry_cu
+        # The number of replicas of Schema Registry.
         self.schema_registry_replica = schema_registry_replica
+        # The number of CPU cores of ZooKeeper.
         self.zoo_keeper_cu = zoo_keeper_cu
+        # The number of replicas of ZooKeeper.
         self.zoo_keeper_replica = zoo_keeper_replica
+        # The disk capacity of ZooKeeper. Unit: GB.
         self.zoo_keeper_storage = zoo_keeper_storage
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5462,93 +6507,108 @@
         v_switch_id: str = None,
         view_instance_status_code: int = None,
         vpc_id: str = None,
         zone_id: str = None,
     ):
         # The configurations of the deployed ApsaraMQ for Kafka instance.
         self.all_config = all_config
+        # The parameters that are returned for the ApsaraMQ for Confluent instance.
         self.confluent_config = confluent_config
         # The time when the instance was created. Unit: milliseconds.
         self.create_time = create_time
         # The type of the network in which the instance is deployed. Valid values:
         # 
         # *   **4**: Internet and VPC
         # *   **5**: VPC
         self.deploy_type = deploy_type
-        # The disk size. Unit: GB.
+        # The disk size. Unit: GB
         self.disk_size = disk_size
         # The disk type. Valid values:
         # 
         # *   **0**: ultra disk
         # *   **1**: standard SSD
         self.disk_type = disk_type
         # The default endpoint of the instance in domain name mode. ApsaraMQ for Kafka instances support endpoints in domain name mode and IP address mode.
         # 
         # *   Endpoints in domain name mode: An endpoint in this mode consists of the domain name of the instance and a port number. The format of an endpoint in this mode is `{Instance domain name}:{Port number}`.
         # *   Endpoints in IP address mode: An endpoint in this mode consists of the IP address of the broker and a port number. The format of an endpoint in this mode is `{Broker IP address}:{Port number}`.
         self.domain_endpoint = domain_endpoint
-        # The peak Internet traffic allowed for the instance.
+        # The maximum Internet traffic in the instance.
         self.eip_max = eip_max
         # The default endpoint of the instance in IP address mode. ApsaraMQ for Kafka instances support endpoints in domain name mode and IP address mode.
         # 
         # *   Endpoints in domain name mode: An endpoint in this mode consists of the domain name of the instance and a port number. The format of an endpoint in this mode is `{Instance domain name}:{Port number}`.
         # *   Endpoints in IP address mode: An endpoint in this mode consists of the IP address of the broker and a port number. The format of an endpoint in this mode is `{Broker IP address}:{Port number}`.
         self.end_point = end_point
         # The time when the instance expires. Unit: milliseconds.
         self.expired_time = expired_time
         # The instance ID.
         self.instance_id = instance_id
-        # The peak traffic allowed for the instance.
+        # The maximum traffic in the instance.
         self.io_max = io_max
+        # The maximum read traffic in the instance. Unit: Mbit/s.
         self.io_max_read = io_max_read
         # The traffic specification.
         self.io_max_spec = io_max_spec
+        # The maximum write traffic. Unit: Mbit/s.
         self.io_max_write = io_max_write
         # The ID of the key that is used for disk encryption in the region where the instance is deployed.
         self.kms_key_id = kms_key_id
         # The retention period of messages in the instance. Unit: hours.
         self.msg_retain = msg_retain
         # The instance name.
         self.name = name
         # The billing method of the instance. Valid values:
         # 
-        # *   **0**: subscription
-        # *   **1**: pay-as-you-go
+        # *   **0**: the subscription billing method
+        # *   **1**: the pay-as-you-go billing method
+        # *   **3**: the pay-as-you-go billing method for serverless ApsaraMQ for Kafka V3 instances
+        # *   **4**: the pay-as-you-go billing method for ApsaraMQ for Confluent instances
         self.paid_type = paid_type
         # The ID of the region where the instance resides.
         self.region_id = region_id
+        # The traffic reserved for message publishing. Unit: MB/s.
+        # 
+        # >  This parameter is returned only if the instance is a serverless ApsaraMQ for Kafka V3 instance.
         self.reserved_publish_capacity = reserved_publish_capacity
+        # The traffic reserved for message subscription. Unit: MB/s.
+        # 
+        # >  This parameter is returned only if the instance is a serverless ApsaraMQ for Kafka V3 instance.
         self.reserved_subscribe_capacity = reserved_subscribe_capacity
         # The resource group ID.
         self.resource_group_id = resource_group_id
         # The Simple Authentication and Security Layer (SASL) endpoint of the instance in domain name mode. ApsaraMQ for Kafka instances support endpoints in domain name mode and IP address mode.
         # 
         # *   Endpoints in domain name mode: An endpoint in this mode consists of the domain name of the instance and a port number. The format of an endpoint in this mode is `{Instance domain name}:{Port number}`.
         # *   Endpoints in IP address mode: An endpoint in this mode consists of the IP address of the broker and a port number. The format of an endpoint in this mode is `{Broker IP address}:{Port number}`.
         self.sasl_domain_endpoint = sasl_domain_endpoint
-        # The security group of the instance.
+        # The security group to which the instance belongs.
         # 
-        # *   If the instance is deployed by using the ApsaraMQ for Kafka console or calling the [StartInstance](~~157786~~) operation without a security group configured, no value is returned.
-        # *   If the instance is deployed by calling the [StartInstance](~~157786~~) operation with a security group configured, the returned value is the configured security group.
+        # *   If the instance is deployed in the ApsaraMQ for Kafka console or by calling the [StartInstance](https://help.aliyun.com/document_detail/157786.html) operation without a security group configured, no value is returned.
+        # *   If the instance is deployed by calling the [StartInstance](https://help.aliyun.com/document_detail/157786.html) operation with a security group configured, the returned value is the configured security group.
         self.security_group = security_group
+        # 实例系列标识。返回值有 v2 ，v3，confluent。
         self.series = series
+        # >  This parameter is out of date. We recommend that you refer to the ViewInstanceStatusCode parameter.
+        # 
         # The instance status. Valid values:
         # 
         # *   **0**: pending
         # *   **1**: preparing hardware resources
         # *   **2**: initializing
         # *   **3**: starting
         # *   **5**: running
         # *   **6**: migrating
         # *   **7**: ready for upgrade
         # *   **8**: upgrading
-        # *   **9**: ready for changes
+        # *   **9**: ready for change
         # *   **10**: released
         # *   **11**: changing
         # *   **15**: expired
+        # *   **30**: scaling
         self.service_status = service_status
         # The instance edition. Valid values:
         # 
         # *   **professional**: Professional Edition (High Write)
         # *   **professionalForHighRead**: Professional Edition (High Read)
         # *   **normal**: Standard Edition
         self.spec_type = spec_type
@@ -5564,24 +6624,44 @@
         self.ssl_end_point = ssl_end_point
         # The zone ID.
         self.standard_zone_id = standard_zone_id
         # The tags.
         self.tags = tags
         # The maximum number of topics on the instance.
         self.topic_num_limit = topic_num_limit
-        # The upgrade information of the instance.
+        # The upgrade information about the instance.
         self.upgrade_service_detail_info = upgrade_service_detail_info
         # The number of used groups.
         self.used_group_count = used_group_count
         # The number of used partitions.
         self.used_partition_count = used_partition_count
         # The number of used topics.
         self.used_topic_count = used_topic_count
-        # The vSwitch ID of the instance.
+        # The ID of the vSwitch to which the instance belongs.
         self.v_switch_id = v_switch_id
+        # The instance status. The valid values are consistent with the values displayed in the ApsaraMQ for Kafka console. This parameter is used in the new version of ApsaraMQ for Kafka.
+        # 
+        # Valid values:
+        # 
+        # *   **0**: pending
+        # *   **1**: deploying
+        # *   **2**: running
+        # *   **3**: stopped
+        # *   **4**: expiring
+        # *   **5**: expired
+        # *   **6**: released
+        # *   **7**: upgrading
+        # *   **8**: migrating
+        # *   **21**: stopping
+        # *   **22**: starting
+        # *   **23**: releasing
+        # *   **30**: auto scaling
+        # *   **101**: deployment failed
+        # *   **102**: upgrade failed
+        # *   **103**: migration failed
         self.view_instance_status_code = view_instance_status_code
         # The virtual private cloud (VPC) ID.
         self.vpc_id = vpc_id
         # The zone ID.
         self.zone_id = zone_id
 
     def validate(self):
@@ -5909,16 +6989,20 @@
 class GetQuotaTipRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the region in which the instance resides.
+        # 
+        # This parameter is required.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6146,19 +7230,21 @@
         self,
         current_page: str = None,
         instance_id: str = None,
         page_size: str = None,
         region_id: str = None,
         topic: str = None,
     ):
-        # The page number of the page to return. Default value: 1.
+        # The page number. Default value: 1
         self.current_page = current_page
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
-        # The number of entries to return on each page. Default value: 10
+        # The number of entries to return on each page. Default value: 10.
         self.page_size = page_size
         # The region ID of the instance to which the topics that you want to query belong.
         self.region_id = region_id
         # The name of the topic that you want to query.
         self.topic = topic
 
     def validate(self):
@@ -6278,58 +7364,61 @@
         partition_num: int = None,
         region_id: str = None,
         remark: str = None,
         status: int = None,
         status_name: str = None,
         tags: GetTopicListResponseBodyTopicListTopicVOTags = None,
         topic: str = None,
+        topic_config: str = None,
     ):
+        # Indicates whether the topic was automatically created.
         self.auto_create = auto_create
-        # The log cleanup policy that is used for the topic. This parameter is returned when the **LocalTopic** parameter is set to **true**. Valid values:
+        # The log cleanup policy for the topic. This parameter is returned only if **LocalTopic** is set to **true**. Valid values:
         # 
-        # *   false: The topic uses the default log cleanup policy.
-        # *   true: The topic uses the log compaction policy.
+        # *   false: the default log cleanup policy.
+        # *   true: the Apache Kafka log compaction policy.
         self.compact_topic = compact_topic
         # The timestamp that indicates when the topic was created. Unit: milliseconds.
         self.create_time = create_time
-        # The ID of the instance
+        # The instance ID.
         self.instance_id = instance_id
-        # The type of storage used by the topic. Valid values:
+        # The storage type that is used for the topic. Valid values:
         # 
-        # *   false: The topic uses cloud storage.
-        # *   true: The topic uses local storage.
+        # *   false: cloud storage
+        # *   true: local storage
         self.local_topic = local_topic
         # The number of partitions in the topic.
         self.partition_num = partition_num
-        # The region ID of the instance to which the topics that you want to query belong.
+        # The ID of the region where the instance resides.
         self.region_id = region_id
-        # The description of the topic. Valid values:
+        # The topic description. Valid values:
         # 
-        # *   The description contains only letters, digits, hyphens (-), and underscores (\_).
-        # *   The description is 3 to 64 characters in length.
+        # *   The description can contain only letters, digits, hyphens (-), and underscores (_).
+        # *   The description must be 3 to 64 characters in length.
         self.remark = remark
-        # The status of the topic. Valid values:
+        # The topic status. Valid value:
         # 
-        # **0:** indicates that the topic is running.
+        # **0**: running.
         # 
         # If the topic is deleted, this parameter is not returned.
         self.status = status
-        # The status of the topic. Valid values:
+        # The topic status. Valid value:
         # 
-        # **Running**\
+        # **Running**.
         # 
         # If the topic is deleted, this parameter is not returned.
         self.status_name = status_name
         # The tags.
         self.tags = tags
-        # The name of the topic. Valid values:
+        # The topic name. Valid values:
         # 
-        # *   The name contains only letters, digits, hyphens (-), and underscores (\_).
-        # *   The name is 3 to 64 characters in length. If the name that you specified contains more than 64 characters, the returned name is automatically truncated.
+        # *   The name can contain only letters, digits, hyphens (-), and underscores (_).
+        # *   The name must be 3 to 64 characters in length. If the name contains more than 64 characters, the system automatically truncates the name.
         self.topic = topic
+        self.topic_config = topic_config
 
     def validate(self):
         if self.tags:
             self.tags.validate()
 
     def to_map(self):
         _map = super().to_map()
@@ -6357,14 +7446,16 @@
             result['Status'] = self.status
         if self.status_name is not None:
             result['StatusName'] = self.status_name
         if self.tags is not None:
             result['Tags'] = self.tags.to_map()
         if self.topic is not None:
             result['Topic'] = self.topic
+        if self.topic_config is not None:
+            result['TopicConfig'] = self.topic_config
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AutoCreate') is not None:
             self.auto_create = m.get('AutoCreate')
         if m.get('CompactTopic') is not None:
@@ -6386,14 +7477,16 @@
         if m.get('StatusName') is not None:
             self.status_name = m.get('StatusName')
         if m.get('Tags') is not None:
             temp_model = GetTopicListResponseBodyTopicListTopicVOTags()
             self.tags = temp_model.from_map(m['Tags'])
         if m.get('Topic') is not None:
             self.topic = m.get('Topic')
+        if m.get('TopicConfig') is not None:
+            self.topic_config = m.get('TopicConfig')
         return self
 
 
 class GetTopicListResponseBodyTopicList(TeaModel):
     def __init__(
         self,
         topic_vo: List[GetTopicListResponseBodyTopicListTopicVO] = None,
@@ -6448,15 +7541,15 @@
         self.message = message
         # The number of entries returned on each page.
         self.page_size = page_size
         # The ID of the request.
         self.request_id = request_id
         # Indicates whether the request was successful.
         self.success = success
-        # The information about the topic.
+        # The topics.
         self.topic_list = topic_list
         # The number of topics.
         self.total = total
 
     def validate(self):
         if self.topic_list:
             self.topic_list.validate()
@@ -6552,18 +7645,22 @@
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
         topic: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The region ID of the instance.
         self.region_id = region_id
         # The name of the topic.
+        # 
+        # This parameter is required.
         self.topic = topic
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6829,21 +7926,27 @@
         self,
         instance_id: str = None,
         region_id: str = None,
         topic: str = None,
     ):
         # The instance ID.
         # 
-        # You can call the [GetInstanceList](~~437663~~) operation to query instances.
+        # You can call the [GetInstanceList](https://help.aliyun.com/document_detail/437663.html) operation to query instances.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The region ID.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The topic name.
         # 
-        # You can call the [GetTopicList](~~437677~~) operation to query topics.
+        # You can call the [GetTopicList](https://help.aliyun.com/document_detail/437677.html) operation to query topics.
+        # 
+        # This parameter is required.
         self.topic = topic
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7053,14 +8156,16 @@
         resource_id: List[str] = None,
         resource_type: str = None,
         tag: List[ListTagResourcesRequestTag] = None,
     ):
         # The token that determines the start point of the next query.
         self.next_token = next_token
         # The ID of the region in which the resource is deployed.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The resource ID. The following items describe the formats of resource IDs:
         # 
         # *   Instance ID: instanceId
         # *   Topic ID: Kafka_alikafka_instanceId_topic
         # *   Group ID: Kafka_alikafka_instanceId_consumerGroup
         # 
@@ -7069,14 +8174,16 @@
         # >  You must specify one of the **ResourceId** and **Tag** parameters to query the tags that are attached to a resource. Otherwise, the call fails.
         self.resource_id = resource_id
         # The type of the resource whose tags you want to query. The value is an enumerated value. Valid values:
         # 
         # *   **INSTANCE**\
         # *   **TOPIC**\
         # *   **CONSUMERGROUP**\
+        # 
+        # This parameter is required.
         self.resource_type = resource_type
         # The tags.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
@@ -7304,21 +8411,27 @@
     def __init__(
         self,
         instance_id: str = None,
         instance_name: str = None,
         region_id: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The instance name. Valid values:
         # 
-        # *   The name can contain only letters, digits, hyphens (-), and underscores (\_).
+        # *   The name can contain only letters, digits, hyphens (-), and underscores (_).
         # *   The name must be 3 to 64 characters in length. A name that contains more than 64 characters is automatically truncated.
+        # 
+        # This parameter is required.
         self.instance_name = instance_name
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7444,20 +8557,28 @@
         topic: str = None,
     ):
         # The number of partitions that you want to add to the topic.
         # 
         # *   The value must be an integer that is greater than 0.
         # *   To reduce the risk of data skew, we recommend that you set the value to a multiple of 6.
         # *   The number of total partitions ranges from 1 to 360.
+        # 
+        # This parameter is required.
         self.add_partition_num = add_partition_num
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The topic name.
+        # 
+        # This parameter is required.
         self.topic = topic
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7574,29 +8695,171 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyPartitionNumResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyScheduledScalingRuleRequest(TeaModel):
+    def __init__(
+        self,
+        enable: bool = None,
+        instance_id: str = None,
+        region_id: str = None,
+        rule_name: str = None,
+    ):
+        # This parameter is required.
+        self.enable = enable
+        # This parameter is required.
+        self.instance_id = instance_id
+        # This parameter is required.
+        self.region_id = region_id
+        # This parameter is required.
+        self.rule_name = rule_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.enable is not None:
+            result['Enable'] = self.enable
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.rule_name is not None:
+            result['RuleName'] = self.rule_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Enable') is not None:
+            self.enable = m.get('Enable')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RuleName') is not None:
+            self.rule_name = m.get('RuleName')
+        return self
+
+
+class ModifyScheduledScalingRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        # Id of the request
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class ModifyScheduledScalingRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ModifyScheduledScalingRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ModifyScheduledScalingRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ModifyTopicRemarkRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
         remark: str = None,
         topic: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The description of the topic.
         self.remark = remark
         # The name of the topic.
+        # 
+        # This parameter is required.
         self.topic = topic
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7727,27 +8990,49 @@
         query_type: str = None,
         region_id: str = None,
         topic: str = None,
     ):
         # The beginning of the time range to query. The value of this parameter is a UNIX timestamp in milliseconds.
         self.begin_time = begin_time
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The consumer offset of the partition.
         self.offset = offset
         # The partition ID.
         self.partition = partition
         # The query type. Valid values:
         # 
         # *   byOffset: queries messages by offset. If you select this value, you must configure Partition and Offset.
         # *   byTimestamp: queries messages by time. If you select this value, you must configure BeginTime.
+        # 
+        # <!---->
+        # 
+        # *   <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        # *   <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        # This parameter is required.
         self.query_type = query_type
         # The ID of the region where the resource resides.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The topic name.
+        # 
+        # This parameter is required.
         self.topic = topic
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7826,19 +9111,19 @@
         self.timestamp = timestamp
         # The time type.
         self.timestamp_type = timestamp_type
         # The topic name.
         self.topic = topic
         # The truncated size of the message key. Unit: bytes.
         # 
-        # *   A message is truncated only if the message exceeds 10 MB in size.
+        # >  A maximum of 1 KB content can be displayed for each message. Content that exceeds 1 KB is automatically truncated. For more information, see [Query messages](https://help.aliyun.com/zh/apsaramq-for-kafka/query-messages).
         self.truncated_key_size = truncated_key_size
         # The truncated size of the message value. Unit: bytes.
         # 
-        # *   A message is truncated only if the message exceeds 10 MB in size.
+        # >  A maximum of 1 KB content can be displayed for each message. Content that exceeds 1 KB is automatically truncated. For more information, see [Query messages](https://help.aliyun.com/zh/apsaramq-for-kafka/query-messages).
         self.truncated_value_size = truncated_value_size
         # The message value.
         self.value = value
         # Indicates whether the value is truncated.
         self.value_truncated = value_truncated
 
     def validate(self):
@@ -8030,16 +9315,20 @@
     ):
         # Specifies whether to immediately release the physical resources of the instance. Valid values:
         # 
         # *   **true**: The physical resources of the instance are immediately released.
         # *   **false**: The physical resources of the instance are retained for a period of time before they are released.
         self.force_delete_instance = force_delete_instance
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8159,16 +9448,20 @@
 class ReopenInstanceRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the region where the instance resides.
+        # 
+        # This parameter is required.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8337,14 +9630,16 @@
         # 
         # *   **vpc**: deploys the instance that allows access only from a VPC.
         # *   **eip**: deploys the instance that allows access from the Internet and a VPC.
         # 
         # The deployment mode of the instance must match the type of the instance. If the instance allows access only from a VPC, set the value to **vpc**. If the instance allows access from the Internet and a VPC, set the value to **eip**.
         self.deploy_module = deploy_module
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # Specifies whether the instance supports elastic IP addresses (EIPs). Valid values:
         # 
         # *   **true**: supports EIPs and allows access from the Internet and a VPC.
         # *   **false**: does not support EIPs and allows access only from a VPC.
         # 
         # The value of this parameter must match the type of the instance. For example, if the instance allows access only from a VPC, set this parameter to **false**.
@@ -8354,61 +9649,70 @@
         # Specifies whether to set a new username and password. Valid values:
         # 
         # *   **true**: sets a new username and password.
         # *   **false**: does not set a new username or password.
         # 
         # This parameter is available only if you deploy an instance that allows access from the Internet and a VPC.
         self.is_set_user_and_password = is_set_user_and_password
-        # The ID of the key that is used for disk encryption in the region where the instance is deployed. You can obtain the ID of the key in the [Key Management Service (KMS) console](https://kms.console.aliyun.com/?spm=a2c4g.11186623.2.5.336745b8hfiU21) or create a key. For more information, see [Manage CMKs](~~181610~~).
+        # The ID of the key that is used for disk encryption in the region where the instance is deployed. You can obtain the ID of the key in the [Key Management Service (KMS) console](https://kms.console.aliyun.com/?spm=a2c4g.11186623.2.5.336745b8hfiU21) or create a key. For more information, see [Manage CMKs](https://help.aliyun.com/document_detail/181610.html).
         # 
-        # If this parameter is configured, disk encryption is enabled for the instance. You cannot disable disk encryption after disk encryption is enabled. When you call this operation, the system checks whether the AliyunServiceRoleForAlikafkaInstanceEncryption service-linked role is created. If the role is not created, the system automatically creates the role. For more information, see [Service-linked roles](~~190460~~).
+        # If this parameter is configured, disk encryption is enabled for the instance. You cannot disable disk encryption after disk encryption is enabled. When you call this operation, the system checks whether the AliyunServiceRoleForAlikafkaInstanceEncryption service-linked role is created. If the role is not created, the system automatically creates the role. For more information, see [Service-linked roles](https://help.aliyun.com/document_detail/190460.html).
         self.kmskey_id = kmskey_id
         # The name of the instance.
         # 
         # >  If you specify a value for this parameter, make sure that the specified value is unique in the region of the instance.
         self.name = name
         # The alert contact.
         self.notifier = notifier
         # The password that corresponds to the username.
         # 
         # This parameter is available only if you deploy an instance that allows access from the Internet and a VPC.
         self.password = password
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The security group of the instance.
         # 
-        # If you do not specify this parameter, ApsaraMQ for Kafka automatically configures a security group for your instance. If you specify this parameter, you must create a security group in advance. For more information, see [Create a security group](~~25468~~).
+        # If you do not specify this parameter, ApsaraMQ for Kafka automatically configures a security group for your instance. If you specify this parameter, you must create a security group in advance. For more information, see [Create a security group](https://help.aliyun.com/document_detail/25468.html).
         self.security_group = security_group
         # The two-dimensional arrays that consist of the candidate set for primary zones and the candidate set for secondary zones.
         # 
-        # *   If you set CrossZone to true and specify Zone H and Zone F as the candidate set for primary zones and Zone K as the candidate set for secondary zones, set this parameter to `[[\"zoneh\",\"zonef\"],[\"zonek\"]]`.
+        # *   If you set CrossZone to true and specify Zone H and Zone F as the candidate set for primary zones and Zone K as the candidate set for secondary zones, set this parameter to `[[\\"zoneh\\",\\"zonef\\"],[\\"zonek\\"]]`.
         # 
         #     **\
         # 
-        #     **Note** If you specify multiple zones as the primary or secondary zones, the system deploys the instance in one of the zones without prioritizing them. For example, if you set this parameter to `[[\"zoneh\",\"zonef\"],[\"zonek\"]]`, the primary zone in which the instance is deployed can be Zone H or Zone F, and the secondary zone is Zone K.
+        #     **Note** If you specify multiple zones as the primary or secondary zones, the system deploys the instance in one of the zones without prioritizing them. For example, if you set this parameter to `[[\\"zoneh\\",\\"zonef\\"],[\\"zonek\\"]]`, the primary zone in which the instance is deployed can be Zone H or Zone F, and the secondary zone is Zone K.
         # 
-        # *   If you set CrossZone to false and want to deploy the instance in Zone K, set this parameter to `[[\"zonek\"],[]]`. In this case, the value of this parameter must still be two-dimensional arrays, but the array that specifies the candidate for secondary zones is left empty.
+        # *   If you set CrossZone to false and want to deploy the instance in Zone K, set this parameter to `[[\\"zonek\\"],[]]`. In this case, the value of this parameter must still be two-dimensional arrays, but the array that specifies the candidate for secondary zones is left empty.
         self.selected_zones = selected_zones
         # The version of ApsaraMQ for Kafka. Valid values: 0.10.2 and 2.2.0.
         self.service_version = service_version
         # The mobile phone number of the alert contact.
         self.user_phone_num = user_phone_num
         # The username that is used to access the instance.
         # 
         # This parameter is available only if you deploy an instance that allows access from the Internet and a VPC.
         self.username = username
         # The ID of the vSwitch to which you want to connect the instance.
+        # 
+        # This parameter is required.
         self.v_switch_id = v_switch_id
+        # The vSwitch IDs.
         self.v_switch_ids = v_switch_ids
         # The ID of the virtual private cloud (VPC) in which you want to deploy the instance.
+        # 
+        # This parameter is required.
         self.vpc_id = vpc_id
-        # The ID of the zone in which you want to deploy the instance.
+        # The ID of the zone where you want to deploy the ApsaraMQ for Kafka instance.
+        # 
+        # *   The zone ID of the ApsaraMQ for Kafka instance must be the same as that of the vSwitch.
+        # *   The value must be in the zoneX or Region ID-X format. Examples: zonea and cn-hangzhou-k.
         # 
-        # *   The zone ID of the instance must be the same as that of the vSwitch.
-        # *   The value must be in the format of zoneX or Region ID-X. For example, you can set this parameter to zonea or cn-hangzhou-k.
+        # >  If resources in the specified zone is insufficient, the instance may be deployed in another zone.
         self.zone_id = zone_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8600,16 +9904,20 @@
 class StopInstanceRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the region where the instance resides.
+        # 
+        # This parameter is required.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8728,14 +10036,16 @@
         key: str = None,
         value: str = None,
     ):
         # The tag key.
         # 
         # *   You must specify this parameter.
         # *   The tag key must be 1 to 128 characters in length and cannot start with `acs:` or `aliyun`. The tag key cannot contain `http://` or `https://`.
+        # 
+        # This parameter is required.
         self.key = key
         # The tag value.
         # 
         # *   You can leave this parameter empty.
         # *   The tag value must be 1 to 128 characters in length and cannot start with acs: or aliyun. The tag key cannot contain http:// or https://.
         self.value = value
 
@@ -8771,26 +10081,34 @@
         resource_id: List[str] = None,
         resource_type: str = None,
         tag: List[TagResourcesRequestTag] = None,
     ):
         # The ID of the Message Queue for Apache RocketMQ instance which contains the resource to which you want to attach tags.
         self.instance_id = instance_id
         # The ID of the region in which the resource is deployed.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The list of resource IDs.
+        # 
+        # This parameter is required.
         self.resource_id = resource_id
         # The type of the resources. The value is an enumerated value. Valid values:
         # 
         # *   **INSTANCE**\
         # *   **TOPIC**\
         # *   **CONSUMERGROUP**\
         # 
         # >  The value of this parameter is not case-sensitive.
+        # 
+        # This parameter is required.
         self.resource_type = resource_type
         # The tags that you want to add.
+        # 
+        # This parameter is required.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -8910,24 +10228,30 @@
         resource_id: List[str] = None,
         resource_type: str = None,
         tag_key: List[str] = None,
     ):
         # Specifies whether to detach all tags from the resource. This parameter only takes effect when the TagKey.N parameter is not configured. Default value: **false**.
         self.all = all
         # The ID of the region in which the resource is deployed.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The IDs of the resources from which you want to detach tags.
+        # 
+        # This parameter is required.
         self.resource_id = resource_id
         # The type of the resources. Valid values:
         # 
         # *   **INSTANCE**\
         # *   **TOPIC**\
         # *   **CONSUMERGROUP**\
         # 
         # >  The value of this parameter is not case-sensitive.
+        # 
+        # This parameter is required.
         self.resource_type = resource_type
         # The tag key.
         self.tag_key = tag_key
 
     def validate(self):
         pass
 
@@ -9045,39 +10369,51 @@
         update_type: str = None,
     ):
         # The IP addresses that you want to manage. You can specify a CIDR block. Example: **192.168.0.0/16**.
         # 
         # *   If the **UpdateType** parameter is set to **add**, specify one or more IP addresses for this parameter. Separate multiple IP addresses with commas (,).
         # *   If the **UpdateType** parameter is set to **delete**, specify only one IP address.
         # *   Exercise caution when you delete IP addresses.
+        # 
+        # This parameter is required.
         self.allowed_list_ip = allowed_list_ip
         # The type of the whitelist. Valid values:
         # 
         # *   **vpc**: a whitelist for access from a VPC.
         # *   **internet**: a whitelist for access from the Internet.
+        # 
+        # This parameter is required.
         self.allowed_list_type = allowed_list_type
         # The description of the whitelist.
         self.description = description
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The port range. Valid values:
         # 
         # *   **9092/9092**: the port range for access from virtual private clouds (VPCs) by using the default endpoint.
         # *   **9093/9093**: the port range for access from the Internet.
         # *   **9094/9094**: the port range for access from VPCs by using the Simple Authentication and Security Layer (SASL) endpoint.
         # *   **9095/9095**: the port range for access from VPCs by using the Secure Sockets Layer (SSL) endpoint.
         # 
         # This parameter must correspond to **AllowdedListType**.
+        # 
+        # This parameter is required.
         self.port_range = port_range
         # The ID of the region where the instance resides.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The type of configuration change. Valid values:
         # 
         # *   **add**\
         # *   **delete**\
+        # 
+        # This parameter is required.
         self.update_type = update_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9254,41 +10590,49 @@
         region_id: str = None,
         reset_type: str = None,
         time: str = None,
         topic: str = None,
     ):
         # The name of the consumer group.
         # 
-        # *   The name can contain letters, digits, hyphens (-), and underscores (\_).
+        # *   The name can contain letters, digits, hyphens (-), and underscores (_).
         # *   The name must be **3 to 64** characters in length. If a name contains more than **64** characters, the name is automatically truncated.
         # *   The name of a consumer group cannot be changed after the consumer group is created.
+        # 
+        # This parameter is required.
         self.consumer_id = consumer_id
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # If you set resetType to offset, you can use this parameter to reset the consumer offset of each partition of a specific topic in the consumer group.
         self.offsets = offsets
         # The region ID of the instance to which the consumer group belongs.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The method that is used to reset the consumer offsets of the subscribed topics of a consumer group. Valid values:
         # 
         # *   **timestamp** (default)
         # *   **offset**\
         self.reset_type = reset_type
         # The point in time when message consumption starts. The value of this parameter is a UNIX timestamp in milliseconds. The value of this parameter must be **less than 0** or **within the retention period of the consumer offset**. This parameter takes effect only if you set resetType to timestamp.
         # 
         # *   If you want to reset the consumer offset to the latest offset, set this parameter to -1.
         # *   If you want to reset the consumer offset to the earliest offset, set this parameter to -2.
         self.time = time
         # The topic name.
         # 
-        # *   The name can contain letters, digits, underscores (\_), and hyphens (-).
+        # *   The name can contain letters, digits, underscores (_), and hyphens (-).
         # *   The name must be **3 to 64** characters in length. If a name contains more than **64** characters, the name is automatically truncated.
         # *   The name of a topic cannot be changed after the topic is created.
         # 
         # **If you want to reset the consumer offsets of all topics to which the consumer subscribes, specify an empty string.
+        # 
+        # This parameter is required.
         self.topic = topic
 
     def validate(self):
         if self.offsets:
             for k in self.offsets:
                 if k:
                     k.validate()
@@ -9348,41 +10692,49 @@
         region_id: str = None,
         reset_type: str = None,
         time: str = None,
         topic: str = None,
     ):
         # The name of the consumer group.
         # 
-        # *   The name can contain letters, digits, hyphens (-), and underscores (\_).
+        # *   The name can contain letters, digits, hyphens (-), and underscores (_).
         # *   The name must be **3 to 64** characters in length. If a name contains more than **64** characters, the name is automatically truncated.
         # *   The name of a consumer group cannot be changed after the consumer group is created.
+        # 
+        # This parameter is required.
         self.consumer_id = consumer_id
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # If you set resetType to offset, you can use this parameter to reset the consumer offset of each partition of a specific topic in the consumer group.
         self.offsets_shrink = offsets_shrink
         # The region ID of the instance to which the consumer group belongs.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The method that is used to reset the consumer offsets of the subscribed topics of a consumer group. Valid values:
         # 
         # *   **timestamp** (default)
         # *   **offset**\
         self.reset_type = reset_type
         # The point in time when message consumption starts. The value of this parameter is a UNIX timestamp in milliseconds. The value of this parameter must be **less than 0** or **within the retention period of the consumer offset**. This parameter takes effect only if you set resetType to timestamp.
         # 
         # *   If you want to reset the consumer offset to the latest offset, set this parameter to -1.
         # *   If you want to reset the consumer offset to the earliest offset, set this parameter to -2.
         self.time = time
         # The topic name.
         # 
-        # *   The name can contain letters, digits, underscores (\_), and hyphens (-).
+        # *   The name can contain letters, digits, underscores (_), and hyphens (-).
         # *   The name must be **3 to 64** characters in length. If a name contains more than **64** characters, the name is automatically truncated.
         # *   The name of a topic cannot be changed after the topic is created.
         # 
         # **If you want to reset the consumer offsets of all topics to which the consumer subscribes, specify an empty string.
+        # 
+        # This parameter is required.
         self.topic = topic
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9519,18 +10871,24 @@
     def __init__(
         self,
         config: str = None,
         instance_id: str = None,
         region_id: str = None,
     ):
         # The configurations that you want to update for the ApsaraMQ for Kafka instance. The value must be a valid JSON string.
+        # 
+        # This parameter is required.
         self.config = config
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9658,25 +11016,35 @@
     ):
         # The key of the topic configuration.
         # 
         # *   ApsaraMQ for Kafka V2 instances allow you to modify configurations only for topics that use local storage.
         # *   ApsaraMQ for Kafka V3 instances allow you to modify configurations for all topics.
         # *   The following keys are supported by `local topic` of ApsaraMQ for Kafka V2 instances: retention.ms, retention.bytes, and replications.
         # *   The following keys are supported by ApsaraMQ for Kafka V3 instances: retention.hours and max.message.bytes.
+        # 
+        # This parameter is required.
         self.config = config
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the region where the instance resides.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The topic name.
+        # 
+        # This parameter is required.
         self.topic = topic
-        # The value of the topic configuration.
+        # The configuration item that you want to update for the topic. The following configuration items are supported by ApsaraMQ for Kafka V3 instances:
         # 
         # *   `retention.hours` specifies the message retention period. Value type: string. Valid values: 24 to 8760.
         # *   `max.message.bytes` specifies the maximum size of a sent message. Value type: string. Valid values: 1048576 to 10485760.
+        # 
+        # This parameter is required.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9812,23 +11180,29 @@
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
         target_version: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the region where the instance resides.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The major version to be upgraded to. Valid values:
         # 
         # *   **0.10.2**\
         # *   **2.2.0**\
         # 
         # If you set this parameter to the current major version, the system upgrades the instance to the latest minor version.
+        # 
+        # This parameter is required.
         self.target_version = target_version
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9947,17 +11321,21 @@
 
 class UpgradePostPayOrderRequestServerlessConfig(TeaModel):
     def __init__(
         self,
         reserved_publish_capacity: int = None,
         reserved_subscribe_capacity: int = None,
     ):
-        # The traffic reserved for message publishing. Unit: MB/s. Valid values: 1 to 31457280. You can specify only integers for this parameter.
+        # The reserved capacity for publishing messages. You can specify only integers for this parameter. Minimum value: 60.
+        # 
+        # >  The maximum capacity that you can reserve for an instance varies based on available resources in a region. The reserved capacity range displayed on the buy page shall prevail.
         self.reserved_publish_capacity = reserved_publish_capacity
-        # The traffic reserved for message subscription. Unit: MB/s. Valid values: 1 to 31457280. You can specify only integers for this parameter.
+        # The reserved capacity for subscribing to messages. You can specify only integers for this parameter. Minimum value: 50.
+        # 
+        # >  The maximum capacity that you can reserve for an instance varies based on available resources in a region. The reserved capacity range displayed on the buy page shall prevail.
         self.reserved_subscribe_capacity = reserved_subscribe_capacity
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9994,22 +11372,22 @@
         serverless_config: UpgradePostPayOrderRequestServerlessConfig = None,
         spec_type: str = None,
         topic_quota: int = None,
     ):
         # The disk size. Unit: GB.
         # 
         # *   The disk size that you specify must be greater than or equal to the current disk size of the instance.
-        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         # 
         # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.disk_size = disk_size
         # The Internet traffic for the instance.
         # 
         # *   The Internet traffic that you specify must be greater than or equal to the current Internet traffic of the instance.
-        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         # 
         # > 
         # 
         # *   If you set **EipModel** to **true**, set **EipMax** to a value that is greater than 0.
         # 
         # *   If you set **EipModel** to **false**, set **EipMax** to **0**.
         # 
@@ -10017,64 +11395,68 @@
         self.eip_max = eip_max
         # Specifies whether to enable Internet access for the instance. Valid values:
         # 
         # *   true: enables Internet access.
         # *   false: disables Internet access.
         self.eip_model = eip_model
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The maximum traffic for the instance. We recommend that you do not configure this parameter.
         # 
         # *   The maximum traffic that you specify must be greater than or equal to the current maximum traffic of the instance.
         # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
-        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         # 
         # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.io_max = io_max
         # The traffic specification of the instance. We recommend that you configure this parameter.
         # 
         # *   The traffic specification that you specify must be greater than or equal to the current traffic specification of the instance.
         # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
-        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         # 
         # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.io_max_spec = io_max_spec
         # The number of partitions. We recommend that you configure this parameter.
         # 
         # *   You must configure one of PartitionNum and TopicQuota. We recommend that you configure only ParittionNum.
         # *   If you configure PartitionNum and TopicQuota at the same time, the system verifies whether the price of the partitions equals the price of the topics based on the previous topic-based selling mode. If the price of the partitions does not equal the price of the topics, an error is returned. If the price of the partitions equals the price of the topics, the instance is purchased based on the partition number.
-        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         # 
         # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.partition_num = partition_num
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
-        # The parameters configured for the Serverless instance. When you create an ApsaraMQ for Kafka V3 serverless instance, you must configure these parameters.
+        # The parameters that are configured for the ApsaraMQ for Kafka serverless instance. When you create a serverless ApsaraMQ for Kafka instance, you must configure these parameters.
         self.serverless_config = serverless_config
         # The instance edition.
         # 
         # Valid values for this parameter if you set PaidType to 1:
         # 
         # *   normal: Standard Edition (High Write)
         # *   professional: Professional Edition (High Write)
         # *   professionalForHighRead: Professional Edition (High Read)
         # 
         # Valid values for this parameter if you set PaidType to 3:
         # 
         # *   normal: Serverless Standard Edition
         # *   professional: Serverless Professional Edition
         # 
-        # For more information, see [Billing](~~84737~~).
+        # For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.spec_type = spec_type
         # The number of topics. We recommend that you do not configure this parameter.
         # 
         # *   You must configure one of PartitionNum and TopicQuota. We recommend that you configure only ParittionNum.
         # *   If you configure PartitionNum and TopicQuota at the same time, the system verifies whether the price of the partitions equals the price of the topics based on the previous topic-based selling mode. If the price of the partitions does not equal the price of the topics, an error is returned. If the price of the partitions equals the price of the topics, the instance is purchased based on the partition number.
         # *   The default value of TopicQuota varies based on the value of IoMaxSpec. If the number of topics that you consume exceeds the default value, you are charged additional fees.
-        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         # 
         # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.topic_quota = topic_quota
 
     def validate(self):
         if self.serverless_config:
             self.serverless_config.validate()
@@ -10151,22 +11533,22 @@
         serverless_config_shrink: str = None,
         spec_type: str = None,
         topic_quota: int = None,
     ):
         # The disk size. Unit: GB.
         # 
         # *   The disk size that you specify must be greater than or equal to the current disk size of the instance.
-        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         # 
         # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.disk_size = disk_size
         # The Internet traffic for the instance.
         # 
         # *   The Internet traffic that you specify must be greater than or equal to the current Internet traffic of the instance.
-        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         # 
         # > 
         # 
         # *   If you set **EipModel** to **true**, set **EipMax** to a value that is greater than 0.
         # 
         # *   If you set **EipModel** to **false**, set **EipMax** to **0**.
         # 
@@ -10174,64 +11556,68 @@
         self.eip_max = eip_max
         # Specifies whether to enable Internet access for the instance. Valid values:
         # 
         # *   true: enables Internet access.
         # *   false: disables Internet access.
         self.eip_model = eip_model
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The maximum traffic for the instance. We recommend that you do not configure this parameter.
         # 
         # *   The maximum traffic that you specify must be greater than or equal to the current maximum traffic of the instance.
         # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
-        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         # 
         # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.io_max = io_max
         # The traffic specification of the instance. We recommend that you configure this parameter.
         # 
         # *   The traffic specification that you specify must be greater than or equal to the current traffic specification of the instance.
         # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
-        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         # 
         # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.io_max_spec = io_max_spec
         # The number of partitions. We recommend that you configure this parameter.
         # 
         # *   You must configure one of PartitionNum and TopicQuota. We recommend that you configure only ParittionNum.
         # *   If you configure PartitionNum and TopicQuota at the same time, the system verifies whether the price of the partitions equals the price of the topics based on the previous topic-based selling mode. If the price of the partitions does not equal the price of the topics, an error is returned. If the price of the partitions equals the price of the topics, the instance is purchased based on the partition number.
-        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         # 
         # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.partition_num = partition_num
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
-        # The parameters configured for the Serverless instance. When you create an ApsaraMQ for Kafka V3 serverless instance, you must configure these parameters.
+        # The parameters that are configured for the ApsaraMQ for Kafka serverless instance. When you create a serverless ApsaraMQ for Kafka instance, you must configure these parameters.
         self.serverless_config_shrink = serverless_config_shrink
         # The instance edition.
         # 
         # Valid values for this parameter if you set PaidType to 1:
         # 
         # *   normal: Standard Edition (High Write)
         # *   professional: Professional Edition (High Write)
         # *   professionalForHighRead: Professional Edition (High Read)
         # 
         # Valid values for this parameter if you set PaidType to 3:
         # 
         # *   normal: Serverless Standard Edition
         # *   professional: Serverless Professional Edition
         # 
-        # For more information, see [Billing](~~84737~~).
+        # For more information, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         self.spec_type = spec_type
         # The number of topics. We recommend that you do not configure this parameter.
         # 
         # *   You must configure one of PartitionNum and TopicQuota. We recommend that you configure only ParittionNum.
         # *   If you configure PartitionNum and TopicQuota at the same time, the system verifies whether the price of the partitions equals the price of the topics based on the previous topic-based selling mode. If the price of the partitions does not equal the price of the topics, an error is returned. If the price of the partitions equals the price of the topics, the instance is purchased based on the partition number.
         # *   The default value of TopicQuota varies based on the value of IoMaxSpec. If the number of topics that you consume exceeds the default value, you are charged additional fees.
-        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](https://help.aliyun.com/document_detail/84737.html).
         # 
         # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.topic_quota = topic_quota
 
     def validate(self):
         pass
 
@@ -10527,65 +11913,69 @@
         spec_type: str = None,
         topic_quota: int = None,
     ):
         self.confluent_config = confluent_config
         # The size of the disk.
         # 
         # *   The disk size that you specify must be greater than or equal to the current disk size of the instance.
-        # *   For more information about the valid values, see [Billing overview](~~84737~~).
+        # *   For more information about the valid values, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         self.disk_size = disk_size
         # The Internet traffic for the instance.
         # 
         # *   The Internet traffic volume that you specify must be greater than or equal to the current Internet traffic volume of the instance.
-        # *   For more information about the valid values, see [Billing overview](~~84737~~).
+        # *   For more information about the valid values, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         # > - If the **EipModel** parameter is set to **true**, set the **EipMax** parameter to a value that is greater than 0.
         # > - If the **EipModel** parameter is set to **false**, set the **EipMax** parameter to **0**.
         self.eip_max = eip_max
         # Specifies whether to enable Internet access for the instance. Valid values:
         # 
         # *   true: enables Internet access.
         # *   false: disables Internet access.
         self.eip_model = eip_model
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The maximum traffic for the instance. We recommend that you do not configure this parameter.
         # 
         # *   The maximum traffic volume that you specify must be greater than or equal to the current maximum traffic volume of the instance.
         # *   You must configure at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you configure only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing overview](~~84737~~).
+        # *   For more information about the valid values, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         self.io_max = io_max
         # The traffic specification of the instance. We recommend that you configure this parameter.
         # 
         # *   The traffic specification that you specify must be greater than or equal to the current traffic specification of the instance.
         # *   You must configure at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you configure only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing overview](~~84737~~).
+        # *   For more information about the valid values, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         self.io_max_spec = io_max_spec
         self.paid_type = paid_type
         # The number of partitions. We recommend that you configure this parameter.
         # 
         # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
         # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
-        # *   For more information about the valid values, see [Billing overview](~~84737~~).
+        # *   For more information about the valid values, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         self.partition_num = partition_num
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The edition of the instance. Valid values:
         # 
         # *   **normal**: Standard Edition (High Write)
         # *   **professional**: Professional Edition (High Write)
         # *   **professionalForHighRead**: Professional Edition (High Read)
         # 
-        # You cannot downgrade an instance from the Professional Edition to the Standard Edition. For more information about these instance editions, see [Billing overview](~~84737~~).
+        # You cannot downgrade an instance from the Professional Edition to the Standard Edition. For more information about these instance editions, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         self.spec_type = spec_type
         # The number of topics. We recommend that you do not configure this parameter.
         # 
         # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
         # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
         # *   The default value of the TopicQuota parameter varies based on the value of the IoMaxSpec parameter. If the number of topics that you consume exceeds the default value, you are charged additional fees.
-        # *   For more information about the valid values, see [Billing overview](~~84737~~).
+        # *   For more information about the valid values, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         self.topic_quota = topic_quota
 
     def validate(self):
         if self.confluent_config:
             self.confluent_config.validate()
 
     def to_map(self):
@@ -10666,65 +12056,69 @@
         spec_type: str = None,
         topic_quota: int = None,
     ):
         self.confluent_config_shrink = confluent_config_shrink
         # The size of the disk.
         # 
         # *   The disk size that you specify must be greater than or equal to the current disk size of the instance.
-        # *   For more information about the valid values, see [Billing overview](~~84737~~).
+        # *   For more information about the valid values, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         self.disk_size = disk_size
         # The Internet traffic for the instance.
         # 
         # *   The Internet traffic volume that you specify must be greater than or equal to the current Internet traffic volume of the instance.
-        # *   For more information about the valid values, see [Billing overview](~~84737~~).
+        # *   For more information about the valid values, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         # > - If the **EipModel** parameter is set to **true**, set the **EipMax** parameter to a value that is greater than 0.
         # > - If the **EipModel** parameter is set to **false**, set the **EipMax** parameter to **0**.
         self.eip_max = eip_max
         # Specifies whether to enable Internet access for the instance. Valid values:
         # 
         # *   true: enables Internet access.
         # *   false: disables Internet access.
         self.eip_model = eip_model
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The maximum traffic for the instance. We recommend that you do not configure this parameter.
         # 
         # *   The maximum traffic volume that you specify must be greater than or equal to the current maximum traffic volume of the instance.
         # *   You must configure at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you configure only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing overview](~~84737~~).
+        # *   For more information about the valid values, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         self.io_max = io_max
         # The traffic specification of the instance. We recommend that you configure this parameter.
         # 
         # *   The traffic specification that you specify must be greater than or equal to the current traffic specification of the instance.
         # *   You must configure at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you configure only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing overview](~~84737~~).
+        # *   For more information about the valid values, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         self.io_max_spec = io_max_spec
         self.paid_type = paid_type
         # The number of partitions. We recommend that you configure this parameter.
         # 
         # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
         # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
-        # *   For more information about the valid values, see [Billing overview](~~84737~~).
+        # *   For more information about the valid values, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         self.partition_num = partition_num
         # The region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The edition of the instance. Valid values:
         # 
         # *   **normal**: Standard Edition (High Write)
         # *   **professional**: Professional Edition (High Write)
         # *   **professionalForHighRead**: Professional Edition (High Read)
         # 
-        # You cannot downgrade an instance from the Professional Edition to the Standard Edition. For more information about these instance editions, see [Billing overview](~~84737~~).
+        # You cannot downgrade an instance from the Professional Edition to the Standard Edition. For more information about these instance editions, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         self.spec_type = spec_type
         # The number of topics. We recommend that you do not configure this parameter.
         # 
         # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
         # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
         # *   The default value of the TopicQuota parameter varies based on the value of the IoMaxSpec parameter. If the number of topics that you consume exceeds the default value, you are charged additional fees.
-        # *   For more information about the valid values, see [Billing overview](~~84737~~).
+        # *   For more information about the valid values, see [Billing overview](https://help.aliyun.com/document_detail/84737.html).
         self.topic_quota = topic_quota
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916.egg-info/PKG-INFO` & `alibabacloud_alikafka20190916-2.7.0/alibabacloud_alikafka20190916.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alikafka20190916
-Version: 2.6.6
+Version: 2.7.0
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916-2.6.6/setup.py` & `alibabacloud_alikafka20190916-2.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alikafka20190916.
 
-Created on 23/04/2024
+Created on 16/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alikafka20190916"
 NAME = "alibabacloud_alikafka20190916" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

