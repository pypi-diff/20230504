# Comparing `tmp/alibabacloud_dyplsapi20170525-1.0.6.tar.gz` & `tmp/alibabacloud_dyplsapi20170525-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dyplsapi20170525-1.0.6.tar", last modified: Fri Feb 24 09:23:29 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dyplsapi20170525-1.0.7.tar", last modified: Thu May  4 02:43:39 2023, max compression
```

## Comparing `alibabacloud_dyplsapi20170525-1.0.6.tar` & `alibabacloud_dyplsapi20170525-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:23:29.000000 alibabacloud_dyplsapi20170525-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      388 2023-02-24 09:23:28.000000 alibabacloud_dyplsapi20170525-1.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-24 09:23:28.000000 alibabacloud_dyplsapi20170525-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-24 09:23:28.000000 alibabacloud_dyplsapi20170525-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-02-24 09:23:29.000000 alibabacloud_dyplsapi20170525-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-02-24 09:23:28.000000 alibabacloud_dyplsapi20170525-1.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-02-24 09:23:28.000000 alibabacloud_dyplsapi20170525-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:23:29.000000 alibabacloud_dyplsapi20170525-1.0.6/alibabacloud_dyplsapi20170525/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-24 09:23:28.000000 alibabacloud_dyplsapi20170525-1.0.6/alibabacloud_dyplsapi20170525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   121678 2023-02-24 09:23:28.000000 alibabacloud_dyplsapi20170525-1.0.6/alibabacloud_dyplsapi20170525/client.py
--rw-r--r--   0 root         (0) root         (0)   195974 2023-02-24 09:23:28.000000 alibabacloud_dyplsapi20170525-1.0.6/alibabacloud_dyplsapi20170525/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:23:29.000000 alibabacloud_dyplsapi20170525-1.0.6/alibabacloud_dyplsapi20170525.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-02-24 09:23:29.000000 alibabacloud_dyplsapi20170525-1.0.6/alibabacloud_dyplsapi20170525.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-02-24 09:23:29.000000 alibabacloud_dyplsapi20170525-1.0.6/alibabacloud_dyplsapi20170525.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-24 09:23:29.000000 alibabacloud_dyplsapi20170525-1.0.6/alibabacloud_dyplsapi20170525.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-02-24 09:23:29.000000 alibabacloud_dyplsapi20170525-1.0.6/alibabacloud_dyplsapi20170525.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-02-24 09:23:29.000000 alibabacloud_dyplsapi20170525-1.0.6/alibabacloud_dyplsapi20170525.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-24 09:23:29.000000 alibabacloud_dyplsapi20170525-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2023-02-24 09:23:28.000000 alibabacloud_dyplsapi20170525-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:43:39.000000 alibabacloud_dyplsapi20170525-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      446 2023-05-04 02:43:38.000000 alibabacloud_dyplsapi20170525-1.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-04 02:43:38.000000 alibabacloud_dyplsapi20170525-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-04 02:43:38.000000 alibabacloud_dyplsapi20170525-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-05-04 02:43:39.000000 alibabacloud_dyplsapi20170525-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-05-04 02:43:38.000000 alibabacloud_dyplsapi20170525-1.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-05-04 02:43:38.000000 alibabacloud_dyplsapi20170525-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:43:39.000000 alibabacloud_dyplsapi20170525-1.0.7/alibabacloud_dyplsapi20170525/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-04 02:43:38.000000 alibabacloud_dyplsapi20170525-1.0.7/alibabacloud_dyplsapi20170525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   129342 2023-05-04 02:43:38.000000 alibabacloud_dyplsapi20170525-1.0.7/alibabacloud_dyplsapi20170525/client.py
+-rw-r--r--   0 root         (0) root         (0)   214066 2023-05-04 02:43:38.000000 alibabacloud_dyplsapi20170525-1.0.7/alibabacloud_dyplsapi20170525/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:43:39.000000 alibabacloud_dyplsapi20170525-1.0.7/alibabacloud_dyplsapi20170525.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-05-04 02:43:39.000000 alibabacloud_dyplsapi20170525-1.0.7/alibabacloud_dyplsapi20170525.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-05-04 02:43:39.000000 alibabacloud_dyplsapi20170525-1.0.7/alibabacloud_dyplsapi20170525.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 02:43:39.000000 alibabacloud_dyplsapi20170525-1.0.7/alibabacloud_dyplsapi20170525.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-04 02:43:39.000000 alibabacloud_dyplsapi20170525-1.0.7/alibabacloud_dyplsapi20170525.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-04 02:43:39.000000 alibabacloud_dyplsapi20170525-1.0.7/alibabacloud_dyplsapi20170525.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-04 02:43:39.000000 alibabacloud_dyplsapi20170525-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-05-04 02:43:38.000000 alibabacloud_dyplsapi20170525-1.0.7/setup.py
```

### Comparing `alibabacloud_dyplsapi20170525-1.0.6/LICENSE` & `alibabacloud_dyplsapi20170525-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dyplsapi20170525-1.0.6/PKG-INFO` & `alibabacloud_dyplsapi20170525-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dyplsapi20170525
-Version: 1.0.6
+Version: 1.0.7
 Summary: Alibaba Cloud Dyplsapi (20170525) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dyplsapi20170525-1.0.6/README-CN.md` & `alibabacloud_dyplsapi20170525-1.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dyplsapi20170525-1.0.6/README.md` & `alibabacloud_dyplsapi20170525-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dyplsapi20170525-1.0.6/alibabacloud_dyplsapi20170525/client.py` & `alibabacloud_dyplsapi20170525-1.0.7/alibabacloud_dyplsapi20170525/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -778,14 +778,108 @@
     async def bind_axn_extension_async(
         self,
         request: dyplsapi_20170525_models.BindAxnExtensionRequest,
     ) -> dyplsapi_20170525_models.BindAxnExtensionResponse:
         runtime = util_models.RuntimeOptions()
         return await self.bind_axn_extension_with_options_async(request, runtime)
 
+    def bind_batch_axg_with_options(
+        self,
+        tmp_req: dyplsapi_20170525_models.BindBatchAxgRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dyplsapi_20170525_models.BindBatchAxgResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dyplsapi_20170525_models.BindBatchAxgShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.axg_bind_list):
+            request.axg_bind_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.axg_bind_list, 'AxgBindList', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.axg_bind_list_shrink):
+            query['AxgBindList'] = request.axg_bind_list_shrink
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.pool_key):
+            query['PoolKey'] = request.pool_key
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='BindBatchAxg',
+            version='2017-05-25',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dyplsapi_20170525_models.BindBatchAxgResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def bind_batch_axg_with_options_async(
+        self,
+        tmp_req: dyplsapi_20170525_models.BindBatchAxgRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dyplsapi_20170525_models.BindBatchAxgResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dyplsapi_20170525_models.BindBatchAxgShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.axg_bind_list):
+            request.axg_bind_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.axg_bind_list, 'AxgBindList', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.axg_bind_list_shrink):
+            query['AxgBindList'] = request.axg_bind_list_shrink
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.pool_key):
+            query['PoolKey'] = request.pool_key
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='BindBatchAxg',
+            version='2017-05-25',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dyplsapi_20170525_models.BindBatchAxgResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def bind_batch_axg(
+        self,
+        request: dyplsapi_20170525_models.BindBatchAxgRequest,
+    ) -> dyplsapi_20170525_models.BindBatchAxgResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.bind_batch_axg_with_options(request, runtime)
+
+    async def bind_batch_axg_async(
+        self,
+        request: dyplsapi_20170525_models.BindBatchAxgRequest,
+    ) -> dyplsapi_20170525_models.BindBatchAxgResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.bind_batch_axg_with_options_async(request, runtime)
+
     def buy_secret_no_with_options(
         self,
         request: dyplsapi_20170525_models.BuySecretNoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dyplsapi_20170525_models.BuySecretNoResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1304,14 +1398,100 @@
     async def create_pick_up_waybill_pre_query_async(
         self,
         request: dyplsapi_20170525_models.CreatePickUpWaybillPreQueryRequest,
     ) -> dyplsapi_20170525_models.CreatePickUpWaybillPreQueryResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_pick_up_waybill_pre_query_with_options_async(request, runtime)
 
+    def delete_axg_group_with_options(
+        self,
+        request: dyplsapi_20170525_models.DeleteAxgGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dyplsapi_20170525_models.DeleteAxgGroupResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.group_id):
+            query['GroupId'] = request.group_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.pool_key):
+            query['PoolKey'] = request.pool_key
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteAxgGroup',
+            version='2017-05-25',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dyplsapi_20170525_models.DeleteAxgGroupResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_axg_group_with_options_async(
+        self,
+        request: dyplsapi_20170525_models.DeleteAxgGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dyplsapi_20170525_models.DeleteAxgGroupResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.group_id):
+            query['GroupId'] = request.group_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.pool_key):
+            query['PoolKey'] = request.pool_key
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteAxgGroup',
+            version='2017-05-25',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dyplsapi_20170525_models.DeleteAxgGroupResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_axg_group(
+        self,
+        request: dyplsapi_20170525_models.DeleteAxgGroupRequest,
+    ) -> dyplsapi_20170525_models.DeleteAxgGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_axg_group_with_options(request, runtime)
+
+    async def delete_axg_group_async(
+        self,
+        request: dyplsapi_20170525_models.DeleteAxgGroupRequest,
+    ) -> dyplsapi_20170525_models.DeleteAxgGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_axg_group_with_options_async(request, runtime)
+
     def delete_secret_blacklist_with_options(
         self,
         request: dyplsapi_20170525_models.DeleteSecretBlacklistRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dyplsapi_20170525_models.DeleteSecretBlacklistResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_dyplsapi20170525-1.0.6/alibabacloud_dyplsapi20170525/models.py` & `alibabacloud_dyplsapi20170525-1.0.7/alibabacloud_dyplsapi20170525/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1328,14 +1328,418 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = BindAxnExtensionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class BindBatchAxgRequestAxgBindList(TeaModel):
+    def __init__(
+        self,
+        asrmodel_id: str = None,
+        asrstatus: bool = None,
+        call_display_type: int = None,
+        call_restrict: str = None,
+        expect_city: str = None,
+        expiration: str = None,
+        group_id: str = None,
+        is_recording_enabled: bool = None,
+        out_id: str = None,
+        out_order_id: str = None,
+        phone_no_a: str = None,
+        phone_no_b: str = None,
+        phone_no_x: str = None,
+        ring_config: str = None,
+    ):
+        self.asrmodel_id = asrmodel_id
+        self.asrstatus = asrstatus
+        self.call_display_type = call_display_type
+        self.call_restrict = call_restrict
+        self.expect_city = expect_city
+        self.expiration = expiration
+        self.group_id = group_id
+        self.is_recording_enabled = is_recording_enabled
+        self.out_id = out_id
+        self.out_order_id = out_order_id
+        self.phone_no_a = phone_no_a
+        self.phone_no_b = phone_no_b
+        self.phone_no_x = phone_no_x
+        self.ring_config = ring_config
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
+        if self.asrmodel_id is not None:
+            result['ASRModelId'] = self.asrmodel_id
+        if self.asrstatus is not None:
+            result['ASRStatus'] = self.asrstatus
+        if self.call_display_type is not None:
+            result['CallDisplayType'] = self.call_display_type
+        if self.call_restrict is not None:
+            result['CallRestrict'] = self.call_restrict
+        if self.expect_city is not None:
+            result['ExpectCity'] = self.expect_city
+        if self.expiration is not None:
+            result['Expiration'] = self.expiration
+        if self.group_id is not None:
+            result['GroupId'] = self.group_id
+        if self.is_recording_enabled is not None:
+            result['IsRecordingEnabled'] = self.is_recording_enabled
+        if self.out_id is not None:
+            result['OutId'] = self.out_id
+        if self.out_order_id is not None:
+            result['OutOrderId'] = self.out_order_id
+        if self.phone_no_a is not None:
+            result['PhoneNoA'] = self.phone_no_a
+        if self.phone_no_b is not None:
+            result['PhoneNoB'] = self.phone_no_b
+        if self.phone_no_x is not None:
+            result['PhoneNoX'] = self.phone_no_x
+        if self.ring_config is not None:
+            result['RingConfig'] = self.ring_config
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ASRModelId') is not None:
+            self.asrmodel_id = m.get('ASRModelId')
+        if m.get('ASRStatus') is not None:
+            self.asrstatus = m.get('ASRStatus')
+        if m.get('CallDisplayType') is not None:
+            self.call_display_type = m.get('CallDisplayType')
+        if m.get('CallRestrict') is not None:
+            self.call_restrict = m.get('CallRestrict')
+        if m.get('ExpectCity') is not None:
+            self.expect_city = m.get('ExpectCity')
+        if m.get('Expiration') is not None:
+            self.expiration = m.get('Expiration')
+        if m.get('GroupId') is not None:
+            self.group_id = m.get('GroupId')
+        if m.get('IsRecordingEnabled') is not None:
+            self.is_recording_enabled = m.get('IsRecordingEnabled')
+        if m.get('OutId') is not None:
+            self.out_id = m.get('OutId')
+        if m.get('OutOrderId') is not None:
+            self.out_order_id = m.get('OutOrderId')
+        if m.get('PhoneNoA') is not None:
+            self.phone_no_a = m.get('PhoneNoA')
+        if m.get('PhoneNoB') is not None:
+            self.phone_no_b = m.get('PhoneNoB')
+        if m.get('PhoneNoX') is not None:
+            self.phone_no_x = m.get('PhoneNoX')
+        if m.get('RingConfig') is not None:
+            self.ring_config = m.get('RingConfig')
+        return self
+
+
+class BindBatchAxgRequest(TeaModel):
+    def __init__(
+        self,
+        axg_bind_list: List[BindBatchAxgRequestAxgBindList] = None,
+        owner_id: int = None,
+        pool_key: str = None,
+        resource_owner_account: str = None,
+        resource_owner_id: int = None,
+    ):
+        self.axg_bind_list = axg_bind_list
+        self.owner_id = owner_id
+        self.pool_key = pool_key
+        self.resource_owner_account = resource_owner_account
+        self.resource_owner_id = resource_owner_id
+
+    def validate(self):
+        if self.axg_bind_list:
+            for k in self.axg_bind_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['AxgBindList'] = []
+        if self.axg_bind_list is not None:
+            for k in self.axg_bind_list:
+                result['AxgBindList'].append(k.to_map() if k else None)
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.pool_key is not None:
+            result['PoolKey'] = self.pool_key
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.axg_bind_list = []
+        if m.get('AxgBindList') is not None:
+            for k in m.get('AxgBindList'):
+                temp_model = BindBatchAxgRequestAxgBindList()
+                self.axg_bind_list.append(temp_model.from_map(k))
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('PoolKey') is not None:
+            self.pool_key = m.get('PoolKey')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        return self
+
+
+class BindBatchAxgShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        axg_bind_list_shrink: str = None,
+        owner_id: int = None,
+        pool_key: str = None,
+        resource_owner_account: str = None,
+        resource_owner_id: int = None,
+    ):
+        self.axg_bind_list_shrink = axg_bind_list_shrink
+        self.owner_id = owner_id
+        self.pool_key = pool_key
+        self.resource_owner_account = resource_owner_account
+        self.resource_owner_id = resource_owner_id
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
+        if self.axg_bind_list_shrink is not None:
+            result['AxgBindList'] = self.axg_bind_list_shrink
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.pool_key is not None:
+            result['PoolKey'] = self.pool_key
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AxgBindList') is not None:
+            self.axg_bind_list_shrink = m.get('AxgBindList')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('PoolKey') is not None:
+            self.pool_key = m.get('PoolKey')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        return self
+
+
+class BindBatchAxgResponseBodySecretBindListSecretBind(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        extension: str = None,
+        group_id: str = None,
+        message: str = None,
+        phone_no_a: str = None,
+        secret_no: str = None,
+        subs_id: str = None,
+    ):
+        self.code = code
+        self.extension = extension
+        self.group_id = group_id
+        self.message = message
+        self.phone_no_a = phone_no_a
+        self.secret_no = secret_no
+        self.subs_id = subs_id
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
+        if self.extension is not None:
+            result['Extension'] = self.extension
+        if self.group_id is not None:
+            result['GroupId'] = self.group_id
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.phone_no_a is not None:
+            result['PhoneNoA'] = self.phone_no_a
+        if self.secret_no is not None:
+            result['SecretNo'] = self.secret_no
+        if self.subs_id is not None:
+            result['SubsId'] = self.subs_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Extension') is not None:
+            self.extension = m.get('Extension')
+        if m.get('GroupId') is not None:
+            self.group_id = m.get('GroupId')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('PhoneNoA') is not None:
+            self.phone_no_a = m.get('PhoneNoA')
+        if m.get('SecretNo') is not None:
+            self.secret_no = m.get('SecretNo')
+        if m.get('SubsId') is not None:
+            self.subs_id = m.get('SubsId')
+        return self
+
+
+class BindBatchAxgResponseBodySecretBindList(TeaModel):
+    def __init__(
+        self,
+        secret_bind: List[BindBatchAxgResponseBodySecretBindListSecretBind] = None,
+    ):
+        self.secret_bind = secret_bind
+
+    def validate(self):
+        if self.secret_bind:
+            for k in self.secret_bind:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['SecretBind'] = []
+        if self.secret_bind is not None:
+            for k in self.secret_bind:
+                result['SecretBind'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.secret_bind = []
+        if m.get('SecretBind') is not None:
+            for k in m.get('SecretBind'):
+                temp_model = BindBatchAxgResponseBodySecretBindListSecretBind()
+                self.secret_bind.append(temp_model.from_map(k))
+        return self
+
+
+class BindBatchAxgResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        message: str = None,
+        request_id: str = None,
+        secret_bind_list: BindBatchAxgResponseBodySecretBindList = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.secret_bind_list = secret_bind_list
+
+    def validate(self):
+        if self.secret_bind_list:
+            self.secret_bind_list.validate()
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
+        if self.secret_bind_list is not None:
+            result['SecretBindList'] = self.secret_bind_list.to_map()
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
+        if m.get('SecretBindList') is not None:
+            temp_model = BindBatchAxgResponseBodySecretBindList()
+            self.secret_bind_list = temp_model.from_map(m['SecretBindList'])
+        return self
+
+
+class BindBatchAxgResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: BindBatchAxgResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
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
+            temp_model = BindBatchAxgResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class BuySecretNoRequest(TeaModel):
     def __init__(
         self,
         city: str = None,
         display_pool: bool = None,
         owner_id: int = None,
         pool_key: str = None,
@@ -3031,14 +3435,148 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreatePickUpWaybillPreQueryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteAxgGroupRequest(TeaModel):
+    def __init__(
+        self,
+        group_id: int = None,
+        owner_id: int = None,
+        pool_key: str = None,
+        resource_owner_account: str = None,
+        resource_owner_id: int = None,
+    ):
+        self.group_id = group_id
+        self.owner_id = owner_id
+        self.pool_key = pool_key
+        self.resource_owner_account = resource_owner_account
+        self.resource_owner_id = resource_owner_id
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
+        if self.group_id is not None:
+            result['GroupId'] = self.group_id
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.pool_key is not None:
+            result['PoolKey'] = self.pool_key
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('GroupId') is not None:
+            self.group_id = m.get('GroupId')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('PoolKey') is not None:
+            self.pool_key = m.get('PoolKey')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        return self
+
+
+class DeleteAxgGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
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
+        return self
+
+
+class DeleteAxgGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteAxgGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
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
+            temp_model = DeleteAxgGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteSecretBlacklistRequest(TeaModel):
     def __init__(
         self,
         black_no: str = None,
         black_type: str = None,
         pool_key: str = None,
         remark: str = None,
```

### Comparing `alibabacloud_dyplsapi20170525-1.0.6/alibabacloud_dyplsapi20170525.egg-info/PKG-INFO` & `alibabacloud_dyplsapi20170525-1.0.7/alibabacloud_dyplsapi20170525.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dyplsapi20170525
-Version: 1.0.6
+Version: 1.0.7
 Summary: Alibaba Cloud Dyplsapi (20170525) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dyplsapi20170525-1.0.6/setup.py` & `alibabacloud_dyplsapi20170525-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dyplsapi20170525.
 
-Created on 24/02/2023
+Created on 04/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dyplsapi20170525"
 NAME = "alibabacloud_dyplsapi20170525" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dyplsapi (20170525) SDK Library for Python"
```

