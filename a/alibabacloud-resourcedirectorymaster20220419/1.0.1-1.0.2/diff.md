# Comparing `tmp/alibabacloud_resourcedirectorymaster20220419-1.0.1.tar.gz` & `tmp/alibabacloud_resourcedirectorymaster20220419-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcedirectorymaster20220419-1.0.1.tar", last modified: Wed Apr 12 09:31:31 2023, max compression
+gzip compressed data, was "dist/alibabacloud_resourcedirectorymaster20220419-1.0.2.tar", last modified: Thu May  4 11:31:56 2023, max compression
```

## Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.1.tar` & `alibabacloud_resourcedirectorymaster20220419-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2448 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1082 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1167 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419/__init__.py
--rw-r--r--   0 root         (0) root         (0)   259967 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419/client.py
--rw-r--r--   0 root         (0) root         (0)   397637 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2448 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      580 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2710 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   226837 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419/client.py
+-rw-r--r--   0 root         (0) root         (0)   368465 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/setup.py
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.1/LICENSE` & `alibabacloud_resourcedirectorymaster20220419-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.1/PKG-INFO` & `alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_resourcedirectorymaster20220419
-Version: 1.0.1
+Name: alibabacloud-resourcedirectorymaster20220419
+Version: 1.0.2
 Summary: Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.1/README-CN.md` & `alibabacloud_resourcedirectorymaster20220419-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.1/README.md` & `alibabacloud_resourcedirectorymaster20220419-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419/client.py` & `alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -42,21 +42,14 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def accept_handshake_with_options(
         self,
         request: resource_directory_master_20220419_models.AcceptHandshakeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.AcceptHandshakeResponse:
-        """
-        After an invited Alibaba Cloud account joins a resource directory, it becomes a member of the resource directory. By default, the name of the invited Alibaba Cloud account is used as the display name of the account in the resource directory.
-        
-        @param request: AcceptHandshakeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AcceptHandshakeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.handshake_id):
             query['HandshakeId'] = request.handshake_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -77,21 +70,14 @@
         )
 
     async def accept_handshake_with_options_async(
         self,
         request: resource_directory_master_20220419_models.AcceptHandshakeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.AcceptHandshakeResponse:
-        """
-        After an invited Alibaba Cloud account joins a resource directory, it becomes a member of the resource directory. By default, the name of the invited Alibaba Cloud account is used as the display name of the account in the resource directory.
-        
-        @param request: AcceptHandshakeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AcceptHandshakeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.handshake_id):
             query['HandshakeId'] = request.handshake_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -111,33 +97,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def accept_handshake(
         self,
         request: resource_directory_master_20220419_models.AcceptHandshakeRequest,
     ) -> resource_directory_master_20220419_models.AcceptHandshakeResponse:
-        """
-        After an invited Alibaba Cloud account joins a resource directory, it becomes a member of the resource directory. By default, the name of the invited Alibaba Cloud account is used as the display name of the account in the resource directory.
-        
-        @param request: AcceptHandshakeRequest
-        @return: AcceptHandshakeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.accept_handshake_with_options(request, runtime)
 
     async def accept_handshake_async(
         self,
         request: resource_directory_master_20220419_models.AcceptHandshakeRequest,
     ) -> resource_directory_master_20220419_models.AcceptHandshakeResponse:
-        """
-        After an invited Alibaba Cloud account joins a resource directory, it becomes a member of the resource directory. By default, the name of the invited Alibaba Cloud account is used as the display name of the account in the resource directory.
-        
-        @param request: AcceptHandshakeRequest
-        @return: AcceptHandshakeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.accept_handshake_with_options_async(request, runtime)
 
     def add_message_contact_with_options(
         self,
         request: resource_directory_master_20220419_models.AddMessageContactRequest,
         runtime: util_models.RuntimeOptions,
@@ -299,18 +273,15 @@
 
     def attach_control_policy_with_options(
         self,
         request: resource_directory_master_20220419_models.AttachControlPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.AttachControlPolicyResponse:
         """
-        After you attach a custom access control policy, the operations performed on resources by using members are limited by the policy. Make sure that the attached policy meets your expectations. Otherwise, your business may be affected.
-        By default, the system access control policy FullAliyunAccess is attached to each folder and member.
-        The access control policy that is attached to a folder also applies to all its subfolders and all members in the subfolders.
-        A maximum of 10 access control policies can be attached to a folder or member.
+        The ID of the request.
         
         @param request: AttachControlPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: AttachControlPolicyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -339,18 +310,15 @@
 
     async def attach_control_policy_with_options_async(
         self,
         request: resource_directory_master_20220419_models.AttachControlPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.AttachControlPolicyResponse:
         """
-        After you attach a custom access control policy, the operations performed on resources by using members are limited by the policy. Make sure that the attached policy meets your expectations. Otherwise, your business may be affected.
-        By default, the system access control policy FullAliyunAccess is attached to each folder and member.
-        The access control policy that is attached to a folder also applies to all its subfolders and all members in the subfolders.
-        A maximum of 10 access control policies can be attached to a folder or member.
+        The ID of the request.
         
         @param request: AttachControlPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: AttachControlPolicyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -378,49 +346,42 @@
         )
 
     def attach_control_policy(
         self,
         request: resource_directory_master_20220419_models.AttachControlPolicyRequest,
     ) -> resource_directory_master_20220419_models.AttachControlPolicyResponse:
         """
-        After you attach a custom access control policy, the operations performed on resources by using members are limited by the policy. Make sure that the attached policy meets your expectations. Otherwise, your business may be affected.
-        By default, the system access control policy FullAliyunAccess is attached to each folder and member.
-        The access control policy that is attached to a folder also applies to all its subfolders and all members in the subfolders.
-        A maximum of 10 access control policies can be attached to a folder or member.
+        The ID of the request.
         
         @param request: AttachControlPolicyRequest
         @return: AttachControlPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.attach_control_policy_with_options(request, runtime)
 
     async def attach_control_policy_async(
         self,
         request: resource_directory_master_20220419_models.AttachControlPolicyRequest,
     ) -> resource_directory_master_20220419_models.AttachControlPolicyResponse:
         """
-        After you attach a custom access control policy, the operations performed on resources by using members are limited by the policy. Make sure that the attached policy meets your expectations. Otherwise, your business may be affected.
-        By default, the system access control policy FullAliyunAccess is attached to each folder and member.
-        The access control policy that is attached to a folder also applies to all its subfolders and all members in the subfolders.
-        A maximum of 10 access control policies can be attached to a folder or member.
+        The ID of the request.
         
         @param request: AttachControlPolicyRequest
         @return: AttachControlPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.attach_control_policy_with_options_async(request, runtime)
 
     def bind_secure_mobile_phone_with_options(
         self,
         request: resource_directory_master_20220419_models.BindSecureMobilePhoneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.BindSecureMobilePhoneResponse:
         """
-        You can call this API operation only to bind a mobile phone number to a member of the resource account type. You cannot call this API operation to change the mobile phone number that is bound to a member of the resource account type.
-        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this API operation.
+        The ID of the request.
         
         @param request: BindSecureMobilePhoneRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BindSecureMobilePhoneResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -451,16 +412,15 @@
 
     async def bind_secure_mobile_phone_with_options_async(
         self,
         request: resource_directory_master_20220419_models.BindSecureMobilePhoneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.BindSecureMobilePhoneResponse:
         """
-        You can call this API operation only to bind a mobile phone number to a member of the resource account type. You cannot call this API operation to change the mobile phone number that is bound to a member of the resource account type.
-        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this API operation.
+        The ID of the request.
         
         @param request: BindSecureMobilePhoneRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BindSecureMobilePhoneResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -490,30 +450,28 @@
         )
 
     def bind_secure_mobile_phone(
         self,
         request: resource_directory_master_20220419_models.BindSecureMobilePhoneRequest,
     ) -> resource_directory_master_20220419_models.BindSecureMobilePhoneResponse:
         """
-        You can call this API operation only to bind a mobile phone number to a member of the resource account type. You cannot call this API operation to change the mobile phone number that is bound to a member of the resource account type.
-        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this API operation.
+        The ID of the request.
         
         @param request: BindSecureMobilePhoneRequest
         @return: BindSecureMobilePhoneResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.bind_secure_mobile_phone_with_options(request, runtime)
 
     async def bind_secure_mobile_phone_async(
         self,
         request: resource_directory_master_20220419_models.BindSecureMobilePhoneRequest,
     ) -> resource_directory_master_20220419_models.BindSecureMobilePhoneResponse:
         """
-        You can call this API operation only to bind a mobile phone number to a member of the resource account type. You cannot call this API operation to change the mobile phone number that is bound to a member of the resource account type.
-        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this API operation.
+        The ID of the request.
         
         @param request: BindSecureMobilePhoneRequest
         @return: BindSecureMobilePhoneResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.bind_secure_mobile_phone_with_options_async(request, runtime)
 
@@ -811,15 +769,15 @@
 
     def check_account_delete_with_options(
         self,
         request: resource_directory_master_20220419_models.CheckAccountDeleteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.CheckAccountDeleteResponse:
         """
-        Before you delete a member, you must call this API operation to check whether the member can be deleted.
+        The returned result.
         
         @param request: CheckAccountDeleteRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CheckAccountDeleteResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -846,15 +804,15 @@
 
     async def check_account_delete_with_options_async(
         self,
         request: resource_directory_master_20220419_models.CheckAccountDeleteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.CheckAccountDeleteResponse:
         """
-        Before you delete a member, you must call this API operation to check whether the member can be deleted.
+        The returned result.
         
         @param request: CheckAccountDeleteRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CheckAccountDeleteResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -880,28 +838,28 @@
         )
 
     def check_account_delete(
         self,
         request: resource_directory_master_20220419_models.CheckAccountDeleteRequest,
     ) -> resource_directory_master_20220419_models.CheckAccountDeleteResponse:
         """
-        Before you delete a member, you must call this API operation to check whether the member can be deleted.
+        The returned result.
         
         @param request: CheckAccountDeleteRequest
         @return: CheckAccountDeleteResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.check_account_delete_with_options(request, runtime)
 
     async def check_account_delete_async(
         self,
         request: resource_directory_master_20220419_models.CheckAccountDeleteRequest,
     ) -> resource_directory_master_20220419_models.CheckAccountDeleteResponse:
         """
-        Before you delete a member, you must call this API operation to check whether the member can be deleted.
+        The returned result.
         
         @param request: CheckAccountDeleteRequest
         @return: CheckAccountDeleteResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.check_account_delete_with_options_async(request, runtime)
 
@@ -989,15 +947,15 @@
 
     def create_folder_with_options(
         self,
         request: resource_directory_master_20220419_models.CreateFolderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.CreateFolderResponse:
         """
-        A maximum of five levels of folders can be created under the Root folder.
+        The name of the folder.
         
         @param request: CreateFolderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateFolderResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1026,15 +984,15 @@
 
     async def create_folder_with_options_async(
         self,
         request: resource_directory_master_20220419_models.CreateFolderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.CreateFolderResponse:
         """
-        A maximum of five levels of folders can be created under the Root folder.
+        The name of the folder.
         
         @param request: CreateFolderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateFolderResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1062,43 +1020,42 @@
         )
 
     def create_folder(
         self,
         request: resource_directory_master_20220419_models.CreateFolderRequest,
     ) -> resource_directory_master_20220419_models.CreateFolderResponse:
         """
-        A maximum of five levels of folders can be created under the Root folder.
+        The name of the folder.
         
         @param request: CreateFolderRequest
         @return: CreateFolderResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_folder_with_options(request, runtime)
 
     async def create_folder_async(
         self,
         request: resource_directory_master_20220419_models.CreateFolderRequest,
     ) -> resource_directory_master_20220419_models.CreateFolderResponse:
         """
-        A maximum of five levels of folders can be created under the Root folder.
+        The name of the folder.
         
         @param request: CreateFolderRequest
         @return: CreateFolderResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_folder_with_options_async(request, runtime)
 
     def create_resource_account_with_options(
         self,
         request: resource_directory_master_20220419_models.CreateResourceAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.CreateResourceAccountResponse:
         """
-        A member serves as a container for resources and is also an organizational unit in a resource directory. A member indicates a project or application. The resources of different members are isolated.
-        This topic provides an example on how to call the API operation to create a member in the `fd-r23M55****` folder. The display name of the member is `Dev`, and the prefix for the Alibaba Cloud account name of the member is `alice`.
+        The Alibaba Cloud account name of the member.
         
         @param request: CreateResourceAccountRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateResourceAccountResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1135,16 +1092,15 @@
 
     async def create_resource_account_with_options_async(
         self,
         request: resource_directory_master_20220419_models.CreateResourceAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.CreateResourceAccountResponse:
         """
-        A member serves as a container for resources and is also an organizational unit in a resource directory. A member indicates a project or application. The resources of different members are isolated.
-        This topic provides an example on how to call the API operation to create a member in the `fd-r23M55****` folder. The display name of the member is `Dev`, and the prefix for the Alibaba Cloud account name of the member is `alice`.
+        The Alibaba Cloud account name of the member.
         
         @param request: CreateResourceAccountRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateResourceAccountResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1180,30 +1136,28 @@
         )
 
     def create_resource_account(
         self,
         request: resource_directory_master_20220419_models.CreateResourceAccountRequest,
     ) -> resource_directory_master_20220419_models.CreateResourceAccountResponse:
         """
-        A member serves as a container for resources and is also an organizational unit in a resource directory. A member indicates a project or application. The resources of different members are isolated.
-        This topic provides an example on how to call the API operation to create a member in the `fd-r23M55****` folder. The display name of the member is `Dev`, and the prefix for the Alibaba Cloud account name of the member is `alice`.
+        The Alibaba Cloud account name of the member.
         
         @param request: CreateResourceAccountRequest
         @return: CreateResourceAccountResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_resource_account_with_options(request, runtime)
 
     async def create_resource_account_async(
         self,
         request: resource_directory_master_20220419_models.CreateResourceAccountRequest,
     ) -> resource_directory_master_20220419_models.CreateResourceAccountResponse:
         """
-        A member serves as a container for resources and is also an organizational unit in a resource directory. A member indicates a project or application. The resources of different members are isolated.
-        This topic provides an example on how to call the API operation to create a member in the `fd-r23M55****` folder. The display name of the member is `Dev`, and the prefix for the Alibaba Cloud account name of the member is `alice`.
+        The Alibaba Cloud account name of the member.
         
         @param request: CreateResourceAccountRequest
         @return: CreateResourceAccountResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_resource_account_with_options_async(request, runtime)
 
@@ -1278,23 +1232,14 @@
         return await self.decline_handshake_with_options_async(request, runtime)
 
     def delete_account_with_options(
         self,
         tmp_req: resource_directory_master_20220419_models.DeleteAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeleteAccountResponse:
-        """
-        > The member deletion feature is in invitational preview. You can contact the customer business manager (CBM) of Alibaba Cloud to apply for a trial.
-        Before you delete a member, we recommend that you call the [CheckAccountDelete](~~CheckAccountDelete~~) and [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operations to check whether the member meets deletion requirements. You can call the DeleteAccount operation to delete only members that meet the deletion requirements.
-        After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
-        
-        @param tmp_req: DeleteAccountRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteAccountResponse
-        """
         UtilClient.validate_model(tmp_req)
         request = resource_directory_master_20220419_models.DeleteAccountShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.abandonable_check_id):
             request.abandonable_check_id_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.abandonable_check_id, 'AbandonableCheckId', 'json')
         query = {}
         if not UtilClient.is_unset(request.abandonable_check_id_shrink):
@@ -1321,23 +1266,14 @@
         )
 
     async def delete_account_with_options_async(
         self,
         tmp_req: resource_directory_master_20220419_models.DeleteAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeleteAccountResponse:
-        """
-        > The member deletion feature is in invitational preview. You can contact the customer business manager (CBM) of Alibaba Cloud to apply for a trial.
-        Before you delete a member, we recommend that you call the [CheckAccountDelete](~~CheckAccountDelete~~) and [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operations to check whether the member meets deletion requirements. You can call the DeleteAccount operation to delete only members that meet the deletion requirements.
-        After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
-        
-        @param tmp_req: DeleteAccountRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteAccountResponse
-        """
         UtilClient.validate_model(tmp_req)
         request = resource_directory_master_20220419_models.DeleteAccountShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.abandonable_check_id):
             request.abandonable_check_id_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.abandonable_check_id, 'AbandonableCheckId', 'json')
         query = {}
         if not UtilClient.is_unset(request.abandonable_check_id_shrink):
@@ -1363,47 +1299,31 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_account(
         self,
         request: resource_directory_master_20220419_models.DeleteAccountRequest,
     ) -> resource_directory_master_20220419_models.DeleteAccountResponse:
-        """
-        > The member deletion feature is in invitational preview. You can contact the customer business manager (CBM) of Alibaba Cloud to apply for a trial.
-        Before you delete a member, we recommend that you call the [CheckAccountDelete](~~CheckAccountDelete~~) and [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operations to check whether the member meets deletion requirements. You can call the DeleteAccount operation to delete only members that meet the deletion requirements.
-        After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
-        
-        @param request: DeleteAccountRequest
-        @return: DeleteAccountResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.delete_account_with_options(request, runtime)
 
     async def delete_account_async(
         self,
         request: resource_directory_master_20220419_models.DeleteAccountRequest,
     ) -> resource_directory_master_20220419_models.DeleteAccountResponse:
-        """
-        > The member deletion feature is in invitational preview. You can contact the customer business manager (CBM) of Alibaba Cloud to apply for a trial.
-        Before you delete a member, we recommend that you call the [CheckAccountDelete](~~CheckAccountDelete~~) and [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operations to check whether the member meets deletion requirements. You can call the DeleteAccount operation to delete only members that meet the deletion requirements.
-        After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
-        
-        @param request: DeleteAccountRequest
-        @return: DeleteAccountResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_account_with_options_async(request, runtime)
 
     def delete_control_policy_with_options(
         self,
         request: resource_directory_master_20220419_models.DeleteControlPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeleteControlPolicyResponse:
         """
-        If you want to delete a custom access control policy that is attached to folders or members, you must call the [DetachControlPolicy](~~DetachControlPolicy~~) operation to detach the policy before you delete it.
+        The ID of the request.
         
         @param request: DeleteControlPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteControlPolicyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1430,15 +1350,15 @@
 
     async def delete_control_policy_with_options_async(
         self,
         request: resource_directory_master_20220419_models.DeleteControlPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeleteControlPolicyResponse:
         """
-        If you want to delete a custom access control policy that is attached to folders or members, you must call the [DetachControlPolicy](~~DetachControlPolicy~~) operation to detach the policy before you delete it.
+        The ID of the request.
         
         @param request: DeleteControlPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteControlPolicyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1464,42 +1384,42 @@
         )
 
     def delete_control_policy(
         self,
         request: resource_directory_master_20220419_models.DeleteControlPolicyRequest,
     ) -> resource_directory_master_20220419_models.DeleteControlPolicyResponse:
         """
-        If you want to delete a custom access control policy that is attached to folders or members, you must call the [DetachControlPolicy](~~DetachControlPolicy~~) operation to detach the policy before you delete it.
+        The ID of the request.
         
         @param request: DeleteControlPolicyRequest
         @return: DeleteControlPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_control_policy_with_options(request, runtime)
 
     async def delete_control_policy_async(
         self,
         request: resource_directory_master_20220419_models.DeleteControlPolicyRequest,
     ) -> resource_directory_master_20220419_models.DeleteControlPolicyResponse:
         """
-        If you want to delete a custom access control policy that is attached to folders or members, you must call the [DetachControlPolicy](~~DetachControlPolicy~~) operation to detach the policy before you delete it.
+        The ID of the request.
         
         @param request: DeleteControlPolicyRequest
         @return: DeleteControlPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_control_policy_with_options_async(request, runtime)
 
     def delete_folder_with_options(
         self,
         request: resource_directory_master_20220419_models.DeleteFolderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeleteFolderResponse:
         """
-        Before you delete a folder, you must make sure that the folder does not contain members or subfolders.
+        The ID of the request.
         
         @param request: DeleteFolderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteFolderResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1526,15 +1446,15 @@
 
     async def delete_folder_with_options_async(
         self,
         request: resource_directory_master_20220419_models.DeleteFolderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeleteFolderResponse:
         """
-        Before you delete a folder, you must make sure that the folder does not contain members or subfolders.
+        The ID of the request.
         
         @param request: DeleteFolderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteFolderResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1560,28 +1480,28 @@
         )
 
     def delete_folder(
         self,
         request: resource_directory_master_20220419_models.DeleteFolderRequest,
     ) -> resource_directory_master_20220419_models.DeleteFolderResponse:
         """
-        Before you delete a folder, you must make sure that the folder does not contain members or subfolders.
+        The ID of the request.
         
         @param request: DeleteFolderRequest
         @return: DeleteFolderResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_folder_with_options(request, runtime)
 
     async def delete_folder_async(
         self,
         request: resource_directory_master_20220419_models.DeleteFolderRequest,
     ) -> resource_directory_master_20220419_models.DeleteFolderResponse:
         """
-        Before you delete a folder, you must make sure that the folder does not contain members or subfolders.
+        The ID of the request.
         
         @param request: DeleteFolderRequest
         @return: DeleteFolderResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_folder_with_options_async(request, runtime)
 
@@ -1660,21 +1580,14 @@
         return await self.delete_message_contact_with_options_async(request, runtime)
 
     def deregister_delegated_administrator_with_options(
         self,
         request: resource_directory_master_20220419_models.DeregisterDelegatedAdministratorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeregisterDelegatedAdministratorResponse:
-        """
-        If the delegated administrator account that you want to remove has historical management tasks in the related trusted service, the trusted service may be affected after the delegated administrator account is removed. Therefore, proceed with caution.
-        
-        @param request: DeregisterDelegatedAdministratorRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeregisterDelegatedAdministratorResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.service_principal):
             query['ServicePrincipal'] = request.service_principal
         req = open_api_models.OpenApiRequest(
@@ -1697,21 +1610,14 @@
         )
 
     async def deregister_delegated_administrator_with_options_async(
         self,
         request: resource_directory_master_20220419_models.DeregisterDelegatedAdministratorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeregisterDelegatedAdministratorResponse:
-        """
-        If the delegated administrator account that you want to remove has historical management tasks in the related trusted service, the trusted service may be affected after the delegated administrator account is removed. Therefore, proceed with caution.
-        
-        @param request: DeregisterDelegatedAdministratorRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeregisterDelegatedAdministratorResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.service_principal):
             query['ServicePrincipal'] = request.service_principal
         req = open_api_models.OpenApiRequest(
@@ -1733,44 +1639,30 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def deregister_delegated_administrator(
         self,
         request: resource_directory_master_20220419_models.DeregisterDelegatedAdministratorRequest,
     ) -> resource_directory_master_20220419_models.DeregisterDelegatedAdministratorResponse:
-        """
-        If the delegated administrator account that you want to remove has historical management tasks in the related trusted service, the trusted service may be affected after the delegated administrator account is removed. Therefore, proceed with caution.
-        
-        @param request: DeregisterDelegatedAdministratorRequest
-        @return: DeregisterDelegatedAdministratorResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.deregister_delegated_administrator_with_options(request, runtime)
 
     async def deregister_delegated_administrator_async(
         self,
         request: resource_directory_master_20220419_models.DeregisterDelegatedAdministratorRequest,
     ) -> resource_directory_master_20220419_models.DeregisterDelegatedAdministratorResponse:
-        """
-        If the delegated administrator account that you want to remove has historical management tasks in the related trusted service, the trusted service may be affected after the delegated administrator account is removed. Therefore, proceed with caution.
-        
-        @param request: DeregisterDelegatedAdministratorRequest
-        @return: DeregisterDelegatedAdministratorResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.deregister_delegated_administrator_with_options_async(request, runtime)
 
     def destroy_resource_directory_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DestroyResourceDirectoryResponse:
         """
-        Before you disable a resource directory, you must make sure that the following requirements are met:
-        *   All members of the cloud account type in the resource directory are removed. You can call the [RemoveCloudAccount](~~RemoveCloudAccount~~) operation to remove a member of the cloud account type.
-        *   All folders except the Root folder are deleted from the resource directory. You can call the [DeleteFolder](~~DeleteFolder~~) operation to delete a folder.
+        The ID of the request.
         
         @param request: DestroyResourceDirectoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DestroyResourceDirectoryResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -1790,17 +1682,15 @@
         )
 
     async def destroy_resource_directory_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DestroyResourceDirectoryResponse:
         """
-        Before you disable a resource directory, you must make sure that the following requirements are met:
-        *   All members of the cloud account type in the resource directory are removed. You can call the [RemoveCloudAccount](~~RemoveCloudAccount~~) operation to remove a member of the cloud account type.
-        *   All folders except the Root folder are deleted from the resource directory. You can call the [DeleteFolder](~~DeleteFolder~~) operation to delete a folder.
+        The ID of the request.
         
         @param request: DestroyResourceDirectoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DestroyResourceDirectoryResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -1817,47 +1707,35 @@
         return TeaCore.from_map(
             resource_directory_master_20220419_models.DestroyResourceDirectoryResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def destroy_resource_directory(self) -> resource_directory_master_20220419_models.DestroyResourceDirectoryResponse:
         """
-        Before you disable a resource directory, you must make sure that the following requirements are met:
-        *   All members of the cloud account type in the resource directory are removed. You can call the [RemoveCloudAccount](~~RemoveCloudAccount~~) operation to remove a member of the cloud account type.
-        *   All folders except the Root folder are deleted from the resource directory. You can call the [DeleteFolder](~~DeleteFolder~~) operation to delete a folder.
+        The ID of the request.
         
         @return: DestroyResourceDirectoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.destroy_resource_directory_with_options(runtime)
 
     async def destroy_resource_directory_async(self) -> resource_directory_master_20220419_models.DestroyResourceDirectoryResponse:
         """
-        Before you disable a resource directory, you must make sure that the following requirements are met:
-        *   All members of the cloud account type in the resource directory are removed. You can call the [RemoveCloudAccount](~~RemoveCloudAccount~~) operation to remove a member of the cloud account type.
-        *   All folders except the Root folder are deleted from the resource directory. You can call the [DeleteFolder](~~DeleteFolder~~) operation to delete a folder.
+        The ID of the request.
         
         @return: DestroyResourceDirectoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.destroy_resource_directory_with_options_async(runtime)
 
     def detach_control_policy_with_options(
         self,
         request: resource_directory_master_20220419_models.DetachControlPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DetachControlPolicyResponse:
-        """
-        After you detach an access control policy, the operations performed on resources by using members are not limited by the policy. Make sure that the detached policy meets your expectations. Otherwise, your business may be affected.
-        Both the system and custom access control policies can be detached. If an object has only one access control policy attached, the policy cannot be detached.
-        
-        @param request: DetachControlPolicyRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DetachControlPolicyResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.policy_id):
             query['PolicyId'] = request.policy_id
         if not UtilClient.is_unset(request.target_id):
             query['TargetId'] = request.target_id
         req = open_api_models.OpenApiRequest(
@@ -1880,22 +1758,14 @@
         )
 
     async def detach_control_policy_with_options_async(
         self,
         request: resource_directory_master_20220419_models.DetachControlPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DetachControlPolicyResponse:
-        """
-        After you detach an access control policy, the operations performed on resources by using members are not limited by the policy. Make sure that the detached policy meets your expectations. Otherwise, your business may be affected.
-        Both the system and custom access control policies can be detached. If an object has only one access control policy attached, the policy cannot be detached.
-        
-        @param request: DetachControlPolicyRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DetachControlPolicyResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.policy_id):
             query['PolicyId'] = request.policy_id
         if not UtilClient.is_unset(request.target_id):
             query['TargetId'] = request.target_id
         req = open_api_models.OpenApiRequest(
@@ -1917,45 +1787,30 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def detach_control_policy(
         self,
         request: resource_directory_master_20220419_models.DetachControlPolicyRequest,
     ) -> resource_directory_master_20220419_models.DetachControlPolicyResponse:
-        """
-        After you detach an access control policy, the operations performed on resources by using members are not limited by the policy. Make sure that the detached policy meets your expectations. Otherwise, your business may be affected.
-        Both the system and custom access control policies can be detached. If an object has only one access control policy attached, the policy cannot be detached.
-        
-        @param request: DetachControlPolicyRequest
-        @return: DetachControlPolicyResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.detach_control_policy_with_options(request, runtime)
 
     async def detach_control_policy_async(
         self,
         request: resource_directory_master_20220419_models.DetachControlPolicyRequest,
     ) -> resource_directory_master_20220419_models.DetachControlPolicyResponse:
-        """
-        After you detach an access control policy, the operations performed on resources by using members are not limited by the policy. Make sure that the detached policy meets your expectations. Otherwise, your business may be affected.
-        Both the system and custom access control policies can be detached. If an object has only one access control policy attached, the policy cannot be detached.
-        
-        @param request: DetachControlPolicyRequest
-        @return: DetachControlPolicyResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.detach_control_policy_with_options_async(request, runtime)
 
     def disable_control_policy_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DisableControlPolicyResponse:
         """
-        After you disable the Control Policy feature, the system automatically detaches all access control policies that are attached to folders and members. The system does not delete these access control policies, but you cannot attach them to folders or members again.
-        > If you disable the Control Policy feature, the permissions of all folders and members in your resource directory are affected. Therefore, proceed with caution.
+        The ID of the request.
         
         @param request: DisableControlPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DisableControlPolicyResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -1975,16 +1830,15 @@
         )
 
     async def disable_control_policy_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DisableControlPolicyResponse:
         """
-        After you disable the Control Policy feature, the system automatically detaches all access control policies that are attached to folders and members. The system does not delete these access control policies, but you cannot attach them to folders or members again.
-        > If you disable the Control Policy feature, the permissions of all folders and members in your resource directory are affected. Therefore, proceed with caution.
+        The ID of the request.
         
         @param request: DisableControlPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DisableControlPolicyResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -2001,26 +1855,24 @@
         return TeaCore.from_map(
             resource_directory_master_20220419_models.DisableControlPolicyResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def disable_control_policy(self) -> resource_directory_master_20220419_models.DisableControlPolicyResponse:
         """
-        After you disable the Control Policy feature, the system automatically detaches all access control policies that are attached to folders and members. The system does not delete these access control policies, but you cannot attach them to folders or members again.
-        > If you disable the Control Policy feature, the permissions of all folders and members in your resource directory are affected. Therefore, proceed with caution.
+        The ID of the request.
         
         @return: DisableControlPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.disable_control_policy_with_options(runtime)
 
     async def disable_control_policy_async(self) -> resource_directory_master_20220419_models.DisableControlPolicyResponse:
         """
-        After you disable the Control Policy feature, the system automatically detaches all access control policies that are attached to folders and members. The system does not delete these access control policies, but you cannot attach them to folders or members again.
-        > If you disable the Control Policy feature, the permissions of all folders and members in your resource directory are affected. Therefore, proceed with caution.
+        The ID of the request.
         
         @return: DisableControlPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.disable_control_policy_with_options_async(runtime)
 
     def disassociate_members_with_options(
@@ -2098,15 +1950,15 @@
         return await self.disassociate_members_with_options_async(request, runtime)
 
     def enable_control_policy_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.EnableControlPolicyResponse:
         """
-        The Control Policy feature provided by the Resource Directory service allows you to manage the permission boundaries of the folders or members in your resource directory in a centralized manner. This feature is implemented based on the resource directory. You can use this feature to develop common or dedicated rules for access control. The Control Policy feature does not grant permissions but only defines permission boundaries. A member in a resource directory can be used to access resources only after it is granted the required permissions by using the Resource Access Management (RAM) service. For more information, see [Overview of the Control Policy feature](~~178671~~).
+        The ID of the request.
         
         @param request: EnableControlPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: EnableControlPolicyResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -2126,15 +1978,15 @@
         )
 
     async def enable_control_policy_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.EnableControlPolicyResponse:
         """
-        The Control Policy feature provided by the Resource Directory service allows you to manage the permission boundaries of the folders or members in your resource directory in a centralized manner. This feature is implemented based on the resource directory. You can use this feature to develop common or dedicated rules for access control. The Control Policy feature does not grant permissions but only defines permission boundaries. A member in a resource directory can be used to access resources only after it is granted the required permissions by using the Resource Access Management (RAM) service. For more information, see [Overview of the Control Policy feature](~~178671~~).
+        The ID of the request.
         
         @param request: EnableControlPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: EnableControlPolicyResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -2151,37 +2003,37 @@
         return TeaCore.from_map(
             resource_directory_master_20220419_models.EnableControlPolicyResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def enable_control_policy(self) -> resource_directory_master_20220419_models.EnableControlPolicyResponse:
         """
-        The Control Policy feature provided by the Resource Directory service allows you to manage the permission boundaries of the folders or members in your resource directory in a centralized manner. This feature is implemented based on the resource directory. You can use this feature to develop common or dedicated rules for access control. The Control Policy feature does not grant permissions but only defines permission boundaries. A member in a resource directory can be used to access resources only after it is granted the required permissions by using the Resource Access Management (RAM) service. For more information, see [Overview of the Control Policy feature](~~178671~~).
+        The ID of the request.
         
         @return: EnableControlPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.enable_control_policy_with_options(runtime)
 
     async def enable_control_policy_async(self) -> resource_directory_master_20220419_models.EnableControlPolicyResponse:
         """
-        The Control Policy feature provided by the Resource Directory service allows you to manage the permission boundaries of the folders or members in your resource directory in a centralized manner. This feature is implemented based on the resource directory. You can use this feature to develop common or dedicated rules for access control. The Control Policy feature does not grant permissions but only defines permission boundaries. A member in a resource directory can be used to access resources only after it is granted the required permissions by using the Resource Access Management (RAM) service. For more information, see [Overview of the Control Policy feature](~~178671~~).
+        The ID of the request.
         
         @return: EnableControlPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.enable_control_policy_with_options_async(runtime)
 
     def enable_resource_directory_with_options(
         self,
         request: resource_directory_master_20220419_models.EnableResourceDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.EnableResourceDirectoryResponse:
         """
-        You can use the current account or a newly created account to enable a resource directory. For more information, see [Enable a resource directory](~~111215~~).
+        The ID of the request.
         
         @param request: EnableResourceDirectoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: EnableResourceDirectoryResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2214,15 +2066,15 @@
 
     async def enable_resource_directory_with_options_async(
         self,
         request: resource_directory_master_20220419_models.EnableResourceDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.EnableResourceDirectoryResponse:
         """
-        You can use the current account or a newly created account to enable a resource directory. For more information, see [Enable a resource directory](~~111215~~).
+        The ID of the request.
         
         @param request: EnableResourceDirectoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: EnableResourceDirectoryResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2254,28 +2106,28 @@
         )
 
     def enable_resource_directory(
         self,
         request: resource_directory_master_20220419_models.EnableResourceDirectoryRequest,
     ) -> resource_directory_master_20220419_models.EnableResourceDirectoryResponse:
         """
-        You can use the current account or a newly created account to enable a resource directory. For more information, see [Enable a resource directory](~~111215~~).
+        The ID of the request.
         
         @param request: EnableResourceDirectoryRequest
         @return: EnableResourceDirectoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.enable_resource_directory_with_options(request, runtime)
 
     async def enable_resource_directory_async(
         self,
         request: resource_directory_master_20220419_models.EnableResourceDirectoryRequest,
     ) -> resource_directory_master_20220419_models.EnableResourceDirectoryResponse:
         """
-        You can use the current account or a newly created account to enable a resource directory. For more information, see [Enable a resource directory](~~111215~~).
+        The ID of the request.
         
         @param request: EnableResourceDirectoryRequest
         @return: EnableResourceDirectoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.enable_resource_directory_with_options_async(request, runtime)
 
@@ -2355,15 +2207,15 @@
 
     def get_account_deletion_check_result_with_options(
         self,
         request: resource_directory_master_20220419_models.GetAccountDeletionCheckResultRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.GetAccountDeletionCheckResultResponse:
         """
-        After you call the [CheckAccountDelete](~~CheckAccountDelete~~) operation to perform a member deletion check, you can call the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation to query the check result. If the check result shows that the member meets deletion requirements, you can delete the member. Otherwise, you need to first modify the items that do not meet requirements.
+        Container Service for Kubernetes
         
         @param request: GetAccountDeletionCheckResultRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAccountDeletionCheckResultResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2390,15 +2242,15 @@
 
     async def get_account_deletion_check_result_with_options_async(
         self,
         request: resource_directory_master_20220419_models.GetAccountDeletionCheckResultRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.GetAccountDeletionCheckResultResponse:
         """
-        After you call the [CheckAccountDelete](~~CheckAccountDelete~~) operation to perform a member deletion check, you can call the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation to query the check result. If the check result shows that the member meets deletion requirements, you can delete the member. Otherwise, you need to first modify the items that do not meet requirements.
+        Container Service for Kubernetes
         
         @param request: GetAccountDeletionCheckResultRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAccountDeletionCheckResultResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2424,28 +2276,28 @@
         )
 
     def get_account_deletion_check_result(
         self,
         request: resource_directory_master_20220419_models.GetAccountDeletionCheckResultRequest,
     ) -> resource_directory_master_20220419_models.GetAccountDeletionCheckResultResponse:
         """
-        After you call the [CheckAccountDelete](~~CheckAccountDelete~~) operation to perform a member deletion check, you can call the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation to query the check result. If the check result shows that the member meets deletion requirements, you can delete the member. Otherwise, you need to first modify the items that do not meet requirements.
+        Container Service for Kubernetes
         
         @param request: GetAccountDeletionCheckResultRequest
         @return: GetAccountDeletionCheckResultResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_account_deletion_check_result_with_options(request, runtime)
 
     async def get_account_deletion_check_result_async(
         self,
         request: resource_directory_master_20220419_models.GetAccountDeletionCheckResultRequest,
     ) -> resource_directory_master_20220419_models.GetAccountDeletionCheckResultResponse:
         """
-        After you call the [CheckAccountDelete](~~CheckAccountDelete~~) operation to perform a member deletion check, you can call the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation to query the check result. If the check result shows that the member meets deletion requirements, you can delete the member. Otherwise, you need to first modify the items that do not meet requirements.
+        Container Service for Kubernetes
         
         @param request: GetAccountDeletionCheckResultRequest
         @return: GetAccountDeletionCheckResultResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_account_deletion_check_result_with_options_async(request, runtime)
 
@@ -3048,14 +2900,16 @@
         request: resource_directory_master_20220419_models.InviteAccountToResourceDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.InviteAccountToResourceDirectoryResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.note):
             query['Note'] = request.note
+        if not UtilClient.is_unset(request.parent_folder_id):
+            query['ParentFolderId'] = request.parent_folder_id
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         if not UtilClient.is_unset(request.target_entity):
             query['TargetEntity'] = request.target_entity
         if not UtilClient.is_unset(request.target_type):
             query['TargetType'] = request.target_type
         req = open_api_models.OpenApiRequest(
@@ -3082,14 +2936,16 @@
         request: resource_directory_master_20220419_models.InviteAccountToResourceDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.InviteAccountToResourceDirectoryResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.note):
             query['Note'] = request.note
+        if not UtilClient.is_unset(request.parent_folder_id):
+            query['ParentFolderId'] = request.parent_folder_id
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         if not UtilClient.is_unset(request.target_entity):
             query['TargetEntity'] = request.target_entity
         if not UtilClient.is_unset(request.target_type):
             query['TargetType'] = request.target_type
         req = open_api_models.OpenApiRequest(
@@ -4283,15 +4139,15 @@
 
     def list_trusted_service_status_with_options(
         self,
         request: resource_directory_master_20220419_models.ListTrustedServiceStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.ListTrustedServiceStatusResponse:
         """
-        Only a management account or delegated administrator account can be used to call this operation.
+        The time when the trusted service was enabled.
         
         @param request: ListTrustedServiceStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListTrustedServiceStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4322,15 +4178,15 @@
 
     async def list_trusted_service_status_with_options_async(
         self,
         request: resource_directory_master_20220419_models.ListTrustedServiceStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.ListTrustedServiceStatusResponse:
         """
-        Only a management account or delegated administrator account can be used to call this operation.
+        The time when the trusted service was enabled.
         
         @param request: ListTrustedServiceStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListTrustedServiceStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4360,28 +4216,28 @@
         )
 
     def list_trusted_service_status(
         self,
         request: resource_directory_master_20220419_models.ListTrustedServiceStatusRequest,
     ) -> resource_directory_master_20220419_models.ListTrustedServiceStatusResponse:
         """
-        Only a management account or delegated administrator account can be used to call this operation.
+        The time when the trusted service was enabled.
         
         @param request: ListTrustedServiceStatusRequest
         @return: ListTrustedServiceStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_trusted_service_status_with_options(request, runtime)
 
     async def list_trusted_service_status_async(
         self,
         request: resource_directory_master_20220419_models.ListTrustedServiceStatusRequest,
     ) -> resource_directory_master_20220419_models.ListTrustedServiceStatusResponse:
         """
-        Only a management account or delegated administrator account can be used to call this operation.
+        The time when the trusted service was enabled.
         
         @param request: ListTrustedServiceStatusRequest
         @return: ListTrustedServiceStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_trusted_service_status_with_options_async(request, runtime)
 
@@ -4460,24 +4316,14 @@
         return await self.move_account_with_options_async(request, runtime)
 
     def register_delegated_administrator_with_options(
         self,
         request: resource_directory_master_20220419_models.RegisterDelegatedAdministratorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.RegisterDelegatedAdministratorResponse:
-        """
-        The delegated administrator account can be used to access the information of the resource directory and view the structure and members of the resource directory. The delegated administrator account can also be used to perform service-related management operations in the trusted service on behalf of the management account of the resource directory. When you call this operation, you must take note of the following limits:
-        *   Only some trusted services support delegated administrator accounts. For more information, see [Supported trusted services](~~208133~~).
-        *   Only the management account of a resource directory or an authorized RAM user or RAM role of the management account can be used to call this operation.
-        *   The number of delegated administrator accounts that are allowed for a trusted service is defined by the trusted service.
-        
-        @param request: RegisterDelegatedAdministratorRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: RegisterDelegatedAdministratorResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.service_principal):
             query['ServicePrincipal'] = request.service_principal
         req = open_api_models.OpenApiRequest(
@@ -4500,24 +4346,14 @@
         )
 
     async def register_delegated_administrator_with_options_async(
         self,
         request: resource_directory_master_20220419_models.RegisterDelegatedAdministratorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.RegisterDelegatedAdministratorResponse:
-        """
-        The delegated administrator account can be used to access the information of the resource directory and view the structure and members of the resource directory. The delegated administrator account can also be used to perform service-related management operations in the trusted service on behalf of the management account of the resource directory. When you call this operation, you must take note of the following limits:
-        *   Only some trusted services support delegated administrator accounts. For more information, see [Supported trusted services](~~208133~~).
-        *   Only the management account of a resource directory or an authorized RAM user or RAM role of the management account can be used to call this operation.
-        *   The number of delegated administrator accounts that are allowed for a trusted service is defined by the trusted service.
-        
-        @param request: RegisterDelegatedAdministratorRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: RegisterDelegatedAdministratorResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.service_principal):
             query['ServicePrincipal'] = request.service_principal
         req = open_api_models.OpenApiRequest(
@@ -4539,39 +4375,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def register_delegated_administrator(
         self,
         request: resource_directory_master_20220419_models.RegisterDelegatedAdministratorRequest,
     ) -> resource_directory_master_20220419_models.RegisterDelegatedAdministratorResponse:
-        """
-        The delegated administrator account can be used to access the information of the resource directory and view the structure and members of the resource directory. The delegated administrator account can also be used to perform service-related management operations in the trusted service on behalf of the management account of the resource directory. When you call this operation, you must take note of the following limits:
-        *   Only some trusted services support delegated administrator accounts. For more information, see [Supported trusted services](~~208133~~).
-        *   Only the management account of a resource directory or an authorized RAM user or RAM role of the management account can be used to call this operation.
-        *   The number of delegated administrator accounts that are allowed for a trusted service is defined by the trusted service.
-        
-        @param request: RegisterDelegatedAdministratorRequest
-        @return: RegisterDelegatedAdministratorResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.register_delegated_administrator_with_options(request, runtime)
 
     async def register_delegated_administrator_async(
         self,
         request: resource_directory_master_20220419_models.RegisterDelegatedAdministratorRequest,
     ) -> resource_directory_master_20220419_models.RegisterDelegatedAdministratorResponse:
-        """
-        The delegated administrator account can be used to access the information of the resource directory and view the structure and members of the resource directory. The delegated administrator account can also be used to perform service-related management operations in the trusted service on behalf of the management account of the resource directory. When you call this operation, you must take note of the following limits:
-        *   Only some trusted services support delegated administrator accounts. For more information, see [Supported trusted services](~~208133~~).
-        *   Only the management account of a resource directory or an authorized RAM user or RAM role of the management account can be used to call this operation.
-        *   The number of delegated administrator accounts that are allowed for a trusted service is defined by the trusted service.
-        
-        @param request: RegisterDelegatedAdministratorRequest
-        @return: RegisterDelegatedAdministratorResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.register_delegated_administrator_with_options_async(request, runtime)
 
     def remove_cloud_account_with_options(
         self,
         request: resource_directory_master_20220419_models.RemoveCloudAccountRequest,
         runtime: util_models.RuntimeOptions,
@@ -5312,24 +5130,14 @@
         return await self.untag_resources_with_options_async(request, runtime)
 
     def update_account_with_options(
         self,
         request: resource_directory_master_20220419_models.UpdateAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.UpdateAccountResponse:
-        """
-        ### Prerequisites
-        *   To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this operation.
-        *   Before you switch the type of a member from resource account to cloud account, make sure that specific conditions are met. For more information about the conditions, see [Switch a resource account to a cloud account](~~111233~~).
-        *   Before you switch the type of a member from cloud account to resource account, make sure that specific conditions are met. For more information about the conditions, see [Switch a cloud account to a resource account](~~209980~~).
-        
-        @param request: UpdateAccountRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: UpdateAccountResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.new_account_type):
             query['NewAccountType'] = request.new_account_type
         if not UtilClient.is_unset(request.new_display_name):
@@ -5354,24 +5162,14 @@
         )
 
     async def update_account_with_options_async(
         self,
         request: resource_directory_master_20220419_models.UpdateAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.UpdateAccountResponse:
-        """
-        ### Prerequisites
-        *   To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this operation.
-        *   Before you switch the type of a member from resource account to cloud account, make sure that specific conditions are met. For more information about the conditions, see [Switch a resource account to a cloud account](~~111233~~).
-        *   Before you switch the type of a member from cloud account to resource account, make sure that specific conditions are met. For more information about the conditions, see [Switch a cloud account to a resource account](~~209980~~).
-        
-        @param request: UpdateAccountRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: UpdateAccountResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.new_account_type):
             query['NewAccountType'] = request.new_account_type
         if not UtilClient.is_unset(request.new_display_name):
@@ -5395,39 +5193,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_account(
         self,
         request: resource_directory_master_20220419_models.UpdateAccountRequest,
     ) -> resource_directory_master_20220419_models.UpdateAccountResponse:
-        """
-        ### Prerequisites
-        *   To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this operation.
-        *   Before you switch the type of a member from resource account to cloud account, make sure that specific conditions are met. For more information about the conditions, see [Switch a resource account to a cloud account](~~111233~~).
-        *   Before you switch the type of a member from cloud account to resource account, make sure that specific conditions are met. For more information about the conditions, see [Switch a cloud account to a resource account](~~209980~~).
-        
-        @param request: UpdateAccountRequest
-        @return: UpdateAccountResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.update_account_with_options(request, runtime)
 
     async def update_account_async(
         self,
         request: resource_directory_master_20220419_models.UpdateAccountRequest,
     ) -> resource_directory_master_20220419_models.UpdateAccountResponse:
-        """
-        ### Prerequisites
-        *   To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this operation.
-        *   Before you switch the type of a member from resource account to cloud account, make sure that specific conditions are met. For more information about the conditions, see [Switch a resource account to a cloud account](~~111233~~).
-        *   Before you switch the type of a member from cloud account to resource account, make sure that specific conditions are met. For more information about the conditions, see [Switch a cloud account to a resource account](~~209980~~).
-        
-        @param request: UpdateAccountRequest
-        @return: UpdateAccountResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.update_account_with_options_async(request, runtime)
 
     def update_control_policy_with_options(
         self,
         request: resource_directory_master_20220419_models.UpdateControlPolicyRequest,
         runtime: util_models.RuntimeOptions,
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419/models.py` & `alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 
 
 class AcceptHandshakeRequest(TeaModel):
     def __init__(
         self,
         handshake_id: str = None,
     ):
-        # The ID of the invitation.
-        # 
-        # You can call the [ListHandshakesForAccount](~~ListHandshakesForAccount~~) operation to obtain the ID.
         self.handshake_id = handshake_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -45,44 +42,24 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
-        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time
-        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time
-        # The ID of the invitation.
         self.handshake_id = handshake_id
-        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
-        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
-        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time
-        # The description of the invitation.
         self.note = note
-        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
-        # The status of the invitation. Valid values:
-        # 
-        # *   Pending: The invitation is waiting for confirmation.
-        # *   Accepted: The invitation is accepted.
-        # *   Cancelled: The invitation is canceled.
-        # *   Declined: The invitation is rejected.
-        # *   Expired: The invitation expires.
         self.status = status
-        # The ID or logon email address of the invited Alibaba Cloud account.
         self.target_entity = target_entity
-        # The type of the invited Alibaba Cloud account. Valid values:
-        # 
-        # *   Account: indicates the ID of the Alibaba Cloud account.
-        # *   Email: indicates the logon email address of the Alibaba Cloud account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -143,17 +120,15 @@
 
 class AcceptHandshakeResponseBody(TeaModel):
     def __init__(
         self,
         handshake: AcceptHandshakeResponseBodyHandshake = None,
         request_id: str = None,
     ):
-        # The information of the invitation.
         self.handshake = handshake
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -544,21 +519,15 @@
 
 class AttachControlPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_id: str = None,
         target_id: str = None,
     ):
-        # The ID of the access control policy.
         self.policy_id = policy_id
-        # The ID of the object to which you want to attach the access control policy. Access control policies can be attached to the following objects:
-        # 
-        # *   Root folder
-        # *   Subfolders of the Root folder
-        # *   Members
         self.target_id = target_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -582,15 +551,14 @@
 
 
 class AttachControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -656,27 +624,16 @@
 class BindSecureMobilePhoneRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         secure_mobile_phone: str = None,
         verification_code: str = None,
     ):
-        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
-        # The mobile phone number that you want to bind to the member for security purposes.
-        # 
-        # The mobile phone number you specify must be the same as the mobile phone number that you specify when you call the [SendVerificationCodeForBindSecureMobilePhone](~~SendVerificationCodeForBindSecureMobilePhone~~) operation to obtain a verification code.
-        # 
-        # Specify the mobile phone number in the \<Country code>-\<Mobile phone number> format.
-        # 
-        # > Mobile phone numbers in the `86-<Mobile phone number>` format in the Chinese mainland are not supported.
         self.secure_mobile_phone = secure_mobile_phone
-        # The verification code.
-        # 
-        # You can call the [SendVerificationCodeForBindSecureMobilePhone](~~SendVerificationCodeForBindSecureMobilePhone~~) operation to obtain the verification code.
         self.verification_code = verification_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -704,15 +661,14 @@
 
 
 class BindSecureMobilePhoneResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -776,15 +732,14 @@
 
 
 class CancelChangeAccountEmailRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
     ):
-        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -804,15 +759,14 @@
 
 
 class CancelChangeAccountEmailResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -876,15 +830,14 @@
 
 
 class CancelHandshakeRequest(TeaModel):
     def __init__(
         self,
         handshake_id: str = None,
     ):
-        # The ID of the invitation.
         self.handshake_id = handshake_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -914,44 +867,24 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
-        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time
-        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time
-        # The ID of the invitation.
         self.handshake_id = handshake_id
-        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
-        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
-        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time
-        # The description of the invitation.
         self.note = note
-        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
-        # The status of the invitation. Valid values:
-        # 
-        # *   Pending: The invitation is waiting for confirmation.
-        # *   Accepted: The invitation is accepted.
-        # *   Cancelled: The invitation is canceled.
-        # *   Declined: The invitation is rejected.
-        # *   Expired: The invitation expires.
         self.status = status
-        # The ID or logon email address of the invited account.
         self.target_entity = target_entity
-        # The type of the invited account. Valid values:
-        # 
-        # *   Account: indicates the ID of the account.
-        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1012,17 +945,15 @@
 
 class CancelHandshakeResponseBody(TeaModel):
     def __init__(
         self,
         handshake: CancelHandshakeResponseBodyHandshake = None,
         request_id: str = None,
     ):
-        # The information of the invitation.
         self.handshake = handshake
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -1203,19 +1134,15 @@
 
 class ChangeAccountEmailRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         email: str = None,
     ):
-        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
-        # The email address to be bound to the member.
-        # 
-        # > The system automatically sends a verification email to the email address. After the verification is passed, the email address takes effect, and the system changes both the logon email address and secure email address of the member.
         self.email = email
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1239,15 +1166,14 @@
 
 
 class ChangeAccountEmailResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1311,15 +1237,14 @@
 
 
 class CheckAccountDeleteRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
     ):
-        # The Alibaba Cloud account ID of the member that you want to delete.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1339,15 +1264,14 @@
 
 
 class CheckAccountDeleteResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1414,33 +1338,17 @@
     def __init__(
         self,
         description: str = None,
         effect_scope: str = None,
         policy_document: str = None,
         policy_name: str = None,
     ):
-        # The description of the access control policy.
-        # 
-        # The description must be 1 to 1,024 characters in length. The description can contain letters, digits, underscores (\_), and hyphens (-) and must start with a letter.
         self.description = description
-        # The effective scope of the access control policy.
-        # 
-        # The value RAM indicates that the access control policy takes effect only for RAM users and RAM roles.
         self.effect_scope = effect_scope
-        # The document of the access control policy.
-        # 
-        # The document can be a maximum of 4,096 characters in length.
-        # 
-        # For more information about the languages of access control policies, see [Languages of access control policies](~~179096~~).
-        # 
-        # For more information about the examples of access control policies, see [Examples of custom access control policies](~~181474~~).
         self.policy_document = policy_document
-        # The name of the access control policy.
-        # 
-        # The name must be 1 to 128 characters in length. The name can contain letters, digits, and hyphens (-) and must start with a letter.
         self.policy_name = policy_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1479,34 +1387,21 @@
         description: str = None,
         effect_scope: str = None,
         policy_id: str = None,
         policy_name: str = None,
         policy_type: str = None,
         update_date: str = None,
     ):
-        # The number of times that the access control policy is referenced.
         self.attachment_count = attachment_count
-        # The time when the access control policy was created.
         self.create_date = create_date
-        # The description of the access control policy.
         self.description = description
-        # The effective scope of the access control policy.
-        # 
-        # The value RAM indicates that the access control policy takes effect only for RAM users and RAM roles.
         self.effect_scope = effect_scope
-        # The ID of the access control policy.
         self.policy_id = policy_id
-        # The name of the access control policy.
         self.policy_name = policy_name
-        # The type of the access control policy. Valid values:
-        # 
-        # *   System: system access control policy
-        # *   Custom: custom access control policy
         self.policy_type = policy_type
-        # The time when the access control policy was updated.
         self.update_date = update_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1555,17 +1450,15 @@
 
 class CreateControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         control_policy: CreateControlPolicyResponseBodyControlPolicy = None,
         request_id: str = None,
     ):
-        # The details of the access control policy.
         self.control_policy = control_policy
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.control_policy:
             self.control_policy.validate()
 
     def to_map(self):
@@ -1636,19 +1529,15 @@
 
 class CreateFolderRequest(TeaModel):
     def __init__(
         self,
         folder_name: str = None,
         parent_folder_id: str = None,
     ):
-        # The name of the folder.
-        # 
-        # The name must be 1 to 24 characters in length and can contain letters, digits, underscores (\_), periods (.),and hyphens (-).
         self.folder_name = folder_name
-        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1675,21 +1564,17 @@
     def __init__(
         self,
         create_time: str = None,
         folder_id: str = None,
         folder_name: str = None,
         parent_folder_id: str = None,
     ):
-        # The time when the folder was created.
         self.create_time = create_time
-        # The ID of the folder.
         self.folder_id = folder_id
-        # The name of the folder.
         self.folder_name = folder_name
-        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1722,17 +1607,15 @@
 
 class CreateFolderResponseBody(TeaModel):
     def __init__(
         self,
         folder: CreateFolderResponseBodyFolder = None,
         request_id: str = None,
     ):
-        # The information about the folder.
         self.folder = folder
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.folder:
             self.folder.validate()
 
     def to_map(self):
@@ -1803,17 +1686,15 @@
 
 class CreateResourceAccountRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # The key of the tag.
         self.key = key
-        # The value of the tag.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1842,44 +1723,19 @@
         account_name_prefix: str = None,
         display_name: str = None,
         parent_folder_id: str = None,
         payer_account_id: str = None,
         resell_account_type: str = None,
         tag: List[CreateResourceAccountRequestTag] = None,
     ):
-        # The prefix for the Alibaba Cloud account name of the member. If you leave this parameter empty, the system randomly generates a prefix.
-        # 
-        # The prefix must be 2 to 37 characters in length.
-        # 
-        # The prefix can contain letters, digits, and special characters but cannot contain consecutive special characters. The prefix must start with a letter or digit and end with a letter or digit. Valid special characters include underscores (`_`), periods (.), and hyphens (`-`).
-        # 
-        # The complete Alibaba Cloud account name of a member in a resource directory is in the @.aliyunid.com format, such as `alice@rd-3G****.aliyunid.com`.
-        # 
-        # Each name must be unique in the resource directory.
         self.account_name_prefix = account_name_prefix
-        # The display name of the member.
-        # 
-        # The name must be 2 to 50 characters in length.
-        # 
-        # The name can contain letters, digits, underscores (\_), periods (.), hyphens (-), and spaces.
-        # 
-        # The name must be unique in the resource directory.
         self.display_name = display_name
-        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
-        # The ID of the billing account. If you leave this parameter empty, the member is used as its own billing account.
         self.payer_account_id = payer_account_id
-        # The identity type of the member. Valid values:
-        # 
-        # *   resell: The member is an account for a reseller. This is the default value. A relationship is automatically established between the member and the reseller. The management account of the resource directory must be used as the billing account of the member.
-        # *   non_resell: The member is not an account for a reseller. The member is an account that is not associated with a reseller. You can directly use the account to purchase Alibaba Cloud resources. The member is used as its own billing account.
-        # 
-        # > This parameter is available only for resellers at the international site (alibabacloud.com).
         self.resell_account_type = resell_account_type
-        # The tag of the member.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -1936,36 +1792,23 @@
         join_method: str = None,
         join_time: str = None,
         modify_time: str = None,
         resource_directory_id: str = None,
         status: str = None,
         type: str = None,
     ):
-        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
-        # The Alibaba Cloud account name of the member.
         self.account_name = account_name
-        # The display name of the member.
         self.display_name = display_name
-        # The ID of the folder.
         self.folder_id = folder_id
-        # The way in which the member joins the resource directory. Valid values:
-        # 
-        # *   invited: The member is invited to join the resource directory.
-        # *   created: The member is directly created in the resource directory.
         self.join_method = join_method
-        # The time when the member joined the resource directory. The time is displayed in UTC.
         self.join_time = join_time
-        # The time when the member was modified. The time is displayed in UTC.
         self.modify_time = modify_time
-        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
-        # The status of the member. The value CreateSuccess indicates that the member is created.
         self.status = status
-        # The type of the member. The value ResourceAccount indicates that the member is a resource account.
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2022,17 +1865,15 @@
 
 class CreateResourceAccountResponseBody(TeaModel):
     def __init__(
         self,
         account: CreateResourceAccountResponseBodyAccount = None,
         request_id: str = None,
     ):
-        # The information of the member.
         self.account = account
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
@@ -2102,15 +1943,14 @@
 
 
 class DeclineHandshakeRequest(TeaModel):
     def __init__(
         self,
         handshake_id: str = None,
     ):
-        # The ID of the invitation.
         self.handshake_id = handshake_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2140,44 +1980,24 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
-        # The time when the invitation was created.
         self.create_time = create_time
-        # The time when the invitation expires.
         self.expire_time = expire_time
-        # The ID of the invitation.
         self.handshake_id = handshake_id
-        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
-        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
-        # The time when the invitation was modified.
         self.modify_time = modify_time
-        # The description of the invitation.
         self.note = note
-        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
-        # The status of the invitation. Valid values:
-        # 
-        # *   Pending: The invitation is waiting for confirmation.
-        # *   Accepted: The invitation is accepted.
-        # *   Cancelled: The invitation is canceled.
-        # *   Declined: The invitation is rejected.
-        # *   Expired: The invitation expires.
         self.status = status
-        # The ID or logon email address of the invited account.
         self.target_entity = target_entity
-        # The type of the invited account. Valid values:
-        # 
-        # *   Account: indicates the ID of the account.
-        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2238,17 +2058,15 @@
 
 class DeclineHandshakeResponseBody(TeaModel):
     def __init__(
         self,
         handshake: DeclineHandshakeResponseBodyHandshake = None,
         request_id: str = None,
     ):
-        # The information of the invitation.
         self.handshake = handshake
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -2319,19 +2137,15 @@
 
 class DeleteAccountRequest(TeaModel):
     def __init__(
         self,
         abandonable_check_id: List[str] = None,
         account_id: str = None,
     ):
-        # The IDs of the check items that you can choose to ignore for the member deletion.
-        # 
-        # You can obtain the IDs from the response of the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation.
         self.abandonable_check_id = abandonable_check_id
-        # The Alibaba Cloud account ID of the member that you want to delete.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2356,19 +2170,15 @@
 
 class DeleteAccountShrinkRequest(TeaModel):
     def __init__(
         self,
         abandonable_check_id_shrink: str = None,
         account_id: str = None,
     ):
-        # The IDs of the check items that you can choose to ignore for the member deletion.
-        # 
-        # You can obtain the IDs from the response of the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation.
         self.abandonable_check_id_shrink = abandonable_check_id_shrink
-        # The Alibaba Cloud account ID of the member that you want to delete.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2393,20 +2203,15 @@
 
 class DeleteAccountResponseBody(TeaModel):
     def __init__(
         self,
         deletion_type: str = None,
         request_id: str = None,
     ):
-        # The type of the deletion. Valid values:
-        # 
-        # *   0: direct deletion. If the member does not have pay-as-you-go resources that are purchased within the previous 30 days, the system directly deletes the member.
-        # *   1: deletion with a silence period. If the member has pay-as-you-go resources that are purchased within the previous 30 days, the member enters a silence period of 45 days. The system starts to delete the member until the silence period ends. For more information about the silence period, see [What is the silence period for member deletion?](~~446079~~)
         self.deletion_type = deletion_type
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2474,15 +2279,14 @@
 
 
 class DeleteControlPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_id: str = None,
     ):
-        # The ID of the access control policy.
         self.policy_id = policy_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2502,15 +2306,14 @@
 
 
 class DeleteControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2574,15 +2377,14 @@
 
 
 class DeleteFolderRequest(TeaModel):
     def __init__(
         self,
         folder_id: str = None,
     ):
-        # The ID of the folder.
         self.folder_id = folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2602,15 +2404,14 @@
 
 
 class DeleteFolderResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2785,17 +2586,15 @@
 
 class DeregisterDelegatedAdministratorRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         service_principal: str = None,
     ):
-        # The Alibaba Cloud account ID of the member in the resource directory.
         self.account_id = account_id
-        # The identifier of the trusted service.
         self.service_principal = service_principal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2819,15 +2618,14 @@
 
 
 class DeregisterDelegatedAdministratorResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2891,15 +2689,14 @@
 
 
 class DestroyResourceDirectoryResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2964,21 +2761,15 @@
 
 class DetachControlPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_id: str = None,
         target_id: str = None,
     ):
-        # The ID of the access control policy.
         self.policy_id = policy_id
-        # The ID of the object from which you want to detach the access control policy. Access control policies can be attached to the following objects:
-        # 
-        # *   Root folder
-        # *   Subfolders of the Root folder
-        # *   Members
         self.target_id = target_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3002,15 +2793,14 @@
 
 
 class DetachControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3075,22 +2865,15 @@
 
 class DisableControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         enablement_status: str = None,
         request_id: str = None,
     ):
-        # The status of the Control Policy feature. Valid values:
-        # 
-        # *   Enabled: The feature is enabled.
-        # *   PendingEnable: The feature is being enabled.
-        # *   Disabled: The feature is disabled.
-        # *   PendingDisable: The feature is being disabled.
         self.enablement_status = enablement_status
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3316,22 +3099,15 @@
 
 class EnableControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         enablement_status: str = None,
         request_id: str = None,
     ):
-        # The status of the Control Policy feature. Valid values:
-        # 
-        # *   Enabled: The feature is enabled.
-        # *   PendingEnable: The feature is being enabled.
-        # *   Disabled: The feature is disabled.
-        # *   PendingDisable: The feature is being disabled.
         self.enablement_status = enablement_status
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3402,34 +3178,17 @@
     def __init__(
         self,
         enable_mode: str = None,
         maname: str = None,
         masecure_mobile_phone: str = None,
         verification_code: str = None,
     ):
-        # The mode in which you enable a resource directory. Valid values:
-        # 
-        # *   CurrentAccount: The current account is used to enable a resource directory.
-        # *   NewManagementAccount: A newly created account is used to enable a resource directory. If you select this mode, you must configure the `MAName`, `MASecureMobilePhone`, and `VerificationCode` parameters.
         self.enable_mode = enable_mode
-        # The name of the newly created account.
-        # 
-        # Specify the name in the `<Prefix>@rdadmin.aliyunid.com` format. The prefix can contain letters, digits, and special characters but cannot contain consecutive special characters. The prefix must start and end with a letter or digit. Valid special characters include underscores (`_`), periods (.), and hyphens (-). The prefix must be 2 to 50 characters in length.
         self.maname = maname
-        # The mobile phone number that is bound to the newly created account.
-        # 
-        # If you leave this parameter empty, the mobile phone number that is bound to the current account is used. The mobile phone number you specify must be the same as the mobile phone number that you specify when you call the [SendVerificationCodeForEnableRD](~~SendVerificationCodeForEnableRD~~) operation to obtain a verification code.
-        # 
-        # Specify the mobile phone number in the `<Country code>-<Mobile phone number>` format.
-        # 
-        # > Mobile phone numbers in the `86-<Mobile phone number>` format in the Chinese mainland are not supported.
         self.masecure_mobile_phone = masecure_mobile_phone
-        # The verification code.
-        # 
-        # You can call the [SendVerificationCodeForEnableRD](~~SendVerificationCodeForEnableRD~~) operation to obtain the verification code.
         self.verification_code = verification_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3465,23 +3224,18 @@
         self,
         create_time: str = None,
         master_account_id: str = None,
         master_account_name: str = None,
         resource_directory_id: str = None,
         root_folder_id: str = None,
     ):
-        # The time when the resource directory was enabled.
         self.create_time = create_time
-        # The ID of the management account.
         self.master_account_id = master_account_id
-        # The name of the management account.
         self.master_account_name = master_account_name
-        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
-        # The ID of the Root folder.
         self.root_folder_id = root_folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3518,17 +3272,15 @@
 
 class EnableResourceDirectoryResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_directory: EnableResourceDirectoryResponseBodyResourceDirectory = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
-        # The information about the resource directory.
         self.resource_directory = resource_directory
 
     def validate(self):
         if self.resource_directory:
             self.resource_directory.validate()
 
     def to_map(self):
@@ -3599,20 +3351,15 @@
 
 class GetAccountRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         include_tags: bool = None,
     ):
-        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
-        # Specifies whether to return the information of tags. Valid values:
-        # 
-        # *   false (default value)
-        # *   true
         self.include_tags = include_tags
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3637,17 +3384,15 @@
 
 class GetAccountResponseBodyAccountTags(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # A tag key.
         self.key = key
-        # A tag value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3685,62 +3430,28 @@
         modify_time: str = None,
         resource_directory_id: str = None,
         resource_directory_path: str = None,
         status: str = None,
         tags: List[GetAccountResponseBodyAccountTags] = None,
         type: str = None,
     ):
-        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
-        # The Alibaba Cloud account name of the member.
         self.account_name = account_name
-        # The display name of the member.
         self.display_name = display_name
-        # The status of the modification for the email address bound to the member. Valid values:
-        # 
-        # *   If the value of this parameter is empty, no modification is performed for the email address.
-        # *   WAIT_MODIFY: The modification is being performed.
-        # *   CANCELLED: The modification is canceled.
-        # *   EXPIRED: The modification expires.
         self.email_status = email_status
-        # The ID of the folder.
         self.folder_id = folder_id
-        # The real-name verification information.
         self.identity_information = identity_information
-        # The way in which the member joins the resource directory. Valid values:
-        # 
-        # *   invited: The member is invited to join the resource directory.
-        # *   created: The member is directly created in the resource directory.
         self.join_method = join_method
-        # The time when the member joined the resource directory.
         self.join_time = join_time
-        # The location of the member in the resource directory.
         self.location = location
-        # The time when the member was modified.
         self.modify_time = modify_time
-        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
-        # The path of the member in the resource directory.
         self.resource_directory_path = resource_directory_path
-        # The status of the member. Valid values:
-        # 
-        # *   CreateSuccess: The member is created.
-        # *   PromoteVerifying: The upgrade of the member is being confirmed.
-        # *   PromoteFailed: The upgrade of the member fails.
-        # *   PromoteExpired: The upgrade of the member expires.
-        # *   PromoteCancelled: The upgrade of the member is canceled.
-        # *   PromoteSuccess: The member is upgraded.
-        # *   InviteSuccess: The member accepts the invitation.
         self.status = status
-        # The tags of the member.
         self.tags = tags
-        # The type of the member. Valid values:
-        # 
-        # *   CloudAccount: cloud account
-        # *   ResourceAccount: resource account
         self.type = type
 
     def validate(self):
         if self.tags:
             for k in self.tags:
                 if k:
                     k.validate()
@@ -3825,17 +3536,15 @@
 
 class GetAccountResponseBody(TeaModel):
     def __init__(
         self,
         account: GetAccountResponseBodyAccount = None,
         request_id: str = None,
     ):
-        # The information of the member.
         self.account = account
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
@@ -3905,15 +3614,14 @@
 
 
 class GetAccountDeletionCheckResultRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
     ):
-        # The Alibaba Cloud account ID of the member that you want to delete.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3935,19 +3643,16 @@
 class GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoAbandonableChecks(TeaModel):
     def __init__(
         self,
         check_id: str = None,
         check_name: str = None,
         description: str = None,
     ):
-        # The ID of the check item.
         self.check_id = check_id
-        # The name of the cloud service to which the check item belongs.
         self.check_name = check_name
-        # The description of the check item.
         self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3977,19 +3682,16 @@
 class GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoNotAllowReason(TeaModel):
     def __init__(
         self,
         check_id: str = None,
         check_name: str = None,
         description: str = None,
     ):
-        # The ID of the check item.
         self.check_id = check_id
-        # The name of the cloud service to which the check item belongs.
         self.check_name = check_name
-        # The description of the check item.
         self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4020,31 +3722,17 @@
     def __init__(
         self,
         abandonable_checks: List[GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoAbandonableChecks] = None,
         allow_delete: str = None,
         not_allow_reason: List[GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoNotAllowReason] = None,
         status: str = None,
     ):
-        # The check items that you can choose to ignore for the member deletion.
-        # 
-        # > This parameter may be returned if the value of AllowDelete is true.
         self.abandonable_checks = abandonable_checks
-        # Indicates whether the member can be deleted. Valid values:
-        # 
-        # *   true: The member can be deleted.
-        # *   false: The member cannot be deleted.
         self.allow_delete = allow_delete
-        # The reasons why the member cannot be deleted.
-        # 
-        # > This parameter is returned only if the value of AllowDelete is false.
         self.not_allow_reason = not_allow_reason
-        # The status of the check. Valid values:
-        # 
-        # *   PreCheckComplete: The check is complete.
-        # *   PreChecking: The check is in progress.
         self.status = status
 
     def validate(self):
         if self.abandonable_checks:
             for k in self.abandonable_checks:
                 if k:
                     k.validate()
@@ -4094,17 +3782,15 @@
 
 class GetAccountDeletionCheckResultResponseBody(TeaModel):
     def __init__(
         self,
         account_deletion_check_result_info: GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfo = None,
         request_id: str = None,
     ):
-        # The result of the deletion check for the member.
         self.account_deletion_check_result_info = account_deletion_check_result_info
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account_deletion_check_result_info:
             self.account_deletion_check_result_info.validate()
 
     def to_map(self):
@@ -4174,15 +3860,14 @@
 
 
 class GetAccountDeletionStatusRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
     ):
-        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4203,17 +3888,15 @@
 
 class GetAccountDeletionStatusResponseBodyRdAccountDeletionStatusFailReasonList(TeaModel):
     def __init__(
         self,
         description: str = None,
         name: str = None,
     ):
-        # The description of the check item.
         self.description = description
-        # The name of the cloud service to which the check item belongs.
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4242,34 +3925,19 @@
         account_id: str = None,
         create_time: str = None,
         deletion_time: str = None,
         deletion_type: str = None,
         fail_reason_list: List[GetAccountDeletionStatusResponseBodyRdAccountDeletionStatusFailReasonList] = None,
         status: str = None,
     ):
-        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
-        # The start time of the deletion.
         self.create_time = create_time
-        # The end time of the deletion.
         self.deletion_time = deletion_time
-        # The type of the deletion. Valid values:
-        # 
-        # *   0: direct deletion. If the member does not have pay-as-you-go resources that are purchased within the previous 30 days, the system directly deletes the member.
-        # *   1: deletion with a silence period. If the member has pay-as-you-go resources that are purchased within the previous 30 days, the member enters a silence period of 45 days. The system starts to delete the member until the silence period ends. For more information about the silence period, see [What is the silence period for member deletion?](~~446079~~)
         self.deletion_type = deletion_type
-        # The reasons why the member fails to be deleted.
         self.fail_reason_list = fail_reason_list
-        # The status. Valid values:
-        # 
-        # *   Success: The member is deleted.
-        # *   Checking: A deletion check is being performed for the member.
-        # *   Deleting: The member is being deleted.
-        # *   CheckFailed: The deletion check for the member fails.
-        # *   DeleteFailed: The member fails to be deleted.
         self.status = status
 
     def validate(self):
         if self.fail_reason_list:
             for k in self.fail_reason_list:
                 if k:
                     k.validate()
@@ -4318,17 +3986,15 @@
 
 class GetAccountDeletionStatusResponseBody(TeaModel):
     def __init__(
         self,
         rd_account_deletion_status: GetAccountDeletionStatusResponseBodyRdAccountDeletionStatus = None,
         request_id: str = None,
     ):
-        # The deletion status of the member.
         self.rd_account_deletion_status = rd_account_deletion_status
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.rd_account_deletion_status:
             self.rd_account_deletion_status.validate()
 
     def to_map(self):
@@ -4399,23 +4065,15 @@
 
 class GetControlPolicyRequest(TeaModel):
     def __init__(
         self,
         language: str = None,
         policy_id: str = None,
     ):
-        # The language in which you want to return the description of the access control policy. Valid values:
-        # 
-        # *   zh-CN (default value): Chinese
-        # *   en: English
-        # *   ja: Japanese
-        # 
-        # > This parameter is valid only for system access control policies.
         self.language = language
-        # The ID of the access control policy.
         self.policy_id = policy_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4447,37 +4105,22 @@
         effect_scope: str = None,
         policy_document: str = None,
         policy_id: str = None,
         policy_name: str = None,
         policy_type: str = None,
         update_date: str = None,
     ):
-        # The number of times that the access control policy is referenced.
         self.attachment_count = attachment_count
-        # The time when the access control policy was created.
         self.create_date = create_date
-        # The description of the access control policy.
         self.description = description
-        # The effective scope of the access control policy. Valid values:
-        # 
-        # *   All: The access control policy is in effect for Alibaba Cloud accounts, RAM users, and RAM roles.
-        # *   RAM: The access control policy is in effect only for RAM users and RAM roles.
         self.effect_scope = effect_scope
-        # The document of the access control policy.
         self.policy_document = policy_document
-        # The ID of the access control policy.
         self.policy_id = policy_id
-        # The name of the access control policy.
         self.policy_name = policy_name
-        # The type of the access control policy. Valid values:
-        # 
-        # *   System: system access control policy
-        # *   Custom: custom access control policy
         self.policy_type = policy_type
-        # The time when the access control policy was updated.
         self.update_date = update_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4530,17 +4173,15 @@
 
 class GetControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         control_policy: GetControlPolicyResponseBodyControlPolicy = None,
         request_id: str = None,
     ):
-        # The details of the access control policy.
         self.control_policy = control_policy
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.control_policy:
             self.control_policy.validate()
 
     def to_map(self):
@@ -4611,22 +4252,15 @@
 
 class GetControlPolicyEnablementStatusResponseBody(TeaModel):
     def __init__(
         self,
         enablement_status: str = None,
         request_id: str = None,
     ):
-        # The status of the Control Policy feature. Valid values:
-        # 
-        # *   Enabled: The feature is enabled.
-        # *   PendingEnable: The feature is being enabled.
-        # *   Disabled: The feature is disabled.
-        # *   PendingDisable: The feature is being disabled.
         self.enablement_status = enablement_status
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4694,15 +4328,14 @@
 
 
 class GetFolderRequest(TeaModel):
     def __init__(
         self,
         folder_id: str = None,
     ):
-        # The ID of the folder.
         self.folder_id = folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4726,23 +4359,18 @@
         self,
         create_time: str = None,
         folder_id: str = None,
         folder_name: str = None,
         parent_folder_id: str = None,
         resource_directory_path: str = None,
     ):
-        # The time when the folder was created.
         self.create_time = create_time
-        # The ID of the folder.
         self.folder_id = folder_id
-        # The name of the folder.
         self.folder_name = folder_name
-        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
-        # The path of the folder in the resource directory.
         self.resource_directory_path = resource_directory_path
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4779,17 +4407,15 @@
 
 class GetFolderResponseBody(TeaModel):
     def __init__(
         self,
         folder: GetFolderResponseBodyFolder = None,
         request_id: str = None,
     ):
-        # The information about the folder.
         self.folder = folder
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.folder:
             self.folder.validate()
 
     def to_map(self):
@@ -4859,15 +4485,14 @@
 
 
 class GetHandshakeRequest(TeaModel):
     def __init__(
         self,
         handshake_id: str = None,
     ):
-        # The ID of the invitation.
         self.handshake_id = handshake_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4899,52 +4524,26 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
-        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time
-        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time
-        # The ID of the invitation.
         self.handshake_id = handshake_id
-        # The real-name verification information of the invitee.
-        # 
-        # > This parameter is available only when an invitee calls this operation.
         self.invited_account_real_name = invited_account_real_name
-        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
-        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
-        # The real-name verification information of the management account of the resource directory.
-        # 
-        # > This parameter is available only when an invitee calls this operation.
         self.master_account_real_name = master_account_real_name
-        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time
-        # The description of the invitation.
         self.note = note
-        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
-        # The status of the invitation. Valid values:
-        # 
-        # *   Pending: The invitation is waiting for confirmation.
-        # *   Accepted: The invitation is accepted.
-        # *   Cancelled: The invitation is canceled.
-        # *   Declined: The invitation is rejected.
-        # *   Expired: The invitation expires.
         self.status = status
-        # The ID or logon email address of the invited account.
         self.target_entity = target_entity
-        # The type of the invited account. Valid values:
-        # 
-        # *   Account: indicates the ID of the account.
-        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5013,17 +4612,15 @@
 
 class GetHandshakeResponseBody(TeaModel):
     def __init__(
         self,
         handshake: GetHandshakeResponseBodyHandshake = None,
         request_id: str = None,
     ):
-        # The information of the invitation.
         self.handshake = handshake
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -5581,37 +5178,21 @@
         identity_information: str = None,
         master_account_id: str = None,
         master_account_name: str = None,
         member_deletion_status: str = None,
         resource_directory_id: str = None,
         root_folder_id: str = None,
     ):
-        # The status of the Control Policy feature. Valid values:
-        # 
-        # *   Enabled: The feature is enabled.
-        # *   PendingEnable: The feature is being enabled.
-        # *   Disabled: The feature is disabled.
-        # *   PendingDisable: The feature is being disabled.
         self.control_policy_status = control_policy_status
-        # The time when the resource directory was enabled.
         self.create_time = create_time
-        # The real-name verification information.
         self.identity_information = identity_information
-        # The ID of the management account.
         self.master_account_id = master_account_id
-        # The name of the management account.
         self.master_account_name = master_account_name
-        # The status of the member deletion feature. Valid values:
-        # 
-        # *   Enabled: The feature is enabled. You can call the [DeleteAccount](~~DeleteAccount~~) operation to delete members of the resource account type.
-        # *   Disabled: The feature is disabled. You cannot delete members of the resource account type.
         self.member_deletion_status = member_deletion_status
-        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
-        # The ID of the Root folder.
         self.root_folder_id = root_folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5660,17 +5241,15 @@
 
 class GetResourceDirectoryResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_directory: GetResourceDirectoryResponseBodyResourceDirectory = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
-        # The information of the resource directory.
         self.resource_directory = resource_directory
 
     def validate(self):
         if self.resource_directory:
             self.resource_directory.validate()
 
     def to_map(self):
@@ -5741,17 +5320,15 @@
 
 class InviteAccountToResourceDirectoryRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # The tag key.
         self.key = key
-        # The tag value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5774,30 +5351,23 @@
         return self
 
 
 class InviteAccountToResourceDirectoryRequest(TeaModel):
     def __init__(
         self,
         note: str = None,
+        parent_folder_id: str = None,
         tag: List[InviteAccountToResourceDirectoryRequestTag] = None,
         target_entity: str = None,
         target_type: str = None,
     ):
-        # The description of the invitation.
-        # 
-        # The description can be up to 1,024 characters in length.
         self.note = note
-        # The tags.
+        self.parent_folder_id = parent_folder_id
         self.tag = tag
-        # The ID or logon email address of the account that you want to invite.
         self.target_entity = target_entity
-        # The type of the account. Valid values:
-        # 
-        # *   Account: indicates the ID of the account.
-        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -5806,28 +5376,32 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.note is not None:
             result['Note'] = self.note
+        if self.parent_folder_id is not None:
+            result['ParentFolderId'] = self.parent_folder_id
         result['Tag'] = []
         if self.tag is not None:
             for k in self.tag:
                 result['Tag'].append(k.to_map() if k else None)
         if self.target_entity is not None:
             result['TargetEntity'] = self.target_entity
         if self.target_type is not None:
             result['TargetType'] = self.target_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Note') is not None:
             self.note = m.get('Note')
+        if m.get('ParentFolderId') is not None:
+            self.parent_folder_id = m.get('ParentFolderId')
         self.tag = []
         if m.get('Tag') is not None:
             for k in m.get('Tag'):
                 temp_model = InviteAccountToResourceDirectoryRequestTag()
                 self.tag.append(temp_model.from_map(k))
         if m.get('TargetEntity') is not None:
             self.target_entity = m.get('TargetEntity')
@@ -5847,44 +5421,24 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
-        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time
-        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time
-        # The ID of the invitation.
         self.handshake_id = handshake_id
-        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
-        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
-        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time
-        # The description of the invitation.
         self.note = note
-        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
-        # The status of the invitation. Valid values:
-        # 
-        # *   Pending: The invitation is waiting for confirmation.
-        # *   Accepted: The invitation is accepted.
-        # *   Cancelled: The invitation is canceled.
-        # *   Declined: The invitation is rejected.
-        # *   Expired: The invitation expires.
         self.status = status
-        # The ID or logon email address of the invited account.
         self.target_entity = target_entity
-        # The type of the invited account. Valid values:
-        # 
-        # *   Account: indicates the ID of the account.
-        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5945,17 +5499,15 @@
 
 class InviteAccountToResourceDirectoryResponseBody(TeaModel):
     def __init__(
         self,
         handshake: InviteAccountToResourceDirectoryResponseBodyHandshake = None,
         request_id: str = None,
     ):
-        # The information of the invitation.
         self.handshake = handshake
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -9727,28 +9279,16 @@
 class ListTrustedServiceStatusRequest(TeaModel):
     def __init__(
         self,
         admin_account_id: str = None,
         page_number: int = None,
         page_size: int = None,
     ):
-        # The ID of the management account or delegated administrator account.
-        # 
-        # *   If you set this parameter to the ID of a management account, the trusted services that are enabled within the management account are queried. The default value of this parameter is the ID of an management account.
-        # *   If you set this parameter to the ID of a delegated administrator account, the trusted services that are enabled within the delegated administrator account are queried.
-        # 
-        # For more information about trusted services and delegated administrator accounts, see [Overview of trusted services](~~208133~~) and [Delegated administrator accounts](~~208117~~).
         self.admin_account_id = admin_account_id
-        # The number of the page to return.
-        # 
-        # Pages start from page 1. Default value: 1.
         self.page_number = page_number
-        # The number of entries to return on each page.
-        # 
-        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9777,17 +9317,15 @@
 
 class ListTrustedServiceStatusResponseBodyEnabledServicePrincipalsEnabledServicePrincipal(TeaModel):
     def __init__(
         self,
         enable_time: str = None,
         service_principal: str = None,
     ):
-        # The time when the trusted service was enabled.
         self.enable_time = enable_time
-        # The identifier of the trusted service.
         self.service_principal = service_principal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9850,23 +9388,18 @@
         self,
         enabled_service_principals: ListTrustedServiceStatusResponseBodyEnabledServicePrincipals = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The information about the trusted services that are enabled.
         self.enabled_service_principals = enabled_service_principals
-        # The page number of the returned page.
         self.page_number = page_number
-        # The number of entries returned per page.
         self.page_size = page_size
-        # The ID of the request.
         self.request_id = request_id
-        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.enabled_service_principals:
             self.enabled_service_principals.validate()
 
     def to_map(self):
@@ -10056,19 +9589,15 @@
 
 class RegisterDelegatedAdministratorRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         service_principal: str = None,
     ):
-        # The Alibaba Cloud account ID of the member in the resource directory.
         self.account_id = account_id
-        # The identifier of the trusted service.
-        # 
-        # For more information, see the `Trusted service identifier` column in [Supported trusted services](~~208133~~).
         self.service_principal = service_principal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10092,15 +9621,14 @@
 
 
 class RegisterDelegatedAdministratorResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11222,26 +10750,16 @@
 class UpdateAccountRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         new_account_type: str = None,
         new_display_name: str = None,
     ):
-        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
-        # The new type of the member. Valid values:
-        # 
-        # *   ResourceAccount: resource account
-        # *   CloudAccount: cloud account
-        # 
-        # > You can specify either `NewDisplayName` or `NewAccountType`.
         self.new_account_type = new_account_type
-        # The new display name of the member.
-        # 
-        # > You can specify either `NewDisplayName` or `NewAccountType`.
         self.new_display_name = new_display_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11278,44 +10796,23 @@
         join_method: str = None,
         join_time: str = None,
         modify_time: str = None,
         resource_directory_id: str = None,
         status: str = None,
         type: str = None,
     ):
-        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
-        # The Alibaba Cloud account name of the member.
         self.account_name = account_name
-        # The display name of the member.
         self.display_name = display_name
-        # The ID of the folder.
         self.folder_id = folder_id
-        # The way in which the member joins the resource directory. Valid values:
-        # 
-        # *   invited: The member is invited to join the resource directory.
-        # *   created: The member is directly created in the resource directory.
         self.join_method = join_method
-        # The time when the member joined the resource directory. The time is displayed in UTC.
         self.join_time = join_time
-        # The time when the member was modified. The time is displayed in UTC.
         self.modify_time = modify_time
-        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
-        # The status of the member. Valid values:
-        # 
-        # *   CreateSuccess: The member is created.
-        # *   InviteSuccess: The member accepts the invitation.
-        # *   Removed: The member is removed.
-        # *   SwitchSuccess: The type of the member is switched.
         self.status = status
-        # The type of the member. Valid values:
-        # 
-        # *   CloudAccount: cloud account
-        # *   ResourceAccount: resource account
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11372,17 +10869,15 @@
 
 class UpdateAccountResponseBody(TeaModel):
     def __init__(
         self,
         account: UpdateAccountResponseBodyAccount = None,
         request_id: str = None,
     ):
-        # The information of the member.
         self.account = account
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO` & `alibabacloud_resourcedirectorymaster20220419-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-resourcedirectorymaster20220419
-Version: 1.0.1
+Name: alibabacloud_resourcedirectorymaster20220419
+Version: 1.0.2
 Summary: Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt` & `alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.1/setup.py` & `alibabacloud_resourcedirectorymaster20220419-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcedirectorymaster20220419.
 
-Created on 12/04/2023
+Created on 04/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcedirectorymaster20220419"
 NAME = "alibabacloud_resourcedirectorymaster20220419" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python"
```

