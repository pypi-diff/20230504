# Comparing `tmp/alibabacloud_dyplsapi20170525_py2-1.0.0.tar.gz` & `tmp/alibabacloud_dyplsapi20170525_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dyplsapi20170525_py2-1.0.0.tar", last modified: Fri Feb 24 09:23:25 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dyplsapi20170525_py2-1.0.1.tar", last modified: Thu May  4 02:43:47 2023, max compression
```

## Comparing `alibabacloud_dyplsapi20170525_py2-1.0.0.tar` & `alibabacloud_dyplsapi20170525_py2-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/alibabacloud_dyplsapi20170525/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/alibabacloud_dyplsapi20170525/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53044 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/alibabacloud_dyplsapi20170525/client.py
--rw-r--r--   0 root         (0) root         (0)   197221 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/alibabacloud_dyplsapi20170525/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/alibabacloud_dyplsapi20170525_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/alibabacloud_dyplsapi20170525_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      467 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/alibabacloud_dyplsapi20170525_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/alibabacloud_dyplsapi20170525_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/alibabacloud_dyplsapi20170525_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/alibabacloud_dyplsapi20170525_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2023-02-24 09:23:25.000000 alibabacloud_dyplsapi20170525_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/alibabacloud_dyplsapi20170525/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/alibabacloud_dyplsapi20170525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56276 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/alibabacloud_dyplsapi20170525/client.py
+-rw-r--r--   0 root         (0) root         (0)   215425 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/alibabacloud_dyplsapi20170525/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/alibabacloud_dyplsapi20170525_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/alibabacloud_dyplsapi20170525_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/alibabacloud_dyplsapi20170525_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/alibabacloud_dyplsapi20170525_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/alibabacloud_dyplsapi20170525_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/alibabacloud_dyplsapi20170525_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-05-04 02:43:47.000000 alibabacloud_dyplsapi20170525_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_dyplsapi20170525_py2-1.0.0/LICENSE` & `alibabacloud_dyplsapi20170525_py2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dyplsapi20170525_py2-1.0.0/PKG-INFO` & `alibabacloud_dyplsapi20170525_py2-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dyplsapi20170525_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Dyplsapi (20170525) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dyplsapi20170525_py2-1.0.0/README-CN.md` & `alibabacloud_dyplsapi20170525_py2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dyplsapi20170525_py2-1.0.0/README.md` & `alibabacloud_dyplsapi20170525_py2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dyplsapi20170525_py2-1.0.0/alibabacloud_dyplsapi20170525/client.py` & `alibabacloud_dyplsapi20170525_py2-1.0.1/alibabacloud_dyplsapi20170525/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,14 +355,54 @@
             self.call_api(params, req, runtime)
         )
 
     def bind_axn_extension(self, request):
         runtime = util_models.RuntimeOptions()
         return self.bind_axn_extension_with_options(request, runtime)
 
+    def bind_batch_axg_with_options(self, tmp_req, runtime):
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
+    def bind_batch_axg(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.bind_batch_axg_with_options(request, runtime)
+
     def buy_secret_no_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.city):
             query['City'] = request.city
         if not UtilClient.is_unset(request.display_pool):
             query['DisplayPool'] = request.display_pool
@@ -583,14 +623,50 @@
             self.call_api(params, req, runtime)
         )
 
     def create_pick_up_waybill_pre_query(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_pick_up_waybill_pre_query_with_options(request, runtime)
 
+    def delete_axg_group_with_options(self, request, runtime):
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
+    def delete_axg_group(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_axg_group_with_options(request, runtime)
+
     def delete_secret_blacklist_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.black_no):
             query['BlackNo'] = request.black_no
         if not UtilClient.is_unset(request.black_type):
             query['BlackType'] = request.black_type
```

### Comparing `alibabacloud_dyplsapi20170525_py2-1.0.0/alibabacloud_dyplsapi20170525/models.py` & `alibabacloud_dyplsapi20170525_py2-1.0.1/alibabacloud_dyplsapi20170525/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1158,14 +1158,370 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = BindAxnExtensionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class BindBatchAxgRequestAxgBindList(TeaModel):
+    def __init__(self, asrmodel_id=None, asrstatus=None, call_display_type=None, call_restrict=None,
+                 expect_city=None, expiration=None, group_id=None, is_recording_enabled=None, out_id=None, out_order_id=None,
+                 phone_no_a=None, phone_no_b=None, phone_no_x=None, ring_config=None):
+        self.asrmodel_id = asrmodel_id  # type: str
+        self.asrstatus = asrstatus  # type: bool
+        self.call_display_type = call_display_type  # type: int
+        self.call_restrict = call_restrict  # type: str
+        self.expect_city = expect_city  # type: str
+        self.expiration = expiration  # type: str
+        self.group_id = group_id  # type: str
+        self.is_recording_enabled = is_recording_enabled  # type: bool
+        self.out_id = out_id  # type: str
+        self.out_order_id = out_order_id  # type: str
+        self.phone_no_a = phone_no_a  # type: str
+        self.phone_no_b = phone_no_b  # type: str
+        self.phone_no_x = phone_no_x  # type: str
+        self.ring_config = ring_config  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(BindBatchAxgRequestAxgBindList, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, axg_bind_list=None, owner_id=None, pool_key=None, resource_owner_account=None,
+                 resource_owner_id=None):
+        self.axg_bind_list = axg_bind_list  # type: list[BindBatchAxgRequestAxgBindList]
+        self.owner_id = owner_id  # type: long
+        self.pool_key = pool_key  # type: str
+        self.resource_owner_account = resource_owner_account  # type: str
+        self.resource_owner_id = resource_owner_id  # type: long
+
+    def validate(self):
+        if self.axg_bind_list:
+            for k in self.axg_bind_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(BindBatchAxgRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, axg_bind_list_shrink=None, owner_id=None, pool_key=None, resource_owner_account=None,
+                 resource_owner_id=None):
+        self.axg_bind_list_shrink = axg_bind_list_shrink  # type: str
+        self.owner_id = owner_id  # type: long
+        self.pool_key = pool_key  # type: str
+        self.resource_owner_account = resource_owner_account  # type: str
+        self.resource_owner_id = resource_owner_id  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(BindBatchAxgShrinkRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, extension=None, group_id=None, message=None, phone_no_a=None, secret_no=None,
+                 subs_id=None):
+        self.code = code  # type: str
+        self.extension = extension  # type: str
+        self.group_id = group_id  # type: str
+        self.message = message  # type: str
+        self.phone_no_a = phone_no_a  # type: str
+        self.secret_no = secret_no  # type: str
+        self.subs_id = subs_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(BindBatchAxgResponseBodySecretBindListSecretBind, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, secret_bind=None):
+        self.secret_bind = secret_bind  # type: list[BindBatchAxgResponseBodySecretBindListSecretBind]
+
+    def validate(self):
+        if self.secret_bind:
+            for k in self.secret_bind:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(BindBatchAxgResponseBodySecretBindList, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, message=None, request_id=None, secret_bind_list=None):
+        self.code = code  # type: str
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+        self.secret_bind_list = secret_bind_list  # type: BindBatchAxgResponseBodySecretBindList
+
+    def validate(self):
+        if self.secret_bind_list:
+            self.secret_bind_list.validate()
+
+    def to_map(self):
+        _map = super(BindBatchAxgResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: BindBatchAxgResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(BindBatchAxgResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, city=None, display_pool=None, owner_id=None, pool_key=None, resource_owner_account=None,
                  resource_owner_id=None, secret_no=None, spec_id=None):
         self.city = city  # type: str
         self.display_pool = display_pool  # type: bool
         self.owner_id = owner_id  # type: long
         self.pool_key = pool_key  # type: str
@@ -2651,14 +3007,132 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreatePickUpWaybillPreQueryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteAxgGroupRequest(TeaModel):
+    def __init__(self, group_id=None, owner_id=None, pool_key=None, resource_owner_account=None,
+                 resource_owner_id=None):
+        self.group_id = group_id  # type: long
+        self.owner_id = owner_id  # type: long
+        self.pool_key = pool_key  # type: str
+        self.resource_owner_account = resource_owner_account  # type: str
+        self.resource_owner_id = resource_owner_id  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteAxgGroupRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, message=None, request_id=None):
+        self.code = code  # type: str
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteAxgGroupResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeleteAxgGroupResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeleteAxgGroupResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, black_no=None, black_type=None, pool_key=None, remark=None, way_control=None):
         self.black_no = black_no  # type: str
         self.black_type = black_type  # type: str
         self.pool_key = pool_key  # type: str
         self.remark = remark  # type: str
         self.way_control = way_control  # type: str
```

### Comparing `alibabacloud_dyplsapi20170525_py2-1.0.0/alibabacloud_dyplsapi20170525_py2.egg-info/PKG-INFO` & `alibabacloud_dyplsapi20170525_py2-1.0.1/alibabacloud_dyplsapi20170525_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dyplsapi20170525-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Dyplsapi (20170525) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dyplsapi20170525_py2-1.0.0/setup.py` & `alibabacloud_dyplsapi20170525_py2-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dyplsapi20170525_py2.
 
-Created on 24/02/2023
+Created on 04/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dyplsapi20170525"
 NAME = "alibabacloud_dyplsapi20170525_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dyplsapi (20170525) SDK Library for Python2"
```

