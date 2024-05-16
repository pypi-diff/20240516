# Comparing `tmp/antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0.tar.gz` & `tmp/antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0.tar", last modified: Tue Sep 12 07:13:29 2023, max compression
+gzip compressed data, was "dist/antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1.tar", last modified: Thu May 16 06:04:42 2024, max compression
```

## Comparing `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0.tar` & `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-12 07:13:29.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-09-12 07:13:28.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-09-12 07:13:28.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-09-12 07:13:29.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-09-12 07:13:28.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-09-12 07:13:28.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-12 07:13:29.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-09-12 07:13:28.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-09-12 07:13:28.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-12 07:13:28.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-09-12 07:13:28.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-09-12 07:13:28.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-12 07:13:29.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/antchain_sdk_ak_55afdde95cc7448bad87a98d904c1f44/
--rw-r--r--   0 root         (0) root         (0)       21 2023-09-12 07:13:28.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/antchain_sdk_ak_55afdde95cc7448bad87a98d904c1f44/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15724 2023-09-12 07:13:28.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/antchain_sdk_ak_55afdde95cc7448bad87a98d904c1f44/client.py
--rw-r--r--   0 root         (0) root         (0)     9843 2023-09-12 07:13:28.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/antchain_sdk_ak_55afdde95cc7448bad87a98d904c1f44/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-09-12 07:13:29.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2651 2023-09-12 07:13:28.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:04:42.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-16 06:04:41.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-16 06:04:41.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2024-05-16 06:04:42.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2024-05-16 06:04:41.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-05-16 06:04:41.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:04:42.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2024-05-16 06:04:42.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2024-05-16 06:04:42.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 06:04:42.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-05-16 06:04:42.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-16 06:04:42.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:04:42.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/antchain_sdk_ak_55afdde95cc7448bad87a98d904c1f44/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-16 06:04:41.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/antchain_sdk_ak_55afdde95cc7448bad87a98d904c1f44/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18652 2024-05-16 06:04:41.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/antchain_sdk_ak_55afdde95cc7448bad87a98d904c1f44/client.py
+-rw-r--r--   0 root         (0) root         (0)    13307 2024-05-16 06:04:41.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/antchain_sdk_ak_55afdde95cc7448bad87a98d904c1f44/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-16 06:04:42.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-05-16 06:04:41.000000 antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/setup.py
```

### Comparing `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/LICENSE` & `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/PKG-INFO` & `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_55afdde95cc7448bad87a98d904c1f44
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ant Chain Ak_55afdde95cc7448bad87a98d904c1f44 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/README-CN.md` & `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/README.md` & `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/PKG-INFO` & `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-55afdde95cc7448bad87a98d904c1f44
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ant Chain Ak_55afdde95cc7448bad87a98d904c1f44 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/SOURCES.txt` & `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/antchain_ak_55afdde95cc7448bad87a98d904c1f44.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/antchain_sdk_ak_55afdde95cc7448bad87a98d904c1f44/client.py` & `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/antchain_sdk_ak_55afdde95cc7448bad87a98d904c1f44/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.0',
+                    'sdk_version': '1.0.1',
                     '_prod_code': 'ak_55afdde95cc7448bad87a98d904c1f44',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -233,15 +233,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.0',
+                    'sdk_version': '1.0.1',
                     '_prod_code': 'ak_55afdde95cc7448bad87a98d904c1f44',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -324,7 +324,63 @@
         Summary: 数字人交互接口
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__55afdde_95cc_7448bad_87a_98d_904c_1f_44_models.QueryUniversalsaasDigitalhumanRobotResponse(),
             await self.do_request_async('1.0', 'universalsaas.digitalhuman.robot.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def get_universalsaas_digitalhuman_nls_token(
+        self,
+        request: ak__55afdde_95cc_7448bad_87a_98d_904c_1f_44_models.GetUniversalsaasDigitalhumanNlsTokenRequest,
+    ) -> ak__55afdde_95cc_7448bad_87a_98d_904c_1f_44_models.GetUniversalsaasDigitalhumanNlsTokenResponse:
+        """
+        Description: 数字人获取语音服务token接口
+        Summary: 数字人获取语音服务token接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_universalsaas_digitalhuman_nls_token_ex(request, headers, runtime)
+
+    async def get_universalsaas_digitalhuman_nls_token_async(
+        self,
+        request: ak__55afdde_95cc_7448bad_87a_98d_904c_1f_44_models.GetUniversalsaasDigitalhumanNlsTokenRequest,
+    ) -> ak__55afdde_95cc_7448bad_87a_98d_904c_1f_44_models.GetUniversalsaasDigitalhumanNlsTokenResponse:
+        """
+        Description: 数字人获取语音服务token接口
+        Summary: 数字人获取语音服务token接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_universalsaas_digitalhuman_nls_token_ex_async(request, headers, runtime)
+
+    def get_universalsaas_digitalhuman_nls_token_ex(
+        self,
+        request: ak__55afdde_95cc_7448bad_87a_98d_904c_1f_44_models.GetUniversalsaasDigitalhumanNlsTokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__55afdde_95cc_7448bad_87a_98d_904c_1f_44_models.GetUniversalsaasDigitalhumanNlsTokenResponse:
+        """
+        Description: 数字人获取语音服务token接口
+        Summary: 数字人获取语音服务token接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__55afdde_95cc_7448bad_87a_98d_904c_1f_44_models.GetUniversalsaasDigitalhumanNlsTokenResponse(),
+            self.do_request('1.0', 'universalsaas.digitalhuman.nls.token.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_universalsaas_digitalhuman_nls_token_ex_async(
+        self,
+        request: ak__55afdde_95cc_7448bad_87a_98d_904c_1f_44_models.GetUniversalsaasDigitalhumanNlsTokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__55afdde_95cc_7448bad_87a_98d_904c_1f_44_models.GetUniversalsaasDigitalhumanNlsTokenResponse:
+        """
+        Description: 数字人获取语音服务token接口
+        Summary: 数字人获取语音服务token接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__55afdde_95cc_7448bad_87a_98d_904c_1f_44_models.GetUniversalsaasDigitalhumanNlsTokenResponse(),
+            await self.do_request_async('1.0', 'universalsaas.digitalhuman.nls.token.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/antchain_sdk_ak_55afdde95cc7448bad87a98d904c1f44/models.py` & `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/antchain_sdk_ak_55afdde95cc7448bad87a98d904c1f44/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -254,7 +254,112 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('result_data') is not None:
             self.result_data = m.get('result_data')
         return self
 
 
+class GetUniversalsaasDigitalhumanNlsTokenRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户code&租户id，对于子部门客户需要上传子部门id
+        self.tenant_code = tenant_code
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
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.tenant_code is not None:
+            result['tenant_code'] = self.tenant_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_code') is not None:
+            self.tenant_code = m.get('tenant_code')
+        return self
+
+
+class GetUniversalsaasDigitalhumanNlsTokenResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        app_key: str = None,
+        app_token: str = None,
+        expire_time: int = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # appkey
+        # 
+        self.app_key = app_key
+        # token
+        self.app_token = app_token
+        # token的有效期时间戳
+        self.expire_time = expire_time
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.app_key is not None:
+            result['app_key'] = self.app_key
+        if self.app_token is not None:
+            result['app_token'] = self.app_token
+        if self.expire_time is not None:
+            result['expire_time'] = self.expire_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('app_key') is not None:
+            self.app_key = m.get('app_key')
+        if m.get('app_token') is not None:
+            self.app_token = m.get('app_token')
+        if m.get('expire_time') is not None:
+            self.expire_time = m.get('expire_time')
+        return self
+
+
```

### Comparing `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.0/setup.py` & `antchain_ak_55afdde95cc7448bad87a98d904c1f44-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_55afdde95cc7448bad87a98d904c1f44.
 
-Created on 12/09/2023
+Created on 16/05/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_55afdde95cc7448bad87a98d904c1f44"
 NAME = "antchain_ak_55afdde95cc7448bad87a98d904c1f44" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_55afdde95cc7448bad87a98d904c1f44 SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

