# Comparing `tmp/alibabacloud_expressconnectrouter20230901-3.0.1.tar.gz` & `tmp/alibabacloud_expressconnectrouter20230901-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_expressconnectrouter20230901-3.0.1.tar", last modified: Tue Mar 26 17:10:47 2024, max compression
+gzip compressed data, was "dist/alibabacloud_expressconnectrouter20230901-3.0.2.tar", last modified: Thu May 16 17:18:59 2024, max compression
```

## Comparing `alibabacloud_expressconnectrouter20230901-3.0.1.tar` & `alibabacloud_expressconnectrouter20230901-3.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/
--rw-r--r--   0 root         (0) root         (0)      355 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2520 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1163 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1248 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/alibabacloud_expressconnectrouter20230901/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/alibabacloud_expressconnectrouter20230901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112582 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/alibabacloud_expressconnectrouter20230901/client.py
--rw-r--r--   0 root         (0) root         (0)   188907 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/alibabacloud_expressconnectrouter20230901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/alibabacloud_expressconnectrouter20230901.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2520 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/alibabacloud_expressconnectrouter20230901.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/alibabacloud_expressconnectrouter20230901.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/alibabacloud_expressconnectrouter20230901.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/alibabacloud_expressconnectrouter20230901.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/alibabacloud_expressconnectrouter20230901.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2696 2024-03-26 17:10:47.000000 alibabacloud_expressconnectrouter20230901-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:18:59.000000 alibabacloud_expressconnectrouter20230901-3.0.2/
+-rw-r--r--   0 root         (0) root         (0)      462 2024-05-16 17:18:58.000000 alibabacloud_expressconnectrouter20230901-3.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-16 17:18:58.000000 alibabacloud_expressconnectrouter20230901-3.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-16 17:18:58.000000 alibabacloud_expressconnectrouter20230901-3.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-05-16 17:18:59.000000 alibabacloud_expressconnectrouter20230901-3.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1163 2024-05-16 17:18:58.000000 alibabacloud_expressconnectrouter20230901-3.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1248 2024-05-16 17:18:58.000000 alibabacloud_expressconnectrouter20230901-3.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:18:59.000000 alibabacloud_expressconnectrouter20230901-3.0.2/alibabacloud_expressconnectrouter20230901/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-16 17:18:58.000000 alibabacloud_expressconnectrouter20230901-3.0.2/alibabacloud_expressconnectrouter20230901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   133098 2024-05-16 17:18:58.000000 alibabacloud_expressconnectrouter20230901-3.0.2/alibabacloud_expressconnectrouter20230901/client.py
+-rw-r--r--   0 root         (0) root         (0)   191998 2024-05-16 17:18:58.000000 alibabacloud_expressconnectrouter20230901-3.0.2/alibabacloud_expressconnectrouter20230901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:18:59.000000 alibabacloud_expressconnectrouter20230901-3.0.2/alibabacloud_expressconnectrouter20230901.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-05-16 17:18:59.000000 alibabacloud_expressconnectrouter20230901-3.0.2/alibabacloud_expressconnectrouter20230901.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2024-05-16 17:18:59.000000 alibabacloud_expressconnectrouter20230901-3.0.2/alibabacloud_expressconnectrouter20230901.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 17:18:59.000000 alibabacloud_expressconnectrouter20230901-3.0.2/alibabacloud_expressconnectrouter20230901.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-16 17:18:59.000000 alibabacloud_expressconnectrouter20230901-3.0.2/alibabacloud_expressconnectrouter20230901.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-16 17:18:59.000000 alibabacloud_expressconnectrouter20230901-3.0.2/alibabacloud_expressconnectrouter20230901.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-16 17:18:59.000000 alibabacloud_expressconnectrouter20230901-3.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2696 2024-05-16 17:18:58.000000 alibabacloud_expressconnectrouter20230901-3.0.2/setup.py
```

### Comparing `alibabacloud_expressconnectrouter20230901-3.0.1/LICENSE` & `alibabacloud_expressconnectrouter20230901-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_expressconnectrouter20230901-3.0.1/PKG-INFO` & `alibabacloud_expressconnectrouter20230901-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_expressconnectrouter20230901
-Version: 3.0.1
+Version: 3.0.2
 Summary: Alibaba Cloud ExpressConnectRouter (20230901) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_expressconnectrouter20230901-3.0.1/README-CN.md` & `alibabacloud_expressconnectrouter20230901-3.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_expressconnectrouter20230901-3.0.1/README.md` & `alibabacloud_expressconnectrouter20230901-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_expressconnectrouter20230901-3.0.1/alibabacloud_expressconnectrouter20230901/client.py` & `alibabacloud_expressconnectrouter20230901-3.0.2/alibabacloud_expressconnectrouter20230901/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,14 +42,19 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def attach_express_connect_router_child_instance_with_options(
         self,
         request: express_connect_router_20230901_models.AttachExpressConnectRouterChildInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.AttachExpressConnectRouterChildInstanceResponse:
+        """
+        @param request: AttachExpressConnectRouterChildInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AttachExpressConnectRouterChildInstanceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.child_instance_id):
             body['ChildInstanceId'] = request.child_instance_id
         if not UtilClient.is_unset(request.child_instance_owner_id):
             body['ChildInstanceOwnerId'] = request.child_instance_owner_id
         if not UtilClient.is_unset(request.child_instance_region_id):
@@ -82,14 +87,19 @@
         )
 
     async def attach_express_connect_router_child_instance_with_options_async(
         self,
         request: express_connect_router_20230901_models.AttachExpressConnectRouterChildInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.AttachExpressConnectRouterChildInstanceResponse:
+        """
+        @param request: AttachExpressConnectRouterChildInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AttachExpressConnectRouterChildInstanceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.child_instance_id):
             body['ChildInstanceId'] = request.child_instance_id
         if not UtilClient.is_unset(request.child_instance_owner_id):
             body['ChildInstanceOwnerId'] = request.child_instance_owner_id
         if not UtilClient.is_unset(request.child_instance_region_id):
@@ -121,29 +131,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def attach_express_connect_router_child_instance(
         self,
         request: express_connect_router_20230901_models.AttachExpressConnectRouterChildInstanceRequest,
     ) -> express_connect_router_20230901_models.AttachExpressConnectRouterChildInstanceResponse:
+        """
+        @param request: AttachExpressConnectRouterChildInstanceRequest
+        @return: AttachExpressConnectRouterChildInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.attach_express_connect_router_child_instance_with_options(request, runtime)
 
     async def attach_express_connect_router_child_instance_async(
         self,
         request: express_connect_router_20230901_models.AttachExpressConnectRouterChildInstanceRequest,
     ) -> express_connect_router_20230901_models.AttachExpressConnectRouterChildInstanceResponse:
+        """
+        @param request: AttachExpressConnectRouterChildInstanceRequest
+        @return: AttachExpressConnectRouterChildInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.attach_express_connect_router_child_instance_with_options_async(request, runtime)
 
     def check_add_region_to_express_connect_router_with_options(
         self,
         request: express_connect_router_20230901_models.CheckAddRegionToExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.CheckAddRegionToExpressConnectRouterResponse:
+        """
+        @param request: CheckAddRegionToExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CheckAddRegionToExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -170,14 +193,19 @@
         )
 
     async def check_add_region_to_express_connect_router_with_options_async(
         self,
         request: express_connect_router_20230901_models.CheckAddRegionToExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.CheckAddRegionToExpressConnectRouterResponse:
+        """
+        @param request: CheckAddRegionToExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CheckAddRegionToExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -203,43 +231,58 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def check_add_region_to_express_connect_router(
         self,
         request: express_connect_router_20230901_models.CheckAddRegionToExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.CheckAddRegionToExpressConnectRouterResponse:
+        """
+        @param request: CheckAddRegionToExpressConnectRouterRequest
+        @return: CheckAddRegionToExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.check_add_region_to_express_connect_router_with_options(request, runtime)
 
     async def check_add_region_to_express_connect_router_async(
         self,
         request: express_connect_router_20230901_models.CheckAddRegionToExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.CheckAddRegionToExpressConnectRouterResponse:
+        """
+        @param request: CheckAddRegionToExpressConnectRouterRequest
+        @return: CheckAddRegionToExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.check_add_region_to_express_connect_router_with_options_async(request, runtime)
 
     def create_express_connect_router_with_options(
         self,
         request: express_connect_router_20230901_models.CreateExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.CreateExpressConnectRouterResponse:
+        """
+        @param request: CreateExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.alibaba_side_asn):
             body['AlibabaSideAsn'] = request.alibaba_side_asn
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.resource_group_id):
             body['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.tags):
+            body['Tags'] = request.tags
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CreateExpressConnectRouter',
             version='2023-09-01',
             protocol='HTTPS',
@@ -256,28 +299,35 @@
         )
 
     async def create_express_connect_router_with_options_async(
         self,
         request: express_connect_router_20230901_models.CreateExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.CreateExpressConnectRouterResponse:
+        """
+        @param request: CreateExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.alibaba_side_asn):
             body['AlibabaSideAsn'] = request.alibaba_side_asn
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.resource_group_id):
             body['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.tags):
+            body['Tags'] = request.tags
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CreateExpressConnectRouter',
             version='2023-09-01',
             protocol='HTTPS',
@@ -293,29 +343,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_express_connect_router(
         self,
         request: express_connect_router_20230901_models.CreateExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.CreateExpressConnectRouterResponse:
+        """
+        @param request: CreateExpressConnectRouterRequest
+        @return: CreateExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_express_connect_router_with_options(request, runtime)
 
     async def create_express_connect_router_async(
         self,
         request: express_connect_router_20230901_models.CreateExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.CreateExpressConnectRouterResponse:
+        """
+        @param request: CreateExpressConnectRouterRequest
+        @return: CreateExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_express_connect_router_with_options_async(request, runtime)
 
     def create_express_connect_router_association_with_options(
         self,
         request: express_connect_router_20230901_models.CreateExpressConnectRouterAssociationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.CreateExpressConnectRouterAssociationResponse:
+        """
+        @param request: CreateExpressConnectRouterAssociationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateExpressConnectRouterAssociationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.allowed_prefixes):
             body['AllowedPrefixes'] = request.allowed_prefixes
         if not UtilClient.is_unset(request.association_region_id):
             body['AssociationRegionId'] = request.association_region_id
         if not UtilClient.is_unset(request.cen_id):
@@ -356,14 +419,19 @@
         )
 
     async def create_express_connect_router_association_with_options_async(
         self,
         request: express_connect_router_20230901_models.CreateExpressConnectRouterAssociationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.CreateExpressConnectRouterAssociationResponse:
+        """
+        @param request: CreateExpressConnectRouterAssociationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateExpressConnectRouterAssociationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.allowed_prefixes):
             body['AllowedPrefixes'] = request.allowed_prefixes
         if not UtilClient.is_unset(request.association_region_id):
             body['AssociationRegionId'] = request.association_region_id
         if not UtilClient.is_unset(request.cen_id):
@@ -403,29 +471,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_express_connect_router_association(
         self,
         request: express_connect_router_20230901_models.CreateExpressConnectRouterAssociationRequest,
     ) -> express_connect_router_20230901_models.CreateExpressConnectRouterAssociationResponse:
+        """
+        @param request: CreateExpressConnectRouterAssociationRequest
+        @return: CreateExpressConnectRouterAssociationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_express_connect_router_association_with_options(request, runtime)
 
     async def create_express_connect_router_association_async(
         self,
         request: express_connect_router_20230901_models.CreateExpressConnectRouterAssociationRequest,
     ) -> express_connect_router_20230901_models.CreateExpressConnectRouterAssociationResponse:
+        """
+        @param request: CreateExpressConnectRouterAssociationRequest
+        @return: CreateExpressConnectRouterAssociationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_express_connect_router_association_with_options_async(request, runtime)
 
     def delete_express_connect_router_with_options(
         self,
         request: express_connect_router_20230901_models.DeleteExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DeleteExpressConnectRouterResponse:
+        """
+        @param request: DeleteExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -450,14 +531,19 @@
         )
 
     async def delete_express_connect_router_with_options_async(
         self,
         request: express_connect_router_20230901_models.DeleteExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DeleteExpressConnectRouterResponse:
+        """
+        @param request: DeleteExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -481,29 +567,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_express_connect_router(
         self,
         request: express_connect_router_20230901_models.DeleteExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.DeleteExpressConnectRouterResponse:
+        """
+        @param request: DeleteExpressConnectRouterRequest
+        @return: DeleteExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_express_connect_router_with_options(request, runtime)
 
     async def delete_express_connect_router_async(
         self,
         request: express_connect_router_20230901_models.DeleteExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.DeleteExpressConnectRouterResponse:
+        """
+        @param request: DeleteExpressConnectRouterRequest
+        @return: DeleteExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_express_connect_router_with_options_async(request, runtime)
 
     def delete_express_connect_router_association_with_options(
         self,
         request: express_connect_router_20230901_models.DeleteExpressConnectRouterAssociationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DeleteExpressConnectRouterAssociationResponse:
+        """
+        @param request: DeleteExpressConnectRouterAssociationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteExpressConnectRouterAssociationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.association_id):
             body['AssociationId'] = request.association_id
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.delete_attachment):
@@ -532,14 +631,19 @@
         )
 
     async def delete_express_connect_router_association_with_options_async(
         self,
         request: express_connect_router_20230901_models.DeleteExpressConnectRouterAssociationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DeleteExpressConnectRouterAssociationResponse:
+        """
+        @param request: DeleteExpressConnectRouterAssociationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteExpressConnectRouterAssociationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.association_id):
             body['AssociationId'] = request.association_id
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.delete_attachment):
@@ -567,29 +671,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_express_connect_router_association(
         self,
         request: express_connect_router_20230901_models.DeleteExpressConnectRouterAssociationRequest,
     ) -> express_connect_router_20230901_models.DeleteExpressConnectRouterAssociationResponse:
+        """
+        @param request: DeleteExpressConnectRouterAssociationRequest
+        @return: DeleteExpressConnectRouterAssociationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_express_connect_router_association_with_options(request, runtime)
 
     async def delete_express_connect_router_association_async(
         self,
         request: express_connect_router_20230901_models.DeleteExpressConnectRouterAssociationRequest,
     ) -> express_connect_router_20230901_models.DeleteExpressConnectRouterAssociationResponse:
+        """
+        @param request: DeleteExpressConnectRouterAssociationRequest
+        @return: DeleteExpressConnectRouterAssociationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_express_connect_router_association_with_options_async(request, runtime)
 
     def describe_disabled_express_connect_router_route_entries_with_options(
         self,
         request: express_connect_router_20230901_models.DescribeDisabledExpressConnectRouterRouteEntriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeDisabledExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: DescribeDisabledExpressConnectRouterRouteEntriesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDisabledExpressConnectRouterRouteEntriesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -618,14 +735,19 @@
         )
 
     async def describe_disabled_express_connect_router_route_entries_with_options_async(
         self,
         request: express_connect_router_20230901_models.DescribeDisabledExpressConnectRouterRouteEntriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeDisabledExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: DescribeDisabledExpressConnectRouterRouteEntriesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDisabledExpressConnectRouterRouteEntriesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -653,29 +775,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_disabled_express_connect_router_route_entries(
         self,
         request: express_connect_router_20230901_models.DescribeDisabledExpressConnectRouterRouteEntriesRequest,
     ) -> express_connect_router_20230901_models.DescribeDisabledExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: DescribeDisabledExpressConnectRouterRouteEntriesRequest
+        @return: DescribeDisabledExpressConnectRouterRouteEntriesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_disabled_express_connect_router_route_entries_with_options(request, runtime)
 
     async def describe_disabled_express_connect_router_route_entries_async(
         self,
         request: express_connect_router_20230901_models.DescribeDisabledExpressConnectRouterRouteEntriesRequest,
     ) -> express_connect_router_20230901_models.DescribeDisabledExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: DescribeDisabledExpressConnectRouterRouteEntriesRequest
+        @return: DescribeDisabledExpressConnectRouterRouteEntriesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_disabled_express_connect_router_route_entries_with_options_async(request, runtime)
 
     def describe_express_connect_router_with_options(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterResponse:
+        """
+        @param request: DescribeExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -710,14 +845,19 @@
         )
 
     async def describe_express_connect_router_with_options_async(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterResponse:
+        """
+        @param request: DescribeExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -751,29 +891,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_express_connect_router(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterResponse:
+        """
+        @param request: DescribeExpressConnectRouterRequest
+        @return: DescribeExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_express_connect_router_with_options(request, runtime)
 
     async def describe_express_connect_router_async(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterResponse:
+        """
+        @param request: DescribeExpressConnectRouterRequest
+        @return: DescribeExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_express_connect_router_with_options_async(request, runtime)
 
     def describe_express_connect_router_allowed_prefix_history_with_options(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterAllowedPrefixHistoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterAllowedPrefixHistoryResponse:
+        """
+        @param request: DescribeExpressConnectRouterAllowedPrefixHistoryRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeExpressConnectRouterAllowedPrefixHistoryResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.association_id):
             body['AssociationId'] = request.association_id
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
@@ -804,14 +957,19 @@
         )
 
     async def describe_express_connect_router_allowed_prefix_history_with_options_async(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterAllowedPrefixHistoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterAllowedPrefixHistoryResponse:
+        """
+        @param request: DescribeExpressConnectRouterAllowedPrefixHistoryRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeExpressConnectRouterAllowedPrefixHistoryResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.association_id):
             body['AssociationId'] = request.association_id
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
@@ -841,29 +999,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_express_connect_router_allowed_prefix_history(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterAllowedPrefixHistoryRequest,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterAllowedPrefixHistoryResponse:
+        """
+        @param request: DescribeExpressConnectRouterAllowedPrefixHistoryRequest
+        @return: DescribeExpressConnectRouterAllowedPrefixHistoryResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_express_connect_router_allowed_prefix_history_with_options(request, runtime)
 
     async def describe_express_connect_router_allowed_prefix_history_async(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterAllowedPrefixHistoryRequest,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterAllowedPrefixHistoryResponse:
+        """
+        @param request: DescribeExpressConnectRouterAllowedPrefixHistoryRequest
+        @return: DescribeExpressConnectRouterAllowedPrefixHistoryResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_express_connect_router_allowed_prefix_history_with_options_async(request, runtime)
 
     def describe_express_connect_router_association_with_options(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterAssociationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterAssociationResponse:
+        """
+        @param request: DescribeExpressConnectRouterAssociationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeExpressConnectRouterAssociationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.association_id):
             body['AssociationId'] = request.association_id
         if not UtilClient.is_unset(request.association_node_type):
             body['AssociationNodeType'] = request.association_node_type
         if not UtilClient.is_unset(request.association_region_id):
@@ -904,14 +1075,19 @@
         )
 
     async def describe_express_connect_router_association_with_options_async(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterAssociationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterAssociationResponse:
+        """
+        @param request: DescribeExpressConnectRouterAssociationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeExpressConnectRouterAssociationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.association_id):
             body['AssociationId'] = request.association_id
         if not UtilClient.is_unset(request.association_node_type):
             body['AssociationNodeType'] = request.association_node_type
         if not UtilClient.is_unset(request.association_region_id):
@@ -951,29 +1127,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_express_connect_router_association(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterAssociationRequest,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterAssociationResponse:
+        """
+        @param request: DescribeExpressConnectRouterAssociationRequest
+        @return: DescribeExpressConnectRouterAssociationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_express_connect_router_association_with_options(request, runtime)
 
     async def describe_express_connect_router_association_async(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterAssociationRequest,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterAssociationResponse:
+        """
+        @param request: DescribeExpressConnectRouterAssociationRequest
+        @return: DescribeExpressConnectRouterAssociationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_express_connect_router_association_with_options_async(request, runtime)
 
     def describe_express_connect_router_child_instance_with_options(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterChildInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterChildInstanceResponse:
+        """
+        @param request: DescribeExpressConnectRouterChildInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeExpressConnectRouterChildInstanceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.association_id):
             body['AssociationId'] = request.association_id
         if not UtilClient.is_unset(request.child_instance_id):
             body['ChildInstanceId'] = request.child_instance_id
         if not UtilClient.is_unset(request.child_instance_region_id):
@@ -1010,14 +1199,19 @@
         )
 
     async def describe_express_connect_router_child_instance_with_options_async(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterChildInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterChildInstanceResponse:
+        """
+        @param request: DescribeExpressConnectRouterChildInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeExpressConnectRouterChildInstanceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.association_id):
             body['AssociationId'] = request.association_id
         if not UtilClient.is_unset(request.child_instance_id):
             body['ChildInstanceId'] = request.child_instance_id
         if not UtilClient.is_unset(request.child_instance_region_id):
@@ -1053,29 +1247,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_express_connect_router_child_instance(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterChildInstanceRequest,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterChildInstanceResponse:
+        """
+        @param request: DescribeExpressConnectRouterChildInstanceRequest
+        @return: DescribeExpressConnectRouterChildInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_express_connect_router_child_instance_with_options(request, runtime)
 
     async def describe_express_connect_router_child_instance_async(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterChildInstanceRequest,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterChildInstanceResponse:
+        """
+        @param request: DescribeExpressConnectRouterChildInstanceRequest
+        @return: DescribeExpressConnectRouterChildInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_express_connect_router_child_instance_with_options_async(request, runtime)
 
     def describe_express_connect_router_inter_region_transit_mode_with_options(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterInterRegionTransitModeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterInterRegionTransitModeResponse:
+        """
+        @param request: DescribeExpressConnectRouterInterRegionTransitModeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeExpressConnectRouterInterRegionTransitModeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -1100,14 +1307,19 @@
         )
 
     async def describe_express_connect_router_inter_region_transit_mode_with_options_async(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterInterRegionTransitModeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterInterRegionTransitModeResponse:
+        """
+        @param request: DescribeExpressConnectRouterInterRegionTransitModeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeExpressConnectRouterInterRegionTransitModeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -1131,29 +1343,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_express_connect_router_inter_region_transit_mode(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterInterRegionTransitModeRequest,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterInterRegionTransitModeResponse:
+        """
+        @param request: DescribeExpressConnectRouterInterRegionTransitModeRequest
+        @return: DescribeExpressConnectRouterInterRegionTransitModeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_express_connect_router_inter_region_transit_mode_with_options(request, runtime)
 
     async def describe_express_connect_router_inter_region_transit_mode_async(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterInterRegionTransitModeRequest,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterInterRegionTransitModeResponse:
+        """
+        @param request: DescribeExpressConnectRouterInterRegionTransitModeRequest
+        @return: DescribeExpressConnectRouterInterRegionTransitModeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_express_connect_router_inter_region_transit_mode_with_options_async(request, runtime)
 
     def describe_express_connect_router_region_with_options(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterRegionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterRegionResponse:
+        """
+        @param request: DescribeExpressConnectRouterRegionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeExpressConnectRouterRegionResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -1178,14 +1403,19 @@
         )
 
     async def describe_express_connect_router_region_with_options_async(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterRegionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterRegionResponse:
+        """
+        @param request: DescribeExpressConnectRouterRegionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeExpressConnectRouterRegionResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -1209,29 +1439,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_express_connect_router_region(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterRegionRequest,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterRegionResponse:
+        """
+        @param request: DescribeExpressConnectRouterRegionRequest
+        @return: DescribeExpressConnectRouterRegionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_express_connect_router_region_with_options(request, runtime)
 
     async def describe_express_connect_router_region_async(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterRegionRequest,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterRegionResponse:
+        """
+        @param request: DescribeExpressConnectRouterRegionRequest
+        @return: DescribeExpressConnectRouterRegionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_express_connect_router_region_with_options_async(request, runtime)
 
     def describe_express_connect_router_route_entries_with_options(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterRouteEntriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: DescribeExpressConnectRouterRouteEntriesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeExpressConnectRouterRouteEntriesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.as_path):
             body['AsPath'] = request.as_path
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.community):
@@ -1270,14 +1513,19 @@
         )
 
     async def describe_express_connect_router_route_entries_with_options_async(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterRouteEntriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: DescribeExpressConnectRouterRouteEntriesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeExpressConnectRouterRouteEntriesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.as_path):
             body['AsPath'] = request.as_path
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.community):
@@ -1315,29 +1563,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_express_connect_router_route_entries(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterRouteEntriesRequest,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: DescribeExpressConnectRouterRouteEntriesRequest
+        @return: DescribeExpressConnectRouterRouteEntriesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_express_connect_router_route_entries_with_options(request, runtime)
 
     async def describe_express_connect_router_route_entries_async(
         self,
         request: express_connect_router_20230901_models.DescribeExpressConnectRouterRouteEntriesRequest,
     ) -> express_connect_router_20230901_models.DescribeExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: DescribeExpressConnectRouterRouteEntriesRequest
+        @return: DescribeExpressConnectRouterRouteEntriesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_express_connect_router_route_entries_with_options_async(request, runtime)
 
     def describe_instance_granted_to_express_connect_router_with_options(
         self,
         request: express_connect_router_20230901_models.DescribeInstanceGrantedToExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeInstanceGrantedToExpressConnectRouterResponse:
+        """
+        @param request: DescribeInstanceGrantedToExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeInstanceGrantedToExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -1378,14 +1639,19 @@
         )
 
     async def describe_instance_granted_to_express_connect_router_with_options_async(
         self,
         request: express_connect_router_20230901_models.DescribeInstanceGrantedToExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DescribeInstanceGrantedToExpressConnectRouterResponse:
+        """
+        @param request: DescribeInstanceGrantedToExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeInstanceGrantedToExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -1425,29 +1691,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_instance_granted_to_express_connect_router(
         self,
         request: express_connect_router_20230901_models.DescribeInstanceGrantedToExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.DescribeInstanceGrantedToExpressConnectRouterResponse:
+        """
+        @param request: DescribeInstanceGrantedToExpressConnectRouterRequest
+        @return: DescribeInstanceGrantedToExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_instance_granted_to_express_connect_router_with_options(request, runtime)
 
     async def describe_instance_granted_to_express_connect_router_async(
         self,
         request: express_connect_router_20230901_models.DescribeInstanceGrantedToExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.DescribeInstanceGrantedToExpressConnectRouterResponse:
+        """
+        @param request: DescribeInstanceGrantedToExpressConnectRouterRequest
+        @return: DescribeInstanceGrantedToExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_instance_granted_to_express_connect_router_with_options_async(request, runtime)
 
     def detach_express_connect_router_child_instance_with_options(
         self,
         request: express_connect_router_20230901_models.DetachExpressConnectRouterChildInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DetachExpressConnectRouterChildInstanceResponse:
+        """
+        @param request: DetachExpressConnectRouterChildInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DetachExpressConnectRouterChildInstanceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.child_instance_id):
             body['ChildInstanceId'] = request.child_instance_id
         if not UtilClient.is_unset(request.child_instance_type):
             body['ChildInstanceType'] = request.child_instance_type
         if not UtilClient.is_unset(request.client_token):
@@ -1476,14 +1755,19 @@
         )
 
     async def detach_express_connect_router_child_instance_with_options_async(
         self,
         request: express_connect_router_20230901_models.DetachExpressConnectRouterChildInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DetachExpressConnectRouterChildInstanceResponse:
+        """
+        @param request: DetachExpressConnectRouterChildInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DetachExpressConnectRouterChildInstanceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.child_instance_id):
             body['ChildInstanceId'] = request.child_instance_id
         if not UtilClient.is_unset(request.child_instance_type):
             body['ChildInstanceType'] = request.child_instance_type
         if not UtilClient.is_unset(request.client_token):
@@ -1511,29 +1795,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def detach_express_connect_router_child_instance(
         self,
         request: express_connect_router_20230901_models.DetachExpressConnectRouterChildInstanceRequest,
     ) -> express_connect_router_20230901_models.DetachExpressConnectRouterChildInstanceResponse:
+        """
+        @param request: DetachExpressConnectRouterChildInstanceRequest
+        @return: DetachExpressConnectRouterChildInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.detach_express_connect_router_child_instance_with_options(request, runtime)
 
     async def detach_express_connect_router_child_instance_async(
         self,
         request: express_connect_router_20230901_models.DetachExpressConnectRouterChildInstanceRequest,
     ) -> express_connect_router_20230901_models.DetachExpressConnectRouterChildInstanceResponse:
+        """
+        @param request: DetachExpressConnectRouterChildInstanceRequest
+        @return: DetachExpressConnectRouterChildInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.detach_express_connect_router_child_instance_with_options_async(request, runtime)
 
     def disable_express_connect_router_route_entries_with_options(
         self,
         request: express_connect_router_20230901_models.DisableExpressConnectRouterRouteEntriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DisableExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: DisableExpressConnectRouterRouteEntriesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DisableExpressConnectRouterRouteEntriesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.destination_cidr_block):
             body['DestinationCidrBlock'] = request.destination_cidr_block
         if not UtilClient.is_unset(request.dry_run):
@@ -1562,14 +1859,19 @@
         )
 
     async def disable_express_connect_router_route_entries_with_options_async(
         self,
         request: express_connect_router_20230901_models.DisableExpressConnectRouterRouteEntriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.DisableExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: DisableExpressConnectRouterRouteEntriesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DisableExpressConnectRouterRouteEntriesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.destination_cidr_block):
             body['DestinationCidrBlock'] = request.destination_cidr_block
         if not UtilClient.is_unset(request.dry_run):
@@ -1597,29 +1899,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def disable_express_connect_router_route_entries(
         self,
         request: express_connect_router_20230901_models.DisableExpressConnectRouterRouteEntriesRequest,
     ) -> express_connect_router_20230901_models.DisableExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: DisableExpressConnectRouterRouteEntriesRequest
+        @return: DisableExpressConnectRouterRouteEntriesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.disable_express_connect_router_route_entries_with_options(request, runtime)
 
     async def disable_express_connect_router_route_entries_async(
         self,
         request: express_connect_router_20230901_models.DisableExpressConnectRouterRouteEntriesRequest,
     ) -> express_connect_router_20230901_models.DisableExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: DisableExpressConnectRouterRouteEntriesRequest
+        @return: DisableExpressConnectRouterRouteEntriesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.disable_express_connect_router_route_entries_with_options_async(request, runtime)
 
     def enable_express_connect_router_route_entries_with_options(
         self,
         request: express_connect_router_20230901_models.EnableExpressConnectRouterRouteEntriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.EnableExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: EnableExpressConnectRouterRouteEntriesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableExpressConnectRouterRouteEntriesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.destination_cidr_block):
             body['DestinationCidrBlock'] = request.destination_cidr_block
         if not UtilClient.is_unset(request.dry_run):
@@ -1648,14 +1963,19 @@
         )
 
     async def enable_express_connect_router_route_entries_with_options_async(
         self,
         request: express_connect_router_20230901_models.EnableExpressConnectRouterRouteEntriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.EnableExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: EnableExpressConnectRouterRouteEntriesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableExpressConnectRouterRouteEntriesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.destination_cidr_block):
             body['DestinationCidrBlock'] = request.destination_cidr_block
         if not UtilClient.is_unset(request.dry_run):
@@ -1683,29 +2003,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def enable_express_connect_router_route_entries(
         self,
         request: express_connect_router_20230901_models.EnableExpressConnectRouterRouteEntriesRequest,
     ) -> express_connect_router_20230901_models.EnableExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: EnableExpressConnectRouterRouteEntriesRequest
+        @return: EnableExpressConnectRouterRouteEntriesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.enable_express_connect_router_route_entries_with_options(request, runtime)
 
     async def enable_express_connect_router_route_entries_async(
         self,
         request: express_connect_router_20230901_models.EnableExpressConnectRouterRouteEntriesRequest,
     ) -> express_connect_router_20230901_models.EnableExpressConnectRouterRouteEntriesResponse:
+        """
+        @param request: EnableExpressConnectRouterRouteEntriesRequest
+        @return: EnableExpressConnectRouterRouteEntriesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.enable_express_connect_router_route_entries_with_options_async(request, runtime)
 
     def force_delete_express_connect_router_with_options(
         self,
         request: express_connect_router_20230901_models.ForceDeleteExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.ForceDeleteExpressConnectRouterResponse:
+        """
+        @param request: ForceDeleteExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ForceDeleteExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -1730,14 +2063,19 @@
         )
 
     async def force_delete_express_connect_router_with_options_async(
         self,
         request: express_connect_router_20230901_models.ForceDeleteExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.ForceDeleteExpressConnectRouterResponse:
+        """
+        @param request: ForceDeleteExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ForceDeleteExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -1761,29 +2099,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def force_delete_express_connect_router(
         self,
         request: express_connect_router_20230901_models.ForceDeleteExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.ForceDeleteExpressConnectRouterResponse:
+        """
+        @param request: ForceDeleteExpressConnectRouterRequest
+        @return: ForceDeleteExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.force_delete_express_connect_router_with_options(request, runtime)
 
     async def force_delete_express_connect_router_async(
         self,
         request: express_connect_router_20230901_models.ForceDeleteExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.ForceDeleteExpressConnectRouterResponse:
+        """
+        @param request: ForceDeleteExpressConnectRouterRequest
+        @return: ForceDeleteExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.force_delete_express_connect_router_with_options_async(request, runtime)
 
     def grant_instance_to_express_connect_router_with_options(
         self,
         request: express_connect_router_20230901_models.GrantInstanceToExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.GrantInstanceToExpressConnectRouterResponse:
+        """
+        @param request: GrantInstanceToExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GrantInstanceToExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -1816,14 +2167,19 @@
         )
 
     async def grant_instance_to_express_connect_router_with_options_async(
         self,
         request: express_connect_router_20230901_models.GrantInstanceToExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.GrantInstanceToExpressConnectRouterResponse:
+        """
+        @param request: GrantInstanceToExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GrantInstanceToExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -1855,29 +2211,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def grant_instance_to_express_connect_router(
         self,
         request: express_connect_router_20230901_models.GrantInstanceToExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.GrantInstanceToExpressConnectRouterResponse:
+        """
+        @param request: GrantInstanceToExpressConnectRouterRequest
+        @return: GrantInstanceToExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.grant_instance_to_express_connect_router_with_options(request, runtime)
 
     async def grant_instance_to_express_connect_router_async(
         self,
         request: express_connect_router_20230901_models.GrantInstanceToExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.GrantInstanceToExpressConnectRouterResponse:
+        """
+        @param request: GrantInstanceToExpressConnectRouterRequest
+        @return: GrantInstanceToExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.grant_instance_to_express_connect_router_with_options_async(request, runtime)
 
     def list_express_connect_router_supported_region_with_options(
         self,
         request: express_connect_router_20230901_models.ListExpressConnectRouterSupportedRegionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.ListExpressConnectRouterSupportedRegionResponse:
+        """
+        @param request: ListExpressConnectRouterSupportedRegionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListExpressConnectRouterSupportedRegionResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.node_type):
             body['NodeType'] = request.node_type
         req = open_api_models.OpenApiRequest(
@@ -1900,14 +2269,19 @@
         )
 
     async def list_express_connect_router_supported_region_with_options_async(
         self,
         request: express_connect_router_20230901_models.ListExpressConnectRouterSupportedRegionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.ListExpressConnectRouterSupportedRegionResponse:
+        """
+        @param request: ListExpressConnectRouterSupportedRegionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListExpressConnectRouterSupportedRegionResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.node_type):
             body['NodeType'] = request.node_type
         req = open_api_models.OpenApiRequest(
@@ -1929,29 +2303,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_express_connect_router_supported_region(
         self,
         request: express_connect_router_20230901_models.ListExpressConnectRouterSupportedRegionRequest,
     ) -> express_connect_router_20230901_models.ListExpressConnectRouterSupportedRegionResponse:
+        """
+        @param request: ListExpressConnectRouterSupportedRegionRequest
+        @return: ListExpressConnectRouterSupportedRegionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_express_connect_router_supported_region_with_options(request, runtime)
 
     async def list_express_connect_router_supported_region_async(
         self,
         request: express_connect_router_20230901_models.ListExpressConnectRouterSupportedRegionRequest,
     ) -> express_connect_router_20230901_models.ListExpressConnectRouterSupportedRegionResponse:
+        """
+        @param request: ListExpressConnectRouterSupportedRegionRequest
+        @return: ListExpressConnectRouterSupportedRegionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_express_connect_router_supported_region_with_options_async(request, runtime)
 
     def modify_express_connect_router_with_options(
         self,
         request: express_connect_router_20230901_models.ModifyExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.ModifyExpressConnectRouterResponse:
+        """
+        @param request: ModifyExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.dry_run):
@@ -1980,14 +2367,19 @@
         )
 
     async def modify_express_connect_router_with_options_async(
         self,
         request: express_connect_router_20230901_models.ModifyExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.ModifyExpressConnectRouterResponse:
+        """
+        @param request: ModifyExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.dry_run):
@@ -2015,29 +2407,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_express_connect_router(
         self,
         request: express_connect_router_20230901_models.ModifyExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.ModifyExpressConnectRouterResponse:
+        """
+        @param request: ModifyExpressConnectRouterRequest
+        @return: ModifyExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_express_connect_router_with_options(request, runtime)
 
     async def modify_express_connect_router_async(
         self,
         request: express_connect_router_20230901_models.ModifyExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.ModifyExpressConnectRouterResponse:
+        """
+        @param request: ModifyExpressConnectRouterRequest
+        @return: ModifyExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_express_connect_router_with_options_async(request, runtime)
 
     def modify_express_connect_router_association_allowed_prefix_with_options(
         self,
         request: express_connect_router_20230901_models.ModifyExpressConnectRouterAssociationAllowedPrefixRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.ModifyExpressConnectRouterAssociationAllowedPrefixResponse:
+        """
+        @param request: ModifyExpressConnectRouterAssociationAllowedPrefixRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyExpressConnectRouterAssociationAllowedPrefixResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.allowed_prefixes):
             body['AllowedPrefixes'] = request.allowed_prefixes
         if not UtilClient.is_unset(request.association_id):
             body['AssociationId'] = request.association_id
         if not UtilClient.is_unset(request.client_token):
@@ -2068,14 +2473,19 @@
         )
 
     async def modify_express_connect_router_association_allowed_prefix_with_options_async(
         self,
         request: express_connect_router_20230901_models.ModifyExpressConnectRouterAssociationAllowedPrefixRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.ModifyExpressConnectRouterAssociationAllowedPrefixResponse:
+        """
+        @param request: ModifyExpressConnectRouterAssociationAllowedPrefixRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyExpressConnectRouterAssociationAllowedPrefixResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.allowed_prefixes):
             body['AllowedPrefixes'] = request.allowed_prefixes
         if not UtilClient.is_unset(request.association_id):
             body['AssociationId'] = request.association_id
         if not UtilClient.is_unset(request.client_token):
@@ -2105,29 +2515,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_express_connect_router_association_allowed_prefix(
         self,
         request: express_connect_router_20230901_models.ModifyExpressConnectRouterAssociationAllowedPrefixRequest,
     ) -> express_connect_router_20230901_models.ModifyExpressConnectRouterAssociationAllowedPrefixResponse:
+        """
+        @param request: ModifyExpressConnectRouterAssociationAllowedPrefixRequest
+        @return: ModifyExpressConnectRouterAssociationAllowedPrefixResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_express_connect_router_association_allowed_prefix_with_options(request, runtime)
 
     async def modify_express_connect_router_association_allowed_prefix_async(
         self,
         request: express_connect_router_20230901_models.ModifyExpressConnectRouterAssociationAllowedPrefixRequest,
     ) -> express_connect_router_20230901_models.ModifyExpressConnectRouterAssociationAllowedPrefixResponse:
+        """
+        @param request: ModifyExpressConnectRouterAssociationAllowedPrefixRequest
+        @return: ModifyExpressConnectRouterAssociationAllowedPrefixResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_express_connect_router_association_allowed_prefix_with_options_async(request, runtime)
 
     def modify_express_connect_router_inter_region_transit_mode_with_options(
         self,
         request: express_connect_router_20230901_models.ModifyExpressConnectRouterInterRegionTransitModeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.ModifyExpressConnectRouterInterRegionTransitModeResponse:
+        """
+        @param request: ModifyExpressConnectRouterInterRegionTransitModeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyExpressConnectRouterInterRegionTransitModeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -2154,14 +2577,19 @@
         )
 
     async def modify_express_connect_router_inter_region_transit_mode_with_options_async(
         self,
         request: express_connect_router_20230901_models.ModifyExpressConnectRouterInterRegionTransitModeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.ModifyExpressConnectRouterInterRegionTransitModeResponse:
+        """
+        @param request: ModifyExpressConnectRouterInterRegionTransitModeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyExpressConnectRouterInterRegionTransitModeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -2187,29 +2615,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_express_connect_router_inter_region_transit_mode(
         self,
         request: express_connect_router_20230901_models.ModifyExpressConnectRouterInterRegionTransitModeRequest,
     ) -> express_connect_router_20230901_models.ModifyExpressConnectRouterInterRegionTransitModeResponse:
+        """
+        @param request: ModifyExpressConnectRouterInterRegionTransitModeRequest
+        @return: ModifyExpressConnectRouterInterRegionTransitModeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_express_connect_router_inter_region_transit_mode_with_options(request, runtime)
 
     async def modify_express_connect_router_inter_region_transit_mode_async(
         self,
         request: express_connect_router_20230901_models.ModifyExpressConnectRouterInterRegionTransitModeRequest,
     ) -> express_connect_router_20230901_models.ModifyExpressConnectRouterInterRegionTransitModeResponse:
+        """
+        @param request: ModifyExpressConnectRouterInterRegionTransitModeRequest
+        @return: ModifyExpressConnectRouterInterRegionTransitModeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_express_connect_router_inter_region_transit_mode_with_options_async(request, runtime)
 
     def revoke_instance_from_express_connect_router_with_options(
         self,
         request: express_connect_router_20230901_models.RevokeInstanceFromExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.RevokeInstanceFromExpressConnectRouterResponse:
+        """
+        @param request: RevokeInstanceFromExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RevokeInstanceFromExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -2242,14 +2683,19 @@
         )
 
     async def revoke_instance_from_express_connect_router_with_options_async(
         self,
         request: express_connect_router_20230901_models.RevokeInstanceFromExpressConnectRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.RevokeInstanceFromExpressConnectRouterResponse:
+        """
+        @param request: RevokeInstanceFromExpressConnectRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RevokeInstanceFromExpressConnectRouterResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -2281,29 +2727,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def revoke_instance_from_express_connect_router(
         self,
         request: express_connect_router_20230901_models.RevokeInstanceFromExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.RevokeInstanceFromExpressConnectRouterResponse:
+        """
+        @param request: RevokeInstanceFromExpressConnectRouterRequest
+        @return: RevokeInstanceFromExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.revoke_instance_from_express_connect_router_with_options(request, runtime)
 
     async def revoke_instance_from_express_connect_router_async(
         self,
         request: express_connect_router_20230901_models.RevokeInstanceFromExpressConnectRouterRequest,
     ) -> express_connect_router_20230901_models.RevokeInstanceFromExpressConnectRouterResponse:
+        """
+        @param request: RevokeInstanceFromExpressConnectRouterRequest
+        @return: RevokeInstanceFromExpressConnectRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.revoke_instance_from_express_connect_router_with_options_async(request, runtime)
 
     def synchronize_express_connect_router_inter_region_bandwidth_with_options(
         self,
         request: express_connect_router_20230901_models.SynchronizeExpressConnectRouterInterRegionBandwidthRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.SynchronizeExpressConnectRouterInterRegionBandwidthResponse:
+        """
+        @param request: SynchronizeExpressConnectRouterInterRegionBandwidthRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SynchronizeExpressConnectRouterInterRegionBandwidthResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -2328,14 +2787,19 @@
         )
 
     async def synchronize_express_connect_router_inter_region_bandwidth_with_options_async(
         self,
         request: express_connect_router_20230901_models.SynchronizeExpressConnectRouterInterRegionBandwidthRequest,
         runtime: util_models.RuntimeOptions,
     ) -> express_connect_router_20230901_models.SynchronizeExpressConnectRouterInterRegionBandwidthResponse:
+        """
+        @param request: SynchronizeExpressConnectRouterInterRegionBandwidthRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SynchronizeExpressConnectRouterInterRegionBandwidthResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             body['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.ecr_id):
@@ -2359,16 +2823,24 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def synchronize_express_connect_router_inter_region_bandwidth(
         self,
         request: express_connect_router_20230901_models.SynchronizeExpressConnectRouterInterRegionBandwidthRequest,
     ) -> express_connect_router_20230901_models.SynchronizeExpressConnectRouterInterRegionBandwidthResponse:
+        """
+        @param request: SynchronizeExpressConnectRouterInterRegionBandwidthRequest
+        @return: SynchronizeExpressConnectRouterInterRegionBandwidthResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.synchronize_express_connect_router_inter_region_bandwidth_with_options(request, runtime)
 
     async def synchronize_express_connect_router_inter_region_bandwidth_async(
         self,
         request: express_connect_router_20230901_models.SynchronizeExpressConnectRouterInterRegionBandwidthRequest,
     ) -> express_connect_router_20230901_models.SynchronizeExpressConnectRouterInterRegionBandwidthResponse:
+        """
+        @param request: SynchronizeExpressConnectRouterInterRegionBandwidthRequest
+        @return: SynchronizeExpressConnectRouterInterRegionBandwidthResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.synchronize_express_connect_router_inter_region_bandwidth_with_options_async(request, runtime)
```

### Comparing `alibabacloud_expressconnectrouter20230901-3.0.1/alibabacloud_expressconnectrouter20230901/models.py` & `alibabacloud_expressconnectrouter20230901-3.0.2/alibabacloud_expressconnectrouter20230901/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,24 @@
         child_instance_owner_id: int = None,
         child_instance_region_id: str = None,
         child_instance_type: str = None,
         client_token: str = None,
         dry_run: bool = None,
         ecr_id: str = None,
     ):
+        # This parameter is required.
         self.child_instance_id = child_instance_id
         self.child_instance_owner_id = child_instance_owner_id
+        # This parameter is required.
         self.child_instance_region_id = child_instance_region_id
+        # This parameter is required.
         self.child_instance_type = child_instance_type
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -183,15 +187,17 @@
         client_token: str = None,
         dry_run: bool = None,
         ecr_id: str = None,
         fresh_region_id: str = None,
     ):
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
+        # This parameter is required.
         self.fresh_region_id = fresh_region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -358,33 +364,72 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CheckAddRegionToExpressConnectRouterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateExpressConnectRouterRequestTags(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
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
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class CreateExpressConnectRouterRequest(TeaModel):
     def __init__(
         self,
         alibaba_side_asn: int = None,
         client_token: str = None,
         description: str = None,
         dry_run: bool = None,
         name: str = None,
         resource_group_id: str = None,
+        tags: List[CreateExpressConnectRouterRequestTags] = None,
     ):
+        # This parameter is required.
         self.alibaba_side_asn = alibaba_side_asn
         self.client_token = client_token
         self.description = description
         self.dry_run = dry_run
         self.name = name
         self.resource_group_id = resource_group_id
+        self.tags = tags
 
     def validate(self):
-        pass
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -396,14 +441,18 @@
             result['Description'] = self.description
         if self.dry_run is not None:
             result['DryRun'] = self.dry_run
         if self.name is not None:
             result['Name'] = self.name
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
+        result['Tags'] = []
+        if self.tags is not None:
+            for k in self.tags:
+                result['Tags'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AlibabaSideAsn') is not None:
             self.alibaba_side_asn = m.get('AlibabaSideAsn')
         if m.get('ClientToken') is not None:
@@ -412,14 +461,19 @@
             self.description = m.get('Description')
         if m.get('DryRun') is not None:
             self.dry_run = m.get('DryRun')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
+        self.tags = []
+        if m.get('Tags') is not None:
+            for k in m.get('Tags'):
+                temp_model = CreateExpressConnectRouterRequestTags()
+                self.tags.append(temp_model.from_map(k))
         return self
 
 
 class CreateExpressConnectRouterResponseBody(TeaModel):
     def __init__(
         self,
         access_denied_detail: str = None,
@@ -547,19 +601,21 @@
         ecr_id: str = None,
         transit_router_id: str = None,
         transit_router_owner_id: int = None,
         vpc_id: str = None,
         vpc_owner_id: int = None,
     ):
         self.allowed_prefixes = allowed_prefixes
+        # This parameter is required.
         self.association_region_id = association_region_id
         self.cen_id = cen_id
         self.client_token = client_token
         self.create_attachment = create_attachment
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
         self.transit_router_id = transit_router_id
         self.transit_router_owner_id = transit_router_owner_id
         self.vpc_id = vpc_id
         self.vpc_owner_id = vpc_owner_id
 
     def validate(self):
@@ -743,14 +799,15 @@
         self,
         client_token: str = None,
         dry_run: bool = None,
         ecr_id: str = None,
     ):
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -892,18 +949,20 @@
         self,
         association_id: str = None,
         client_token: str = None,
         delete_attachment: bool = None,
         dry_run: bool = None,
         ecr_id: str = None,
     ):
+        # This parameter is required.
         self.association_id = association_id
         self.client_token = client_token
         self.delete_attachment = delete_attachment
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1055,14 +1114,15 @@
         dry_run: bool = None,
         ecr_id: str = None,
         max_results: int = None,
         next_token: str = None,
     ):
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
         self.max_results = max_results
         self.next_token = next_token
 
     def validate(self):
         pass
 
@@ -1723,14 +1783,15 @@
         ecr_id: str = None,
         instance_id: str = None,
         instance_type: str = None,
     ):
         self.association_id = association_id
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
         self.instance_id = instance_id
         self.instance_type = instance_type
 
     def validate(self):
         pass
 
@@ -1945,14 +2006,15 @@
     ):
         self.association_id = association_id
         self.association_node_type = association_node_type
         self.association_region_id = association_region_id
         self.cen_id = cen_id
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
         self.max_results = max_results
         self.next_token = next_token
         self.transit_router_id = transit_router_id
         self.vpc_id = vpc_id
 
     def validate(self):
@@ -2277,14 +2339,15 @@
     ):
         self.association_id = association_id
         self.child_instance_id = child_instance_id
         self.child_instance_region_id = child_instance_region_id
         self.child_instance_type = child_instance_type
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
         self.max_results = max_results
         self.next_token = next_token
 
     def validate(self):
         pass
 
@@ -2571,14 +2634,15 @@
         self,
         client_token: str = None,
         dry_run: bool = None,
         ecr_id: str = None,
     ):
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2767,14 +2831,15 @@
         self,
         client_token: str = None,
         dry_run: bool = None,
         ecr_id: str = None,
     ):
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2932,14 +2997,15 @@
         query_region_id: str = None,
     ):
         self.as_path = as_path
         self.client_token = client_token
         self.community = community
         self.destination_cidr_block = destination_cidr_block
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
         self.max_results = max_results
         self.next_token = next_token
         self.nexthop_instance_id = nexthop_instance_id
         self.query_region_id = query_region_id
 
     def validate(self):
@@ -3243,14 +3309,15 @@
         max_results: int = None,
         next_token: str = None,
         resource_group_id: str = None,
         tag_models: List[DescribeInstanceGrantedToExpressConnectRouterRequestTagModels] = None,
     ):
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
         self.instance_id = instance_id
         self.instance_owner_id = instance_owner_id
         self.instance_region_id = instance_region_id
         self.instance_type = instance_type
         self.max_results = max_results
         self.next_token = next_token
@@ -3553,18 +3620,21 @@
         self,
         child_instance_id: str = None,
         child_instance_type: str = None,
         client_token: str = None,
         dry_run: bool = None,
         ecr_id: str = None,
     ):
+        # This parameter is required.
         self.child_instance_id = child_instance_id
+        # This parameter is required.
         self.child_instance_type = child_instance_type
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3715,17 +3785,20 @@
         client_token: str = None,
         destination_cidr_block: str = None,
         dry_run: bool = None,
         ecr_id: str = None,
         nexthop_instance_id: str = None,
     ):
         self.client_token = client_token
+        # This parameter is required.
         self.destination_cidr_block = destination_cidr_block
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
+        # This parameter is required.
         self.nexthop_instance_id = nexthop_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3876,17 +3949,20 @@
         client_token: str = None,
         destination_cidr_block: str = None,
         dry_run: bool = None,
         ecr_id: str = None,
         nexthop_instance_id: str = None,
     ):
         self.client_token = client_token
+        # This parameter is required.
         self.destination_cidr_block = destination_cidr_block
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
+        # This parameter is required.
         self.nexthop_instance_id = nexthop_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4036,14 +4112,15 @@
         self,
         client_token: str = None,
         dry_run: bool = None,
         ecr_id: str = None,
     ):
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4189,18 +4266,23 @@
         ecr_owner_ali_uid: int = None,
         instance_id: str = None,
         instance_region_id: str = None,
         instance_type: str = None,
     ):
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
+        # This parameter is required.
         self.ecr_owner_ali_uid = ecr_owner_ali_uid
+        # This parameter is required.
         self.instance_id = instance_id
+        # This parameter is required.
         self.instance_region_id = instance_region_id
+        # This parameter is required.
         self.instance_type = instance_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4356,14 +4438,15 @@
 class ListExpressConnectRouterSupportedRegionRequest(TeaModel):
     def __init__(
         self,
         client_token: str = None,
         node_type: str = None,
     ):
         self.client_token = client_token
+        # This parameter is required.
         self.node_type = node_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4492,14 +4575,15 @@
         dry_run: bool = None,
         ecr_id: str = None,
         name: str = None,
     ):
         self.client_token = client_token
         self.description = description
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4652,17 +4736,19 @@
         association_id: str = None,
         client_token: str = None,
         dry_run: bool = None,
         ecr_id: str = None,
         owner_account: str = None,
     ):
         self.allowed_prefixes = allowed_prefixes
+        # This parameter is required.
         self.association_id = association_id
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
         self.owner_account = owner_account
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4851,14 +4937,15 @@
         client_token: str = None,
         dry_run: bool = None,
         ecr_id: str = None,
         transit_mode_list: List[ModifyExpressConnectRouterInterRegionTransitModeRequestTransitModeList] = None,
     ):
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
         self.transit_mode_list = transit_mode_list
 
     def validate(self):
         if self.transit_mode_list:
             for k in self.transit_mode_list:
                 if k:
@@ -5017,18 +5104,23 @@
         ecr_owner_ali_uid: int = None,
         instance_id: str = None,
         instance_region_id: str = None,
         instance_type: str = None,
     ):
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
+        # This parameter is required.
         self.ecr_owner_ali_uid = ecr_owner_ali_uid
+        # This parameter is required.
         self.instance_id = instance_id
+        # This parameter is required.
         self.instance_region_id = instance_region_id
+        # This parameter is required.
         self.instance_type = instance_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5186,14 +5278,15 @@
         self,
         client_token: str = None,
         dry_run: bool = None,
         ecr_id: str = None,
     ):
         self.client_token = client_token
         self.dry_run = dry_run
+        # This parameter is required.
         self.ecr_id = ecr_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_expressconnectrouter20230901-3.0.1/alibabacloud_expressconnectrouter20230901.egg-info/PKG-INFO` & `alibabacloud_expressconnectrouter20230901-3.0.2/alibabacloud_expressconnectrouter20230901.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-expressconnectrouter20230901
-Version: 3.0.1
+Version: 3.0.2
 Summary: Alibaba Cloud ExpressConnectRouter (20230901) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_expressconnectrouter20230901-3.0.1/alibabacloud_expressconnectrouter20230901.egg-info/SOURCES.txt` & `alibabacloud_expressconnectrouter20230901-3.0.2/alibabacloud_expressconnectrouter20230901.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_expressconnectrouter20230901-3.0.1/setup.py` & `alibabacloud_expressconnectrouter20230901-3.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_expressconnectrouter20230901.
 
-Created on 26/03/2024
+Created on 16/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_expressconnectrouter20230901"
 NAME = "alibabacloud_expressconnectrouter20230901" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ExpressConnectRouter (20230901) SDK Library for Python"
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

