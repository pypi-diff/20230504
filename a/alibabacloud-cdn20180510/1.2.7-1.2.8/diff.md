# Comparing `tmp/alibabacloud_cdn20180510-1.2.7.tar.gz` & `tmp/alibabacloud_cdn20180510-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cdn20180510-1.2.7.tar", last modified: Tue Apr 25 07:17:23 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cdn20180510-1.2.8.tar", last modified: Thu May  4 07:55:48 2023, max compression
```

## Comparing `alibabacloud_cdn20180510-1.2.7.tar` & `alibabacloud_cdn20180510-1.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/
--rw-r--r--   0 root         (0) root         (0)     1791 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2342 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510/__init__.py
--rw-r--r--   0 root         (0) root         (0)   803713 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510/client.py
--rw-r--r--   0 root         (0) root         (0)  1064220 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2342 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2624 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:55:48.000000 alibabacloud_cdn20180510-1.2.8/
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-05-04 07:55:47.000000 alibabacloud_cdn20180510-1.2.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-04 07:55:47.000000 alibabacloud_cdn20180510-1.2.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-04 07:55:47.000000 alibabacloud_cdn20180510-1.2.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-05-04 07:55:48.000000 alibabacloud_cdn20180510-1.2.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-05-04 07:55:47.000000 alibabacloud_cdn20180510-1.2.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-05-04 07:55:47.000000 alibabacloud_cdn20180510-1.2.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:55:48.000000 alibabacloud_cdn20180510-1.2.8/alibabacloud_cdn20180510/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-04 07:55:47.000000 alibabacloud_cdn20180510-1.2.8/alibabacloud_cdn20180510/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   762533 2023-05-04 07:55:47.000000 alibabacloud_cdn20180510-1.2.8/alibabacloud_cdn20180510/client.py
+-rw-r--r--   0 root         (0) root         (0)  1054638 2023-05-04 07:55:47.000000 alibabacloud_cdn20180510-1.2.8/alibabacloud_cdn20180510/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:55:48.000000 alibabacloud_cdn20180510-1.2.8/alibabacloud_cdn20180510.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-05-04 07:55:48.000000 alibabacloud_cdn20180510-1.2.8/alibabacloud_cdn20180510.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-04 07:55:48.000000 alibabacloud_cdn20180510-1.2.8/alibabacloud_cdn20180510.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 07:55:48.000000 alibabacloud_cdn20180510-1.2.8/alibabacloud_cdn20180510.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-04 07:55:48.000000 alibabacloud_cdn20180510-1.2.8/alibabacloud_cdn20180510.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-04 07:55:48.000000 alibabacloud_cdn20180510-1.2.8/alibabacloud_cdn20180510.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-04 07:55:48.000000 alibabacloud_cdn20180510-1.2.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-05-04 07:55:47.000000 alibabacloud_cdn20180510-1.2.8/setup.py
```

### Comparing `alibabacloud_cdn20180510-1.2.7/ChangeLog.md` & `alibabacloud_cdn20180510-1.2.8/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-04-25 Version: 1.2.7
+- Add CheckCdnDomainExist.
+
 2023-03-29 Version: 1.2.6
 - Delete DescribeConfigOfVersion.
 
 2023-03-29 Version: 1.2.5
 - Delete SetConfigOfVersion.
 
 2023-02-25 Version: 1.2.4
```

### Comparing `alibabacloud_cdn20180510-1.2.7/LICENSE` & `alibabacloud_cdn20180510-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cdn20180510-1.2.7/PKG-INFO` & `alibabacloud_cdn20180510-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cdn20180510
-Version: 1.2.7
+Version: 1.2.8
 Summary: Alibaba Cloud Alibaba Cloud CDN (20180510) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cdn20180510-1.2.7/README-CN.md` & `alibabacloud_cdn20180510-1.2.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cdn20180510-1.2.7/README.md` & `alibabacloud_cdn20180510-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510/client.py` & `alibabacloud_cdn20180510-1.2.8/alibabacloud_cdn20180510/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,25 +55,14 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def add_cdn_domain_with_options(
         self,
         request: cdn_20180510_models.AddCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.AddCdnDomainResponse:
-        """
-        You must activate Alibaba Cloud CDN before you can add a domain name to it. For more information, see [Activate Alibaba Cloud CDN](~~27272~~).
-        *   If the acceleration region is Chinese Mainland Only or Global, you must apply for an ICP filing for the domain name.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
-        *   For more information, see [Add a domain name](~~122181~~).
-        *   You can call this operation up to 30 times per second per account.
-        
-        @param request: AddCdnDomainRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AddCdnDomainResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cdn_type):
             query['CdnType'] = request.cdn_type
         if not UtilClient.is_unset(request.check_url):
             query['CheckUrl'] = request.check_url
         if not UtilClient.is_unset(request.domain_name):
@@ -114,25 +103,14 @@
         )
 
     async def add_cdn_domain_with_options_async(
         self,
         request: cdn_20180510_models.AddCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.AddCdnDomainResponse:
-        """
-        You must activate Alibaba Cloud CDN before you can add a domain name to it. For more information, see [Activate Alibaba Cloud CDN](~~27272~~).
-        *   If the acceleration region is Chinese Mainland Only or Global, you must apply for an ICP filing for the domain name.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
-        *   For more information, see [Add a domain name](~~122181~~).
-        *   You can call this operation up to 30 times per second per account.
-        
-        @param request: AddCdnDomainRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AddCdnDomainResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cdn_type):
             query['CdnType'] = request.cdn_type
         if not UtilClient.is_unset(request.check_url):
             query['CheckUrl'] = request.check_url
         if not UtilClient.is_unset(request.domain_name):
@@ -172,41 +150,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def add_cdn_domain(
         self,
         request: cdn_20180510_models.AddCdnDomainRequest,
     ) -> cdn_20180510_models.AddCdnDomainResponse:
-        """
-        You must activate Alibaba Cloud CDN before you can add a domain name to it. For more information, see [Activate Alibaba Cloud CDN](~~27272~~).
-        *   If the acceleration region is Chinese Mainland Only or Global, you must apply for an ICP filing for the domain name.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
-        *   For more information, see [Add a domain name](~~122181~~).
-        *   You can call this operation up to 30 times per second per account.
-        
-        @param request: AddCdnDomainRequest
-        @return: AddCdnDomainResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.add_cdn_domain_with_options(request, runtime)
 
     async def add_cdn_domain_async(
         self,
         request: cdn_20180510_models.AddCdnDomainRequest,
     ) -> cdn_20180510_models.AddCdnDomainResponse:
-        """
-        You must activate Alibaba Cloud CDN before you can add a domain name to it. For more information, see [Activate Alibaba Cloud CDN](~~27272~~).
-        *   If the acceleration region is Chinese Mainland Only or Global, you must apply for an ICP filing for the domain name.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
-        *   For more information, see [Add a domain name](~~122181~~).
-        *   You can call this operation up to 30 times per second per account.
-        
-        @param request: AddCdnDomainRequest
-        @return: AddCdnDomainResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.add_cdn_domain_with_options_async(request, runtime)
 
     def add_fctrigger_with_options(
         self,
         request: cdn_20180510_models.AddFCTriggerRequest,
         runtime: util_models.RuntimeOptions,
@@ -306,19 +264,15 @@
 
     def batch_add_cdn_domain_with_options(
         self,
         request: cdn_20180510_models.BatchAddCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.BatchAddCdnDomainResponse:
         """
-        You must activate Alibaba Cloud CDN before you can add a domain name to it. For more information, see [Activate Alibaba Cloud CDN](~~27272~~).
-        *   If the acceleration region is Chinese Mainland Only or Global, you must apply for an ICP filing for the domain name.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
-        *   For more information, see [Add a domain name](~~122181~~).
-        *   You can call this operation up to 30 times per second per account.
+        The top-level domain.
         
         @param request: BatchAddCdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchAddCdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -363,19 +317,15 @@
 
     async def batch_add_cdn_domain_with_options_async(
         self,
         request: cdn_20180510_models.BatchAddCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.BatchAddCdnDomainResponse:
         """
-        You must activate Alibaba Cloud CDN before you can add a domain name to it. For more information, see [Activate Alibaba Cloud CDN](~~27272~~).
-        *   If the acceleration region is Chinese Mainland Only or Global, you must apply for an ICP filing for the domain name.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
-        *   For more information, see [Add a domain name](~~122181~~).
-        *   You can call this operation up to 30 times per second per account.
+        The top-level domain.
         
         @param request: BatchAddCdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchAddCdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -419,51 +369,43 @@
         )
 
     def batch_add_cdn_domain(
         self,
         request: cdn_20180510_models.BatchAddCdnDomainRequest,
     ) -> cdn_20180510_models.BatchAddCdnDomainResponse:
         """
-        You must activate Alibaba Cloud CDN before you can add a domain name to it. For more information, see [Activate Alibaba Cloud CDN](~~27272~~).
-        *   If the acceleration region is Chinese Mainland Only or Global, you must apply for an ICP filing for the domain name.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
-        *   For more information, see [Add a domain name](~~122181~~).
-        *   You can call this operation up to 30 times per second per account.
+        The top-level domain.
         
         @param request: BatchAddCdnDomainRequest
         @return: BatchAddCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_add_cdn_domain_with_options(request, runtime)
 
     async def batch_add_cdn_domain_async(
         self,
         request: cdn_20180510_models.BatchAddCdnDomainRequest,
     ) -> cdn_20180510_models.BatchAddCdnDomainResponse:
         """
-        You must activate Alibaba Cloud CDN before you can add a domain name to it. For more information, see [Activate Alibaba Cloud CDN](~~27272~~).
-        *   If the acceleration region is Chinese Mainland Only or Global, you must apply for an ICP filing for the domain name.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
-        *   For more information, see [Add a domain name](~~122181~~).
-        *   You can call this operation up to 30 times per second per account.
+        The top-level domain.
         
         @param request: BatchAddCdnDomainRequest
         @return: BatchAddCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.batch_add_cdn_domain_with_options_async(request, runtime)
 
     def batch_delete_cdn_domain_config_with_options(
         self,
         request: cdn_20180510_models.BatchDeleteCdnDomainConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.BatchDeleteCdnDomainConfigResponse:
         """
-        > - You can configure features for at most 50 domain names in each API call.
-        - The maximum number of times that each user can call this operation per second is 30.
+        You can specify up to 50 domain names in each request.
+        *   You can call this operation up to 30 times per second per account.
         
         @param request: BatchDeleteCdnDomainConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchDeleteCdnDomainConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -498,16 +440,16 @@
 
     async def batch_delete_cdn_domain_config_with_options_async(
         self,
         request: cdn_20180510_models.BatchDeleteCdnDomainConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.BatchDeleteCdnDomainConfigResponse:
         """
-        > - You can configure features for at most 50 domain names in each API call.
-        - The maximum number of times that each user can call this operation per second is 30.
+        You can specify up to 50 domain names in each request.
+        *   You can call this operation up to 30 times per second per account.
         
         @param request: BatchDeleteCdnDomainConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchDeleteCdnDomainConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -541,46 +483,98 @@
         )
 
     def batch_delete_cdn_domain_config(
         self,
         request: cdn_20180510_models.BatchDeleteCdnDomainConfigRequest,
     ) -> cdn_20180510_models.BatchDeleteCdnDomainConfigResponse:
         """
-        > - You can configure features for at most 50 domain names in each API call.
-        - The maximum number of times that each user can call this operation per second is 30.
+        You can specify up to 50 domain names in each request.
+        *   You can call this operation up to 30 times per second per account.
         
         @param request: BatchDeleteCdnDomainConfigRequest
         @return: BatchDeleteCdnDomainConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_delete_cdn_domain_config_with_options(request, runtime)
 
     async def batch_delete_cdn_domain_config_async(
         self,
         request: cdn_20180510_models.BatchDeleteCdnDomainConfigRequest,
     ) -> cdn_20180510_models.BatchDeleteCdnDomainConfigResponse:
         """
-        > - You can configure features for at most 50 domain names in each API call.
-        - The maximum number of times that each user can call this operation per second is 30.
+        You can specify up to 50 domain names in each request.
+        *   You can call this operation up to 30 times per second per account.
         
         @param request: BatchDeleteCdnDomainConfigRequest
         @return: BatchDeleteCdnDomainConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.batch_delete_cdn_domain_config_with_options_async(request, runtime)
 
     def batch_set_cdn_domain_config_with_options(
         self,
         request: cdn_20180510_models.BatchSetCdnDomainConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.BatchSetCdnDomainConfigResponse:
         """
-        >    You can call this operation up to 30 times per second per account.
-        *   You can specify multiple domain names and must separate them with commas (,). You can specify up to 50 domain names in each call.
-        *   If the BatchSetCdnDomainConfig operation is successful, a unique configuration ID (ConfigId) is generated. You can use configuration IDs to update or delete configurations. For more information, see [Usage notes on ConfigId](~~388994~~).
+        The features that you want to configure. Format:
+        *   **functionName**: the name of the feature. This parameter is required. Separate multiple values with commas (,). For more information, see [A list of features](~~388460~~).
+        *   **argName**: the feature parameter for **functionName**. This parameter is required. You can specify multiple feature parameters.
+        *   **argValue**: the parameter value that is specified for **functionName**. This parameter is required.
+        *   **parentid**: the rule condition ID. This parameter is optional. You can use the **condition** rule engine to create a rule condition. For information, see [BatchSetCdnDomainConfig and SetCdnDomainStagingConfig](~~388460~~). A rule condition can identify parameters that are included in requests and filter requests based on the identified parameters. After you create a rule condition, a [configid](~~388994~~) is generated. configid can be used as parentId that is referenced by other features. This way, you can combine rule conditions and features for flexible configurations.
+        If you set **parentId** to **-1**, the existing rule conditions in the configurations are deleted.
+        [{
+        "functionArgs": [{
+        "argName": "Parameter A",
+        "argValue": Value of parameter A"
+        },
+        {
+        "argName": "Parameter B",
+        "argValue": "Value of parameter B"
+        }],
+        "functionName": "Feature name"
+        "parentId": "Optional, which corresponds to configid of the referenced rule condition"
+        }]
+        The following code shows a sample configuration if **parentId** is not used.
+        In this example, the **origin_request_header** feature is used to add back-to-origin HTTP headers, and the rule condition whose configuration ID is **222728944812032** is referenced.
+        [{
+        "functionArgs": [{
+        "argName": "header_operation_type",
+        "argValue": "add"
+        }, {
+        "argName": "header_name",
+        "argValue": "Accept-Encoding"
+        }, {
+        "argName": "header_value",
+        "argValue": "gzip"
+        }, {
+        "argName": "duplicate",
+        "argValue": "off"
+        }],
+        "functionName": "origin_request_header"
+        }]
+        The following code shows a sample configuration if **parentId** is used.
+        In this example, the **origin_request_header** feature is used to add back-to-origin HTTP headers, and the rule condition whose configuration ID is **222728944812032** is referenced.
+        [{
+        "functionArgs": [{
+        "argName": "header_operation_type",
+        "argValue": "add"
+        }, {
+        "argName": "header_name",
+        "argValue": "Accept-Encoding"
+        }, {
+        "argName": "header_value",
+        "argValue": "gzip"
+        }, {
+        "argName": "duplicate",
+        "argValue": "off"
+        }],
+        "functionName": "origin_request_header",
+        "parentId": "222728944812032"
+        }]
         
         @param request: BatchSetCdnDomainConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchSetCdnDomainConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -615,17 +609,69 @@
 
     async def batch_set_cdn_domain_config_with_options_async(
         self,
         request: cdn_20180510_models.BatchSetCdnDomainConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.BatchSetCdnDomainConfigResponse:
         """
-        >    You can call this operation up to 30 times per second per account.
-        *   You can specify multiple domain names and must separate them with commas (,). You can specify up to 50 domain names in each call.
-        *   If the BatchSetCdnDomainConfig operation is successful, a unique configuration ID (ConfigId) is generated. You can use configuration IDs to update or delete configurations. For more information, see [Usage notes on ConfigId](~~388994~~).
+        The features that you want to configure. Format:
+        *   **functionName**: the name of the feature. This parameter is required. Separate multiple values with commas (,). For more information, see [A list of features](~~388460~~).
+        *   **argName**: the feature parameter for **functionName**. This parameter is required. You can specify multiple feature parameters.
+        *   **argValue**: the parameter value that is specified for **functionName**. This parameter is required.
+        *   **parentid**: the rule condition ID. This parameter is optional. You can use the **condition** rule engine to create a rule condition. For information, see [BatchSetCdnDomainConfig and SetCdnDomainStagingConfig](~~388460~~). A rule condition can identify parameters that are included in requests and filter requests based on the identified parameters. After you create a rule condition, a [configid](~~388994~~) is generated. configid can be used as parentId that is referenced by other features. This way, you can combine rule conditions and features for flexible configurations.
+        If you set **parentId** to **-1**, the existing rule conditions in the configurations are deleted.
+        [{
+        "functionArgs": [{
+        "argName": "Parameter A",
+        "argValue": Value of parameter A"
+        },
+        {
+        "argName": "Parameter B",
+        "argValue": "Value of parameter B"
+        }],
+        "functionName": "Feature name"
+        "parentId": "Optional, which corresponds to configid of the referenced rule condition"
+        }]
+        The following code shows a sample configuration if **parentId** is not used.
+        In this example, the **origin_request_header** feature is used to add back-to-origin HTTP headers, and the rule condition whose configuration ID is **222728944812032** is referenced.
+        [{
+        "functionArgs": [{
+        "argName": "header_operation_type",
+        "argValue": "add"
+        }, {
+        "argName": "header_name",
+        "argValue": "Accept-Encoding"
+        }, {
+        "argName": "header_value",
+        "argValue": "gzip"
+        }, {
+        "argName": "duplicate",
+        "argValue": "off"
+        }],
+        "functionName": "origin_request_header"
+        }]
+        The following code shows a sample configuration if **parentId** is used.
+        In this example, the **origin_request_header** feature is used to add back-to-origin HTTP headers, and the rule condition whose configuration ID is **222728944812032** is referenced.
+        [{
+        "functionArgs": [{
+        "argName": "header_operation_type",
+        "argValue": "add"
+        }, {
+        "argName": "header_name",
+        "argValue": "Accept-Encoding"
+        }, {
+        "argName": "header_value",
+        "argValue": "gzip"
+        }, {
+        "argName": "duplicate",
+        "argValue": "off"
+        }],
+        "functionName": "origin_request_header",
+        "parentId": "222728944812032"
+        }]
         
         @param request: BatchSetCdnDomainConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchSetCdnDomainConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -659,47 +705,150 @@
         )
 
     def batch_set_cdn_domain_config(
         self,
         request: cdn_20180510_models.BatchSetCdnDomainConfigRequest,
     ) -> cdn_20180510_models.BatchSetCdnDomainConfigResponse:
         """
-        >    You can call this operation up to 30 times per second per account.
-        *   You can specify multiple domain names and must separate them with commas (,). You can specify up to 50 domain names in each call.
-        *   If the BatchSetCdnDomainConfig operation is successful, a unique configuration ID (ConfigId) is generated. You can use configuration IDs to update or delete configurations. For more information, see [Usage notes on ConfigId](~~388994~~).
+        The features that you want to configure. Format:
+        *   **functionName**: the name of the feature. This parameter is required. Separate multiple values with commas (,). For more information, see [A list of features](~~388460~~).
+        *   **argName**: the feature parameter for **functionName**. This parameter is required. You can specify multiple feature parameters.
+        *   **argValue**: the parameter value that is specified for **functionName**. This parameter is required.
+        *   **parentid**: the rule condition ID. This parameter is optional. You can use the **condition** rule engine to create a rule condition. For information, see [BatchSetCdnDomainConfig and SetCdnDomainStagingConfig](~~388460~~). A rule condition can identify parameters that are included in requests and filter requests based on the identified parameters. After you create a rule condition, a [configid](~~388994~~) is generated. configid can be used as parentId that is referenced by other features. This way, you can combine rule conditions and features for flexible configurations.
+        If you set **parentId** to **-1**, the existing rule conditions in the configurations are deleted.
+        [{
+        "functionArgs": [{
+        "argName": "Parameter A",
+        "argValue": Value of parameter A"
+        },
+        {
+        "argName": "Parameter B",
+        "argValue": "Value of parameter B"
+        }],
+        "functionName": "Feature name"
+        "parentId": "Optional, which corresponds to configid of the referenced rule condition"
+        }]
+        The following code shows a sample configuration if **parentId** is not used.
+        In this example, the **origin_request_header** feature is used to add back-to-origin HTTP headers, and the rule condition whose configuration ID is **222728944812032** is referenced.
+        [{
+        "functionArgs": [{
+        "argName": "header_operation_type",
+        "argValue": "add"
+        }, {
+        "argName": "header_name",
+        "argValue": "Accept-Encoding"
+        }, {
+        "argName": "header_value",
+        "argValue": "gzip"
+        }, {
+        "argName": "duplicate",
+        "argValue": "off"
+        }],
+        "functionName": "origin_request_header"
+        }]
+        The following code shows a sample configuration if **parentId** is used.
+        In this example, the **origin_request_header** feature is used to add back-to-origin HTTP headers, and the rule condition whose configuration ID is **222728944812032** is referenced.
+        [{
+        "functionArgs": [{
+        "argName": "header_operation_type",
+        "argValue": "add"
+        }, {
+        "argName": "header_name",
+        "argValue": "Accept-Encoding"
+        }, {
+        "argName": "header_value",
+        "argValue": "gzip"
+        }, {
+        "argName": "duplicate",
+        "argValue": "off"
+        }],
+        "functionName": "origin_request_header",
+        "parentId": "222728944812032"
+        }]
         
         @param request: BatchSetCdnDomainConfigRequest
         @return: BatchSetCdnDomainConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_set_cdn_domain_config_with_options(request, runtime)
 
     async def batch_set_cdn_domain_config_async(
         self,
         request: cdn_20180510_models.BatchSetCdnDomainConfigRequest,
     ) -> cdn_20180510_models.BatchSetCdnDomainConfigResponse:
         """
-        >    You can call this operation up to 30 times per second per account.
-        *   You can specify multiple domain names and must separate them with commas (,). You can specify up to 50 domain names in each call.
-        *   If the BatchSetCdnDomainConfig operation is successful, a unique configuration ID (ConfigId) is generated. You can use configuration IDs to update or delete configurations. For more information, see [Usage notes on ConfigId](~~388994~~).
+        The features that you want to configure. Format:
+        *   **functionName**: the name of the feature. This parameter is required. Separate multiple values with commas (,). For more information, see [A list of features](~~388460~~).
+        *   **argName**: the feature parameter for **functionName**. This parameter is required. You can specify multiple feature parameters.
+        *   **argValue**: the parameter value that is specified for **functionName**. This parameter is required.
+        *   **parentid**: the rule condition ID. This parameter is optional. You can use the **condition** rule engine to create a rule condition. For information, see [BatchSetCdnDomainConfig and SetCdnDomainStagingConfig](~~388460~~). A rule condition can identify parameters that are included in requests and filter requests based on the identified parameters. After you create a rule condition, a [configid](~~388994~~) is generated. configid can be used as parentId that is referenced by other features. This way, you can combine rule conditions and features for flexible configurations.
+        If you set **parentId** to **-1**, the existing rule conditions in the configurations are deleted.
+        [{
+        "functionArgs": [{
+        "argName": "Parameter A",
+        "argValue": Value of parameter A"
+        },
+        {
+        "argName": "Parameter B",
+        "argValue": "Value of parameter B"
+        }],
+        "functionName": "Feature name"
+        "parentId": "Optional, which corresponds to configid of the referenced rule condition"
+        }]
+        The following code shows a sample configuration if **parentId** is not used.
+        In this example, the **origin_request_header** feature is used to add back-to-origin HTTP headers, and the rule condition whose configuration ID is **222728944812032** is referenced.
+        [{
+        "functionArgs": [{
+        "argName": "header_operation_type",
+        "argValue": "add"
+        }, {
+        "argName": "header_name",
+        "argValue": "Accept-Encoding"
+        }, {
+        "argName": "header_value",
+        "argValue": "gzip"
+        }, {
+        "argName": "duplicate",
+        "argValue": "off"
+        }],
+        "functionName": "origin_request_header"
+        }]
+        The following code shows a sample configuration if **parentId** is used.
+        In this example, the **origin_request_header** feature is used to add back-to-origin HTTP headers, and the rule condition whose configuration ID is **222728944812032** is referenced.
+        [{
+        "functionArgs": [{
+        "argName": "header_operation_type",
+        "argValue": "add"
+        }, {
+        "argName": "header_name",
+        "argValue": "Accept-Encoding"
+        }, {
+        "argName": "header_value",
+        "argValue": "gzip"
+        }, {
+        "argName": "duplicate",
+        "argValue": "off"
+        }],
+        "functionName": "origin_request_header",
+        "parentId": "222728944812032"
+        }]
         
         @param request: BatchSetCdnDomainConfigRequest
         @return: BatchSetCdnDomainConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.batch_set_cdn_domain_config_with_options_async(request, runtime)
 
     def batch_set_cdn_domain_server_certificate_with_options(
         self,
         request: cdn_20180510_models.BatchSetCdnDomainServerCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.BatchSetCdnDomainServerCertificateResponse:
         """
-        >    The maximum number of times that each user can call this operation per second is 10.
-        *   You can specify multiple domain names (no more than 50) and separate them with commas (,).
+        The content of the SSL certificate. Specify the content of the certificate only if you want to enable the SSL certificate.
         
         @param request: BatchSetCdnDomainServerCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchSetCdnDomainServerCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -744,16 +893,15 @@
 
     async def batch_set_cdn_domain_server_certificate_with_options_async(
         self,
         request: cdn_20180510_models.BatchSetCdnDomainServerCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.BatchSetCdnDomainServerCertificateResponse:
         """
-        >    The maximum number of times that each user can call this operation per second is 10.
-        *   You can specify multiple domain names (no more than 50) and separate them with commas (,).
+        The content of the SSL certificate. Specify the content of the certificate only if you want to enable the SSL certificate.
         
         @param request: BatchSetCdnDomainServerCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchSetCdnDomainServerCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -797,46 +945,42 @@
         )
 
     def batch_set_cdn_domain_server_certificate(
         self,
         request: cdn_20180510_models.BatchSetCdnDomainServerCertificateRequest,
     ) -> cdn_20180510_models.BatchSetCdnDomainServerCertificateResponse:
         """
-        >    The maximum number of times that each user can call this operation per second is 10.
-        *   You can specify multiple domain names (no more than 50) and separate them with commas (,).
+        The content of the SSL certificate. Specify the content of the certificate only if you want to enable the SSL certificate.
         
         @param request: BatchSetCdnDomainServerCertificateRequest
         @return: BatchSetCdnDomainServerCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_set_cdn_domain_server_certificate_with_options(request, runtime)
 
     async def batch_set_cdn_domain_server_certificate_async(
         self,
         request: cdn_20180510_models.BatchSetCdnDomainServerCertificateRequest,
     ) -> cdn_20180510_models.BatchSetCdnDomainServerCertificateResponse:
         """
-        >    The maximum number of times that each user can call this operation per second is 10.
-        *   You can specify multiple domain names (no more than 50) and separate them with commas (,).
+        The content of the SSL certificate. Specify the content of the certificate only if you want to enable the SSL certificate.
         
         @param request: BatchSetCdnDomainServerCertificateRequest
         @return: BatchSetCdnDomainServerCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.batch_set_cdn_domain_server_certificate_with_options_async(request, runtime)
 
     def batch_start_cdn_domain_with_options(
         self,
         request: cdn_20180510_models.BatchStartCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.BatchStartCdnDomainResponse:
         """
-        - If the domain name is in an invalid state or your have an overdue payment in your account, the domain name cannot be enabled.
-        - The maximum number of times that each user can call this operation per second is 30.
-        - The maximum number of domain names configured at a time is 50.
+        The domain names that you want to enable. Separate multiple domain names with commas (,).
         
         @param request: BatchStartCdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchStartCdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -867,17 +1011,15 @@
 
     async def batch_start_cdn_domain_with_options_async(
         self,
         request: cdn_20180510_models.BatchStartCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.BatchStartCdnDomainResponse:
         """
-        - If the domain name is in an invalid state or your have an overdue payment in your account, the domain name cannot be enabled.
-        - The maximum number of times that each user can call this operation per second is 30.
-        - The maximum number of domain names configured at a time is 50.
+        The domain names that you want to enable. Separate multiple domain names with commas (,).
         
         @param request: BatchStartCdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchStartCdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -907,32 +1049,28 @@
         )
 
     def batch_start_cdn_domain(
         self,
         request: cdn_20180510_models.BatchStartCdnDomainRequest,
     ) -> cdn_20180510_models.BatchStartCdnDomainResponse:
         """
-        - If the domain name is in an invalid state or your have an overdue payment in your account, the domain name cannot be enabled.
-        - The maximum number of times that each user can call this operation per second is 30.
-        - The maximum number of domain names configured at a time is 50.
+        The domain names that you want to enable. Separate multiple domain names with commas (,).
         
         @param request: BatchStartCdnDomainRequest
         @return: BatchStartCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_start_cdn_domain_with_options(request, runtime)
 
     async def batch_start_cdn_domain_async(
         self,
         request: cdn_20180510_models.BatchStartCdnDomainRequest,
     ) -> cdn_20180510_models.BatchStartCdnDomainResponse:
         """
-        - If the domain name is in an invalid state or your have an overdue payment in your account, the domain name cannot be enabled.
-        - The maximum number of times that each user can call this operation per second is 30.
-        - The maximum number of domain names configured at a time is 50.
+        The domain names that you want to enable. Separate multiple domain names with commas (,).
         
         @param request: BatchStartCdnDomainRequest
         @return: BatchStartCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.batch_start_cdn_domain_with_options_async(request, runtime)
 
@@ -1298,15 +1436,15 @@
 
     def create_cdn_deliver_task_with_options(
         self,
         request: cdn_20180510_models.CreateCdnDeliverTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.CreateCdnDeliverTaskResponse:
         """
-        > You can call this operation up to three times per second per account.
+        The ID of the tracking task.
         
         @param request: CreateCdnDeliverTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateCdnDeliverTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -1341,15 +1479,15 @@
 
     async def create_cdn_deliver_task_with_options_async(
         self,
         request: cdn_20180510_models.CreateCdnDeliverTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.CreateCdnDeliverTaskResponse:
         """
-        > You can call this operation up to three times per second per account.
+        The ID of the tracking task.
         
         @param request: CreateCdnDeliverTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateCdnDeliverTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -1383,28 +1521,28 @@
         )
 
     def create_cdn_deliver_task(
         self,
         request: cdn_20180510_models.CreateCdnDeliverTaskRequest,
     ) -> cdn_20180510_models.CreateCdnDeliverTaskResponse:
         """
-        > You can call this operation up to three times per second per account.
+        The ID of the tracking task.
         
         @param request: CreateCdnDeliverTaskRequest
         @return: CreateCdnDeliverTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_cdn_deliver_task_with_options(request, runtime)
 
     async def create_cdn_deliver_task_async(
         self,
         request: cdn_20180510_models.CreateCdnDeliverTaskRequest,
     ) -> cdn_20180510_models.CreateCdnDeliverTaskResponse:
         """
-        > You can call this operation up to three times per second per account.
+        The ID of the tracking task.
         
         @param request: CreateCdnDeliverTaskRequest
         @return: CreateCdnDeliverTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_cdn_deliver_task_with_options_async(request, runtime)
 
@@ -1514,17 +1652,17 @@
 
     def create_illegal_url_export_task_with_options(
         self,
         request: cdn_20180510_models.CreateIllegalUrlExportTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.CreateIllegalUrlExportTaskResponse:
         """
-        >    You can query data only by day. You can query data of the last month or later.
-        *   In most cases, a file that contains invalid URLs is generated five minutes after you create an export task. You can call the [DescribeIllegalUrlExportTask](~~156506~~) operation to query the URL where you can download the file.
-        *   The maximum number of times that each user can call this operation per second is 1.
+        You can query data only by day. You can query data within the last 31 days.
+        *   Typically, a file that contains invalid URLs is generated five minutes after you create an export task. You can call the [DescribeIllegalUrlExportTask](~~156506~~) operation to query the URL from which you can download the file.
+        *   You can call this operation only once per second per account.
         
         @param request: CreateIllegalUrlExportTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateIllegalUrlExportTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1553,17 +1691,17 @@
 
     async def create_illegal_url_export_task_with_options_async(
         self,
         request: cdn_20180510_models.CreateIllegalUrlExportTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.CreateIllegalUrlExportTaskResponse:
         """
-        >    You can query data only by day. You can query data of the last month or later.
-        *   In most cases, a file that contains invalid URLs is generated five minutes after you create an export task. You can call the [DescribeIllegalUrlExportTask](~~156506~~) operation to query the URL where you can download the file.
-        *   The maximum number of times that each user can call this operation per second is 1.
+        You can query data only by day. You can query data within the last 31 days.
+        *   Typically, a file that contains invalid URLs is generated five minutes after you create an export task. You can call the [DescribeIllegalUrlExportTask](~~156506~~) operation to query the URL from which you can download the file.
+        *   You can call this operation only once per second per account.
         
         @param request: CreateIllegalUrlExportTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateIllegalUrlExportTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1591,46 +1729,46 @@
         )
 
     def create_illegal_url_export_task(
         self,
         request: cdn_20180510_models.CreateIllegalUrlExportTaskRequest,
     ) -> cdn_20180510_models.CreateIllegalUrlExportTaskResponse:
         """
-        >    You can query data only by day. You can query data of the last month or later.
-        *   In most cases, a file that contains invalid URLs is generated five minutes after you create an export task. You can call the [DescribeIllegalUrlExportTask](~~156506~~) operation to query the URL where you can download the file.
-        *   The maximum number of times that each user can call this operation per second is 1.
+        You can query data only by day. You can query data within the last 31 days.
+        *   Typically, a file that contains invalid URLs is generated five minutes after you create an export task. You can call the [DescribeIllegalUrlExportTask](~~156506~~) operation to query the URL from which you can download the file.
+        *   You can call this operation only once per second per account.
         
         @param request: CreateIllegalUrlExportTaskRequest
         @return: CreateIllegalUrlExportTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_illegal_url_export_task_with_options(request, runtime)
 
     async def create_illegal_url_export_task_async(
         self,
         request: cdn_20180510_models.CreateIllegalUrlExportTaskRequest,
     ) -> cdn_20180510_models.CreateIllegalUrlExportTaskResponse:
         """
-        >    You can query data only by day. You can query data of the last month or later.
-        *   In most cases, a file that contains invalid URLs is generated five minutes after you create an export task. You can call the [DescribeIllegalUrlExportTask](~~156506~~) operation to query the URL where you can download the file.
-        *   The maximum number of times that each user can call this operation per second is 1.
+        You can query data only by day. You can query data within the last 31 days.
+        *   Typically, a file that contains invalid URLs is generated five minutes after you create an export task. You can call the [DescribeIllegalUrlExportTask](~~156506~~) operation to query the URL from which you can download the file.
+        *   You can call this operation only once per second per account.
         
         @param request: CreateIllegalUrlExportTaskRequest
         @return: CreateIllegalUrlExportTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_illegal_url_export_task_with_options_async(request, runtime)
 
     def create_real_time_log_delivery_with_options(
         self,
         request: cdn_20180510_models.CreateRealTimeLogDeliveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.CreateRealTimeLogDeliveryResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        >  You can call this API operation up to 100 times per second per account.
         
         @param request: CreateRealTimeLogDeliveryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateRealTimeLogDeliveryResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -1655,15 +1793,15 @@
 
     async def create_real_time_log_delivery_with_options_async(
         self,
         request: cdn_20180510_models.CreateRealTimeLogDeliveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.CreateRealTimeLogDeliveryResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        >  You can call this API operation up to 100 times per second per account.
         
         @param request: CreateRealTimeLogDeliveryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateRealTimeLogDeliveryResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -1687,28 +1825,28 @@
         )
 
     def create_real_time_log_delivery(
         self,
         request: cdn_20180510_models.CreateRealTimeLogDeliveryRequest,
     ) -> cdn_20180510_models.CreateRealTimeLogDeliveryResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        >  You can call this API operation up to 100 times per second per account.
         
         @param request: CreateRealTimeLogDeliveryRequest
         @return: CreateRealTimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_real_time_log_delivery_with_options(request, runtime)
 
     async def create_real_time_log_delivery_async(
         self,
         request: cdn_20180510_models.CreateRealTimeLogDeliveryRequest,
     ) -> cdn_20180510_models.CreateRealTimeLogDeliveryResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        >  You can call this API operation up to 100 times per second per account.
         
         @param request: CreateRealTimeLogDeliveryRequest
         @return: CreateRealTimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_real_time_log_delivery_with_options_async(request, runtime)
 
@@ -2046,17 +2184,15 @@
 
     def delete_cdn_domain_with_options(
         self,
         request: cdn_20180510_models.DeleteCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DeleteCdnDomainResponse:
         """
-        - We recommend that you add an A record for the domain name in the system of your DNS service provider before you delete the domain name from Alibaba Cloud CDN. Otherwise, the domain name may become inaccessible. Proceed with caution.
-        - After you successfully call the DeleteCdnDomain operation, all records of the deleted domain name are removed. If you need to only disable the domain name, we recommend that you call the StopCdnDomain operation.
-        - The maximum number of times that each user can call this operation per second is 10.
+        The accelerated domain name that you want to delete. You can specify only one domain name in each call.
         
         @param request: DeleteCdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteCdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2087,17 +2223,15 @@
 
     async def delete_cdn_domain_with_options_async(
         self,
         request: cdn_20180510_models.DeleteCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DeleteCdnDomainResponse:
         """
-        - We recommend that you add an A record for the domain name in the system of your DNS service provider before you delete the domain name from Alibaba Cloud CDN. Otherwise, the domain name may become inaccessible. Proceed with caution.
-        - After you successfully call the DeleteCdnDomain operation, all records of the deleted domain name are removed. If you need to only disable the domain name, we recommend that you call the StopCdnDomain operation.
-        - The maximum number of times that each user can call this operation per second is 10.
+        The accelerated domain name that you want to delete. You can specify only one domain name in each call.
         
         @param request: DeleteCdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteCdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2127,32 +2261,28 @@
         )
 
     def delete_cdn_domain(
         self,
         request: cdn_20180510_models.DeleteCdnDomainRequest,
     ) -> cdn_20180510_models.DeleteCdnDomainResponse:
         """
-        - We recommend that you add an A record for the domain name in the system of your DNS service provider before you delete the domain name from Alibaba Cloud CDN. Otherwise, the domain name may become inaccessible. Proceed with caution.
-        - After you successfully call the DeleteCdnDomain operation, all records of the deleted domain name are removed. If you need to only disable the domain name, we recommend that you call the StopCdnDomain operation.
-        - The maximum number of times that each user can call this operation per second is 10.
+        The accelerated domain name that you want to delete. You can specify only one domain name in each call.
         
         @param request: DeleteCdnDomainRequest
         @return: DeleteCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_cdn_domain_with_options(request, runtime)
 
     async def delete_cdn_domain_async(
         self,
         request: cdn_20180510_models.DeleteCdnDomainRequest,
     ) -> cdn_20180510_models.DeleteCdnDomainResponse:
         """
-        - We recommend that you add an A record for the domain name in the system of your DNS service provider before you delete the domain name from Alibaba Cloud CDN. Otherwise, the domain name may become inaccessible. Proceed with caution.
-        - After you successfully call the DeleteCdnDomain operation, all records of the deleted domain name are removed. If you need to only disable the domain name, we recommend that you call the StopCdnDomain operation.
-        - The maximum number of times that each user can call this operation per second is 10.
+        The accelerated domain name that you want to delete. You can specify only one domain name in each call.
         
         @param request: DeleteCdnDomainRequest
         @return: DeleteCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_cdn_domain_with_options_async(request, runtime)
 
@@ -2394,15 +2524,15 @@
 
     def delete_realtime_log_delivery_with_options(
         self,
         request: cdn_20180510_models.DeleteRealtimeLogDeliveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DeleteRealtimeLogDeliveryResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DeleteRealtimeLogDeliveryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteRealtimeLogDeliveryResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -2427,15 +2557,15 @@
 
     async def delete_realtime_log_delivery_with_options_async(
         self,
         request: cdn_20180510_models.DeleteRealtimeLogDeliveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DeleteRealtimeLogDeliveryResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DeleteRealtimeLogDeliveryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteRealtimeLogDeliveryResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -2459,42 +2589,42 @@
         )
 
     def delete_realtime_log_delivery(
         self,
         request: cdn_20180510_models.DeleteRealtimeLogDeliveryRequest,
     ) -> cdn_20180510_models.DeleteRealtimeLogDeliveryResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DeleteRealtimeLogDeliveryRequest
         @return: DeleteRealtimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_realtime_log_delivery_with_options(request, runtime)
 
     async def delete_realtime_log_delivery_async(
         self,
         request: cdn_20180510_models.DeleteRealtimeLogDeliveryRequest,
     ) -> cdn_20180510_models.DeleteRealtimeLogDeliveryResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DeleteRealtimeLogDeliveryRequest
         @return: DeleteRealtimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_realtime_log_delivery_with_options_async(request, runtime)
 
     def delete_specific_config_with_options(
         self,
         request: cdn_20180510_models.DeleteSpecificConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DeleteSpecificConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DeleteSpecificConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteSpecificConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2527,15 +2657,15 @@
 
     async def delete_specific_config_with_options_async(
         self,
         request: cdn_20180510_models.DeleteSpecificConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DeleteSpecificConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DeleteSpecificConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteSpecificConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2567,28 +2697,28 @@
         )
 
     def delete_specific_config(
         self,
         request: cdn_20180510_models.DeleteSpecificConfigRequest,
     ) -> cdn_20180510_models.DeleteSpecificConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DeleteSpecificConfigRequest
         @return: DeleteSpecificConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_specific_config_with_options(request, runtime)
 
     async def delete_specific_config_async(
         self,
         request: cdn_20180510_models.DeleteSpecificConfigRequest,
     ) -> cdn_20180510_models.DeleteSpecificConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DeleteSpecificConfigRequest
         @return: DeleteSpecificConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_specific_config_with_options_async(request, runtime)
 
@@ -2894,15 +3024,15 @@
 
     def describe_blocked_regions_with_options(
         self,
         request: cdn_20180510_models.DescribeBlockedRegionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeBlockedRegionsResponse:
         """
-        >  You can call this operation up to 50 times per second.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeBlockedRegionsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeBlockedRegionsResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -2927,15 +3057,15 @@
 
     async def describe_blocked_regions_with_options_async(
         self,
         request: cdn_20180510_models.DescribeBlockedRegionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeBlockedRegionsResponse:
         """
-        >  You can call this operation up to 50 times per second.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeBlockedRegionsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeBlockedRegionsResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -2959,42 +3089,42 @@
         )
 
     def describe_blocked_regions(
         self,
         request: cdn_20180510_models.DescribeBlockedRegionsRequest,
     ) -> cdn_20180510_models.DescribeBlockedRegionsResponse:
         """
-        >  You can call this operation up to 50 times per second.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeBlockedRegionsRequest
         @return: DescribeBlockedRegionsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_blocked_regions_with_options(request, runtime)
 
     async def describe_blocked_regions_async(
         self,
         request: cdn_20180510_models.DescribeBlockedRegionsRequest,
     ) -> cdn_20180510_models.DescribeBlockedRegionsResponse:
         """
-        >  You can call this operation up to 50 times per second.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeBlockedRegionsRequest
         @return: DescribeBlockedRegionsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_blocked_regions_with_options_async(request, runtime)
 
     def describe_cdn_certificate_detail_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnCertificateDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnCertificateDetailResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeCdnCertificateDetailRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnCertificateDetailResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3025,15 +3155,15 @@
 
     async def describe_cdn_certificate_detail_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnCertificateDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnCertificateDetailResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeCdnCertificateDetailRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnCertificateDetailResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3063,42 +3193,42 @@
         )
 
     def describe_cdn_certificate_detail(
         self,
         request: cdn_20180510_models.DescribeCdnCertificateDetailRequest,
     ) -> cdn_20180510_models.DescribeCdnCertificateDetailResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeCdnCertificateDetailRequest
         @return: DescribeCdnCertificateDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_certificate_detail_with_options(request, runtime)
 
     async def describe_cdn_certificate_detail_async(
         self,
         request: cdn_20180510_models.DescribeCdnCertificateDetailRequest,
     ) -> cdn_20180510_models.DescribeCdnCertificateDetailResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
         @param request: DescribeCdnCertificateDetailRequest
         @return: DescribeCdnCertificateDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_certificate_detail_with_options_async(request, runtime)
 
     def describe_cdn_certificate_list_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnCertificateListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnCertificateListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnCertificateListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnCertificateListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3129,15 +3259,15 @@
 
     async def describe_cdn_certificate_list_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnCertificateListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnCertificateListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnCertificateListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnCertificateListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3167,42 +3297,42 @@
         )
 
     def describe_cdn_certificate_list(
         self,
         request: cdn_20180510_models.DescribeCdnCertificateListRequest,
     ) -> cdn_20180510_models.DescribeCdnCertificateListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnCertificateListRequest
         @return: DescribeCdnCertificateListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_certificate_list_with_options(request, runtime)
 
     async def describe_cdn_certificate_list_async(
         self,
         request: cdn_20180510_models.DescribeCdnCertificateListRequest,
     ) -> cdn_20180510_models.DescribeCdnCertificateListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnCertificateListRequest
         @return: DescribeCdnCertificateListResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_certificate_list_with_options_async(request, runtime)
 
     def describe_cdn_deleted_domains_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnDeletedDomainsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnDeletedDomainsResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 10.
+        > You can call this operation up to 10 times per second per account.
         
         @param request: DescribeCdnDeletedDomainsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnDeletedDomainsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3231,15 +3361,15 @@
 
     async def describe_cdn_deleted_domains_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnDeletedDomainsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnDeletedDomainsResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 10.
+        > You can call this operation up to 10 times per second per account.
         
         @param request: DescribeCdnDeletedDomainsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnDeletedDomainsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3267,28 +3397,28 @@
         )
 
     def describe_cdn_deleted_domains(
         self,
         request: cdn_20180510_models.DescribeCdnDeletedDomainsRequest,
     ) -> cdn_20180510_models.DescribeCdnDeletedDomainsResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 10.
+        > You can call this operation up to 10 times per second per account.
         
         @param request: DescribeCdnDeletedDomainsRequest
         @return: DescribeCdnDeletedDomainsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_deleted_domains_with_options(request, runtime)
 
     async def describe_cdn_deleted_domains_async(
         self,
         request: cdn_20180510_models.DescribeCdnDeletedDomainsRequest,
     ) -> cdn_20180510_models.DescribeCdnDeletedDomainsResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 10.
+        > You can call this operation up to 10 times per second per account.
         
         @param request: DescribeCdnDeletedDomainsRequest
         @return: DescribeCdnDeletedDomainsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_deleted_domains_with_options_async(request, runtime)
 
@@ -3490,15 +3620,15 @@
 
     def describe_cdn_domain_configs_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnDomainConfigsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnDomainConfigsResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnDomainConfigsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnDomainConfigsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3533,15 +3663,15 @@
 
     async def describe_cdn_domain_configs_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnDomainConfigsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnDomainConfigsResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnDomainConfigsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnDomainConfigsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3575,42 +3705,42 @@
         )
 
     def describe_cdn_domain_configs(
         self,
         request: cdn_20180510_models.DescribeCdnDomainConfigsRequest,
     ) -> cdn_20180510_models.DescribeCdnDomainConfigsResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnDomainConfigsRequest
         @return: DescribeCdnDomainConfigsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_domain_configs_with_options(request, runtime)
 
     async def describe_cdn_domain_configs_async(
         self,
         request: cdn_20180510_models.DescribeCdnDomainConfigsRequest,
     ) -> cdn_20180510_models.DescribeCdnDomainConfigsResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnDomainConfigsRequest
         @return: DescribeCdnDomainConfigsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_domain_configs_with_options_async(request, runtime)
 
     def describe_cdn_domain_detail_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnDomainDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnDomainDetailResponse:
         """
-        The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnDomainDetailRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnDomainDetailResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3641,15 +3771,15 @@
 
     async def describe_cdn_domain_detail_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnDomainDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnDomainDetailResponse:
         """
-        The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnDomainDetailRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnDomainDetailResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3679,28 +3809,28 @@
         )
 
     def describe_cdn_domain_detail(
         self,
         request: cdn_20180510_models.DescribeCdnDomainDetailRequest,
     ) -> cdn_20180510_models.DescribeCdnDomainDetailResponse:
         """
-        The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnDomainDetailRequest
         @return: DescribeCdnDomainDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_domain_detail_with_options(request, runtime)
 
     async def describe_cdn_domain_detail_async(
         self,
         request: cdn_20180510_models.DescribeCdnDomainDetailRequest,
     ) -> cdn_20180510_models.DescribeCdnDomainDetailResponse:
         """
-        The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnDomainDetailRequest
         @return: DescribeCdnDomainDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_domain_detail_with_options_async(request, runtime)
 
@@ -3830,15 +3960,15 @@
 
     def describe_cdn_domain_staging_config_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnDomainStagingConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnDomainStagingConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnDomainStagingConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnDomainStagingConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3867,15 +3997,15 @@
 
     async def describe_cdn_domain_staging_config_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnDomainStagingConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnDomainStagingConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnDomainStagingConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnDomainStagingConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3903,28 +4033,28 @@
         )
 
     def describe_cdn_domain_staging_config(
         self,
         request: cdn_20180510_models.DescribeCdnDomainStagingConfigRequest,
     ) -> cdn_20180510_models.DescribeCdnDomainStagingConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnDomainStagingConfigRequest
         @return: DescribeCdnDomainStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_domain_staging_config_with_options(request, runtime)
 
     async def describe_cdn_domain_staging_config_async(
         self,
         request: cdn_20180510_models.DescribeCdnDomainStagingConfigRequest,
     ) -> cdn_20180510_models.DescribeCdnDomainStagingConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnDomainStagingConfigRequest
         @return: DescribeCdnDomainStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_domain_staging_config_with_options_async(request, runtime)
 
@@ -4112,16 +4242,16 @@
 
     def describe_cdn_region_and_isp_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnRegionAndIspRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnRegionAndIspResponse:
         """
-        >    The lists of ISPs and regions that are supported by Alibaba Cloud CDN are updated and published on the Alibaba Cloud International site.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        The lists of ISPs and regions that are supported by Alibaba Cloud CDN are updated and published on the Alibaba Cloud International site.
+        *   You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnRegionAndIspRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnRegionAndIspResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4150,16 +4280,16 @@
 
     async def describe_cdn_region_and_isp_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnRegionAndIspRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnRegionAndIspResponse:
         """
-        >    The lists of ISPs and regions that are supported by Alibaba Cloud CDN are updated and published on the Alibaba Cloud International site.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        The lists of ISPs and regions that are supported by Alibaba Cloud CDN are updated and published on the Alibaba Cloud International site.
+        *   You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnRegionAndIspRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnRegionAndIspResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4187,30 +4317,30 @@
         )
 
     def describe_cdn_region_and_isp(
         self,
         request: cdn_20180510_models.DescribeCdnRegionAndIspRequest,
     ) -> cdn_20180510_models.DescribeCdnRegionAndIspResponse:
         """
-        >    The lists of ISPs and regions that are supported by Alibaba Cloud CDN are updated and published on the Alibaba Cloud International site.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        The lists of ISPs and regions that are supported by Alibaba Cloud CDN are updated and published on the Alibaba Cloud International site.
+        *   You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnRegionAndIspRequest
         @return: DescribeCdnRegionAndIspResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_region_and_isp_with_options(request, runtime)
 
     async def describe_cdn_region_and_isp_async(
         self,
         request: cdn_20180510_models.DescribeCdnRegionAndIspRequest,
     ) -> cdn_20180510_models.DescribeCdnRegionAndIspResponse:
         """
-        >    The lists of ISPs and regions that are supported by Alibaba Cloud CDN are updated and published on the Alibaba Cloud International site.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        The lists of ISPs and regions that are supported by Alibaba Cloud CDN are updated and published on the Alibaba Cloud International site.
+        *   You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnRegionAndIspRequest
         @return: DescribeCdnRegionAndIspResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_region_and_isp_with_options_async(request, runtime)
 
@@ -4336,16 +4466,16 @@
 
     def describe_cdn_report_list_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnReportListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnReportListResponse:
         """
-        > - This operation queries the metadata of all operations reports. The statistics in the reports are not returned.
-        - You can call this API operation up to three times per second per account.
+        This operation queries the metadata of all operations reports. The statistics in the reports are not returned.
+        *   You can call this operation up to three times per second per account.
         
         @param request: DescribeCdnReportListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnReportListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4372,16 +4502,16 @@
 
     async def describe_cdn_report_list_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnReportListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnReportListResponse:
         """
-        > - This operation queries the metadata of all operations reports. The statistics in the reports are not returned.
-        - You can call this API operation up to three times per second per account.
+        This operation queries the metadata of all operations reports. The statistics in the reports are not returned.
+        *   You can call this operation up to three times per second per account.
         
         @param request: DescribeCdnReportListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnReportListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4407,30 +4537,30 @@
         )
 
     def describe_cdn_report_list(
         self,
         request: cdn_20180510_models.DescribeCdnReportListRequest,
     ) -> cdn_20180510_models.DescribeCdnReportListResponse:
         """
-        > - This operation queries the metadata of all operations reports. The statistics in the reports are not returned.
-        - You can call this API operation up to three times per second per account.
+        This operation queries the metadata of all operations reports. The statistics in the reports are not returned.
+        *   You can call this operation up to three times per second per account.
         
         @param request: DescribeCdnReportListRequest
         @return: DescribeCdnReportListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_report_list_with_options(request, runtime)
 
     async def describe_cdn_report_list_async(
         self,
         request: cdn_20180510_models.DescribeCdnReportListRequest,
     ) -> cdn_20180510_models.DescribeCdnReportListResponse:
         """
-        > - This operation queries the metadata of all operations reports. The statistics in the reports are not returned.
-        - You can call this API operation up to three times per second per account.
+        This operation queries the metadata of all operations reports. The statistics in the reports are not returned.
+        *   You can call this operation up to three times per second per account.
         
         @param request: DescribeCdnReportListRequest
         @return: DescribeCdnReportListResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_report_list_with_options_async(request, runtime)
 
@@ -4540,15 +4670,15 @@
 
     def describe_cdn_smcertificate_list_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnSMCertificateListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnSMCertificateListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnSMCertificateListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnSMCertificateListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4579,15 +4709,15 @@
 
     async def describe_cdn_smcertificate_list_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnSMCertificateListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnSMCertificateListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnSMCertificateListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnSMCertificateListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4617,42 +4747,42 @@
         )
 
     def describe_cdn_smcertificate_list(
         self,
         request: cdn_20180510_models.DescribeCdnSMCertificateListRequest,
     ) -> cdn_20180510_models.DescribeCdnSMCertificateListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnSMCertificateListRequest
         @return: DescribeCdnSMCertificateListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_smcertificate_list_with_options(request, runtime)
 
     async def describe_cdn_smcertificate_list_async(
         self,
         request: cdn_20180510_models.DescribeCdnSMCertificateListRequest,
     ) -> cdn_20180510_models.DescribeCdnSMCertificateListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnSMCertificateListRequest
         @return: DescribeCdnSMCertificateListResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_smcertificate_list_with_options_async(request, runtime)
 
     def describe_cdn_service_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnServiceResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnServiceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnServiceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4681,15 +4811,15 @@
 
     async def describe_cdn_service_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnServiceResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnServiceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnServiceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4717,42 +4847,41 @@
         )
 
     def describe_cdn_service(
         self,
         request: cdn_20180510_models.DescribeCdnServiceRequest,
     ) -> cdn_20180510_models.DescribeCdnServiceResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnServiceRequest
         @return: DescribeCdnServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_service_with_options(request, runtime)
 
     async def describe_cdn_service_async(
         self,
         request: cdn_20180510_models.DescribeCdnServiceRequest,
     ) -> cdn_20180510_models.DescribeCdnServiceResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnServiceRequest
         @return: DescribeCdnServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_service_with_options_async(request, runtime)
 
     def describe_cdn_sub_list_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnSubListResponse:
         """
-        By default, this operation queries all custom operations reports. However, only one operations report can be displayed. Therefore, only one operations report is returned.
-        *   You can call this operation up to three times per second per account.
+        {"RequestId":"3250A51D-C11D-46BA-B6B3-95348EEDE652","Description":"Successful","Content":{"data":\\[{"subId":5,"reportId":\\[1,2,3],"createTime":"2020-09-25T09:39:33Z","domains"\\["www.example.com","www.example.com"],"effectiveFrom":"2020-09-17T00:00:00Z","effectiveEnd":"2020-11-17T00:00:00Z","status":"enable"}]}}
         
         @param request: DescribeCdnSubListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnSubListResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -4772,16 +4901,15 @@
         )
 
     async def describe_cdn_sub_list_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnSubListResponse:
         """
-        By default, this operation queries all custom operations reports. However, only one operations report can be displayed. Therefore, only one operations report is returned.
-        *   You can call this operation up to three times per second per account.
+        {"RequestId":"3250A51D-C11D-46BA-B6B3-95348EEDE652","Description":"Successful","Content":{"data":\\[{"subId":5,"reportId":\\[1,2,3],"createTime":"2020-09-25T09:39:33Z","domains"\\["www.example.com","www.example.com"],"effectiveFrom":"2020-09-17T00:00:00Z","effectiveEnd":"2020-11-17T00:00:00Z","status":"enable"}]}}
         
         @param request: DescribeCdnSubListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnSubListResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -4798,26 +4926,24 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnSubListResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_cdn_sub_list(self) -> cdn_20180510_models.DescribeCdnSubListResponse:
         """
-        By default, this operation queries all custom operations reports. However, only one operations report can be displayed. Therefore, only one operations report is returned.
-        *   You can call this operation up to three times per second per account.
+        {"RequestId":"3250A51D-C11D-46BA-B6B3-95348EEDE652","Description":"Successful","Content":{"data":\\[{"subId":5,"reportId":\\[1,2,3],"createTime":"2020-09-25T09:39:33Z","domains"\\["www.example.com","www.example.com"],"effectiveFrom":"2020-09-17T00:00:00Z","effectiveEnd":"2020-11-17T00:00:00Z","status":"enable"}]}}
         
         @return: DescribeCdnSubListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_sub_list_with_options(runtime)
 
     async def describe_cdn_sub_list_async(self) -> cdn_20180510_models.DescribeCdnSubListResponse:
         """
-        By default, this operation queries all custom operations reports. However, only one operations report can be displayed. Therefore, only one operations report is returned.
-        *   You can call this operation up to three times per second per account.
+        {"RequestId":"3250A51D-C11D-46BA-B6B3-95348EEDE652","Description":"Successful","Content":{"data":\\[{"subId":5,"reportId":\\[1,2,3],"createTime":"2020-09-25T09:39:33Z","domains"\\["www.example.com","www.example.com"],"effectiveFrom":"2020-09-17T00:00:00Z","effectiveEnd":"2020-11-17T00:00:00Z","status":"enable"}]}}
         
         @return: DescribeCdnSubListResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_sub_list_with_options_async(runtime)
 
     def describe_cdn_user_bill_history_with_options(
@@ -4926,21 +5052,21 @@
 
     def describe_cdn_user_bill_prediction_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnUserBillPredictionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnUserBillPredictionResponse:
         """
-        You can call this operation to estimate resource usage of the current month based on the metering method set on the first day of the current month. This operation can estimate resource usage only of the current month within your Alibaba Cloud account. The time range used for the estimation starts at 00:00 on the first day of the current month and ends 2 hours earlier than the current time.
-        *   Pay by monthly 95th percentile: The top 5% values between the start time and end time are excluded. The highest value among the remaining values is the estimated value.
+        You can call this operation to estimate resource usage of the current month based on the metering method that is specified on the first day of the current month. You can call this operation to estimate resource usage only of the current month within your Alibaba Cloud account. The time range used for the estimation starts at 00:00 on the first day of the current month and ends 2 hours earlier than the current time.
+        *   Pay by monthly 95th percentile: The top 5% values between the start time and end time are excluded. The estimated value is the highest value among the remaining values.
         *   Pay by average daily peak bandwidth per month: Estimated value = Sum of daily peak bandwidth values/Number of days. The current day is excluded.
-        *   Pay by 4th peak bandwidth per month: The 4th peak bandwidth value between the start time and end time is the estimated value. If the time range is less than 4 days, the estimated value is 0.
+        *   Pay by 4th peak bandwidth per month: The estimated value is the 4th peak bandwidth value between the start time and end time. If the time range is less than four days, the estimated value is 0.
         *   Pay by average daily 95th percentile bandwidth per month: Estimated value = Sum of daily 95th percentile bandwidth values/Number of days. The current day is excluded.
-        *   Pay by 95th percentile bandwidth with 50% off from 00:00 to 08:00: The top 5% values between the start time and end time are excluded. The highest value among the remaining values is the estimated value.
-        >  The maximum number of times that each user can call this operation per second is 1.
+        *   Pay by 95th percentile bandwidth with 50% off from 00:00 to 08:00: The top 5% values between the start time and end time are excluded. The estimated value is the highest value among the remaining values.
+        > You can call this operation only once per second per account.
         
         @param request: DescribeCdnUserBillPredictionRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnUserBillPredictionResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4973,21 +5099,21 @@
 
     async def describe_cdn_user_bill_prediction_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnUserBillPredictionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnUserBillPredictionResponse:
         """
-        You can call this operation to estimate resource usage of the current month based on the metering method set on the first day of the current month. This operation can estimate resource usage only of the current month within your Alibaba Cloud account. The time range used for the estimation starts at 00:00 on the first day of the current month and ends 2 hours earlier than the current time.
-        *   Pay by monthly 95th percentile: The top 5% values between the start time and end time are excluded. The highest value among the remaining values is the estimated value.
+        You can call this operation to estimate resource usage of the current month based on the metering method that is specified on the first day of the current month. You can call this operation to estimate resource usage only of the current month within your Alibaba Cloud account. The time range used for the estimation starts at 00:00 on the first day of the current month and ends 2 hours earlier than the current time.
+        *   Pay by monthly 95th percentile: The top 5% values between the start time and end time are excluded. The estimated value is the highest value among the remaining values.
         *   Pay by average daily peak bandwidth per month: Estimated value = Sum of daily peak bandwidth values/Number of days. The current day is excluded.
-        *   Pay by 4th peak bandwidth per month: The 4th peak bandwidth value between the start time and end time is the estimated value. If the time range is less than 4 days, the estimated value is 0.
+        *   Pay by 4th peak bandwidth per month: The estimated value is the 4th peak bandwidth value between the start time and end time. If the time range is less than four days, the estimated value is 0.
         *   Pay by average daily 95th percentile bandwidth per month: Estimated value = Sum of daily 95th percentile bandwidth values/Number of days. The current day is excluded.
-        *   Pay by 95th percentile bandwidth with 50% off from 00:00 to 08:00: The top 5% values between the start time and end time are excluded. The highest value among the remaining values is the estimated value.
-        >  The maximum number of times that each user can call this operation per second is 1.
+        *   Pay by 95th percentile bandwidth with 50% off from 00:00 to 08:00: The top 5% values between the start time and end time are excluded. The estimated value is the highest value among the remaining values.
+        > You can call this operation only once per second per account.
         
         @param request: DescribeCdnUserBillPredictionRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnUserBillPredictionResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5019,40 +5145,40 @@
         )
 
     def describe_cdn_user_bill_prediction(
         self,
         request: cdn_20180510_models.DescribeCdnUserBillPredictionRequest,
     ) -> cdn_20180510_models.DescribeCdnUserBillPredictionResponse:
         """
-        You can call this operation to estimate resource usage of the current month based on the metering method set on the first day of the current month. This operation can estimate resource usage only of the current month within your Alibaba Cloud account. The time range used for the estimation starts at 00:00 on the first day of the current month and ends 2 hours earlier than the current time.
-        *   Pay by monthly 95th percentile: The top 5% values between the start time and end time are excluded. The highest value among the remaining values is the estimated value.
+        You can call this operation to estimate resource usage of the current month based on the metering method that is specified on the first day of the current month. You can call this operation to estimate resource usage only of the current month within your Alibaba Cloud account. The time range used for the estimation starts at 00:00 on the first day of the current month and ends 2 hours earlier than the current time.
+        *   Pay by monthly 95th percentile: The top 5% values between the start time and end time are excluded. The estimated value is the highest value among the remaining values.
         *   Pay by average daily peak bandwidth per month: Estimated value = Sum of daily peak bandwidth values/Number of days. The current day is excluded.
-        *   Pay by 4th peak bandwidth per month: The 4th peak bandwidth value between the start time and end time is the estimated value. If the time range is less than 4 days, the estimated value is 0.
+        *   Pay by 4th peak bandwidth per month: The estimated value is the 4th peak bandwidth value between the start time and end time. If the time range is less than four days, the estimated value is 0.
         *   Pay by average daily 95th percentile bandwidth per month: Estimated value = Sum of daily 95th percentile bandwidth values/Number of days. The current day is excluded.
-        *   Pay by 95th percentile bandwidth with 50% off from 00:00 to 08:00: The top 5% values between the start time and end time are excluded. The highest value among the remaining values is the estimated value.
-        >  The maximum number of times that each user can call this operation per second is 1.
+        *   Pay by 95th percentile bandwidth with 50% off from 00:00 to 08:00: The top 5% values between the start time and end time are excluded. The estimated value is the highest value among the remaining values.
+        > You can call this operation only once per second per account.
         
         @param request: DescribeCdnUserBillPredictionRequest
         @return: DescribeCdnUserBillPredictionResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_user_bill_prediction_with_options(request, runtime)
 
     async def describe_cdn_user_bill_prediction_async(
         self,
         request: cdn_20180510_models.DescribeCdnUserBillPredictionRequest,
     ) -> cdn_20180510_models.DescribeCdnUserBillPredictionResponse:
         """
-        You can call this operation to estimate resource usage of the current month based on the metering method set on the first day of the current month. This operation can estimate resource usage only of the current month within your Alibaba Cloud account. The time range used for the estimation starts at 00:00 on the first day of the current month and ends 2 hours earlier than the current time.
-        *   Pay by monthly 95th percentile: The top 5% values between the start time and end time are excluded. The highest value among the remaining values is the estimated value.
+        You can call this operation to estimate resource usage of the current month based on the metering method that is specified on the first day of the current month. You can call this operation to estimate resource usage only of the current month within your Alibaba Cloud account. The time range used for the estimation starts at 00:00 on the first day of the current month and ends 2 hours earlier than the current time.
+        *   Pay by monthly 95th percentile: The top 5% values between the start time and end time are excluded. The estimated value is the highest value among the remaining values.
         *   Pay by average daily peak bandwidth per month: Estimated value = Sum of daily peak bandwidth values/Number of days. The current day is excluded.
-        *   Pay by 4th peak bandwidth per month: The 4th peak bandwidth value between the start time and end time is the estimated value. If the time range is less than 4 days, the estimated value is 0.
+        *   Pay by 4th peak bandwidth per month: The estimated value is the 4th peak bandwidth value between the start time and end time. If the time range is less than four days, the estimated value is 0.
         *   Pay by average daily 95th percentile bandwidth per month: Estimated value = Sum of daily 95th percentile bandwidth values/Number of days. The current day is excluded.
-        *   Pay by 95th percentile bandwidth with 50% off from 00:00 to 08:00: The top 5% values between the start time and end time are excluded. The highest value among the remaining values is the estimated value.
-        >  The maximum number of times that each user can call this operation per second is 1.
+        *   Pay by 95th percentile bandwidth with 50% off from 00:00 to 08:00: The top 5% values between the start time and end time are excluded. The estimated value is the highest value among the remaining values.
+        > You can call this operation only once per second per account.
         
         @param request: DescribeCdnUserBillPredictionRequest
         @return: DescribeCdnUserBillPredictionResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_user_bill_prediction_with_options_async(request, runtime)
 
@@ -5158,15 +5284,22 @@
 
     def describe_cdn_user_configs_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnUserConfigsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnUserConfigsResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        The value of the configuration. Valid values:
+        *   **cc_rule**: HTTP flood protection rules
+        *   **ddos_dispatch**: integration with Anti-DDoS
+        *   **edge_safe**: application security settings on edge nodes
+        *   **blocked_regions**: blocked regions
+        *   **http\\_acl\\_policy**: access control list (ACL) rules
+        *   **bot_manager**: bot traffic management
+        *   **ip_reputation**: IP reputation library
         
         @param request: DescribeCdnUserConfigsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnUserConfigsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5193,15 +5326,22 @@
 
     async def describe_cdn_user_configs_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnUserConfigsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnUserConfigsResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        The value of the configuration. Valid values:
+        *   **cc_rule**: HTTP flood protection rules
+        *   **ddos_dispatch**: integration with Anti-DDoS
+        *   **edge_safe**: application security settings on edge nodes
+        *   **blocked_regions**: blocked regions
+        *   **http\\_acl\\_policy**: access control list (ACL) rules
+        *   **bot_manager**: bot traffic management
+        *   **ip_reputation**: IP reputation library
         
         @param request: DescribeCdnUserConfigsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnUserConfigsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5227,47 +5367,54 @@
         )
 
     def describe_cdn_user_configs(
         self,
         request: cdn_20180510_models.DescribeCdnUserConfigsRequest,
     ) -> cdn_20180510_models.DescribeCdnUserConfigsResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        The value of the configuration. Valid values:
+        *   **cc_rule**: HTTP flood protection rules
+        *   **ddos_dispatch**: integration with Anti-DDoS
+        *   **edge_safe**: application security settings on edge nodes
+        *   **blocked_regions**: blocked regions
+        *   **http\\_acl\\_policy**: access control list (ACL) rules
+        *   **bot_manager**: bot traffic management
+        *   **ip_reputation**: IP reputation library
         
         @param request: DescribeCdnUserConfigsRequest
         @return: DescribeCdnUserConfigsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_user_configs_with_options(request, runtime)
 
     async def describe_cdn_user_configs_async(
         self,
         request: cdn_20180510_models.DescribeCdnUserConfigsRequest,
     ) -> cdn_20180510_models.DescribeCdnUserConfigsResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        The value of the configuration. Valid values:
+        *   **cc_rule**: HTTP flood protection rules
+        *   **ddos_dispatch**: integration with Anti-DDoS
+        *   **edge_safe**: application security settings on edge nodes
+        *   **blocked_regions**: blocked regions
+        *   **http\\_acl\\_policy**: access control list (ACL) rules
+        *   **bot_manager**: bot traffic management
+        *   **ip_reputation**: IP reputation library
         
         @param request: DescribeCdnUserConfigsRequest
         @return: DescribeCdnUserConfigsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_user_configs_with_options_async(request, runtime)
 
     def describe_cdn_user_domains_by_func_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnUserDomainsByFuncRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnUserDomainsByFuncResponse:
-        """
-        > You can call this operation up to 100 times per second per account.
-        
-        @param request: DescribeCdnUserDomainsByFuncRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeCdnUserDomainsByFuncResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.func_id):
             query['FuncId'] = request.func_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -5294,21 +5441,14 @@
         )
 
     async def describe_cdn_user_domains_by_func_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnUserDomainsByFuncRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnUserDomainsByFuncResponse:
-        """
-        > You can call this operation up to 100 times per second per account.
-        
-        @param request: DescribeCdnUserDomainsByFuncRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeCdnUserDomainsByFuncResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.func_id):
             query['FuncId'] = request.func_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -5334,43 +5474,31 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_cdn_user_domains_by_func(
         self,
         request: cdn_20180510_models.DescribeCdnUserDomainsByFuncRequest,
     ) -> cdn_20180510_models.DescribeCdnUserDomainsByFuncResponse:
-        """
-        > You can call this operation up to 100 times per second per account.
-        
-        @param request: DescribeCdnUserDomainsByFuncRequest
-        @return: DescribeCdnUserDomainsByFuncResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_user_domains_by_func_with_options(request, runtime)
 
     async def describe_cdn_user_domains_by_func_async(
         self,
         request: cdn_20180510_models.DescribeCdnUserDomainsByFuncRequest,
     ) -> cdn_20180510_models.DescribeCdnUserDomainsByFuncResponse:
-        """
-        > You can call this operation up to 100 times per second per account.
-        
-        @param request: DescribeCdnUserDomainsByFuncRequest
-        @return: DescribeCdnUserDomainsByFuncResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_user_domains_by_func_with_options_async(request, runtime)
 
     def describe_cdn_user_quota_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnUserQuotaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnUserQuotaResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnUserQuotaRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnUserQuotaResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5399,15 +5527,15 @@
 
     async def describe_cdn_user_quota_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnUserQuotaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnUserQuotaResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnUserQuotaRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnUserQuotaResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5435,28 +5563,28 @@
         )
 
     def describe_cdn_user_quota(
         self,
         request: cdn_20180510_models.DescribeCdnUserQuotaRequest,
     ) -> cdn_20180510_models.DescribeCdnUserQuotaResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnUserQuotaRequest
         @return: DescribeCdnUserQuotaResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_user_quota_with_options(request, runtime)
 
     async def describe_cdn_user_quota_async(
         self,
         request: cdn_20180510_models.DescribeCdnUserQuotaRequest,
     ) -> cdn_20180510_models.DescribeCdnUserQuotaResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeCdnUserQuotaRequest
         @return: DescribeCdnUserQuotaResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_user_quota_with_options_async(request, runtime)
 
@@ -5565,14 +5693,21 @@
         return await self.describe_cdn_user_resource_package_with_options_async(request, runtime)
 
     def describe_cdn_waf_domain_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnWafDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnWafDomainResponse:
+        """
+        > You can call this operation up to 150 times per second per account.
+        
+        @param request: DescribeCdnWafDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeCdnWafDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -5597,14 +5732,21 @@
         )
 
     async def describe_cdn_waf_domain_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnWafDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnWafDomainResponse:
+        """
+        > You can call this operation up to 150 times per second per account.
+        
+        @param request: DescribeCdnWafDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeCdnWafDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -5628,21 +5770,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_cdn_waf_domain(
         self,
         request: cdn_20180510_models.DescribeCdnWafDomainRequest,
     ) -> cdn_20180510_models.DescribeCdnWafDomainResponse:
+        """
+        > You can call this operation up to 150 times per second per account.
+        
+        @param request: DescribeCdnWafDomainRequest
+        @return: DescribeCdnWafDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_waf_domain_with_options(request, runtime)
 
     async def describe_cdn_waf_domain_async(
         self,
         request: cdn_20180510_models.DescribeCdnWafDomainRequest,
     ) -> cdn_20180510_models.DescribeCdnWafDomainResponse:
+        """
+        > You can call this operation up to 150 times per second per account.
+        
+        @param request: DescribeCdnWafDomainRequest
+        @return: DescribeCdnWafDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_waf_domain_with_options_async(request, runtime)
 
     def describe_certificate_info_by_idwith_options(
         self,
         request: cdn_20180510_models.DescribeCertificateInfoByIDRequest,
         runtime: util_models.RuntimeOptions,
@@ -5832,18 +5986,15 @@
 
     def describe_domain_average_response_time_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainAverageResponseTimeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainAverageResponseTimeResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - You can call this operation up to 100 times per second per account.
-        - You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
+        The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         
         @param request: DescribeDomainAverageResponseTimeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainAverageResponseTimeResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5884,18 +6035,15 @@
 
     async def describe_domain_average_response_time_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainAverageResponseTimeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainAverageResponseTimeResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - You can call this operation up to 100 times per second per account.
-        - You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
+        The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         
         @param request: DescribeDomainAverageResponseTimeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainAverageResponseTimeResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5935,56 +6083,42 @@
         )
 
     def describe_domain_average_response_time(
         self,
         request: cdn_20180510_models.DescribeDomainAverageResponseTimeRequest,
     ) -> cdn_20180510_models.DescribeDomainAverageResponseTimeResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - You can call this operation up to 100 times per second per account.
-        - You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
+        The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         
         @param request: DescribeDomainAverageResponseTimeRequest
         @return: DescribeDomainAverageResponseTimeResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_average_response_time_with_options(request, runtime)
 
     async def describe_domain_average_response_time_async(
         self,
         request: cdn_20180510_models.DescribeDomainAverageResponseTimeRequest,
     ) -> cdn_20180510_models.DescribeDomainAverageResponseTimeResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - You can call this operation up to 100 times per second per account.
-        - You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
+        The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         
         @param request: DescribeDomainAverageResponseTimeRequest
         @return: DescribeDomainAverageResponseTimeResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_average_response_time_with_options_async(request, runtime)
 
     def describe_domain_bps_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainBpsDataResponse:
         """
-        You can call this operation up to 150 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        The bandwidth value in the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         
         @param request: DescribeDomainBpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainBpsDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6021,23 +6155,15 @@
 
     async def describe_domain_bps_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainBpsDataResponse:
         """
-        You can call this operation up to 150 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        The bandwidth value in the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         
         @param request: DescribeDomainBpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainBpsDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6073,44 +6199,28 @@
         )
 
     def describe_domain_bps_data(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainBpsDataResponse:
         """
-        You can call this operation up to 150 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        The bandwidth value in the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         
         @param request: DescribeDomainBpsDataRequest
         @return: DescribeDomainBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_bps_data_with_options(request, runtime)
 
     async def describe_domain_bps_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainBpsDataResponse:
         """
-        You can call this operation up to 150 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        The bandwidth value in the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         
         @param request: DescribeDomainBpsDataRequest
         @return: DescribeDomainBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_bps_data_with_options_async(request, runtime)
 
@@ -6388,18 +6498,18 @@
 
     def describe_domain_cc_activity_log_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainCcActivityLogRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainCcActivityLogResponse:
         """
-        >    If you do not set the StartTime or EndTime parameter, data within the last 24 hours is queried. If you set both the StartTime and EndTime parameters, data within the specified time range is queried. You must set both parameters or leave both of them empty.
-        *   You can specify multiple domain names (no more than 20) and separate them with commas (,).
-        *   You can query data within the last 30 days.
-        *   The maximum number of times that each user can call this operation per second is 50.
+        If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range. You must set both parameters or leave both parameters empty.
+        *   You can specify up to 20 domain names in reach request. If you specify multiple domain names, separate them with commas (,).
+        *   You can query data collected over the last 30 days.
+        *   You can call this operation up to 50 times per second per account.
         
         @param request: DescribeDomainCcActivityLogRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainCcActivityLogResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6440,18 +6550,18 @@
 
     async def describe_domain_cc_activity_log_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainCcActivityLogRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainCcActivityLogResponse:
         """
-        >    If you do not set the StartTime or EndTime parameter, data within the last 24 hours is queried. If you set both the StartTime and EndTime parameters, data within the specified time range is queried. You must set both parameters or leave both of them empty.
-        *   You can specify multiple domain names (no more than 20) and separate them with commas (,).
-        *   You can query data within the last 30 days.
-        *   The maximum number of times that each user can call this operation per second is 50.
+        If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range. You must set both parameters or leave both parameters empty.
+        *   You can specify up to 20 domain names in reach request. If you specify multiple domain names, separate them with commas (,).
+        *   You can query data collected over the last 30 days.
+        *   You can call this operation up to 50 times per second per account.
         
         @param request: DescribeDomainCcActivityLogRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainCcActivityLogResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6491,48 +6601,48 @@
         )
 
     def describe_domain_cc_activity_log(
         self,
         request: cdn_20180510_models.DescribeDomainCcActivityLogRequest,
     ) -> cdn_20180510_models.DescribeDomainCcActivityLogResponse:
         """
-        >    If you do not set the StartTime or EndTime parameter, data within the last 24 hours is queried. If you set both the StartTime and EndTime parameters, data within the specified time range is queried. You must set both parameters or leave both of them empty.
-        *   You can specify multiple domain names (no more than 20) and separate them with commas (,).
-        *   You can query data within the last 30 days.
-        *   The maximum number of times that each user can call this operation per second is 50.
+        If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range. You must set both parameters or leave both parameters empty.
+        *   You can specify up to 20 domain names in reach request. If you specify multiple domain names, separate them with commas (,).
+        *   You can query data collected over the last 30 days.
+        *   You can call this operation up to 50 times per second per account.
         
         @param request: DescribeDomainCcActivityLogRequest
         @return: DescribeDomainCcActivityLogResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_cc_activity_log_with_options(request, runtime)
 
     async def describe_domain_cc_activity_log_async(
         self,
         request: cdn_20180510_models.DescribeDomainCcActivityLogRequest,
     ) -> cdn_20180510_models.DescribeDomainCcActivityLogResponse:
         """
-        >    If you do not set the StartTime or EndTime parameter, data within the last 24 hours is queried. If you set both the StartTime and EndTime parameters, data within the specified time range is queried. You must set both parameters or leave both of them empty.
-        *   You can specify multiple domain names (no more than 20) and separate them with commas (,).
-        *   You can query data within the last 30 days.
-        *   The maximum number of times that each user can call this operation per second is 50.
+        If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range. You must set both parameters or leave both parameters empty.
+        *   You can specify up to 20 domain names in reach request. If you specify multiple domain names, separate them with commas (,).
+        *   You can query data collected over the last 30 days.
+        *   You can call this operation up to 50 times per second per account.
         
         @param request: DescribeDomainCcActivityLogRequest
         @return: DescribeDomainCcActivityLogResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_cc_activity_log_with_options_async(request, runtime)
 
     def describe_domain_certificate_info_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainCertificateInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainCertificateInfoResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: DescribeDomainCertificateInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainCertificateInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6559,15 +6669,15 @@
 
     async def describe_domain_certificate_info_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainCertificateInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainCertificateInfoResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: DescribeDomainCertificateInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainCertificateInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6593,28 +6703,28 @@
         )
 
     def describe_domain_certificate_info(
         self,
         request: cdn_20180510_models.DescribeDomainCertificateInfoRequest,
     ) -> cdn_20180510_models.DescribeDomainCertificateInfoResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: DescribeDomainCertificateInfoRequest
         @return: DescribeDomainCertificateInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_certificate_info_with_options(request, runtime)
 
     async def describe_domain_certificate_info_async(
         self,
         request: cdn_20180510_models.DescribeDomainCertificateInfoRequest,
     ) -> cdn_20180510_models.DescribeDomainCertificateInfoResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: DescribeDomainCertificateInfoRequest
         @return: DescribeDomainCertificateInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_certificate_info_with_options_async(request, runtime)
 
@@ -6782,23 +6892,15 @@
 
     def describe_domain_detail_data_by_layer_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainDetailDataByLayerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainDetailDataByLayerResponse:
         """
-        - You can call this operation up to 20 times per second per account.
-        - If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The following table describes the time granularity, the time period within which historical data is available, and the data delay, which vary with the maximum time range per query.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 days | 366 days | 366 days | 04:00 on the next day |
+        The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         
         @param request: DescribeDomainDetailDataByLayerRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainDetailDataByLayerResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -6823,23 +6925,15 @@
 
     async def describe_domain_detail_data_by_layer_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainDetailDataByLayerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainDetailDataByLayerResponse:
         """
-        - You can call this operation up to 20 times per second per account.
-        - If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The following table describes the time granularity, the time period within which historical data is available, and the data delay, which vary with the maximum time range per query.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 days | 366 days | 366 days | 04:00 on the next day |
+        The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         
         @param request: DescribeDomainDetailDataByLayerRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainDetailDataByLayerResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -6863,66 +6957,42 @@
         )
 
     def describe_domain_detail_data_by_layer(
         self,
         request: cdn_20180510_models.DescribeDomainDetailDataByLayerRequest,
     ) -> cdn_20180510_models.DescribeDomainDetailDataByLayerResponse:
         """
-        - You can call this operation up to 20 times per second per account.
-        - If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The following table describes the time granularity, the time period within which historical data is available, and the data delay, which vary with the maximum time range per query.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 days | 366 days | 366 days | 04:00 on the next day |
+        The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         
         @param request: DescribeDomainDetailDataByLayerRequest
         @return: DescribeDomainDetailDataByLayerResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_detail_data_by_layer_with_options(request, runtime)
 
     async def describe_domain_detail_data_by_layer_async(
         self,
         request: cdn_20180510_models.DescribeDomainDetailDataByLayerRequest,
     ) -> cdn_20180510_models.DescribeDomainDetailDataByLayerResponse:
         """
-        - You can call this operation up to 20 times per second per account.
-        - If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The following table describes the time granularity, the time period within which historical data is available, and the data delay, which vary with the maximum time range per query.
-        | Time granularity | Maximum time range per query | Historical data available | Data delay |
-        | ---------------- | ---------------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 days | 366 days | 366 days | 04:00 on the next day |
+        The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         
         @param request: DescribeDomainDetailDataByLayerRequest
         @return: DescribeDomainDetailDataByLayerResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_detail_data_by_layer_with_options_async(request, runtime)
 
     def describe_domain_hit_rate_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainHitRateDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainHitRateDataResponse:
         """
-        You can call this operation up to 100 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        The byte hit ratio of HTTPS requests.
         
         @param request: DescribeDomainHitRateDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainHitRateDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6955,23 +7025,15 @@
 
     async def describe_domain_hit_rate_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainHitRateDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainHitRateDataResponse:
         """
-        You can call this operation up to 100 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        The byte hit ratio of HTTPS requests.
         
         @param request: DescribeDomainHitRateDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainHitRateDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7003,66 +7065,50 @@
         )
 
     def describe_domain_hit_rate_data(
         self,
         request: cdn_20180510_models.DescribeDomainHitRateDataRequest,
     ) -> cdn_20180510_models.DescribeDomainHitRateDataResponse:
         """
-        You can call this operation up to 100 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        The byte hit ratio of HTTPS requests.
         
         @param request: DescribeDomainHitRateDataRequest
         @return: DescribeDomainHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_hit_rate_data_with_options(request, runtime)
 
     async def describe_domain_hit_rate_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainHitRateDataRequest,
     ) -> cdn_20180510_models.DescribeDomainHitRateDataResponse:
         """
-        You can call this operation up to 100 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
-        |1 day|366 days|366 days|04:00 on the next day|
+        The byte hit ratio of HTTPS requests.
         
         @param request: DescribeDomainHitRateDataRequest
         @return: DescribeDomainHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_hit_rate_data_with_options_async(request, runtime)
 
     def describe_domain_http_code_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7099,23 +7145,23 @@
 
     async def describe_domain_http_code_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7151,44 +7197,44 @@
         )
 
     def describe_domain_http_code_data(
         self,
         request: cdn_20180510_models.DescribeDomainHttpCodeDataRequest,
     ) -> cdn_20180510_models.DescribeDomainHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainHttpCodeDataRequest
         @return: DescribeDomainHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_http_code_data_with_options(request, runtime)
 
     async def describe_domain_http_code_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainHttpCodeDataRequest,
     ) -> cdn_20180510_models.DescribeDomainHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainHttpCodeDataRequest
         @return: DescribeDomainHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_http_code_data_with_options_async(request, runtime)
 
@@ -7346,18 +7392,15 @@
 
     def describe_domain_ispdata_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainISPDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainISPDataResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - This operation queries proportions of data usage of different ISPs only for a specific accelerated domain name, or for all accelerated domain names that belong your Alibaba Cloud account.
-        - You can call this operation up to 100 times per second per account.
+        The end of the time range that was queried.
         
         @param request: DescribeDomainISPDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainISPDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7388,18 +7431,15 @@
 
     async def describe_domain_ispdata_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainISPDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainISPDataResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - This operation queries proportions of data usage of different ISPs only for a specific accelerated domain name, or for all accelerated domain names that belong your Alibaba Cloud account.
-        - You can call this operation up to 100 times per second per account.
+        The end of the time range that was queried.
         
         @param request: DescribeDomainISPDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainISPDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7429,34 +7469,28 @@
         )
 
     def describe_domain_ispdata(
         self,
         request: cdn_20180510_models.DescribeDomainISPDataRequest,
     ) -> cdn_20180510_models.DescribeDomainISPDataResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - This operation queries proportions of data usage of different ISPs only for a specific accelerated domain name, or for all accelerated domain names that belong your Alibaba Cloud account.
-        - You can call this operation up to 100 times per second per account.
+        The end of the time range that was queried.
         
         @param request: DescribeDomainISPDataRequest
         @return: DescribeDomainISPDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_ispdata_with_options(request, runtime)
 
     async def describe_domain_ispdata_async(
         self,
         request: cdn_20180510_models.DescribeDomainISPDataRequest,
     ) -> cdn_20180510_models.DescribeDomainISPDataResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - This operation queries proportions of data usage of different ISPs only for a specific accelerated domain name, or for all accelerated domain names that belong your Alibaba Cloud account.
-        - You can call this operation up to 100 times per second per account.
+        The end of the time range that was queried.
         
         @param request: DescribeDomainISPDataRequest
         @return: DescribeDomainISPDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_ispdata_with_options_async(request, runtime)
 
@@ -7590,19 +7624,15 @@
 
     def describe_domain_multi_usage_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainMultiUsageDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainMultiUsageDataResponse:
         """
-        >    If you do not set StartTime or EndTime, data collected within the last 10 minutes is queried.
-        *   The maximum time range between StartTime and EndTime can be 1 hour.
-        *   You can query data within the last 90 days.
-        *   You can query the amount of data transfer and the number of requests for accelerated domain names that have been already removed from Alibaba Cloud CDN.
-        *   The maximum number of times that each user can call this operation per second is 50.
+        The end of the time range that was queried.
         
         @param request: DescribeDomainMultiUsageDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainMultiUsageDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7633,19 +7663,15 @@
 
     async def describe_domain_multi_usage_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainMultiUsageDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainMultiUsageDataResponse:
         """
-        >    If you do not set StartTime or EndTime, data collected within the last 10 minutes is queried.
-        *   The maximum time range between StartTime and EndTime can be 1 hour.
-        *   You can query data within the last 90 days.
-        *   You can query the amount of data transfer and the number of requests for accelerated domain names that have been already removed from Alibaba Cloud CDN.
-        *   The maximum number of times that each user can call this operation per second is 50.
+        The end of the time range that was queried.
         
         @param request: DescribeDomainMultiUsageDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainMultiUsageDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7675,36 +7701,28 @@
         )
 
     def describe_domain_multi_usage_data(
         self,
         request: cdn_20180510_models.DescribeDomainMultiUsageDataRequest,
     ) -> cdn_20180510_models.DescribeDomainMultiUsageDataResponse:
         """
-        >    If you do not set StartTime or EndTime, data collected within the last 10 minutes is queried.
-        *   The maximum time range between StartTime and EndTime can be 1 hour.
-        *   You can query data within the last 90 days.
-        *   You can query the amount of data transfer and the number of requests for accelerated domain names that have been already removed from Alibaba Cloud CDN.
-        *   The maximum number of times that each user can call this operation per second is 50.
+        The end of the time range that was queried.
         
         @param request: DescribeDomainMultiUsageDataRequest
         @return: DescribeDomainMultiUsageDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_multi_usage_data_with_options(request, runtime)
 
     async def describe_domain_multi_usage_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainMultiUsageDataRequest,
     ) -> cdn_20180510_models.DescribeDomainMultiUsageDataResponse:
         """
-        >    If you do not set StartTime or EndTime, data collected within the last 10 minutes is queried.
-        *   The maximum time range between StartTime and EndTime can be 1 hour.
-        *   You can query data within the last 90 days.
-        *   You can query the amount of data transfer and the number of requests for accelerated domain names that have been already removed from Alibaba Cloud CDN.
-        *   The maximum number of times that each user can call this operation per second is 50.
+        The end of the time range that was queried.
         
         @param request: DescribeDomainMultiUsageDataRequest
         @return: DescribeDomainMultiUsageDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_multi_usage_data_with_options_async(request, runtime)
 
@@ -7826,17 +7844,15 @@
 
     def describe_domain_pv_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainPvDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainPvDataResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, monitoring data within the last 24 hours is queried. If you set both StartTime and EndTime, monitoring data within the specified time range is queried.
-        - You can call this operation up to 50 times per second per account.
+        The end of the time range during which data was queried.
         
         @param request: DescribeDomainPvDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainPvDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7867,17 +7883,15 @@
 
     async def describe_domain_pv_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainPvDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainPvDataResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, monitoring data within the last 24 hours is queried. If you set both StartTime and EndTime, monitoring data within the specified time range is queried.
-        - You can call this operation up to 50 times per second per account.
+        The end of the time range during which data was queried.
         
         @param request: DescribeDomainPvDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainPvDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7907,32 +7921,28 @@
         )
 
     def describe_domain_pv_data(
         self,
         request: cdn_20180510_models.DescribeDomainPvDataRequest,
     ) -> cdn_20180510_models.DescribeDomainPvDataResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, monitoring data within the last 24 hours is queried. If you set both StartTime and EndTime, monitoring data within the specified time range is queried.
-        - You can call this operation up to 50 times per second per account.
+        The end of the time range during which data was queried.
         
         @param request: DescribeDomainPvDataRequest
         @return: DescribeDomainPvDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_pv_data_with_options(request, runtime)
 
     async def describe_domain_pv_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainPvDataRequest,
     ) -> cdn_20180510_models.DescribeDomainPvDataResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, monitoring data within the last 24 hours is queried. If you set both StartTime and EndTime, monitoring data within the specified time range is queried.
-        - You can call this operation up to 50 times per second per account.
+        The end of the time range during which data was queried.
         
         @param request: DescribeDomainPvDataRequest
         @return: DescribeDomainPvDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_pv_data_with_options_async(request, runtime)
 
@@ -8486,16 +8496,16 @@
 
     def describe_domain_real_time_detail_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeDetailDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeDetailDataResponse:
         """
-        - You can query data within the last seven days. Data is collected every minute.
-        - The maximum number of times that each user can call this operation per second is 10.
+        The beginning of the time range to query.
+        Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. Example: 2019-11-30T05:33:00Z.
         
         @param request: DescribeDomainRealTimeDetailDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeDetailDataResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -8520,16 +8530,16 @@
 
     async def describe_domain_real_time_detail_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeDetailDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeDetailDataResponse:
         """
-        - You can query data within the last seven days. Data is collected every minute.
-        - The maximum number of times that each user can call this operation per second is 10.
+        The beginning of the time range to query.
+        Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. Example: 2019-11-30T05:33:00Z.
         
         @param request: DescribeDomainRealTimeDetailDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeDetailDataResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -8553,52 +8563,44 @@
         )
 
     def describe_domain_real_time_detail_data(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeDetailDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeDetailDataResponse:
         """
-        - You can query data within the last seven days. Data is collected every minute.
-        - The maximum number of times that each user can call this operation per second is 10.
+        The beginning of the time range to query.
+        Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. Example: 2019-11-30T05:33:00Z.
         
         @param request: DescribeDomainRealTimeDetailDataRequest
         @return: DescribeDomainRealTimeDetailDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_detail_data_with_options(request, runtime)
 
     async def describe_domain_real_time_detail_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeDetailDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeDetailDataResponse:
         """
-        - You can query data within the last seven days. Data is collected every minute.
-        - The maximum number of times that each user can call this operation per second is 10.
+        The beginning of the time range to query.
+        Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. Example: 2019-11-30T05:33:00Z.
         
         @param request: DescribeDomainRealTimeDetailDataRequest
         @return: DescribeDomainRealTimeDetailDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_real_time_detail_data_with_options_async(request, runtime)
 
     def describe_domain_real_time_http_code_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataResponse:
         """
-        You can call this operation up to 10 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The total number of entries.
         
         @param request: DescribeDomainRealTimeHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8633,23 +8635,15 @@
 
     async def describe_domain_real_time_http_code_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataResponse:
         """
-        You can call this operation up to 10 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The total number of entries.
         
         @param request: DescribeDomainRealTimeHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8683,44 +8677,28 @@
         )
 
     def describe_domain_real_time_http_code_data(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataResponse:
         """
-        You can call this operation up to 10 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The total number of entries.
         
         @param request: DescribeDomainRealTimeHttpCodeDataRequest
         @return: DescribeDomainRealTimeHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_http_code_data_with_options(request, runtime)
 
     async def describe_domain_real_time_http_code_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataResponse:
         """
-        You can call this operation up to 10 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The total number of entries.
         
         @param request: DescribeDomainRealTimeHttpCodeDataRequest
         @return: DescribeDomainRealTimeHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_real_time_http_code_data_with_options_async(request, runtime)
 
@@ -8850,25 +8828,15 @@
 
     def describe_domain_real_time_req_hit_rate_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeReqHitRateDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeReqHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - By default, requests in the Go programming language use the POST request method. You must manually change the request method to GET by declaring: request.Method="GET".
-        - The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the request hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 Days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        The ID of the request.
         
         @param request: DescribeDomainRealTimeReqHitRateDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeReqHitRateDataResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -8893,25 +8861,15 @@
 
     async def describe_domain_real_time_req_hit_rate_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeReqHitRateDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeReqHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - By default, requests in the Go programming language use the POST request method. You must manually change the request method to GET by declaring: request.Method="GET".
-        - The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the request hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 Days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        The ID of the request.
         
         @param request: DescribeDomainRealTimeReqHitRateDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeReqHitRateDataResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -8935,70 +8893,42 @@
         )
 
     def describe_domain_real_time_req_hit_rate_data(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeReqHitRateDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeReqHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - By default, requests in the Go programming language use the POST request method. You must manually change the request method to GET by declaring: request.Method="GET".
-        - The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the request hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 Days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        The ID of the request.
         
         @param request: DescribeDomainRealTimeReqHitRateDataRequest
         @return: DescribeDomainRealTimeReqHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_req_hit_rate_data_with_options(request, runtime)
 
     async def describe_domain_real_time_req_hit_rate_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeReqHitRateDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeReqHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - By default, requests in the Go programming language use the POST request method. You must manually change the request method to GET by declaring: request.Method="GET".
-        - The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the request hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 Days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        The ID of the request.
         
         @param request: DescribeDomainRealTimeReqHitRateDataRequest
         @return: DescribeDomainRealTimeReqHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_real_time_req_hit_rate_data_with_options_async(request, runtime)
 
     def describe_domain_real_time_src_bps_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataResponse:
         """
-        You can call this operation up to 10 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The timestamp of the returned data.
         
         @param request: DescribeDomainRealTimeSrcBpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeSrcBpsDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9029,23 +8959,15 @@
 
     async def describe_domain_real_time_src_bps_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataResponse:
         """
-        You can call this operation up to 10 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The timestamp of the returned data.
         
         @param request: DescribeDomainRealTimeSrcBpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeSrcBpsDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9075,66 +8997,42 @@
         )
 
     def describe_domain_real_time_src_bps_data(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataResponse:
         """
-        You can call this operation up to 10 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The timestamp of the returned data.
         
         @param request: DescribeDomainRealTimeSrcBpsDataRequest
         @return: DescribeDomainRealTimeSrcBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_src_bps_data_with_options(request, runtime)
 
     async def describe_domain_real_time_src_bps_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataResponse:
         """
-        You can call this operation up to 10 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The timestamp of the returned data.
         
         @param request: DescribeDomainRealTimeSrcBpsDataRequest
         @return: DescribeDomainRealTimeSrcBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_real_time_src_bps_data_with_options_async(request, runtime)
 
     def describe_domain_real_time_src_http_code_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataResponse:
         """
-        You can call this operation up to 10 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The count of each HTTP status code.
         
         @param request: DescribeDomainRealTimeSrcHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeSrcHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9169,23 +9067,15 @@
 
     async def describe_domain_real_time_src_http_code_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataResponse:
         """
-        You can call this operation up to 10 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The count of each HTTP status code.
         
         @param request: DescribeDomainRealTimeSrcHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeSrcHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9219,44 +9109,28 @@
         )
 
     def describe_domain_real_time_src_http_code_data(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataResponse:
         """
-        You can call this operation up to 10 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The count of each HTTP status code.
         
         @param request: DescribeDomainRealTimeSrcHttpCodeDataRequest
         @return: DescribeDomainRealTimeSrcHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_src_http_code_data_with_options(request, runtime)
 
     async def describe_domain_real_time_src_http_code_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataResponse:
         """
-        You can call this operation up to 10 times per second per account.
-        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        |Time granularity|Maximum time range per query|Historical data available|Data delay|
-        |---|---|---|---|
-        |1 minute|1 hour|7 days|5 minutes|
-        |5 minutes|3 days|93 days|15 minutes|
-        |1 hour|31 days|186 days|4 hours|
+        The count of each HTTP status code.
         
         @param request: DescribeDomainRealTimeSrcHttpCodeDataRequest
         @return: DescribeDomainRealTimeSrcHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_real_time_src_http_code_data_with_options_async(request, runtime)
 
@@ -9542,15 +9416,15 @@
 
     def describe_domain_realtime_log_delivery_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainRealtimeLogDeliveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealtimeLogDeliveryResponse:
         """
-        > You can call this operation up to 100 times per second per account.
+        The name of the Log Service project that is used for real-time log delivery.
         
         @param request: DescribeDomainRealtimeLogDeliveryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealtimeLogDeliveryResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -9575,15 +9449,15 @@
 
     async def describe_domain_realtime_log_delivery_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealtimeLogDeliveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealtimeLogDeliveryResponse:
         """
-        > You can call this operation up to 100 times per second per account.
+        The name of the Log Service project that is used for real-time log delivery.
         
         @param request: DescribeDomainRealtimeLogDeliveryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealtimeLogDeliveryResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -9607,45 +9481,42 @@
         )
 
     def describe_domain_realtime_log_delivery(
         self,
         request: cdn_20180510_models.DescribeDomainRealtimeLogDeliveryRequest,
     ) -> cdn_20180510_models.DescribeDomainRealtimeLogDeliveryResponse:
         """
-        > You can call this operation up to 100 times per second per account.
+        The name of the Log Service project that is used for real-time log delivery.
         
         @param request: DescribeDomainRealtimeLogDeliveryRequest
         @return: DescribeDomainRealtimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_realtime_log_delivery_with_options(request, runtime)
 
     async def describe_domain_realtime_log_delivery_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealtimeLogDeliveryRequest,
     ) -> cdn_20180510_models.DescribeDomainRealtimeLogDeliveryResponse:
         """
-        > You can call this operation up to 100 times per second per account.
+        The name of the Log Service project that is used for real-time log delivery.
         
         @param request: DescribeDomainRealtimeLogDeliveryRequest
         @return: DescribeDomainRealtimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_realtime_log_delivery_with_options_async(request, runtime)
 
     def describe_domain_region_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainRegionDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRegionDataResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set **StartTime** or **EndTime**, data collected within the last **24** hours is queried. If you set both **StartTime** and **EndTime**, data collected within the specified time range is queried.
-        - You may fail to query the latest data. If you need to query data collected within the last day, we recommend that you query the data on the next day.
-        - You can call this operation up to 100 times per second per account.
+        The beginning of the time range that was queried.
         
         @param request: DescribeDomainRegionDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRegionDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9676,18 +9547,15 @@
 
     async def describe_domain_region_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainRegionDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRegionDataResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set **StartTime** or **EndTime**, data collected within the last **24** hours is queried. If you set both **StartTime** and **EndTime**, data collected within the specified time range is queried.
-        - You may fail to query the latest data. If you need to query data collected within the last day, we recommend that you query the data on the next day.
-        - You can call this operation up to 100 times per second per account.
+        The beginning of the time range that was queried.
         
         @param request: DescribeDomainRegionDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRegionDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9717,34 +9585,28 @@
         )
 
     def describe_domain_region_data(
         self,
         request: cdn_20180510_models.DescribeDomainRegionDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRegionDataResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set **StartTime** or **EndTime**, data collected within the last **24** hours is queried. If you set both **StartTime** and **EndTime**, data collected within the specified time range is queried.
-        - You may fail to query the latest data. If you need to query data collected within the last day, we recommend that you query the data on the next day.
-        - You can call this operation up to 100 times per second per account.
+        The beginning of the time range that was queried.
         
         @param request: DescribeDomainRegionDataRequest
         @return: DescribeDomainRegionDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_region_data_with_options(request, runtime)
 
     async def describe_domain_region_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainRegionDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRegionDataResponse:
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set **StartTime** or **EndTime**, data collected within the last **24** hours is queried. If you set both **StartTime** and **EndTime**, data collected within the specified time range is queried.
-        - You may fail to query the latest data. If you need to query data collected within the last day, we recommend that you query the data on the next day.
-        - You can call this operation up to 100 times per second per account.
+        The beginning of the time range that was queried.
         
         @param request: DescribeDomainRegionDataRequest
         @return: DescribeDomainRegionDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_region_data_with_options_async(request, runtime)
 
@@ -10566,18 +10428,16 @@
 
     def describe_domain_top_client_ip_visit_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainTopClientIpVisitRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainTopClientIpVisitResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - Data is collected every hour.
-        - You can call this operation up to 10 times per second per account.
+        The name of the region. Separate multiple region names with commas (,).
+        You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         
         @param request: DescribeDomainTopClientIpVisitRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainTopClientIpVisitResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10614,18 +10474,16 @@
 
     async def describe_domain_top_client_ip_visit_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainTopClientIpVisitRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainTopClientIpVisitResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - Data is collected every hour.
-        - You can call this operation up to 10 times per second per account.
+        The name of the region. Separate multiple region names with commas (,).
+        You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         
         @param request: DescribeDomainTopClientIpVisitRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainTopClientIpVisitResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10661,51 +10519,46 @@
         )
 
     def describe_domain_top_client_ip_visit(
         self,
         request: cdn_20180510_models.DescribeDomainTopClientIpVisitRequest,
     ) -> cdn_20180510_models.DescribeDomainTopClientIpVisitResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - Data is collected every hour.
-        - You can call this operation up to 10 times per second per account.
+        The name of the region. Separate multiple region names with commas (,).
+        You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         
         @param request: DescribeDomainTopClientIpVisitRequest
         @return: DescribeDomainTopClientIpVisitResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_top_client_ip_visit_with_options(request, runtime)
 
     async def describe_domain_top_client_ip_visit_async(
         self,
         request: cdn_20180510_models.DescribeDomainTopClientIpVisitRequest,
     ) -> cdn_20180510_models.DescribeDomainTopClientIpVisitResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - Data is collected every hour.
-        - You can call this operation up to 10 times per second per account.
+        The name of the region. Separate multiple region names with commas (,).
+        You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         
         @param request: DescribeDomainTopClientIpVisitRequest
         @return: DescribeDomainTopClientIpVisitResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_top_client_ip_visit_with_options_async(request, runtime)
 
     def describe_domain_top_refer_visit_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainTopReferVisitRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainTopReferVisitResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to analyze data.
-        > - If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
-        - Data is collected at an interval of five minutes.
-        - You can call this operation up to 10 times per second per account.
+        The sorting method. Valid values:
+        *   **traf**: by network traffic.
+        *   **pv**: by the number of page views. This is the default value.
         
         @param request: DescribeDomainTopReferVisitRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainTopReferVisitResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10738,18 +10591,17 @@
 
     async def describe_domain_top_refer_visit_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainTopReferVisitRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainTopReferVisitResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to analyze data.
-        > - If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
-        - Data is collected at an interval of five minutes.
-        - You can call this operation up to 10 times per second per account.
+        The sorting method. Valid values:
+        *   **traf**: by network traffic.
+        *   **pv**: by the number of page views. This is the default value.
         
         @param request: DescribeDomainTopReferVisitRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainTopReferVisitResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10781,34 +10633,32 @@
         )
 
     def describe_domain_top_refer_visit(
         self,
         request: cdn_20180510_models.DescribeDomainTopReferVisitRequest,
     ) -> cdn_20180510_models.DescribeDomainTopReferVisitResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to analyze data.
-        > - If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
-        - Data is collected at an interval of five minutes.
-        - You can call this operation up to 10 times per second per account.
+        The sorting method. Valid values:
+        *   **traf**: by network traffic.
+        *   **pv**: by the number of page views. This is the default value.
         
         @param request: DescribeDomainTopReferVisitRequest
         @return: DescribeDomainTopReferVisitResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_top_refer_visit_with_options(request, runtime)
 
     async def describe_domain_top_refer_visit_async(
         self,
         request: cdn_20180510_models.DescribeDomainTopReferVisitRequest,
     ) -> cdn_20180510_models.DescribeDomainTopReferVisitResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to analyze data.
-        > - If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
-        - Data is collected at an interval of five minutes.
-        - You can call this operation up to 10 times per second per account.
+        The sorting method. Valid values:
+        *   **traf**: by network traffic.
+        *   **pv**: by the number of page views. This is the default value.
         
         @param request: DescribeDomainTopReferVisitRequest
         @return: DescribeDomainTopReferVisitResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_top_refer_visit_with_options_async(request, runtime)
 
@@ -11091,15 +10941,15 @@
     def describe_domain_usage_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainUsageDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainUsageDataResponse:
         """
         You can call this operation up to 10 times per second per account.
-        * The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        * The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
         |Time granularity|Maximum time range per query|Historical data available|Data delay|
         |---|---|---|---|
         |5 minutes|3 days|93 days|15 minutes|
         |1 hour|31 days|186 days|4 hours|
         |1 day|90 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainUsageDataRequest
@@ -11146,15 +10996,15 @@
     async def describe_domain_usage_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainUsageDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainUsageDataResponse:
         """
         You can call this operation up to 10 times per second per account.
-        * The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        * The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
         |Time granularity|Maximum time range per query|Historical data available|Data delay|
         |---|---|---|---|
         |5 minutes|3 days|93 days|15 minutes|
         |1 hour|31 days|186 days|4 hours|
         |1 day|90 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainUsageDataRequest
@@ -11200,15 +11050,15 @@
 
     def describe_domain_usage_data(
         self,
         request: cdn_20180510_models.DescribeDomainUsageDataRequest,
     ) -> cdn_20180510_models.DescribeDomainUsageDataResponse:
         """
         You can call this operation up to 10 times per second per account.
-        * The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        * The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
         |Time granularity|Maximum time range per query|Historical data available|Data delay|
         |---|---|---|---|
         |5 minutes|3 days|93 days|15 minutes|
         |1 hour|31 days|186 days|4 hours|
         |1 day|90 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainUsageDataRequest
@@ -11219,15 +11069,15 @@
 
     async def describe_domain_usage_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainUsageDataRequest,
     ) -> cdn_20180510_models.DescribeDomainUsageDataResponse:
         """
         You can call this operation up to 10 times per second per account.
-        * The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        * The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
         |Time granularity|Maximum time range per query|Historical data available|Data delay|
         |---|---|---|---|
         |5 minutes|3 days|93 days|15 minutes|
         |1 hour|31 days|186 days|4 hours|
         |1 day|90 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainUsageDataRequest
@@ -11358,15 +11208,15 @@
 
     def describe_domains_by_source_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainsBySourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainsBySourceResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDomainsBySourceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainsBySourceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11397,15 +11247,15 @@
 
     async def describe_domains_by_source_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainsBySourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainsBySourceResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDomainsBySourceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainsBySourceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11435,28 +11285,28 @@
         )
 
     def describe_domains_by_source(
         self,
         request: cdn_20180510_models.DescribeDomainsBySourceRequest,
     ) -> cdn_20180510_models.DescribeDomainsBySourceResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDomainsBySourceRequest
         @return: DescribeDomainsBySourceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domains_by_source_with_options(request, runtime)
 
     async def describe_domains_by_source_async(
         self,
         request: cdn_20180510_models.DescribeDomainsBySourceRequest,
     ) -> cdn_20180510_models.DescribeDomainsBySourceResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDomainsBySourceRequest
         @return: DescribeDomainsBySourceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domains_by_source_with_options_async(request, runtime)
 
@@ -11574,15 +11424,15 @@
 
     def describe_es_exception_data_with_options(
         self,
         request: cdn_20180510_models.DescribeEsExceptionDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeEsExceptionDataResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        You can call this operation up to 30 times per second per account.
         
         @param request: DescribeEsExceptionDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeEsExceptionDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11613,15 +11463,15 @@
 
     async def describe_es_exception_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeEsExceptionDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeEsExceptionDataResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        You can call this operation up to 30 times per second per account.
         
         @param request: DescribeEsExceptionDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeEsExceptionDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11651,42 +11501,42 @@
         )
 
     def describe_es_exception_data(
         self,
         request: cdn_20180510_models.DescribeEsExceptionDataRequest,
     ) -> cdn_20180510_models.DescribeEsExceptionDataResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        You can call this operation up to 30 times per second per account.
         
         @param request: DescribeEsExceptionDataRequest
         @return: DescribeEsExceptionDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_es_exception_data_with_options(request, runtime)
 
     async def describe_es_exception_data_async(
         self,
         request: cdn_20180510_models.DescribeEsExceptionDataRequest,
     ) -> cdn_20180510_models.DescribeEsExceptionDataResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        You can call this operation up to 30 times per second per account.
         
         @param request: DescribeEsExceptionDataRequest
         @return: DescribeEsExceptionDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_es_exception_data_with_options_async(request, runtime)
 
     def describe_es_execute_data_with_options(
         self,
         request: cdn_20180510_models.DescribeEsExecuteDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeEsExecuteDataResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        You can call this operation up to 30 times per second per account.
         
         @param request: DescribeEsExecuteDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeEsExecuteDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11717,15 +11567,15 @@
 
     async def describe_es_execute_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeEsExecuteDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeEsExecuteDataResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        You can call this operation up to 30 times per second per account.
         
         @param request: DescribeEsExecuteDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeEsExecuteDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11755,28 +11605,28 @@
         )
 
     def describe_es_execute_data(
         self,
         request: cdn_20180510_models.DescribeEsExecuteDataRequest,
     ) -> cdn_20180510_models.DescribeEsExecuteDataResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        You can call this operation up to 30 times per second per account.
         
         @param request: DescribeEsExecuteDataRequest
         @return: DescribeEsExecuteDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_es_execute_data_with_options(request, runtime)
 
     async def describe_es_execute_data_async(
         self,
         request: cdn_20180510_models.DescribeEsExecuteDataRequest,
     ) -> cdn_20180510_models.DescribeEsExecuteDataResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        You can call this operation up to 30 times per second per account.
         
         @param request: DescribeEsExecuteDataRequest
         @return: DescribeEsExecuteDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_es_execute_data_with_options_async(request, runtime)
 
@@ -11848,16 +11698,15 @@
 
     def describe_illegal_url_export_task_with_options(
         self,
         request: cdn_20180510_models.DescribeIllegalUrlExportTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeIllegalUrlExportTaskResponse:
         """
-        >    Invalid URLs are exported to a CSV file.
-        *   The maximum number of times that each user can call this operation per second is 1.
+        The URL where you can download the file that contains invalid URLs. This parameter is valid only if the export task is successful.
         
         @param request: DescribeIllegalUrlExportTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeIllegalUrlExportTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11884,16 +11733,15 @@
 
     async def describe_illegal_url_export_task_with_options_async(
         self,
         request: cdn_20180510_models.DescribeIllegalUrlExportTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeIllegalUrlExportTaskResponse:
         """
-        >    Invalid URLs are exported to a CSV file.
-        *   The maximum number of times that each user can call this operation per second is 1.
+        The URL where you can download the file that contains invalid URLs. This parameter is valid only if the export task is successful.
         
         @param request: DescribeIllegalUrlExportTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeIllegalUrlExportTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11919,44 +11767,42 @@
         )
 
     def describe_illegal_url_export_task(
         self,
         request: cdn_20180510_models.DescribeIllegalUrlExportTaskRequest,
     ) -> cdn_20180510_models.DescribeIllegalUrlExportTaskResponse:
         """
-        >    Invalid URLs are exported to a CSV file.
-        *   The maximum number of times that each user can call this operation per second is 1.
+        The URL where you can download the file that contains invalid URLs. This parameter is valid only if the export task is successful.
         
         @param request: DescribeIllegalUrlExportTaskRequest
         @return: DescribeIllegalUrlExportTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_illegal_url_export_task_with_options(request, runtime)
 
     async def describe_illegal_url_export_task_async(
         self,
         request: cdn_20180510_models.DescribeIllegalUrlExportTaskRequest,
     ) -> cdn_20180510_models.DescribeIllegalUrlExportTaskResponse:
         """
-        >    Invalid URLs are exported to a CSV file.
-        *   The maximum number of times that each user can call this operation per second is 1.
+        The URL where you can download the file that contains invalid URLs. This parameter is valid only if the export task is successful.
         
         @param request: DescribeIllegalUrlExportTaskRequest
         @return: DescribeIllegalUrlExportTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_illegal_url_export_task_with_options_async(request, runtime)
 
     def describe_ip_info_with_options(
         self,
         request: cdn_20180510_models.DescribeIpInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeIpInfoResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeIpInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeIpInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11983,15 +11829,15 @@
 
     async def describe_ip_info_with_options_async(
         self,
         request: cdn_20180510_models.DescribeIpInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeIpInfoResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeIpInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeIpInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12017,42 +11863,42 @@
         )
 
     def describe_ip_info(
         self,
         request: cdn_20180510_models.DescribeIpInfoRequest,
     ) -> cdn_20180510_models.DescribeIpInfoResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeIpInfoRequest
         @return: DescribeIpInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_ip_info_with_options(request, runtime)
 
     async def describe_ip_info_async(
         self,
         request: cdn_20180510_models.DescribeIpInfoRequest,
     ) -> cdn_20180510_models.DescribeIpInfoResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeIpInfoRequest
         @return: DescribeIpInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_ip_info_with_options_async(request, runtime)
 
     def describe_ip_status_with_options(
         self,
         request: cdn_20180510_models.DescribeIpStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeIpStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeIpStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeIpStatusResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -12077,15 +11923,15 @@
 
     async def describe_ip_status_with_options_async(
         self,
         request: cdn_20180510_models.DescribeIpStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeIpStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeIpStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeIpStatusResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -12109,28 +11955,28 @@
         )
 
     def describe_ip_status(
         self,
         request: cdn_20180510_models.DescribeIpStatusRequest,
     ) -> cdn_20180510_models.DescribeIpStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeIpStatusRequest
         @return: DescribeIpStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_ip_status_with_options(request, runtime)
 
     async def describe_ip_status_async(
         self,
         request: cdn_20180510_models.DescribeIpStatusRequest,
     ) -> cdn_20180510_models.DescribeIpStatusResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
         @param request: DescribeIpStatusRequest
         @return: DescribeIpStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_ip_status_with_options_async(request, runtime)
 
@@ -12430,15 +12276,15 @@
 
     def describe_realtime_delivery_acc_with_options(
         self,
         request: cdn_20180510_models.DescribeRealtimeDeliveryAccRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeRealtimeDeliveryAccResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeRealtimeDeliveryAccRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRealtimeDeliveryAccResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12473,15 +12319,15 @@
 
     async def describe_realtime_delivery_acc_with_options_async(
         self,
         request: cdn_20180510_models.DescribeRealtimeDeliveryAccRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeRealtimeDeliveryAccResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeRealtimeDeliveryAccRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRealtimeDeliveryAccResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12515,43 +12361,43 @@
         )
 
     def describe_realtime_delivery_acc(
         self,
         request: cdn_20180510_models.DescribeRealtimeDeliveryAccRequest,
     ) -> cdn_20180510_models.DescribeRealtimeDeliveryAccResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeRealtimeDeliveryAccRequest
         @return: DescribeRealtimeDeliveryAccResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_realtime_delivery_acc_with_options(request, runtime)
 
     async def describe_realtime_delivery_acc_async(
         self,
         request: cdn_20180510_models.DescribeRealtimeDeliveryAccRequest,
     ) -> cdn_20180510_models.DescribeRealtimeDeliveryAccResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeRealtimeDeliveryAccRequest
         @return: DescribeRealtimeDeliveryAccResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_realtime_delivery_acc_with_options_async(request, runtime)
 
     def describe_refresh_quota_with_options(
         self,
         request: cdn_20180510_models.DescribeRefreshQuotaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeRefreshQuotaResponse:
         """
-        > - You can call the RefreshObjectCaches operation to refresh content and call the PushObjectCache operation to prefetch content.
-        - The maximum number of times that each user can call this operation per second is 20.
+        You can call the [RefreshObjectCaches](~~448057~~) operation to refresh content and call the [PushObjectCache](~~448058~~) operation to prefetch content.
+        *   You can call this operation up to 20 times per second per account.
         
         @param request: DescribeRefreshQuotaRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRefreshQuotaResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12580,16 +12426,16 @@
 
     async def describe_refresh_quota_with_options_async(
         self,
         request: cdn_20180510_models.DescribeRefreshQuotaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeRefreshQuotaResponse:
         """
-        > - You can call the RefreshObjectCaches operation to refresh content and call the PushObjectCache operation to prefetch content.
-        - The maximum number of times that each user can call this operation per second is 20.
+        You can call the [RefreshObjectCaches](~~448057~~) operation to refresh content and call the [PushObjectCache](~~448058~~) operation to prefetch content.
+        *   You can call this operation up to 20 times per second per account.
         
         @param request: DescribeRefreshQuotaRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRefreshQuotaResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12617,45 +12463,44 @@
         )
 
     def describe_refresh_quota(
         self,
         request: cdn_20180510_models.DescribeRefreshQuotaRequest,
     ) -> cdn_20180510_models.DescribeRefreshQuotaResponse:
         """
-        > - You can call the RefreshObjectCaches operation to refresh content and call the PushObjectCache operation to prefetch content.
-        - The maximum number of times that each user can call this operation per second is 20.
+        You can call the [RefreshObjectCaches](~~448057~~) operation to refresh content and call the [PushObjectCache](~~448058~~) operation to prefetch content.
+        *   You can call this operation up to 20 times per second per account.
         
         @param request: DescribeRefreshQuotaRequest
         @return: DescribeRefreshQuotaResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_refresh_quota_with_options(request, runtime)
 
     async def describe_refresh_quota_async(
         self,
         request: cdn_20180510_models.DescribeRefreshQuotaRequest,
     ) -> cdn_20180510_models.DescribeRefreshQuotaResponse:
         """
-        > - You can call the RefreshObjectCaches operation to refresh content and call the PushObjectCache operation to prefetch content.
-        - The maximum number of times that each user can call this operation per second is 20.
+        You can call the [RefreshObjectCaches](~~448057~~) operation to refresh content and call the [PushObjectCache](~~448058~~) operation to prefetch content.
+        *   You can call this operation up to 20 times per second per account.
         
         @param request: DescribeRefreshQuotaRequest
         @return: DescribeRefreshQuotaResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_refresh_quota_with_options_async(request, runtime)
 
     def describe_refresh_task_by_id_with_options(
         self,
         request: cdn_20180510_models.DescribeRefreshTaskByIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeRefreshTaskByIdResponse:
         """
-        > - You can query data within the last three days.
-        - You can call this operation up to 30 times per second per account.
+        The tasks.
         
         @param request: DescribeRefreshTaskByIdRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRefreshTaskByIdResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12682,16 +12527,15 @@
 
     async def describe_refresh_task_by_id_with_options_async(
         self,
         request: cdn_20180510_models.DescribeRefreshTaskByIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeRefreshTaskByIdResponse:
         """
-        > - You can query data within the last three days.
-        - You can call this operation up to 30 times per second per account.
+        The tasks.
         
         @param request: DescribeRefreshTaskByIdRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRefreshTaskByIdResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12717,48 +12561,42 @@
         )
 
     def describe_refresh_task_by_id(
         self,
         request: cdn_20180510_models.DescribeRefreshTaskByIdRequest,
     ) -> cdn_20180510_models.DescribeRefreshTaskByIdResponse:
         """
-        > - You can query data within the last three days.
-        - You can call this operation up to 30 times per second per account.
+        The tasks.
         
         @param request: DescribeRefreshTaskByIdRequest
         @return: DescribeRefreshTaskByIdResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_refresh_task_by_id_with_options(request, runtime)
 
     async def describe_refresh_task_by_id_async(
         self,
         request: cdn_20180510_models.DescribeRefreshTaskByIdRequest,
     ) -> cdn_20180510_models.DescribeRefreshTaskByIdResponse:
         """
-        > - You can query data within the last three days.
-        - You can call this operation up to 30 times per second per account.
+        The tasks.
         
         @param request: DescribeRefreshTaskByIdRequest
         @return: DescribeRefreshTaskByIdResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_refresh_task_by_id_with_options_async(request, runtime)
 
     def describe_refresh_tasks_with_options(
         self,
         request: cdn_20180510_models.DescribeRefreshTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeRefreshTasksResponse:
         """
-        You can query the status of tasks by task ID or URL.
-        *   You can set both the **TaskId** and **ObjectPath** parameters. If you do not set the **TaskId** or **ObjectPath** parameter, data entries on the first page (20 entries) collected in the last 3 days are returned.
-        *   You can query data collected in the last 3 days.
-        *   If auto CDN cache update is enabled in the Object Storage Service (OSS) console, you cannot call the DescribeRefreshTasks operation to query automatic refresh tasks in OSS.
-        *   You can call this operation up to 10 times per second per account. If you want to query tasks at a higher frequency, call the [DescribeRefreshTaskById](~~187709~~) operation. This operation allows you to query tasks by task ID.
+        The ID of the task.
         
         @param request: DescribeRefreshTasksRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRefreshTasksResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12807,19 +12645,15 @@
 
     async def describe_refresh_tasks_with_options_async(
         self,
         request: cdn_20180510_models.DescribeRefreshTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeRefreshTasksResponse:
         """
-        You can query the status of tasks by task ID or URL.
-        *   You can set both the **TaskId** and **ObjectPath** parameters. If you do not set the **TaskId** or **ObjectPath** parameter, data entries on the first page (20 entries) collected in the last 3 days are returned.
-        *   You can query data collected in the last 3 days.
-        *   If auto CDN cache update is enabled in the Object Storage Service (OSS) console, you cannot call the DescribeRefreshTasks operation to query automatic refresh tasks in OSS.
-        *   You can call this operation up to 10 times per second per account. If you want to query tasks at a higher frequency, call the [DescribeRefreshTaskById](~~187709~~) operation. This operation allows you to query tasks by task ID.
+        The ID of the task.
         
         @param request: DescribeRefreshTasksRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRefreshTasksResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12867,36 +12701,28 @@
         )
 
     def describe_refresh_tasks(
         self,
         request: cdn_20180510_models.DescribeRefreshTasksRequest,
     ) -> cdn_20180510_models.DescribeRefreshTasksResponse:
         """
-        You can query the status of tasks by task ID or URL.
-        *   You can set both the **TaskId** and **ObjectPath** parameters. If you do not set the **TaskId** or **ObjectPath** parameter, data entries on the first page (20 entries) collected in the last 3 days are returned.
-        *   You can query data collected in the last 3 days.
-        *   If auto CDN cache update is enabled in the Object Storage Service (OSS) console, you cannot call the DescribeRefreshTasks operation to query automatic refresh tasks in OSS.
-        *   You can call this operation up to 10 times per second per account. If you want to query tasks at a higher frequency, call the [DescribeRefreshTaskById](~~187709~~) operation. This operation allows you to query tasks by task ID.
+        The ID of the task.
         
         @param request: DescribeRefreshTasksRequest
         @return: DescribeRefreshTasksResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_refresh_tasks_with_options(request, runtime)
 
     async def describe_refresh_tasks_async(
         self,
         request: cdn_20180510_models.DescribeRefreshTasksRequest,
     ) -> cdn_20180510_models.DescribeRefreshTasksResponse:
         """
-        You can query the status of tasks by task ID or URL.
-        *   You can set both the **TaskId** and **ObjectPath** parameters. If you do not set the **TaskId** or **ObjectPath** parameter, data entries on the first page (20 entries) collected in the last 3 days are returned.
-        *   You can query data collected in the last 3 days.
-        *   If auto CDN cache update is enabled in the Object Storage Service (OSS) console, you cannot call the DescribeRefreshTasks operation to query automatic refresh tasks in OSS.
-        *   You can call this operation up to 10 times per second per account. If you want to query tasks at a higher frequency, call the [DescribeRefreshTaskById](~~187709~~) operation. This operation allows you to query tasks by task ID.
+        The ID of the task.
         
         @param request: DescribeRefreshTasksRequest
         @return: DescribeRefreshTasksResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_refresh_tasks_with_options_async(request, runtime)
 
@@ -12975,21 +12801,14 @@
         return await self.describe_staging_ip_with_options_async(runtime)
 
     def describe_tag_resources_with_options(
         self,
         request: cdn_20180510_models.DescribeTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeTagResourcesResponse:
-        """
-        > You can call this operation up to 10 times per second per account.
-        
-        @param request: DescribeTagResourcesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeTagResourcesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.tag):
@@ -13014,21 +12833,14 @@
         )
 
     async def describe_tag_resources_with_options_async(
         self,
         request: cdn_20180510_models.DescribeTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeTagResourcesResponse:
-        """
-        > You can call this operation up to 10 times per second per account.
-        
-        @param request: DescribeTagResourcesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeTagResourcesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.tag):
@@ -13052,45 +12864,34 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_tag_resources(
         self,
         request: cdn_20180510_models.DescribeTagResourcesRequest,
     ) -> cdn_20180510_models.DescribeTagResourcesResponse:
-        """
-        > You can call this operation up to 10 times per second per account.
-        
-        @param request: DescribeTagResourcesRequest
-        @return: DescribeTagResourcesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_tag_resources_with_options(request, runtime)
 
     async def describe_tag_resources_async(
         self,
         request: cdn_20180510_models.DescribeTagResourcesRequest,
     ) -> cdn_20180510_models.DescribeTagResourcesResponse:
-        """
-        > You can call this operation up to 10 times per second per account.
-        
-        @param request: DescribeTagResourcesRequest
-        @return: DescribeTagResourcesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_tag_resources_with_options_async(request, runtime)
 
     def describe_top_domains_by_flow_with_options(
         self,
         request: cdn_20180510_models.DescribeTopDomainsByFlowRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeTopDomainsByFlowResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to analyze data.
-        > - If you do not set **StartTime** or **EndTime**, data within the current month is queried. If you set both **StartTime** and **EndTime**, data within the specified time range is queried.
-        - You can call this operation up to 100 times per second per account.
+        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](~~279577~~) feature for data analysis.
+        >
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the current month. If you set both these parameters, the request returns the data collected within the specified time range.********\
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeTopDomainsByFlowRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeTopDomainsByFlowResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -13121,17 +12922,18 @@
 
     async def describe_top_domains_by_flow_with_options_async(
         self,
         request: cdn_20180510_models.DescribeTopDomainsByFlowRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeTopDomainsByFlowResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to analyze data.
-        > - If you do not set **StartTime** or **EndTime**, data within the current month is queried. If you set both **StartTime** and **EndTime**, data within the specified time range is queried.
-        - You can call this operation up to 100 times per second per account.
+        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](~~279577~~) feature for data analysis.
+        >
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the current month. If you set both these parameters, the request returns the data collected within the specified time range.********\
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeTopDomainsByFlowRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeTopDomainsByFlowResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -13161,45 +12963,47 @@
         )
 
     def describe_top_domains_by_flow(
         self,
         request: cdn_20180510_models.DescribeTopDomainsByFlowRequest,
     ) -> cdn_20180510_models.DescribeTopDomainsByFlowResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to analyze data.
-        > - If you do not set **StartTime** or **EndTime**, data within the current month is queried. If you set both **StartTime** and **EndTime**, data within the specified time range is queried.
-        - You can call this operation up to 100 times per second per account.
+        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](~~279577~~) feature for data analysis.
+        >
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the current month. If you set both these parameters, the request returns the data collected within the specified time range.********\
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeTopDomainsByFlowRequest
         @return: DescribeTopDomainsByFlowResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_top_domains_by_flow_with_options(request, runtime)
 
     async def describe_top_domains_by_flow_async(
         self,
         request: cdn_20180510_models.DescribeTopDomainsByFlowRequest,
     ) -> cdn_20180510_models.DescribeTopDomainsByFlowResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to analyze data.
-        > - If you do not set **StartTime** or **EndTime**, data within the current month is queried. If you set both **StartTime** and **EndTime**, data within the specified time range is queried.
-        - You can call this operation up to 100 times per second per account.
+        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](~~279577~~) feature for data analysis.
+        >
+        *   If you do not set the **StartTime** or **EndTime** parameter, the request returns the data collected in the current month. If you set both these parameters, the request returns the data collected within the specified time range.********\
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeTopDomainsByFlowRequest
         @return: DescribeTopDomainsByFlowResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_top_domains_by_flow_with_options_async(request, runtime)
 
     def describe_user_certificate_expire_count_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeUserCertificateExpireCountResponse:
         """
-        > You can call this operation up to 100 times per second per account.
+        The number of domain names whose SSL certificates are about to expire within 30 days.
         
         @param request: DescribeUserCertificateExpireCountRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeUserCertificateExpireCountResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -13219,15 +13023,15 @@
         )
 
     async def describe_user_certificate_expire_count_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeUserCertificateExpireCountResponse:
         """
-        > You can call this operation up to 100 times per second per account.
+        The number of domain names whose SSL certificates are about to expire within 30 days.
         
         @param request: DescribeUserCertificateExpireCountRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeUserCertificateExpireCountResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -13244,24 +13048,24 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeUserCertificateExpireCountResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_user_certificate_expire_count(self) -> cdn_20180510_models.DescribeUserCertificateExpireCountResponse:
         """
-        > You can call this operation up to 100 times per second per account.
+        The number of domain names whose SSL certificates are about to expire within 30 days.
         
         @return: DescribeUserCertificateExpireCountResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_certificate_expire_count_with_options(runtime)
 
     async def describe_user_certificate_expire_count_async(self) -> cdn_20180510_models.DescribeUserCertificateExpireCountResponse:
         """
-        > You can call this operation up to 100 times per second per account.
+        The number of domain names whose SSL certificates are about to expire within 30 days.
         
         @return: DescribeUserCertificateExpireCountResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_user_certificate_expire_count_with_options_async(runtime)
 
     def describe_user_configs_with_options(
@@ -13375,15 +13179,15 @@
     def describe_user_domains_with_options(
         self,
         request: cdn_20180510_models.DescribeUserDomainsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeUserDomainsResponse:
         """
         You can call this operation up to 100 times per second per account.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
+        *   You can specify up to 50 domain names in each request. Separate multiple domain names with commas (,).
         
         @param request: DescribeUserDomainsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeUserDomainsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -13439,15 +13243,15 @@
     async def describe_user_domains_with_options_async(
         self,
         request: cdn_20180510_models.DescribeUserDomainsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeUserDomainsResponse:
         """
         You can call this operation up to 100 times per second per account.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
+        *   You can specify up to 50 domain names in each request. Separate multiple domain names with commas (,).
         
         @param request: DescribeUserDomainsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeUserDomainsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -13502,29 +13306,29 @@
 
     def describe_user_domains(
         self,
         request: cdn_20180510_models.DescribeUserDomainsRequest,
     ) -> cdn_20180510_models.DescribeUserDomainsResponse:
         """
         You can call this operation up to 100 times per second per account.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
+        *   You can specify up to 50 domain names in each request. Separate multiple domain names with commas (,).
         
         @param request: DescribeUserDomainsRequest
         @return: DescribeUserDomainsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_domains_with_options(request, runtime)
 
     async def describe_user_domains_async(
         self,
         request: cdn_20180510_models.DescribeUserDomainsRequest,
     ) -> cdn_20180510_models.DescribeUserDomainsResponse:
         """
         You can call this operation up to 100 times per second per account.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
+        *   You can specify up to 50 domain names in each request. Separate multiple domain names with commas (,).
         
         @param request: DescribeUserDomainsRequest
         @return: DescribeUserDomainsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_user_domains_with_options_async(request, runtime)
 
@@ -13808,15 +13612,15 @@
 
     def describe_user_vips_by_domain_with_options(
         self,
         request: cdn_20180510_models.DescribeUserVipsByDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeUserVipsByDomainResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        The ID of the request.
         
         @param request: DescribeUserVipsByDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeUserVipsByDomainResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -13841,15 +13645,15 @@
 
     async def describe_user_vips_by_domain_with_options_async(
         self,
         request: cdn_20180510_models.DescribeUserVipsByDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeUserVipsByDomainResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        The ID of the request.
         
         @param request: DescribeUserVipsByDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeUserVipsByDomainResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -13873,47 +13677,40 @@
         )
 
     def describe_user_vips_by_domain(
         self,
         request: cdn_20180510_models.DescribeUserVipsByDomainRequest,
     ) -> cdn_20180510_models.DescribeUserVipsByDomainResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        The ID of the request.
         
         @param request: DescribeUserVipsByDomainRequest
         @return: DescribeUserVipsByDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_vips_by_domain_with_options(request, runtime)
 
     async def describe_user_vips_by_domain_async(
         self,
         request: cdn_20180510_models.DescribeUserVipsByDomainRequest,
     ) -> cdn_20180510_models.DescribeUserVipsByDomainResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        The ID of the request.
         
         @param request: DescribeUserVipsByDomainRequest
         @return: DescribeUserVipsByDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_user_vips_by_domain_with_options_async(request, runtime)
 
     def describe_verify_content_with_options(
         self,
         request: cdn_20180510_models.DescribeVerifyContentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeVerifyContentResponse:
-        """
-        > You can call this operation up to 100 times per second per account.
-        
-        @param request: DescribeVerifyContentRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeVerifyContentResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -13934,21 +13731,14 @@
         )
 
     async def describe_verify_content_with_options_async(
         self,
         request: cdn_20180510_models.DescribeVerifyContentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeVerifyContentResponse:
-        """
-        > You can call this operation up to 100 times per second per account.
-        
-        @param request: DescribeVerifyContentRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeVerifyContentResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -13968,33 +13758,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_verify_content(
         self,
         request: cdn_20180510_models.DescribeVerifyContentRequest,
     ) -> cdn_20180510_models.DescribeVerifyContentResponse:
-        """
-        > You can call this operation up to 100 times per second per account.
-        
-        @param request: DescribeVerifyContentRequest
-        @return: DescribeVerifyContentResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_verify_content_with_options(request, runtime)
 
     async def describe_verify_content_async(
         self,
         request: cdn_20180510_models.DescribeVerifyContentRequest,
     ) -> cdn_20180510_models.DescribeVerifyContentResponse:
-        """
-        > You can call this operation up to 100 times per second per account.
-        
-        @param request: DescribeVerifyContentRequest
-        @return: DescribeVerifyContentResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_verify_content_with_options_async(request, runtime)
 
     def disable_realtime_log_delivery_with_options(
         self,
         request: cdn_20180510_models.DisableRealtimeLogDeliveryRequest,
         runtime: util_models.RuntimeOptions,
@@ -14180,15 +13958,15 @@
 
     def list_domains_by_log_config_id_with_options(
         self,
         request: cdn_20180510_models.ListDomainsByLogConfigIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.ListDomainsByLogConfigIdResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: ListDomainsByLogConfigIdRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListDomainsByLogConfigIdResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -14213,15 +13991,15 @@
 
     async def list_domains_by_log_config_id_with_options_async(
         self,
         request: cdn_20180510_models.ListDomainsByLogConfigIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.ListDomainsByLogConfigIdResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: ListDomainsByLogConfigIdRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListDomainsByLogConfigIdResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -14245,42 +14023,42 @@
         )
 
     def list_domains_by_log_config_id(
         self,
         request: cdn_20180510_models.ListDomainsByLogConfigIdRequest,
     ) -> cdn_20180510_models.ListDomainsByLogConfigIdResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: ListDomainsByLogConfigIdRequest
         @return: ListDomainsByLogConfigIdResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_domains_by_log_config_id_with_options(request, runtime)
 
     async def list_domains_by_log_config_id_async(
         self,
         request: cdn_20180510_models.ListDomainsByLogConfigIdRequest,
     ) -> cdn_20180510_models.ListDomainsByLogConfigIdResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: ListDomainsByLogConfigIdRequest
         @return: ListDomainsByLogConfigIdResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_domains_by_log_config_id_with_options_async(request, runtime)
 
     def list_fctrigger_with_options(
         self,
         request: cdn_20180510_models.ListFCTriggerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.ListFCTriggerResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: ListFCTriggerRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListFCTriggerResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -14305,15 +14083,15 @@
 
     async def list_fctrigger_with_options_async(
         self,
         request: cdn_20180510_models.ListFCTriggerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.ListFCTriggerResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: ListFCTriggerRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListFCTriggerResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -14337,42 +14115,42 @@
         )
 
     def list_fctrigger(
         self,
         request: cdn_20180510_models.ListFCTriggerRequest,
     ) -> cdn_20180510_models.ListFCTriggerResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: ListFCTriggerRequest
         @return: ListFCTriggerResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_fctrigger_with_options(request, runtime)
 
     async def list_fctrigger_async(
         self,
         request: cdn_20180510_models.ListFCTriggerRequest,
     ) -> cdn_20180510_models.ListFCTriggerResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: ListFCTriggerRequest
         @return: ListFCTriggerResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_fctrigger_with_options_async(request, runtime)
 
     def list_realtime_log_delivery_domains_with_options(
         self,
         request: cdn_20180510_models.ListRealtimeLogDeliveryDomainsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.ListRealtimeLogDeliveryDomainsResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: ListRealtimeLogDeliveryDomainsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListRealtimeLogDeliveryDomainsResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -14397,15 +14175,15 @@
 
     async def list_realtime_log_delivery_domains_with_options_async(
         self,
         request: cdn_20180510_models.ListRealtimeLogDeliveryDomainsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.ListRealtimeLogDeliveryDomainsResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: ListRealtimeLogDeliveryDomainsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListRealtimeLogDeliveryDomainsResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -14429,41 +14207,41 @@
         )
 
     def list_realtime_log_delivery_domains(
         self,
         request: cdn_20180510_models.ListRealtimeLogDeliveryDomainsRequest,
     ) -> cdn_20180510_models.ListRealtimeLogDeliveryDomainsResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: ListRealtimeLogDeliveryDomainsRequest
         @return: ListRealtimeLogDeliveryDomainsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_realtime_log_delivery_domains_with_options(request, runtime)
 
     async def list_realtime_log_delivery_domains_async(
         self,
         request: cdn_20180510_models.ListRealtimeLogDeliveryDomainsRequest,
     ) -> cdn_20180510_models.ListRealtimeLogDeliveryDomainsResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: ListRealtimeLogDeliveryDomainsRequest
         @return: ListRealtimeLogDeliveryDomainsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_realtime_log_delivery_domains_with_options_async(request, runtime)
 
     def list_realtime_log_delivery_infos_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.ListRealtimeLogDeliveryInfosResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: ListRealtimeLogDeliveryInfosRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListRealtimeLogDeliveryInfosResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -14483,15 +14261,15 @@
         )
 
     async def list_realtime_log_delivery_infos_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.ListRealtimeLogDeliveryInfosResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: ListRealtimeLogDeliveryInfosRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListRealtimeLogDeliveryInfosResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -14508,24 +14286,24 @@
         return TeaCore.from_map(
             cdn_20180510_models.ListRealtimeLogDeliveryInfosResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def list_realtime_log_delivery_infos(self) -> cdn_20180510_models.ListRealtimeLogDeliveryInfosResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @return: ListRealtimeLogDeliveryInfosResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_realtime_log_delivery_infos_with_options(runtime)
 
     async def list_realtime_log_delivery_infos_async(self) -> cdn_20180510_models.ListRealtimeLogDeliveryInfosResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @return: ListRealtimeLogDeliveryInfosResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_realtime_log_delivery_infos_with_options_async(runtime)
 
     def list_user_custom_log_config_with_options(
@@ -14604,15 +14382,15 @@
 
     def modify_cdn_domain_with_options(
         self,
         request: cdn_20180510_models.ModifyCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.ModifyCdnDomainResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: ModifyCdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyCdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -14649,15 +14427,15 @@
 
     async def modify_cdn_domain_with_options_async(
         self,
         request: cdn_20180510_models.ModifyCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.ModifyCdnDomainResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: ModifyCdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyCdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -14693,42 +14471,42 @@
         )
 
     def modify_cdn_domain(
         self,
         request: cdn_20180510_models.ModifyCdnDomainRequest,
     ) -> cdn_20180510_models.ModifyCdnDomainResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: ModifyCdnDomainRequest
         @return: ModifyCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_cdn_domain_with_options(request, runtime)
 
     async def modify_cdn_domain_async(
         self,
         request: cdn_20180510_models.ModifyCdnDomainRequest,
     ) -> cdn_20180510_models.ModifyCdnDomainResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: ModifyCdnDomainRequest
         @return: ModifyCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_cdn_domain_with_options_async(request, runtime)
 
     def modify_cdn_domain_schdm_by_property_with_options(
         self,
         request: cdn_20180510_models.ModifyCdnDomainSchdmByPropertyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.ModifyCdnDomainSchdmByPropertyResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: ModifyCdnDomainSchdmByPropertyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyCdnDomainSchdmByPropertyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -14757,15 +14535,15 @@
 
     async def modify_cdn_domain_schdm_by_property_with_options_async(
         self,
         request: cdn_20180510_models.ModifyCdnDomainSchdmByPropertyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.ModifyCdnDomainSchdmByPropertyResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: ModifyCdnDomainSchdmByPropertyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyCdnDomainSchdmByPropertyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -14793,28 +14571,28 @@
         )
 
     def modify_cdn_domain_schdm_by_property(
         self,
         request: cdn_20180510_models.ModifyCdnDomainSchdmByPropertyRequest,
     ) -> cdn_20180510_models.ModifyCdnDomainSchdmByPropertyResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: ModifyCdnDomainSchdmByPropertyRequest
         @return: ModifyCdnDomainSchdmByPropertyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_cdn_domain_schdm_by_property_with_options(request, runtime)
 
     async def modify_cdn_domain_schdm_by_property_async(
         self,
         request: cdn_20180510_models.ModifyCdnDomainSchdmByPropertyRequest,
     ) -> cdn_20180510_models.ModifyCdnDomainSchdmByPropertyResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: ModifyCdnDomainSchdmByPropertyRequest
         @return: ModifyCdnDomainSchdmByPropertyResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_cdn_domain_schdm_by_property_with_options_async(request, runtime)
 
@@ -14912,16 +14690,16 @@
 
     def open_cdn_service_with_options(
         self,
         request: cdn_20180510_models.OpenCdnServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.OpenCdnServiceResponse:
         """
-        > - Alibaba Cloud CDN can be activated only once per Alibaba Cloud account. The Alibaba Cloud account must pass real-name verification.
-        > - The maximum number of times that each user can call this operation per second is 5.
+        Alibaba Cloud CDN can be activated only once per Alibaba Cloud account. The Alibaba Cloud account must complete real-name verification to activate Alibaba Cloud CDN.
+        *   You can call this operation up to five times per second per user.
         
         @param request: OpenCdnServiceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: OpenCdnServiceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -14952,16 +14730,16 @@
 
     async def open_cdn_service_with_options_async(
         self,
         request: cdn_20180510_models.OpenCdnServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.OpenCdnServiceResponse:
         """
-        > - Alibaba Cloud CDN can be activated only once per Alibaba Cloud account. The Alibaba Cloud account must pass real-name verification.
-        > - The maximum number of times that each user can call this operation per second is 5.
+        Alibaba Cloud CDN can be activated only once per Alibaba Cloud account. The Alibaba Cloud account must complete real-name verification to activate Alibaba Cloud CDN.
+        *   You can call this operation up to five times per second per user.
         
         @param request: OpenCdnServiceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: OpenCdnServiceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -14991,30 +14769,30 @@
         )
 
     def open_cdn_service(
         self,
         request: cdn_20180510_models.OpenCdnServiceRequest,
     ) -> cdn_20180510_models.OpenCdnServiceResponse:
         """
-        > - Alibaba Cloud CDN can be activated only once per Alibaba Cloud account. The Alibaba Cloud account must pass real-name verification.
-        > - The maximum number of times that each user can call this operation per second is 5.
+        Alibaba Cloud CDN can be activated only once per Alibaba Cloud account. The Alibaba Cloud account must complete real-name verification to activate Alibaba Cloud CDN.
+        *   You can call this operation up to five times per second per user.
         
         @param request: OpenCdnServiceRequest
         @return: OpenCdnServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.open_cdn_service_with_options(request, runtime)
 
     async def open_cdn_service_async(
         self,
         request: cdn_20180510_models.OpenCdnServiceRequest,
     ) -> cdn_20180510_models.OpenCdnServiceResponse:
         """
-        > - Alibaba Cloud CDN can be activated only once per Alibaba Cloud account. The Alibaba Cloud account must pass real-name verification.
-        > - The maximum number of times that each user can call this operation per second is 5.
+        Alibaba Cloud CDN can be activated only once per Alibaba Cloud account. The Alibaba Cloud account must complete real-name verification to activate Alibaba Cloud CDN.
+        *   You can call this operation up to five times per second per user.
         
         @param request: OpenCdnServiceRequest
         @return: OpenCdnServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.open_cdn_service_with_options_async(request, runtime)
 
@@ -15276,17 +15054,17 @@
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.RefreshObjectCachesResponse:
         """
         Alibaba Cloud CDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshObjectCaches](~~91164~~) operation to refresh content and call the [PushObjectCache](~~91161~~) operation to prefetch content.
         *   You can call the RefreshObjectCaches operation up to 50 times per second per account.
         *   For more information about how to automatically refresh or prefetch tasks, see [Run scripts to refresh and prefetch content](~~151829~~).
-        ## Usage notes
+        ## Precautions
         *   After a refresh task is submitted and completed, specific resources are removed from POPs. When a POP receives a request for the removed resources, the POP forwards the request to the origin server to retrieve the resources. The retrieved resources are returned to the client and cached on the POP. Multiple refresh tasks may cause a large number of resources to be removed from the POPs. This increases the number of requests that are forwarded to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        *   A refresh task takes effect 5 to 6 minutes after being submitted. If the TTL for the resources you want to refresh is less than 5 minutes, you can wait until the TTL expires instead of performing the refresh operation.
+        *   A refresh task takes effect 5 to 6 minutes after being submitted. This means that if the resource you want to refresh has a TTL of less than five minutes, you wait for it to expire instead of manually running a refresh task.
         *   If you want to use RAM users to refresh or prefetch resources, you must obtain the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
         ### Refresh quota
         *   By default, each Alibaba Cloud account can refresh content from up to 10,000 URLs and 100 directories per day. The directories include subdirectories. If the daily peak bandwidth value exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. Alibaba Cloud CDN evaluates your application based on your workloads.
         *   By default, each Alibaba Cloud account can submit up to 20 refresh rules that contain regular expressions per day. If the daily peak bandwidth of your Alibaba Cloud account exceeds 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex) to request a quota increase.
         *   You can specify up to 1,000 URL refresh rules, 100 directory refresh rules, or 1 refresh rule that contains regular expressions in each call.
         *   You can refresh up to 1,000 URLs per minute for each domain name.
         
@@ -15329,17 +15107,17 @@
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.RefreshObjectCachesResponse:
         """
         Alibaba Cloud CDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshObjectCaches](~~91164~~) operation to refresh content and call the [PushObjectCache](~~91161~~) operation to prefetch content.
         *   You can call the RefreshObjectCaches operation up to 50 times per second per account.
         *   For more information about how to automatically refresh or prefetch tasks, see [Run scripts to refresh and prefetch content](~~151829~~).
-        ## Usage notes
+        ## Precautions
         *   After a refresh task is submitted and completed, specific resources are removed from POPs. When a POP receives a request for the removed resources, the POP forwards the request to the origin server to retrieve the resources. The retrieved resources are returned to the client and cached on the POP. Multiple refresh tasks may cause a large number of resources to be removed from the POPs. This increases the number of requests that are forwarded to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        *   A refresh task takes effect 5 to 6 minutes after being submitted. If the TTL for the resources you want to refresh is less than 5 minutes, you can wait until the TTL expires instead of performing the refresh operation.
+        *   A refresh task takes effect 5 to 6 minutes after being submitted. This means that if the resource you want to refresh has a TTL of less than five minutes, you wait for it to expire instead of manually running a refresh task.
         *   If you want to use RAM users to refresh or prefetch resources, you must obtain the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
         ### Refresh quota
         *   By default, each Alibaba Cloud account can refresh content from up to 10,000 URLs and 100 directories per day. The directories include subdirectories. If the daily peak bandwidth value exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. Alibaba Cloud CDN evaluates your application based on your workloads.
         *   By default, each Alibaba Cloud account can submit up to 20 refresh rules that contain regular expressions per day. If the daily peak bandwidth of your Alibaba Cloud account exceeds 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex) to request a quota increase.
         *   You can specify up to 1,000 URL refresh rules, 100 directory refresh rules, or 1 refresh rule that contains regular expressions in each call.
         *   You can refresh up to 1,000 URLs per minute for each domain name.
         
@@ -15381,17 +15159,17 @@
         request: cdn_20180510_models.RefreshObjectCachesRequest,
     ) -> cdn_20180510_models.RefreshObjectCachesResponse:
         """
         Alibaba Cloud CDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshObjectCaches](~~91164~~) operation to refresh content and call the [PushObjectCache](~~91161~~) operation to prefetch content.
         *   You can call the RefreshObjectCaches operation up to 50 times per second per account.
         *   For more information about how to automatically refresh or prefetch tasks, see [Run scripts to refresh and prefetch content](~~151829~~).
-        ## Usage notes
+        ## Precautions
         *   After a refresh task is submitted and completed, specific resources are removed from POPs. When a POP receives a request for the removed resources, the POP forwards the request to the origin server to retrieve the resources. The retrieved resources are returned to the client and cached on the POP. Multiple refresh tasks may cause a large number of resources to be removed from the POPs. This increases the number of requests that are forwarded to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        *   A refresh task takes effect 5 to 6 minutes after being submitted. If the TTL for the resources you want to refresh is less than 5 minutes, you can wait until the TTL expires instead of performing the refresh operation.
+        *   A refresh task takes effect 5 to 6 minutes after being submitted. This means that if the resource you want to refresh has a TTL of less than five minutes, you wait for it to expire instead of manually running a refresh task.
         *   If you want to use RAM users to refresh or prefetch resources, you must obtain the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
         ### Refresh quota
         *   By default, each Alibaba Cloud account can refresh content from up to 10,000 URLs and 100 directories per day. The directories include subdirectories. If the daily peak bandwidth value exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. Alibaba Cloud CDN evaluates your application based on your workloads.
         *   By default, each Alibaba Cloud account can submit up to 20 refresh rules that contain regular expressions per day. If the daily peak bandwidth of your Alibaba Cloud account exceeds 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex) to request a quota increase.
         *   You can specify up to 1,000 URL refresh rules, 100 directory refresh rules, or 1 refresh rule that contains regular expressions in each call.
         *   You can refresh up to 1,000 URLs per minute for each domain name.
         
@@ -15406,17 +15184,17 @@
         request: cdn_20180510_models.RefreshObjectCachesRequest,
     ) -> cdn_20180510_models.RefreshObjectCachesResponse:
         """
         Alibaba Cloud CDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshObjectCaches](~~91164~~) operation to refresh content and call the [PushObjectCache](~~91161~~) operation to prefetch content.
         *   You can call the RefreshObjectCaches operation up to 50 times per second per account.
         *   For more information about how to automatically refresh or prefetch tasks, see [Run scripts to refresh and prefetch content](~~151829~~).
-        ## Usage notes
+        ## Precautions
         *   After a refresh task is submitted and completed, specific resources are removed from POPs. When a POP receives a request for the removed resources, the POP forwards the request to the origin server to retrieve the resources. The retrieved resources are returned to the client and cached on the POP. Multiple refresh tasks may cause a large number of resources to be removed from the POPs. This increases the number of requests that are forwarded to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        *   A refresh task takes effect 5 to 6 minutes after being submitted. If the TTL for the resources you want to refresh is less than 5 minutes, you can wait until the TTL expires instead of performing the refresh operation.
+        *   A refresh task takes effect 5 to 6 minutes after being submitted. This means that if the resource you want to refresh has a TTL of less than five minutes, you wait for it to expire instead of manually running a refresh task.
         *   If you want to use RAM users to refresh or prefetch resources, you must obtain the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
         ### Refresh quota
         *   By default, each Alibaba Cloud account can refresh content from up to 10,000 URLs and 100 directories per day. The directories include subdirectories. If the daily peak bandwidth value exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. Alibaba Cloud CDN evaluates your application based on your workloads.
         *   By default, each Alibaba Cloud account can submit up to 20 refresh rules that contain regular expressions per day. If the daily peak bandwidth of your Alibaba Cloud account exceeds 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex) to request a quota increase.
         *   You can specify up to 1,000 URL refresh rules, 100 directory refresh rules, or 1 refresh rule that contains regular expressions in each call.
         *   You can refresh up to 1,000 URLs per minute for each domain name.
         
@@ -15428,15 +15206,15 @@
 
     def rollback_staging_config_with_options(
         self,
         request: cdn_20180510_models.RollbackStagingConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.RollbackStagingConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: RollbackStagingConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RollbackStagingConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15463,15 +15241,15 @@
 
     async def rollback_staging_config_with_options_async(
         self,
         request: cdn_20180510_models.RollbackStagingConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.RollbackStagingConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: RollbackStagingConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RollbackStagingConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15497,28 +15275,28 @@
         )
 
     def rollback_staging_config(
         self,
         request: cdn_20180510_models.RollbackStagingConfigRequest,
     ) -> cdn_20180510_models.RollbackStagingConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: RollbackStagingConfigRequest
         @return: RollbackStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.rollback_staging_config_with_options(request, runtime)
 
     async def rollback_staging_config_async(
         self,
         request: cdn_20180510_models.RollbackStagingConfigRequest,
     ) -> cdn_20180510_models.RollbackStagingConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: RollbackStagingConfigRequest
         @return: RollbackStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.rollback_staging_config_with_options_async(request, runtime)
 
@@ -15624,15 +15402,15 @@
 
     def set_cdn_domain_smcertificate_with_options(
         self,
         request: cdn_20180510_models.SetCdnDomainSMCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.SetCdnDomainSMCertificateResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: SetCdnDomainSMCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetCdnDomainSMCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15667,15 +15445,15 @@
 
     async def set_cdn_domain_smcertificate_with_options_async(
         self,
         request: cdn_20180510_models.SetCdnDomainSMCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.SetCdnDomainSMCertificateResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: SetCdnDomainSMCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetCdnDomainSMCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15709,42 +15487,168 @@
         )
 
     def set_cdn_domain_smcertificate(
         self,
         request: cdn_20180510_models.SetCdnDomainSMCertificateRequest,
     ) -> cdn_20180510_models.SetCdnDomainSMCertificateResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: SetCdnDomainSMCertificateRequest
         @return: SetCdnDomainSMCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.set_cdn_domain_smcertificate_with_options(request, runtime)
 
     async def set_cdn_domain_smcertificate_async(
         self,
         request: cdn_20180510_models.SetCdnDomainSMCertificateRequest,
     ) -> cdn_20180510_models.SetCdnDomainSMCertificateResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: SetCdnDomainSMCertificateRequest
         @return: SetCdnDomainSMCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.set_cdn_domain_smcertificate_with_options_async(request, runtime)
 
+    def set_cdn_domain_sslcertificate_with_options(
+        self,
+        request: cdn_20180510_models.SetCdnDomainSSLCertificateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cdn_20180510_models.SetCdnDomainSSLCertificateResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cert_id):
+            query['CertId'] = request.cert_id
+        if not UtilClient.is_unset(request.cert_name):
+            query['CertName'] = request.cert_name
+        if not UtilClient.is_unset(request.cert_region):
+            query['CertRegion'] = request.cert_region
+        if not UtilClient.is_unset(request.cert_type):
+            query['CertType'] = request.cert_type
+        if not UtilClient.is_unset(request.domain_name):
+            query['DomainName'] = request.domain_name
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.sslpri):
+            query['SSLPri'] = request.sslpri
+        if not UtilClient.is_unset(request.sslprotocol):
+            query['SSLProtocol'] = request.sslprotocol
+        if not UtilClient.is_unset(request.sslpub):
+            query['SSLPub'] = request.sslpub
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetCdnDomainSSLCertificate',
+            version='2018-05-10',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cdn_20180510_models.SetCdnDomainSSLCertificateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def set_cdn_domain_sslcertificate_with_options_async(
+        self,
+        request: cdn_20180510_models.SetCdnDomainSSLCertificateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cdn_20180510_models.SetCdnDomainSSLCertificateResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cert_id):
+            query['CertId'] = request.cert_id
+        if not UtilClient.is_unset(request.cert_name):
+            query['CertName'] = request.cert_name
+        if not UtilClient.is_unset(request.cert_region):
+            query['CertRegion'] = request.cert_region
+        if not UtilClient.is_unset(request.cert_type):
+            query['CertType'] = request.cert_type
+        if not UtilClient.is_unset(request.domain_name):
+            query['DomainName'] = request.domain_name
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.sslpri):
+            query['SSLPri'] = request.sslpri
+        if not UtilClient.is_unset(request.sslprotocol):
+            query['SSLProtocol'] = request.sslprotocol
+        if not UtilClient.is_unset(request.sslpub):
+            query['SSLPub'] = request.sslpub
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetCdnDomainSSLCertificate',
+            version='2018-05-10',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cdn_20180510_models.SetCdnDomainSSLCertificateResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def set_cdn_domain_sslcertificate(
+        self,
+        request: cdn_20180510_models.SetCdnDomainSSLCertificateRequest,
+    ) -> cdn_20180510_models.SetCdnDomainSSLCertificateResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.set_cdn_domain_sslcertificate_with_options(request, runtime)
+
+    async def set_cdn_domain_sslcertificate_async(
+        self,
+        request: cdn_20180510_models.SetCdnDomainSSLCertificateRequest,
+    ) -> cdn_20180510_models.SetCdnDomainSSLCertificateResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.set_cdn_domain_sslcertificate_with_options_async(request, runtime)
+
     def set_cdn_domain_staging_config_with_options(
         self,
         request: cdn_20180510_models.SetCdnDomainStagingConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.SetCdnDomainStagingConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        The features that you want to configure. Format:
+        > - **functionName**: The name of the feature. Separate multiple values with commas (,).
+        > - **argName**: The feature parameters for **functionName**.
+        > - **argValue**: The parameter values set for **functionName**.
+        ```
+        [
+        {
+        "functionArgs": [
+        {
+        "argName": "Parameter A",
+        "argValue": "Parameter value"
+        },
+        {
+        "argName": "Parameter B",
+        "argValue": "Parameter value"
+        }
+        ],
+        "functionName": "Feature name"
+        }
+        ]
+        ```
         
         @param request: SetCdnDomainStagingConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetCdnDomainStagingConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15773,15 +15677,35 @@
 
     async def set_cdn_domain_staging_config_with_options_async(
         self,
         request: cdn_20180510_models.SetCdnDomainStagingConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.SetCdnDomainStagingConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        The features that you want to configure. Format:
+        > - **functionName**: The name of the feature. Separate multiple values with commas (,).
+        > - **argName**: The feature parameters for **functionName**.
+        > - **argValue**: The parameter values set for **functionName**.
+        ```
+        [
+        {
+        "functionArgs": [
+        {
+        "argName": "Parameter A",
+        "argValue": "Parameter value"
+        },
+        {
+        "argName": "Parameter B",
+        "argValue": "Parameter value"
+        }
+        ],
+        "functionName": "Feature name"
+        }
+        ]
+        ```
         
         @param request: SetCdnDomainStagingConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetCdnDomainStagingConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15809,43 +15733,82 @@
         )
 
     def set_cdn_domain_staging_config(
         self,
         request: cdn_20180510_models.SetCdnDomainStagingConfigRequest,
     ) -> cdn_20180510_models.SetCdnDomainStagingConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        The features that you want to configure. Format:
+        > - **functionName**: The name of the feature. Separate multiple values with commas (,).
+        > - **argName**: The feature parameters for **functionName**.
+        > - **argValue**: The parameter values set for **functionName**.
+        ```
+        [
+        {
+        "functionArgs": [
+        {
+        "argName": "Parameter A",
+        "argValue": "Parameter value"
+        },
+        {
+        "argName": "Parameter B",
+        "argValue": "Parameter value"
+        }
+        ],
+        "functionName": "Feature name"
+        }
+        ]
+        ```
         
         @param request: SetCdnDomainStagingConfigRequest
         @return: SetCdnDomainStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.set_cdn_domain_staging_config_with_options(request, runtime)
 
     async def set_cdn_domain_staging_config_async(
         self,
         request: cdn_20180510_models.SetCdnDomainStagingConfigRequest,
     ) -> cdn_20180510_models.SetCdnDomainStagingConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        The features that you want to configure. Format:
+        > - **functionName**: The name of the feature. Separate multiple values with commas (,).
+        > - **argName**: The feature parameters for **functionName**.
+        > - **argValue**: The parameter values set for **functionName**.
+        ```
+        [
+        {
+        "functionArgs": [
+        {
+        "argName": "Parameter A",
+        "argValue": "Parameter value"
+        },
+        {
+        "argName": "Parameter B",
+        "argValue": "Parameter value"
+        }
+        ],
+        "functionName": "Feature name"
+        }
+        ]
+        ```
         
         @param request: SetCdnDomainStagingConfigRequest
         @return: SetCdnDomainStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.set_cdn_domain_staging_config_with_options_async(request, runtime)
 
     def set_domain_server_certificate_with_options(
         self,
         request: cdn_20180510_models.SetDomainServerCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.SetDomainServerCertificateResponse:
         """
-        >    The maximum number of times that each user can call this operation per second is 10.
-        *   Method: POST.
+        The content of the SSL certificate. Specify the content of the SSL certificate only if you want to enable the SSL certificate.
         
         @param request: SetDomainServerCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetDomainServerCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15888,16 +15851,15 @@
 
     async def set_domain_server_certificate_with_options_async(
         self,
         request: cdn_20180510_models.SetDomainServerCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.SetDomainServerCertificateResponse:
         """
-        >    The maximum number of times that each user can call this operation per second is 10.
-        *   Method: POST.
+        The content of the SSL certificate. Specify the content of the SSL certificate only if you want to enable the SSL certificate.
         
         @param request: SetDomainServerCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetDomainServerCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15939,30 +15901,28 @@
         )
 
     def set_domain_server_certificate(
         self,
         request: cdn_20180510_models.SetDomainServerCertificateRequest,
     ) -> cdn_20180510_models.SetDomainServerCertificateResponse:
         """
-        >    The maximum number of times that each user can call this operation per second is 10.
-        *   Method: POST.
+        The content of the SSL certificate. Specify the content of the SSL certificate only if you want to enable the SSL certificate.
         
         @param request: SetDomainServerCertificateRequest
         @return: SetDomainServerCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.set_domain_server_certificate_with_options(request, runtime)
 
     async def set_domain_server_certificate_async(
         self,
         request: cdn_20180510_models.SetDomainServerCertificateRequest,
     ) -> cdn_20180510_models.SetDomainServerCertificateResponse:
         """
-        >    The maximum number of times that each user can call this operation per second is 10.
-        *   Method: POST.
+        The content of the SSL certificate. Specify the content of the SSL certificate only if you want to enable the SSL certificate.
         
         @param request: SetDomainServerCertificateRequest
         @return: SetDomainServerCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.set_domain_server_certificate_with_options_async(request, runtime)
 
@@ -16058,15 +16018,15 @@
 
     def set_waiting_room_config_with_options(
         self,
         request: cdn_20180510_models.SetWaitingRoomConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.SetWaitingRoomConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: SetWaitingRoomConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetWaitingRoomConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16103,15 +16063,15 @@
 
     async def set_waiting_room_config_with_options_async(
         self,
         request: cdn_20180510_models.SetWaitingRoomConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.SetWaitingRoomConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: SetWaitingRoomConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetWaitingRoomConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16147,43 +16107,43 @@
         )
 
     def set_waiting_room_config(
         self,
         request: cdn_20180510_models.SetWaitingRoomConfigRequest,
     ) -> cdn_20180510_models.SetWaitingRoomConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: SetWaitingRoomConfigRequest
         @return: SetWaitingRoomConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.set_waiting_room_config_with_options(request, runtime)
 
     async def set_waiting_room_config_async(
         self,
         request: cdn_20180510_models.SetWaitingRoomConfigRequest,
     ) -> cdn_20180510_models.SetWaitingRoomConfigResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: SetWaitingRoomConfigRequest
         @return: SetWaitingRoomConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.set_waiting_room_config_with_options_async(request, runtime)
 
     def start_cdn_domain_with_options(
         self,
         request: cdn_20180510_models.StartCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.StartCdnDomainResponse:
         """
-        - If the domain name is in an invalid state or your have an overdue payment in your account, the domain name cannot be enabled.
-        - The maximum number of times that each user can call this operation per second is 100.
+        If the domain name is in an invalid state or you have an overdue payment in your account, the domain name cannot be enabled.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: StartCdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartCdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16214,16 +16174,16 @@
 
     async def start_cdn_domain_with_options_async(
         self,
         request: cdn_20180510_models.StartCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.StartCdnDomainResponse:
         """
-        - If the domain name is in an invalid state or your have an overdue payment in your account, the domain name cannot be enabled.
-        - The maximum number of times that each user can call this operation per second is 100.
+        If the domain name is in an invalid state or you have an overdue payment in your account, the domain name cannot be enabled.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: StartCdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartCdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16253,45 +16213,45 @@
         )
 
     def start_cdn_domain(
         self,
         request: cdn_20180510_models.StartCdnDomainRequest,
     ) -> cdn_20180510_models.StartCdnDomainResponse:
         """
-        - If the domain name is in an invalid state or your have an overdue payment in your account, the domain name cannot be enabled.
-        - The maximum number of times that each user can call this operation per second is 100.
+        If the domain name is in an invalid state or you have an overdue payment in your account, the domain name cannot be enabled.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: StartCdnDomainRequest
         @return: StartCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.start_cdn_domain_with_options(request, runtime)
 
     async def start_cdn_domain_async(
         self,
         request: cdn_20180510_models.StartCdnDomainRequest,
     ) -> cdn_20180510_models.StartCdnDomainResponse:
         """
-        - If the domain name is in an invalid state or your have an overdue payment in your account, the domain name cannot be enabled.
-        - The maximum number of times that each user can call this operation per second is 100.
+        If the domain name is in an invalid state or you have an overdue payment in your account, the domain name cannot be enabled.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: StartCdnDomainRequest
         @return: StartCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.start_cdn_domain_with_options_async(request, runtime)
 
     def stop_cdn_domain_with_options(
         self,
         request: cdn_20180510_models.StopCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.StopCdnDomainResponse:
         """
-        - After an accelerated domain is disabled, the information about the domain name is retained. Requests destined for the domain name are automatically redirected to the origin server.
-        - The maximum number of times that each user can call this operation per second is 40.
+        After an accelerated domain is disabled, Alibaba Cloud CDN retains its information and routes all the requests that are destined for the accelerated domain to the origin server.
+        *   You can call this operation up to 40 times per second per account.
         
         @param request: StopCdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StopCdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16322,16 +16282,16 @@
 
     async def stop_cdn_domain_with_options_async(
         self,
         request: cdn_20180510_models.StopCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.StopCdnDomainResponse:
         """
-        - After an accelerated domain is disabled, the information about the domain name is retained. Requests destined for the domain name are automatically redirected to the origin server.
-        - The maximum number of times that each user can call this operation per second is 40.
+        After an accelerated domain is disabled, Alibaba Cloud CDN retains its information and routes all the requests that are destined for the accelerated domain to the origin server.
+        *   You can call this operation up to 40 times per second per account.
         
         @param request: StopCdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StopCdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16361,44 +16321,44 @@
         )
 
     def stop_cdn_domain(
         self,
         request: cdn_20180510_models.StopCdnDomainRequest,
     ) -> cdn_20180510_models.StopCdnDomainResponse:
         """
-        - After an accelerated domain is disabled, the information about the domain name is retained. Requests destined for the domain name are automatically redirected to the origin server.
-        - The maximum number of times that each user can call this operation per second is 40.
+        After an accelerated domain is disabled, Alibaba Cloud CDN retains its information and routes all the requests that are destined for the accelerated domain to the origin server.
+        *   You can call this operation up to 40 times per second per account.
         
         @param request: StopCdnDomainRequest
         @return: StopCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.stop_cdn_domain_with_options(request, runtime)
 
     async def stop_cdn_domain_async(
         self,
         request: cdn_20180510_models.StopCdnDomainRequest,
     ) -> cdn_20180510_models.StopCdnDomainResponse:
         """
-        - After an accelerated domain is disabled, the information about the domain name is retained. Requests destined for the domain name are automatically redirected to the origin server.
-        - The maximum number of times that each user can call this operation per second is 40.
+        After an accelerated domain is disabled, Alibaba Cloud CDN retains its information and routes all the requests that are destined for the accelerated domain to the origin server.
+        *   You can call this operation up to 40 times per second per account.
         
         @param request: StopCdnDomainRequest
         @return: StopCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.stop_cdn_domain_with_options_async(request, runtime)
 
     def tag_resources_with_options(
         self,
         request: cdn_20180510_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.TagResourcesResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: TagResourcesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: TagResourcesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16429,15 +16389,15 @@
 
     async def tag_resources_with_options_async(
         self,
         request: cdn_20180510_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.TagResourcesResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: TagResourcesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: TagResourcesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16467,42 +16427,42 @@
         )
 
     def tag_resources(
         self,
         request: cdn_20180510_models.TagResourcesRequest,
     ) -> cdn_20180510_models.TagResourcesResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: TagResourcesRequest
         @return: TagResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.tag_resources_with_options(request, runtime)
 
     async def tag_resources_async(
         self,
         request: cdn_20180510_models.TagResourcesRequest,
     ) -> cdn_20180510_models.TagResourcesResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
         @param request: TagResourcesRequest
         @return: TagResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.tag_resources_with_options_async(request, runtime)
 
     def untag_resources_with_options(
         self,
         request: cdn_20180510_models.UntagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.UntagResourcesResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: UntagResourcesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UntagResourcesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16535,15 +16495,15 @@
 
     async def untag_resources_with_options_async(
         self,
         request: cdn_20180510_models.UntagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.UntagResourcesResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: UntagResourcesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UntagResourcesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -16575,42 +16535,42 @@
         )
 
     def untag_resources(
         self,
         request: cdn_20180510_models.UntagResourcesRequest,
     ) -> cdn_20180510_models.UntagResourcesResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: UntagResourcesRequest
         @return: UntagResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.untag_resources_with_options(request, runtime)
 
     async def untag_resources_async(
         self,
         request: cdn_20180510_models.UntagResourcesRequest,
     ) -> cdn_20180510_models.UntagResourcesResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: UntagResourcesRequest
         @return: UntagResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.untag_resources_with_options_async(request, runtime)
 
     def update_cdn_deliver_task_with_options(
         self,
         request: cdn_20180510_models.UpdateCdnDeliverTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.UpdateCdnDeliverTaskResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
         @param request: UpdateCdnDeliverTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateCdnDeliverTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -16647,15 +16607,15 @@
 
     async def update_cdn_deliver_task_with_options_async(
         self,
         request: cdn_20180510_models.UpdateCdnDeliverTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.UpdateCdnDeliverTaskResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
         @param request: UpdateCdnDeliverTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateCdnDeliverTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -16691,42 +16651,42 @@
         )
 
     def update_cdn_deliver_task(
         self,
         request: cdn_20180510_models.UpdateCdnDeliverTaskRequest,
     ) -> cdn_20180510_models.UpdateCdnDeliverTaskResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
         @param request: UpdateCdnDeliverTaskRequest
         @return: UpdateCdnDeliverTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_cdn_deliver_task_with_options(request, runtime)
 
     async def update_cdn_deliver_task_async(
         self,
         request: cdn_20180510_models.UpdateCdnDeliverTaskRequest,
     ) -> cdn_20180510_models.UpdateCdnDeliverTaskResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
         @param request: UpdateCdnDeliverTaskRequest
         @return: UpdateCdnDeliverTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_cdn_deliver_task_with_options_async(request, runtime)
 
     def update_cdn_sub_task_with_options(
         self,
         request: cdn_20180510_models.UpdateCdnSubTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.UpdateCdnSubTaskResponse:
         """
-        >  You can call this API operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
         @param request: UpdateCdnSubTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateCdnSubTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -16759,15 +16719,15 @@
 
     async def update_cdn_sub_task_with_options_async(
         self,
         request: cdn_20180510_models.UpdateCdnSubTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.UpdateCdnSubTaskResponse:
         """
-        >  You can call this API operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
         @param request: UpdateCdnSubTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateCdnSubTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -16799,28 +16759,28 @@
         )
 
     def update_cdn_sub_task(
         self,
         request: cdn_20180510_models.UpdateCdnSubTaskRequest,
     ) -> cdn_20180510_models.UpdateCdnSubTaskResponse:
         """
-        >  You can call this API operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
         @param request: UpdateCdnSubTaskRequest
         @return: UpdateCdnSubTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_cdn_sub_task_with_options(request, runtime)
 
     async def update_cdn_sub_task_async(
         self,
         request: cdn_20180510_models.UpdateCdnSubTaskRequest,
     ) -> cdn_20180510_models.UpdateCdnSubTaskResponse:
         """
-        >  You can call this API operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
         @param request: UpdateCdnSubTaskRequest
         @return: UpdateCdnSubTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_cdn_sub_task_with_options_async(request, runtime)
```

### Comparing `alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510/models.py` & `alibabacloud_cdn20180510-1.2.8/alibabacloud_cdn20180510/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 class AddCdnDomainRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # The key of a tag.
         self.key = key
-        # The value of a tag.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -50,44 +48,24 @@
         resource_group_id: str = None,
         scope: str = None,
         security_token: str = None,
         sources: str = None,
         tag: List[AddCdnDomainRequestTag] = None,
         top_level_domain: str = None,
     ):
-        # The workload type of the domain name to accelerate. Valid values:
-        # 
-        # *   **web**: images and small files
-        # *   **download**: large files
-        # *   **video**: on-demand video and audio streaming
         self.cdn_type = cdn_type
-        # The URL that is used for health checks.
         self.check_url = check_url
-        # The domain name that you want to add to Alibaba Cloud CDN.
-        # 
-        # A wildcard domain that starts with a period (.) is supported, such as .example.com.
         self.domain_name = domain_name
         self.owner_account = owner_account
         self.owner_id = owner_id
-        # The ID of the resource group.
-        # 
-        # If you do not set this parameter, the system uses the ID of the default resource group.
         self.resource_group_id = resource_group_id
-        # The acceleration region. Default value: domestic. Valid values:
-        # 
-        # *   **domestic**: Chinese mainland
-        # *   **overseas**: global (excluding the Chinese mainland)
-        # *   **global**: global
         self.scope = scope
         self.security_token = security_token
-        # The information about the addresses of origin servers.
         self.sources = sources
-        # Details about the tags. You can specify up to 20 tags.
         self.tag = tag
-        # The top-level domain.
         self.top_level_domain = top_level_domain
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -155,15 +133,14 @@
 
 
 class AddCdnDomainResponseBody(TeaModel):
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
@@ -378,38 +355,23 @@
         owner_id: int = None,
         resource_group_id: str = None,
         scope: str = None,
         security_token: str = None,
         sources: str = None,
         top_level_domain: str = None,
     ):
-        # The workload type of the domain name to accelerate. Valid values:
-        # 
-        # *   **web**: images and small files
-        # *   **download**: large files
-        # *   **video**: on-demand video and audio streaming
         self.cdn_type = cdn_type
-        # The URL that is used for health checks.
         self.check_url = check_url
-        # The domain names that you want to add to Alibaba Cloud CDN. Separate domain names with commas (,).
         self.domain_name = domain_name
         self.owner_account = owner_account
         self.owner_id = owner_id
-        # The ID of the resource group. If you do not specify a value for this parameter, the system uses the ID of the default resource group.
         self.resource_group_id = resource_group_id
-        # The acceleration region. Default value: domestic. Valid values:
-        # 
-        # *   **domestic**: Chinese mainland
-        # *   **overseas**: global (excluding the Chinese mainland)
-        # *   **global**: global
         self.scope = scope
         self.security_token = security_token
-        # The information about the addresses of origin servers.
         self.sources = sources
-        # The top-level domain.
         self.top_level_domain = top_level_domain
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -465,15 +427,14 @@
 
 
 class BatchAddCdnDomainResponseBody(TeaModel):
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
@@ -541,17 +502,17 @@
         self,
         domain_names: str = None,
         function_names: str = None,
         owner_account: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
-        # The accelerated domain names whose configurations you want to delete. Separate accelerated domain names with commas (,).
+        # The accelerated domain names whose configurations you want to delete. Separate multiple accelerated domain names with commas (,).
         self.domain_names = domain_names
-        # The names of the features that you want to manage. Separate feature names with commas (,).
+        # The names of the features that you want to delete. Separate multiple feature names with commas (,). For more information about feature names, see [Parameters for configuring features for domain names](~~388460~~).
         self.function_names = function_names
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
@@ -666,80 +627,17 @@
         self,
         domain_names: str = None,
         functions: str = None,
         owner_account: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
+        # The ID of the request.
         self.domain_names = domain_names
-        # The features that you want to configure. Format:
-        # 
-        # *   **functionName**: the name of the feature. This parameter is required. Separate multiple values with commas (,). For more information, see [A list of features](~~388460~~).
-        # *   **argName**: the feature parameter for **functionName**. This parameter is required. You can specify multiple feature parameters.
-        # *   **argValue**: the parameter value that is specified for **functionName**. This parameter is required.
-        # *   **parentid**: the rule condition ID. This parameter is optional. You can use the **condition** rule engine to create a rule condition. For information, see [BatchSetCdnDomainConfig and SetCdnDomainStagingConfig](~~388460~~). A rule condition can identify parameters that are included in requests and filter requests based on the identified parameters. After you create a rule condition, a [configid](~~388994~~) is generated. configid can be used as parentId that is referenced by other features. This way, you can combine rule conditions and features for flexible configurations.
-        # 
-        # If you set **parentId** to **-1**, the existing rule conditions in the configurations are deleted.
-        # 
-        #     [{
-        #        "functionArgs": [{
-        #          "argName": "Parameter A", 
-        #          "argValue": Value of parameter A"
-        #         }, 
-        #       {
-        #         "argName": "Parameter B", 
-        #         "argValue": "Value of parameter B"
-        #          }], 
-        #      "functionName": "Feature name"
-        #      "parentId": "Optional, which corresponds to configid of the referenced rule condition"
-        #     }]
-        # 
-        # The following code shows a sample configuration if **parentId** is not used.
-        # 
-        # In this example, the **origin_request_header** feature is used to add back-to-origin HTTP headers, and the rule condition whose configuration ID is **222728944812032** is referenced.
-        # 
-        #     [{
-        #             "functionArgs": [{
-        #                 "argName": "header_operation_type",
-        #                 "argValue": "add"
-        #             }, {
-        #                 "argName": "header_name",
-        #                 "argValue": "Accept-Encoding"
-        #             }, {
-        #                 "argName": "header_value",
-        #                 "argValue": "gzip"
-        #             }, {
-        #                 "argName": "duplicate",
-        #                 "argValue": "off"
-        #             }],
-        #             "functionName": "origin_request_header"
-        #     }]
-        # 
-        # The following code shows a sample configuration if **parentId** is used.
-        # 
-        # In this example, the **origin_request_header** feature is used to add back-to-origin HTTP headers, and the rule condition whose configuration ID is **222728944812032** is referenced.
-        # 
-        #     [{
-        #             "functionArgs": [{
-        #                 "argName": "header_operation_type",
-        #                 "argValue": "add"
-        #             }, {
-        #                 "argName": "header_name",
-        #                 "argValue": "Accept-Encoding"
-        #             }, {
-        #                 "argName": "header_value",
-        #                 "argValue": "gzip"
-        #             }, {
-        #                 "argName": "duplicate",
-        #                 "argValue": "off"
-        #             }],
-        #             "functionName": "origin_request_header",
-        #             "parentId": "222728944812032"
-        #     }]
+        # The list of domain configurations.
         self.functions = functions
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
@@ -780,19 +678,21 @@
 class BatchSetCdnDomainConfigResponseBodyDomainConfigListDomainConfigModel(TeaModel):
     def __init__(
         self,
         config_id: int = None,
         domain_name: str = None,
         function_name: str = None,
     ):
-        # The ID of the configuration.
+        # The name of the feature.
         self.config_id = config_id
-        # The domain name.
+        # > *   You can call this operation up to 30 times per second per account.
+        # *   You can specify multiple domain names and must separate them with commas (,). You can specify up to 50 domain names in each call.
+        # *   If the BatchSetCdnDomainConfig operation is successful, a unique configuration ID (ConfigId) is generated. You can use configuration IDs to update or delete configurations. For more information, see [Usage notes on ConfigId](~~388994~~).
         self.domain_name = domain_name
-        # The name of the feature.
+        # The list of domain configurations.
         self.function_name = function_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -856,17 +756,17 @@
 
 class BatchSetCdnDomainConfigResponseBody(TeaModel):
     def __init__(
         self,
         domain_config_list: BatchSetCdnDomainConfigResponseBodyDomainConfigList = None,
         request_id: str = None,
     ):
-        # The list of domain configurations.
+        # The domain name.
         self.domain_config_list = domain_config_list
-        # The ID of the request.
+        # The ID of the configuration.
         self.request_id = request_id
 
     def validate(self):
         if self.domain_config_list:
             self.domain_config_list.validate()
 
     def to_map(self):
@@ -945,38 +845,33 @@
         owner_id: int = None,
         region: str = None,
         sslpri: str = None,
         sslprotocol: str = None,
         sslpub: str = None,
         security_token: str = None,
     ):
-        # The name of the certificate.
+        # The region.
         self.cert_name = cert_name
-        # The type of the SSL certificate. Valid values:
-        # 
-        # *   **upload**: a user-uploaded SSL certificate.
-        # *   **cas**: a certificate that is issued by SSL Certificates Service.
+        # Specifies whether to check the certificate name for duplicates. If you set the value to 1, the system does not perform the check and overwrites the information about the existing certificate that uses the same name.
         self.cert_type = cert_type
-        # The accelerated domain name to which the SSL certificate belongs. The type of request supported by the accelerated domain name must be HTTPS. You can specify multiple accelerated domain names and separate them with commas (,).
-        # 
-        # >  You can manage the SSL certificates of up to 50 accelerated domain names in each call.
+        # The private key. Specify the private key only if you enable the SSL certificate.
         self.domain_name = domain_name
         # Specifies whether to check the certificate name for duplicates. If you set the value to 1, the system does not perform the check and overwrites the information about the existing certificate that uses the same name.
         self.force_set = force_set
         self.owner_id = owner_id
-        # The region.
+        # The accelerated domain name to which the SSL certificate belongs. The type of request supported by the accelerated domain name must be HTTPS. You can specify multiple accelerated domain names and separate them with commas (,).
+        # 
+        # >  You can manage the SSL certificates of up to 50 accelerated domain names in each call.
         self.region = region
         # The private key. Specify the private key only if you enable the SSL certificate.
         self.sslpri = sslpri
-        # Specifies whether to enable the SSL certificate. Valid values:
-        # 
-        # *   **on**: enables the SSL certificate.
-        # *   **off**: disables the SSL certificate. This is the default value.
+        # The ID of the request.
         self.sslprotocol = sslprotocol
-        # The content of the SSL certificate. Specify the content of the certificate only if you want to enable the SSL certificate.
+        # > *   The maximum number of times that each user can call this operation per second is 10.
+        # *   You can specify multiple domain names (no more than 50) and separate them with commas (,).
         self.sslpub = sslpub
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1033,15 +928,15 @@
 
 
 class BatchSetCdnDomainServerCertificateResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
+        # The name of the certificate.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1107,15 +1002,15 @@
 class BatchStartCdnDomainRequest(TeaModel):
     def __init__(
         self,
         domain_names: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
-        # The domain names that you want to enable. Separate multiple domain names with commas (,).
+        # The ID of the request.
         self.domain_names = domain_names
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
@@ -1145,15 +1040,15 @@
 
 
 class BatchStartCdnDomainResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
+        # 1.0.0
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1334,27 +1229,25 @@
         domain_name: str = None,
         owner_id: int = None,
         resource_group_id: str = None,
         security_token: str = None,
         sources: str = None,
         top_level_domain: str = None,
     ):
-        # The accelerated domain names. You can specify one or more accelerated domain names. Separate domain names with commas (,).
+        # The top-level domain name.
+        # 
+        # >  You can set only one of **Sources** and **TopLevelDomain**. If you set both **Sources** and **TopLevelDomain**, **TopLevelDomain** does not take effect.
         self.domain_name = domain_name
         self.owner_id = owner_id
-        # The ID of the resource group.
+        # The ID of the request.
         self.resource_group_id = resource_group_id
         self.security_token = security_token
-        # The information about the addresses of origin servers.
-        # 
-        # >  You can set only one of **Sources** and **TopLevelDomain**. If you set both **Sources** and **TopLevelDomain**, **TopLevelDomain** does not take effect.
+        # The accelerated domain names. You can specify one or more accelerated domain names. Separate domain names with commas (,).
         self.sources = sources
-        # The top-level domain name.
-        # 
-        # >  You can set only one of **Sources** and **TopLevelDomain**. If you set both **Sources** and **TopLevelDomain**, **TopLevelDomain** does not take effect.
+        # The operation that you want to perform. Set the value to **BatchUpdateCdnDomain**.
         self.top_level_domain = top_level_domain
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1394,15 +1287,17 @@
 
 
 class BatchUpdateCdnDomainResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
+        # The information about the addresses of origin servers.
+        # 
+        # >  You can set only one of **Sources** and **TopLevelDomain**. If you set both **Sources** and **TopLevelDomain**, **TopLevelDomain** does not take effect.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1475,27 +1370,27 @@
         organization: str = None,
         organization_unit: str = None,
         sans: str = None,
         state: str = None,
     ):
         # The city to which the organization belongs. Default value: Hangzhou.
         self.city = city
-        # The Common Name of the SSL certificate.
+        # The email address that can be used to contact the organization.
         self.common_name = common_name
-        # The country to which the organization belongs. Default value: CN.
+        # The content of the CSR.
         self.country = country
-        # The email address that can be used to contact the organization.
+        # The operation that you want to perform. Set the value to **CreateCdnCertificateSigningRequest**.
         self.email = email
-        # The name of the organization. Default value: Alibaba Inc.
+        # The Subject Alternative Name (SAN) extension of the SSL certificate. This extension is used to add domain names to the certificate. Separate multiple domain names with commas (,).
         self.organization = organization
-        # The name of the organization unit. Default value: Aliyun CDN.
+        # The MD5 value of the certificate public key.
         self.organization_unit = organization_unit
-        # The Subject Alternative Name (SAN) extension of the SSL certificate. This extension is used to add domain names to the certificate. Separate multiple domain names with commas (,).
+        # The Common Name of the certificate.
         self.sans = sans
-        # The provincial district to which the organization belongs. Default value: Zhejiang.
+        # The name of the organization. Default value: Alibaba Inc.
         self.state = state
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1546,21 +1441,21 @@
     def __init__(
         self,
         common_name: str = None,
         csr: str = None,
         pub_md_5: str = None,
         request_id: str = None,
     ):
-        # The Common Name of the certificate.
+        # The name of the organization unit. Default value: Aliyun CDN.
         self.common_name = common_name
-        # The content of the CSR.
+        # The Common Name of the SSL certificate.
         self.csr = csr
-        # The MD5 value of the certificate public key.
+        # The provincial district to which the organization belongs. Default value: Zhejiang.
         self.pub_md_5 = pub_md_5
-        # The ID of the request.
+        # The country to which the organization belongs. Default value: CN.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1640,21 +1535,19 @@
         self,
         deliver: str = None,
         domain_name: str = None,
         name: str = None,
         reports: str = None,
         schedule: str = None,
     ):
-        # The method that is used to send operations reports. Operations reports are sent to you only by email. The settings must be escaped in JSON.
+        # The ID of the tracking task.
         self.deliver = deliver
-        # The domain names to be tracked. Separate multiple domain names with commas (,). You can specify up to 500 domain names. If you want to specify more than 500 domain names, [submit a ticket](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex).  
-        # 
-        # >  If you do not specify a domain name, the custom operations reports are created for all domain names that belong to your Alibaba Cloud account.
+        # The method that is used to send operations reports. Operations reports are sent to you only by email. The settings must be escaped in JSON.
         self.domain_name = domain_name
-        # The name of the tracking task.
+        # > You can call this operation up to three times per second per account.
         self.name = name
         # The operations reports that are tracked by the task. The data must be escaped in JSON.
         self.reports = reports
         # The parameters that specify the time interval at which the tracking task sends operations reports. The settings must be escaped in JSON.
         self.schedule = schedule
 
     def validate(self):
@@ -1695,17 +1588,56 @@
 
 class CreateCdnDeliverTaskResponseBody(TeaModel):
     def __init__(
         self,
         deliver_id: str = None,
         request_id: str = None,
     ):
-        # The ID of the tracking task.
+        # **Fields of the ReDatas parameter**\
+        # 
+        # | Parameter | Type | Required | Description |
+        # | --------- | ---- | -------- | ----------- |
+        # | reportId | String | Yes | The ID of the operations report. |
+        # | conditions | ConDatas[] | No | The filter conditions for the operations report. |
+        # 
+        # **Fields of the ConDatas parameter**\
+        # 
+        # | Parameter | Type | Required | Description |
+        # | --------- | ---- | -------- | ----------- |
+        # | field | String | No | The filter field. |
+        # | op | String | No | The filter operation. |
+        # | value | String[] | No | The array of field values. |
+        # 
+        # **Fields of the email parameter**\
+        # 
+        # | Parameter | Type | Required | Description |
+        # | --------- | ---- | -------- | ----------- |
+        # | subject | String | Yes | The email subject. |
+        # | to | String[] | Yes | The email addresses to which operations reports are sent. |
+        # 
+        # **Fields of the Deliver parameter**\
+        # 
+        # | Parameter | Type | Required | Description |
+        # | --------- | ---- | -------- | ----------- |
+        # | subject | String | No | The email subject. |
+        # | to | String[] | Yes | The email addresses to which operations reports are sent. |
+        # 
+        # **Fields of the Schedule parameter**\
+        # 
+        # | Parameter | Type | Required | Description |
+        # | --------- | ---- | -------- | ----------- |
+        # | schedName | String | No | The name of the tracking task. |
+        # | description | String | No | The description of the tracking task. |
+        # | crontab | String | Yes | The period during which the operations reports are tracked. |
+        # | frequency | String | Yes | The interval at which the reports are sent. Valid values:<br/>**h**: every hour <br/>**d**: every day <br/>**w**: every week |
+        # | status | String | No | The status of the tracking task. Valid values:<br/>**enable**: enabled<br/>**disable**: disabled |
+        # | effectiveFrom | String | No | The start time of the tracking task. |
+        # | effectiveEnd | String | No | The end time of the tracking task. |
         self.deliver_id = deliver_id
-        # The ID of the request.
+        # Creates a tracking task that generates operations reports. The tracking task sends operations reports to a specified email address based on a specified schedule.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1898,15 +1830,15 @@
     def __init__(
         self,
         task_name: str = None,
         time_point: str = None,
     ):
         # The name of the export task.
         self.task_name = task_name
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-DDThh:mm:ssZ format. The finest granularity is one day.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. The minimum time granularity is 1 day.
         self.time_point = time_point
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2012,17 +1944,17 @@
     def __init__(
         self,
         domain: str = None,
         logstore: str = None,
         project: str = None,
         region: str = None,
     ):
-        # The accelerated domain name for which you want to configure real-time log delivery. You can specify multiple domain names and separate them with commas (,).
+        # The accelerated domain name for which you want to configure real-time log delivery.
         self.domain = domain
-        # The name of the Logstore that collects log data from Alibaba Cloud Content Delivery Network (CDN) in real time.
+        # The name of the Logstore where log entries are stored.
         self.logstore = logstore
         # The name of the Log Service project that is used for real-time log delivery.
         self.project = project
         # The ID of the region where the Log Service project is deployed. For more information, see [Regions that support real-time log delivery](~~144883~~).
         self.region = region
 
     def validate(self):
@@ -2558,15 +2490,15 @@
 class DeleteCdnDomainRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         owner_account: str = None,
         owner_id: int = None,
     ):
-        # The accelerated domain name that you want to delete. You can specify only one domain name in each call.
+        # The ID of the request.
         self.domain_name = domain_name
         self.owner_account = owner_account
         self.owner_id = owner_id
 
     def validate(self):
         pass
 
@@ -2596,15 +2528,15 @@
 
 
 class DeleteCdnDomainResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
+        # 1.0.0
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2842,19 +2774,20 @@
 class DeleteRealTimeLogLogstoreRequest(TeaModel):
     def __init__(
         self,
         logstore: str = None,
         project: str = None,
         region: str = None,
     ):
-        # The name of the Logstore to which log entries are delivered.
+        # The ID of the region where the Log Service project is deployed. For more information, see [Regions that support real-time log delivery](~~144883~~).
         self.logstore = logstore
-        # The name of the Log Service project that is used for real-time log delivery.
+        # Deletes the Logstore that is used by a specified configuration record of real-time
+        #                   log delivery.
         self.project = project
-        # The ID of the region where the Log Service project is deployed. For more information, see [Regions that support real-time log delivery](~~144883~~).
+        # The name of the Log Service project that is used for real-time log delivery.
         self.region = region
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2959,15 +2892,15 @@
         domain: str = None,
         logstore: str = None,
         project: str = None,
         region: str = None,
     ):
         # The acceleration domain name for which you want to disable real-time log delivery. You can specify multiple domain names and separate them with commas (,).
         self.domain = domain
-        # The name of the Logstore that collects log data from Alibaba Cloud Content Delivery Network (CDN) in real time.
+        # The name of the Logstore where log entries are stored.
         self.logstore = logstore
         # The name of the Log Service project that is used for real-time log delivery.
         self.project = project
         # The ID of the region where the Log Service project is deployed. For more information, see [Regions that support real-time log delivery](~~144883~~).
         self.region = region
 
     def validate(self):
@@ -3078,15 +3011,15 @@
     def __init__(
         self,
         config_id: str = None,
         domain_name: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
-        # The configuration IDs. Separate configuration IDs with commas (,). For more information about ConfigId, see [Usage notes on ConfigId](~~388994~~).
+        # The ID of the configuration. Separate multiple configuration IDs with commas (,). For more information about ConfigId, see [Usage notes on ConfigId](~~388994~~).
         self.config_id = config_id
         # The accelerated domain name. You can specify only one domain name.
         self.domain_name = domain_name
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
@@ -3197,15 +3130,15 @@
     def __init__(
         self,
         config_id: str = None,
         domain_name: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
-        # The configuration IDs. Separate configuration IDs with commas (,). For more information about ConfigId, see [Usage notes on ConfigId](~~388994~~).
+        # The ID of the request.
         self.config_id = config_id
         # The accelerated domain names (no more than 50). Separate domain names with commas (,).
         self.domain_name = domain_name
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
@@ -3241,15 +3174,15 @@
 
 
 class DeleteSpecificStagingConfigResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
+        # The operation that you want to perform. Set the value to **DeleteSpecificStagingConfig**.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3515,17 +3448,17 @@
 class DescribeBlockedRegionsRequest(TeaModel):
     def __init__(
         self,
         language: str = None,
     ):
         # The language. Valid values:
         # 
-        # - **zh**: simplified Chinese
-        # - **en**: English
-        # - **jp**: Japanese
+        # *   **zh**: simplified Chinese
+        # *   **en**: English
+        # *   **jp**: Japanese
         self.language = language
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3623,15 +3556,15 @@
 
 class DescribeBlockedRegionsResponseBody(TeaModel):
     def __init__(
         self,
         info_list: DescribeBlockedRegionsResponseBodyInfoList = None,
         request_id: str = None,
     ):
-        # A list of countries and regions.
+        # The information returned.
         self.info_list = info_list
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.info_list:
             self.info_list.validate()
@@ -3747,19 +3680,19 @@
         self,
         cert: str = None,
         cert_id: int = None,
         cert_name: str = None,
         key: str = None,
         request_id: str = None,
     ):
-        # The content of the SSL certificate.
+        # The certificate.
         self.cert = cert
-        # The ID of the SSL certificate.
+        # The ID of the certificate.
         self.cert_id = cert_id
-        # The name of the SSL certificate.
+        # The name of the certificate.
         self.cert_name = cert_name
         # The key of the SSL certificate.
         self.key = key
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
@@ -3845,17 +3778,17 @@
 class DescribeCdnCertificateListRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
-        # The accelerated domain names. Separate multiple accelerated domain names with commas (,).
+        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
         # 
-        # If you do not specify an ID, SSL certificates of all your accelerated domain names are queried.
+        # If you do not specify an accelerated domain name, SSL certificates of all your accelerated domain names are queried.
         self.domain_name = domain_name
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
@@ -3890,25 +3823,25 @@
         cert_id: int = None,
         cert_name: str = None,
         common: str = None,
         fingerprint: str = None,
         issuer: str = None,
         last_time: int = None,
     ):
-        # The ID of the SSL certificate.
+        # The ID of the certificate.
         self.cert_id = cert_id
-        # The name of the SSL certificate.
+        # The name of the certificate.
         self.cert_name = cert_name
-        # The Common Name (CN) attribute of the SSL certificate. In most cases, the value is a domain name.
+        # The Common Name (CN) attribute of the certificate. In most cases, the CN is a domain name.
         self.common = common
-        # The fingerprint of the SSL certificate.
+        # The fingerprint of the certificate.
         self.fingerprint = fingerprint
-        # The certificate authority (CA) that issued the SSL certificate.
+        # The certificate authority (CA) that issued the certificate.
         self.issuer = issuer
-        # The timestamp when the SSL certificate was issued.
+        # The timestamp.
         self.last_time = last_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3984,17 +3917,17 @@
 
 class DescribeCdnCertificateListResponseBodyCertificateListModel(TeaModel):
     def __init__(
         self,
         cert_list: DescribeCdnCertificateListResponseBodyCertificateListModelCertList = None,
         count: int = None,
     ):
-        # The details about each SSL certificate.
+        # The list of certificates.
         self.cert_list = cert_list
-        # The number of SSL certificates returned.
+        # The number of certificates that are returned.
         self.count = count
 
     def validate(self):
         if self.cert_list:
             self.cert_list.validate()
 
     def to_map(self):
@@ -4021,15 +3954,15 @@
 
 class DescribeCdnCertificateListResponseBody(TeaModel):
     def __init__(
         self,
         certificate_list_model: DescribeCdnCertificateListResponseBodyCertificateListModel = None,
         request_id: str = None,
     ):
-        # The data type of the SSL certificate information.
+        # Details about certificates.
         self.certificate_list_model = certificate_list_model
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.certificate_list_model:
             self.certificate_list_model.validate()
@@ -4102,17 +4035,17 @@
 
 class DescribeCdnDeletedDomainsRequest(TeaModel):
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
     ):
-        # The number of the page to return. Pages start from page **1**. Valid values: **1** to **100000**.
+        # The number of the page to return. Valid values: **1** to **100000**. Default value: **1**.
         self.page_number = page_number
-        # The number of entries to return on each page. Default value: **20**. Valid values: **1** to **500**. The value must be an integer.
+        # The number of domain names to return per page. Valid values: an integer between **1** and **500**. Default value: **20**.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4139,15 +4072,15 @@
     def __init__(
         self,
         domain_name: str = None,
         gmt_modified: str = None,
     ):
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The last time when the accelerated domain name was modified. The time is in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC+0.
+        # The time when the accelerated domain name was modified. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.gmt_modified = gmt_modified
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4210,21 +4143,21 @@
         self,
         domains: DescribeCdnDeletedDomainsResponseBodyDomains = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The information about the accelerated domain names.
+        # The list of accelerated domain names and the time each domain name was last modified.
         self.domains = domains
-        # The page number of the returned page. It corresponds to the request parameter **PageNumber**.
+        # The page number of the returned page, which is the same as the **PageNumber** parameter in request parameters.
         self.page_number = page_number
-        # The number of entries returned per page. It corresponds to the request parameter **PageSize**.
+        # The number of domain names returned per page, which is the same as the **PageSize** parameter in request parameters.
         self.page_size = page_size
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
         # The total number of domain names returned.
         self.total_count = total_count
 
     def validate(self):
         if self.domains:
             self.domains.validate()
@@ -4416,22 +4349,22 @@
 
 class DescribeCdnDomainByCertificateRequest(TeaModel):
     def __init__(
         self,
         sslpub: str = None,
         sslstatus: bool = None,
     ):
-        # The public key of the SSL certificate. You must encode the public key in Base64 and then call the encodeURIComponent function to encode the public key again.
+        # The public key of the SSL certificate. You must encode the public key in Base64 before you invoke the encodeURIComponent function to encode a URI component.
         # 
-        # The public key must be in the Privacy-Enhanced Mail (PEM) format.
+        # A public key in the Privacy Enhanced Mail (PEM) format is supported.
         self.sslpub = sslpub
-        # Specifies whether the domain name list to return contains only domain names with HTTPS enabled or disabled.
+        # Specifies whether to return only domain names with HTTPS enabled or disabled.
         # 
-        # *   true: The list contains only domain names with HTTPS enabled.
-        # *   false: The list contains only domain names with HTTPS disabled.
+        # *   true: returns only domain names with HTTPS enabled.
+        # *   false: returns only domain names with HTTPS disabled.
         self.sslstatus = sslstatus
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4465,31 +4398,31 @@
         cert_type: str = None,
         domain_list: str = None,
         domain_names: str = None,
         issuer: str = None,
     ):
         # Indicates whether the SSL certificate is obsolete. Valid values:
         # 
-        # *   **yes**: The SSL certificate is obsolete.
-        # *   **no**: The SSL certificate is working as expected.
+        # *   **yes**\
+        # *   **no**\
         self.cert_ca_is_legacy = cert_ca_is_legacy
-        # The time at which the certificate expires.
+        # The expiration time of the certificate.
         self.cert_expire_time = cert_expire_time
         # Indicates whether the SSL certificate is expired. Valid values:
         # 
-        # *   **yes**: The SSL certificate is expired.
-        # *   **no**: The SSL certificate is not expired.
+        # *   **yes**\
+        # *   **no**\
         self.cert_expired = cert_expired
-        # The time at which the certificate became effective.
+        # The effective time of the certificate.
         self.cert_start_time = cert_start_time
         # The name of the SSL certificate owner.
         self.cert_subject_common_name = cert_subject_common_name
         # The type of the certificate. Valid values: **RSA**, **DSA**, and **ECDSA**.
         self.cert_type = cert_type
-        # If a value is returned, the value matches the SSL certificate. Multiple domain names are separated by commas (,).
+        # The list of domain names. If a value is returned, the value matches the SSL certificate. Multiple domain names are separated by commas (,).
         self.domain_list = domain_list
         # The domain names (DNS fields) that match the SSL certificate. Multiple domain names are separated by commas (,).
         self.domain_names = domain_names
         # The certificate authority (CA) that issued the certificate.
         self.issuer = issuer
 
     def validate(self):
@@ -4667,17 +4600,17 @@
         domain_name: str = None,
         function_names: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
         # The ID of the configuration. For more information about ConfigId, see [Usage notes on ConfigId](~~388994~~).
         self.config_id = config_id
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name
-        # The names of the features. Separate multiple feature names with commas (,). For more information, see [BatchSetCdnDomainConfig](~~388460~~).
+        # The names of the features. Separate multiple feature names with commas (,). For more information, see [Parameters for configuring features for domain names](~~388460~~).
         self.function_names = function_names
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
@@ -4795,15 +4728,17 @@
     ):
         # The ID of the configuration.
         self.config_id = config_id
         # The configuration of each feature.
         self.function_args = function_args
         # The name of the feature.
         self.function_name = function_name
-        # The ID of the rule condition. This parameter is optional. To create a rule condition, you can configure the **condition** feature that is described in the [BatchSetCdnDomainConfig and SetCdnDomainStagingConfig](~~388460~~) topic. A rule condition can identify parameters that are included in requests and filter requests based on the identified parameters. Each rule condition has a [ConfigId](~~388994~~). You can use ConfigId as ParentId that is referenced by other features. This way, you can combine rule conditions and features for flexible configurations.
+        # The ID of the rule condition. This parameter is optional.
+        # 
+        # To create a rule condition, you can configure the **condition** feature that is described in the [Parameters for configuring features for domain names](~~388460~~) topic. A rule condition can identify parameters that are included in requests and filter requests based on the identified parameters. Each rule condition has a [ConfigId](~~388994~~). You can use ConfigId as ParentId that is referenced by other features. This way, you can combine rule conditions and features for flexible configurations.
         # 
         # For more information, see [BatchSetCdnDomainConfig](~~90915~~) or ParentId configuration example in this topic.
         self.parent_id = parent_id
         # The status of the configuration. Valid values:
         # 
         # *   **success**\
         # *   **testing**\
@@ -5021,17 +4956,17 @@
         self.enabled = enabled
         # The port over which requests are redirected to the origin server. Ports 443 and 80 are supported.
         self.port = port
         # The priority.
         self.priority = priority
         # The type of the origin server. Valid values:
         # 
-        # *   **ipaddr:** an IP address.
-        # *   **domain:** a domain name
-        # *   **oss:** the OSS domain of an Object Storage Service (OSS) bucket
+        # *   **ipaddr**: an origin IP address
+        # *   **domain**: an origin domain name
+        # *   **oss**: the domain name of an Object Storage Service (OSS) bucket
         # *   **fc_domain:** a Function Compute domain name
         self.type = type
         # The weight of the origin server if multiple origin servers have been specified.
         self.weight = weight
 
     def validate(self):
         pass
@@ -5128,38 +5063,40 @@
         # 
         # *   **web**: images and small files
         # *   **download**: large files
         # *   **video**: on-demand video and audio streaming
         self.cdn_type = cdn_type
         # The CNAME that is assigned to the accelerated domain name. You must add the CNAME record in the system of your DNS service provider to map the accelerated domain name to the CNAME.
         self.cname = cname
-        # The description of the request.
+        # The description of the domain name.
         self.description = description
         # The accelerated domain name.
         self.domain_name = domain_name
         # The status of the accelerated domain name. Valid values:
         # 
-        # *   **online:** enabled
-        # *   **offline:** disabled
-        # *   **configuring:** configuring
-        # *   **configure_failed:** configuration failed
-        # *   **checking:** reviewing
-        # *   **check_failed:** review failed
+        # *   **online**\
+        # *   **offline**\
+        # *   **configuring**\
+        # *   **configure_failed**\
+        # *   **checking**\
+        # *   **check_failed**\
+        # *   **stopping**\
+        # *   **deleting**\
         self.domain_status = domain_status
-        # The time when the audio or video file was created.
+        # The time when the domain name was created.
         self.gmt_created = gmt_created
         # The time when the domain name was last modified.
         self.gmt_modified = gmt_modified
         # The CNAME for which HTTPS is enabled.
         self.https_cname = https_cname
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         # The acceleration region.
         self.scope = scope
-        # Indicates whether the Security Socket Layer (SSL) certificate is enabled. Valid values:
+        # Indicates whether the SSL certificate is enabled. Valid values:
         # 
         # *   **on**\
         # *   **off**\
         self.server_certificate_status = server_certificate_status
         # The information about the origin server.
         self.source_models = source_models
 
@@ -5677,15 +5614,15 @@
 
 class DescribeCdnDomainStagingConfigRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         function_names: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name
         # The list of feature names. Separate multiple values with commas (,). For more information, see [A list of features](~~388460~~).
         self.function_names = function_names
 
     def validate(self):
         pass
 
@@ -5712,17 +5649,17 @@
 
 class DescribeCdnDomainStagingConfigResponseBodyDomainConfigsFunctionArgs(TeaModel):
     def __init__(
         self,
         arg_name: str = None,
         arg_value: str = None,
     ):
-        # The name of the configuration.
+        # The configuration name.
         self.arg_name = arg_name
-        # The value of the configuration.
+        # The configuration value.
         self.arg_value = arg_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5750,30 +5687,28 @@
         self,
         config_id: str = None,
         function_args: List[DescribeCdnDomainStagingConfigResponseBodyDomainConfigsFunctionArgs] = None,
         function_name: str = None,
         parent_id: str = None,
         status: str = None,
     ):
-        # The ID of the configuration.
+        # The configuration ID.
         self.config_id = config_id
         # The description of each feature.
         self.function_args = function_args
-        # The name of the feature.
+        # The feature name.
         self.function_name = function_name
-        # The ID of the rule condition. This parameter is optional. To create a rule condition, you can configure the **condition** feature that is described in the [BatchSetCdnDomainConfig and SetCdnDomainStagingConfig](~~388460~~) topic. A rule condition can identify parameters that are included in requests and filter requests based on the identified parameters. Each rule condition has a [ConfigId](~~388994~~). You can use ConfigId as ParentId that is referenced by other features. This way, you can combine rule conditions and features for flexible configurations.
-        # 
-        # For more information, see [BatchSetCdnDomainConfig](~~90915~~) or ParentId configuration example in this topic.
+        # The rule condition ID. This parameter is optional. To create a rule condition, you can configure the **condition** feature that is described in the [Parameters for configuring features for domain names](~~388460~~) topic. A rule condition can identify parameters that are included in requests and filter requests based on the identified parameters. Each rule condition has a [ConfigId](~~388994~~). You can reference ConfigId instead of ParentId in other features. This way, you can combine rule conditions and features for flexible configurations. For more information, see [BatchSetCdnDomainConfig](~~90915~~) or ParentId configuration example in this topic.
         self.parent_id = parent_id
-        # The status of the configuration. Valid values:
+        # The configuration status. Valid values:
         # 
-        # *   **testing**: being verified
-        # *   **configuring**: being configured
-        # *   **success**: configured
-        # *   **failed**: failed
+        # *   **testing**\
+        # *   **configuring**\
+        # *   **success**\
+        # *   **failed**\
         self.status = status
 
     def validate(self):
         if self.function_args:
             for k in self.function_args:
                 if k:
                     k.validate()
@@ -5819,19 +5754,19 @@
 class DescribeCdnDomainStagingConfigResponseBody(TeaModel):
     def __init__(
         self,
         domain_configs: List[DescribeCdnDomainStagingConfigResponseBodyDomainConfigs] = None,
         domain_name: str = None,
         request_id: str = None,
     ):
-        # The configurations of the domain name.
+        # The domain name configurations.
         self.domain_configs = domain_configs
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.domain_configs:
             for k in self.domain_configs:
                 if k:
                     k.validate()
@@ -6315,15 +6250,15 @@
 
 class DescribeCdnRegionAndIspResponseBodyIspsIsp(TeaModel):
     def __init__(
         self,
         name_en: str = None,
         name_zh: str = None,
     ):
-        # The English name of the region.
+        # The English name of the ISP.
         self.name_en = name_en
         # The Chinese name of the ISP.
         self.name_zh = name_zh
 
     def validate(self):
         pass
 
@@ -6456,17 +6391,17 @@
 class DescribeCdnRegionAndIspResponseBody(TeaModel):
     def __init__(
         self,
         isps: DescribeCdnRegionAndIspResponseBodyIsps = None,
         regions: DescribeCdnRegionAndIspResponseBodyRegions = None,
         request_id: str = None,
     ):
-        # A list of ISPs.
+        # The list of ISPs.
         self.isps = isps
-        # A list of regions.
+        # The list of regions.
         self.regions = regions
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.isps:
             self.isps.validate()
@@ -6551,40 +6486,40 @@
         domain_name: str = None,
         end_time: str = None,
         http_code: str = None,
         is_overseas: str = None,
         report_id: int = None,
         start_time: str = None,
     ):
-        # The region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
+        # The region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         # 
-        # *   If you do not specify a region, all regions are queried.
-        # *   If you specify a region, data in the specified region is returned. You can specify one or more regions. Separate regions with commas (,).
+        # *   If you do not specify a region, data in all regions is queried.
+        # *   If you specify a region, data in the specified region is queried. You can specify one or more regions. If you specify multiple regions, separate the regions with commas (,).
         self.area = area
-        # The domain names that you want to query. Separate domain names with commas (,).
+        # The domain name that you want to query. Separate domain names with commas (,).
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time
         # The HTTP status code. Valid values:
         # 
-        # *   **2xx**: HTTP 2xx status codes
-        # *   **3xx**: HTTP 3xx status codes
-        # *   **4xx**: HTTP 4xx status codes
-        # *   **5xx**: HTTP 5xx status codes
+        # *   **2xx**\
+        # *   **3xx**\
+        # *   **4xx**\
+        # *   **5xx**\
         # 
-        # If you do not specify an HTTP status code, all HTTP status codes are queried.
+        # If you do not specify this parameter, all HTTP status codes are queried.
         self.http_code = http_code
-        # Specify whether the region is outside the Chinese mainland. Valid values:
+        # Specifies whether the region is outside the Chinese mainland. Valid values:
         # 
         # *   **1**: outside the Chinese mainland
         # *   **0**: inside the Chinese mainland
         self.is_overseas = is_overseas
-        # The ID of the operations report that you want to query. You can enter only one ID in each call. You can call the [DescribeCdnSubList](~~271655~~) operation to query the report ID.
+        # The ID of the operations report that you want to query. You can specify only one ID in each request. You can call the [DescribeCdnSubList](~~271655~~) operation to query report IDs.
         self.report_id = report_id
-        # The beginning of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6736,15 +6671,15 @@
 
 class DescribeCdnReportListResponseBody(TeaModel):
     def __init__(
         self,
         content: str = None,
         request_id: str = None,
     ):
-        # The information about the operations report.
+        # The information about the report that is queried.
         self.content = content
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
@@ -6862,27 +6797,27 @@
         cert_org: str = None,
         common_name: str = None,
         encrypt_certificate: str = None,
         request_id: str = None,
         sans: str = None,
         sign_certificate: str = None,
     ):
-        # The time when the certificate expires. The time is displayed in UTC.
+        # The name of the certificate.
         self.cert_expire_time = cert_expire_time
         # The ID of the certificate.
         self.cert_identifier = cert_identifier
-        # The name of the certificate.
+        # The time when the certificate expires. The time is displayed in UTC.
         self.cert_name = cert_name
         # The certificate authority (CA) that issued the certificate.
         self.cert_org = cert_org
         # The top-level domain name.
         self.common_name = common_name
-        # The content of the encryption certificate.
-        self.encrypt_certificate = encrypt_certificate
         # The ID of the request.
+        self.encrypt_certificate = encrypt_certificate
+        # The content of the encryption certificate.
         self.request_id = request_id
         # The subdomain name.
         self.sans = sans
         # The content of the signature certificate.
         self.sign_certificate = sign_certificate
 
     def validate(self):
@@ -7107,15 +7042,15 @@
 
 class DescribeCdnSMCertificateListResponseBodyCertificateListModel(TeaModel):
     def __init__(
         self,
         cert_list: DescribeCdnSMCertificateListResponseBodyCertificateListModelCertList = None,
         count: int = None,
     ):
-        # A list of certificates.
+        # The list of certificates.
         self.cert_list = cert_list
         # The number of certificates that are returned.
         self.count = count
 
     def validate(self):
         if self.cert_list:
             self.cert_list.validate()
@@ -7257,15 +7192,15 @@
 
 
 class DescribeCdnServiceResponseBodyOperationLocksLockReason(TeaModel):
     def __init__(
         self,
         lock_reason: str = None,
     ):
-        # The reason why Alibaba Cloud CDN is locked. A value of financial indicates that the service is locked due to overdue payments.
+        # The reason why the service is locked. A value of financial indicates that the service is locked due to overdue payments.
         self.lock_reason = lock_reason
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7326,31 +7261,31 @@
         changing_charge_type: str = None,
         instance_id: str = None,
         internet_charge_type: str = None,
         opening_time: str = None,
         operation_locks: DescribeCdnServiceResponseBodyOperationLocks = None,
         request_id: str = None,
     ):
-        # The time when the next billing method takes effect. The time is displayed in GMT.
+        # The time when the metering method for the next cycle takes effect. The time is displayed in GMT.
         self.changing_affect_time = changing_affect_time
-        # The next billing method that Alibaba Cloud CDN will use. Valid values:
+        # The metering method for the next cycle. Valid values:
         # 
-        # *   **PayByTraffic**: pay-by-data-transfer.
-        # *   **PayByBandwidth**: pay-by-bandwidth.
+        # *   **PayByTraffic**: pay-by-data-transfer
+        # *   **PayByBandwidth**: pay-by-bandwidth
         self.changing_charge_type = changing_charge_type
         # The ID of the instance.
         self.instance_id = instance_id
-        # The current billing method of Alibaba Cloud CDN.
+        # The current metering method. Valid values:
         # 
-        # *   **PayByTraffic**: pay-by-data-transfer.
-        # *   **PayByBandwidth**: pay-by-bandwidth.
+        # *   **PayByTraffic**: pay-by-data-transfer
+        # *   **PayByBandwidth**: pay-by-bandwidth
         self.internet_charge_type = internet_charge_type
-        # The time when Alibaba Cloud CDN was activated. The time follows the ISO 8601 standard in the yyyy-MM-ddThh:mmZ format.
+        # The time when the service was activated. The time follows the ISO 8601 standard.
         self.opening_time = opening_time
-        # The lock status of Alibaba Cloud CDN.
+        # The lock status.
         self.operation_locks = operation_locks
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.operation_locks:
             self.operation_locks.validate()
@@ -7443,17 +7378,15 @@
 
 class DescribeCdnSubListResponseBody(TeaModel):
     def __init__(
         self,
         content: str = None,
         request_id: str = None,
     ):
-        # The information about the custom report.
         self.content = content
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7837,35 +7770,35 @@
         area: str = None,
         dimension: str = None,
         end_time: str = None,
         start_time: str = None,
     ):
         # The billable region. Valid values:
         # 
-        # *   **CN**: Chinese mainland
+        # *   **CN**: the Chinese mainland
         # *   **OverSeas**: outside the Chinese mainland
         # *   **AP1**: Asia Pacific 1
         # *   **AP2**: Asia Pacific 2
         # *   **AP3**: Asia Pacific 3
         # *   **NA**: North America
         # *   **SA**: South America
         # *   **EU**: Europe
         # *   **MEAA**: Middle East and Africa
         # 
-        # The default value is the current metering method. Regions inside and outside the Chinese mainland are classified into the **CN** or **OverSeas** billable regions. Billable regions inside the Chinese mainland include **CN**. Billable regions outside the Chinese mainland include **AP1**, **AP2**, **AP3**, **NA**, **SA**, **EU**, and **MEAA**.
+        # By default, the value of this parameter is determined by the metering method that is currently used. Regions inside and outside the Chinese mainland are classified into the **CN** and **OverSeas** billable regions. Billable regions inside the Chinese mainland include **CN**. Billable regions outside the Chinese mainland include **AP1**, **AP2**, **AP3**, **NA**, **SA**, **EU**, and **MEAA**.
         # 
-        # >  For more information about billable regions, see [Billable regions](~~142221~~).
+        # > For more information about billable regions, see [Billable regions](~~142221~~).
         self.area = area
-        # The billable item. A value of flow indicates bandwidth.
+        # The billable item. A value of flow specifies bandwidth.
         self.dimension = dimension
-        # The default value is the current time. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end time of the estimation. The default value is the current time. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The default value is 00:00 on the first day of the current month. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The start time of the estimation. The default value is 00:00 on the first day of the current month. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7901,15 +7834,15 @@
         self,
         area: str = None,
         time_stp: str = None,
         value: float = None,
     ):
         # The billable region.
         self.area = area
-        # The time when the value used as the estimated value is generated. This field is returned only if the metering method is pay by 95th percentile, pay by 95th percentile bandwidth with 50% off from 00:00 to 08:00, or pay by 4th peak bandwidth per month.
+        # The time when the value used as the estimated value is generated. This parameter is returned only if the metering method is pay by 95th percentile, pay by 95th percentile bandwidth with 50% off from 00:00 to 08:00, or pay by 4th peak bandwidth per month.
         self.time_stp = time_stp
         # The estimated value.
         self.value = value
 
     def validate(self):
         pass
 
@@ -7978,31 +7911,31 @@
         self,
         bill_prediction_data: DescribeCdnUserBillPredictionResponseBodyBillPredictionData = None,
         bill_type: str = None,
         end_time: str = None,
         request_id: str = None,
         start_time: str = None,
     ):
-        # The list of bill prediction data.
+        # The estimated bill data.
         self.bill_prediction_data = bill_prediction_data
         # The metering method.
         # 
-        # >  If the metering method ends with **\_overseas**, it indicates that the billable region is outside the Chinese mainland. For example, BillType": "month_avg_day_bandwidth_overseas specifies a billable region outside the Chinese mainland and that the metering method is pay by daily peak bandwidth per month.
+        # > If the metering method ends with \_overseas, the billable region is outside the Chinese mainland. For example, BillType": "month_avg_day_bandwidth_overseas specifies a billable region outside the Chinese mainland and that the metering method is pay by daily peak bandwidth per month.
         # 
         # Valid values:
         # 
-        # *   hour_flow: pay by hourly data transfer.
-        # *   day_bandwidth: pay by daily bandwidth.
+        # *   hour_flow: pay by hourly data transfer
+        # *   day_bandwidth: pay by daily bandwidth
         # *   month\_95: pay by monthly 95th percentile bandwidth.
-        # *   month_avg_day_bandwidth: pay by average daily peak bandwidth per month.
-        # *   month\_4th_day_bandwidth: pay by 4th peak bandwidth per month.
-        # *   month_avg_day\_95: pay by average daily 95th percentile bandwidth per month.
+        # *   month_avg_day_bandwidth: pay by average daily peak bandwidth per month
+        # *   month\_4th_day_bandwidth: pay by monthly 4th peak bandwidth
+        # *   month_avg_day\_95: pay by average daily 95th percentile bandwidth per month
         # *   month\_95\_night_half: pay by 95th percentile bandwidth with 50% off from 00:00 to 08:00.
-        # *   hour_vas: pay by value-added services on an hourly basis.
-        # *   day_count: pay by the number of requests per day.
+        # *   hour_vas: pay by value-added services per hour
+        # *   day_count: pay by daily requests
         self.bill_type = bill_type
         # The end time of the estimation.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
         # The start time of the estimation.
         self.start_time = start_time
@@ -8332,18 +8265,17 @@
 
 
 class DescribeCdnUserConfigsRequest(TeaModel):
     def __init__(
         self,
         function_name: str = None,
     ):
-        # The configuration item that you want to query. Valid values:
+        # The name of the parameter.
         # 
-        # *   **domain\_business\_control**: Alibaba Cloud CDN configurations
-        # *   **waf**: Web Application Firewall (WAF) configurations
+        # The configurations set by enterprise or government users.
         self.function_name = function_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8365,29 +8297,30 @@
 class DescribeCdnUserConfigsResponseBodyConfigs(TeaModel):
     def __init__(
         self,
         arg_name: str = None,
         arg_value: str = None,
         function_name: str = None,
     ):
-        # The name of the parameter.
-        # 
-        # The configurations set by enterprise or government users.
+        # The name of the feature.
         self.arg_name = arg_name
         # The value of the configuration. Valid values:
         # 
         # *   **cc_rule**: HTTP flood protection rules
         # *   **ddos_dispatch**: integration with Anti-DDoS
         # *   **edge_safe**: application security settings on edge nodes
         # *   **blocked_regions**: blocked regions
-        # *   **http\_acl\_policy**: access control list (ACL) rules
+        # *   **http_acl_policy**: access control list (ACL) rules
         # *   **bot_manager**: bot traffic management
         # *   **ip_reputation**: IP reputation library
         self.arg_value = arg_value
-        # The name of the feature.
+        # The configuration item that you want to query. Valid values:
+        # 
+        # *   **domain_business_control**: Alibaba Cloud CDN configurations
+        # *   **waf**: Web Application Firewall (WAF) configurations
         self.function_name = function_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8416,17 +8349,17 @@
 
 class DescribeCdnUserConfigsResponseBody(TeaModel):
     def __init__(
         self,
         configs: List[DescribeCdnUserConfigsResponseBodyConfigs] = None,
         request_id: str = None,
     ):
-        # The configurations of Alibaba Cloud CDN.
+        # >  The maximum number of times that each user can call this operation per second is 30.
         self.configs = configs
-        # The ID of the request.
+        # The name of the feature.
         self.request_id = request_id
 
     def validate(self):
         if self.configs:
             for k in self.configs:
                 if k:
                     k.validate()
@@ -8505,25 +8438,17 @@
     def __init__(
         self,
         func_id: int = None,
         page_number: int = None,
         page_size: int = None,
         resource_group_id: str = None,
     ):
-        # The ID of the feature. For more information about how to query feature IDs, see [Feature settings for a domain name](~~388460~~). For example, the ID of the origin host feature (set_req_host_header) is 18.
         self.func_id = func_id
-        # The number of the page to return. Default value: **1**.
-        # 
-        # Valid values: **1** to **100000**.
         self.page_number = page_number
-        # The number of entries to return on each page. Default value: **20**.
-        # 
-        # Valid values: **1** to **50**.
         self.page_size = page_size
-        # The ID of the resource group.
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8559,28 +8484,18 @@
         self,
         content: str = None,
         port: int = None,
         priority: str = None,
         type: str = None,
         weight: str = None,
     ):
-        # The address of the origin server.
         self.content = content
-        # The port of the origin server.
         self.port = port
-        # The priority.
         self.priority = priority
-        # The type of the origin server. Valid values:
-        # 
-        # *   **ipaddr**: an origin IP address
-        # *   **domain:** a domain name
-        # *   **oss:** the OSS domain of an Object Storage Service (OSS) bucket
-        # *   **fc_domain:** a Function Compute domain name
         self.type = type
-        # The weight of the origin server if multiple origin servers have been specified.
         self.weight = weight
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8660,50 +8575,23 @@
         domain_status: str = None,
         gmt_created: str = None,
         gmt_modified: str = None,
         resource_group_id: str = None,
         sources: DescribeCdnUserDomainsByFuncResponseBodyDomainsPageDataSources = None,
         ssl_protocol: str = None,
     ):
-        # The type of the workload accelerated by Alibaba Cloud CDN. Valid values:
-        # 
-        # *   **web**: image and small file distribution
-        # *   **download**: large file distribution
-        # *   **video**: on-demand video and audio streaming
-        # *   **liveStream**: live streaming
         self.cdn_type = cdn_type
-        # The CNAME assigned to the accelerated domain name.
         self.cname = cname
-        # The description of the accelerated domain name.
         self.description = description
-        # The accelerated domain name.
         self.domain_name = domain_name
-        # The status of the accelerated domain name. Valid values:
-        # 
-        # *   **online:** enabled
-        # *   **offline:** disabled
-        # *   **configuring:** configuring
-        # *   **configure_failed:** configuration failed
-        # *   **checking:** reviewing
-        # *   **check_failed**: failed the review
-        # *   **stopping**: being disabled
-        # *   **deleting**: deleting
         self.domain_status = domain_status
-        # The time when the accelerated domain name was added.
         self.gmt_created = gmt_created
-        # The time when the accelerated domain name was modified.
         self.gmt_modified = gmt_modified
-        # The ID of the resource group.
         self.resource_group_id = resource_group_id
-        # The information about the origin server.
         self.sources = sources
-        # Indicates whether HTTPS is enabled. Valid values:
-        # 
-        # *   **on**\
-        # *   **off**\
         self.ssl_protocol = ssl_protocol
 
     def validate(self):
         if self.sources:
             self.sources.validate()
 
     def to_map(self):
@@ -8800,23 +8688,18 @@
         self,
         domains: DescribeCdnUserDomainsByFuncResponseBodyDomains = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The configurations of the accelerated domain name.
         self.domains = domains
-        # The page number of the returned page.
         self.page_number = page_number
-        # The number of entries returned per page.
         self.page_size = page_size
-        # The ID of the request.
         self.request_id = request_id
-        # The total number of domain names returned.
         self.total_count = total_count
 
     def validate(self):
         if self.domains:
             self.domains.validate()
 
     def to_map(self):
@@ -8946,15 +8829,15 @@
         refresh_url_remain: int = None,
         request_id: str = None,
     ):
         # The maximum number of URLs and directories that can be blocked.
         self.block_quota = block_quota
         # The remaining number of URLs and directories that can be blocked.
         self.block_remain = block_remain
-        # The maximum number of accelerated domain names that can be added to Alibaba Cloud CDN.
+        # The maximum number of accelerated domain names.
         self.domain_quota = domain_quota
         self.ignore_params_quota = ignore_params_quota
         self.ignore_params_remain = ignore_params_remain
         # The maximum number of URLs that can be prefetched.
         self.preload_quota = preload_quota
         # The remaining number of URLs that can be prefetched.
         self.preload_remain = preload_remain
@@ -9082,18 +8965,18 @@
         self,
         owner_id: int = None,
         security_token: str = None,
         status: str = None,
     ):
         self.owner_id = owner_id
         self.security_token = security_token
-        # Resource plan status:
+        # The remaining quota of the resource plan.
         # 
-        # *   **valid**: valid
-        # *   **closed**: invalid
+        # *   The total amount of data transfer provided by the resource plan. Unit: bytes.
+        # *   The remaining number of requests provided by the resource plan.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9129,40 +9012,37 @@
         end_time: str = None,
         init_capacity: str = None,
         instance_id: str = None,
         start_time: str = None,
         status: str = None,
         template_name: str = None,
     ):
-        # The ID of the resource plan.
-        self.commodity_code = commodity_code
-        # The remaining quota of the resource plan.
+        # The total quota of the resource plan.
         # 
         # *   The total amount of data transfer provided by the resource plan. Unit: bytes.
-        # *   The remaining number of requests provided by the resource plan.
+        # *   The total number of requests provided by the resource plan.
+        self.commodity_code = commodity_code
+        # The ID of the instance.
         self.curr_capacity = curr_capacity
-        # The name of the resource plan.
+        # The time when the resource plan took effect.
         self.display_name = display_name
-        # The time when the resource plan expires.
+        # The operation that you want to perform. Set the value to **DescribeCdnUserResourcePackage**.
         self.end_time = end_time
-        # The total quota of the resource plan.
-        # 
-        # *   The total amount of data transfer provided by the resource plan. Unit: bytes.
-        # *   The total number of requests provided by the resource plan.
+        # The ID of the resource plan.
         self.init_capacity = init_capacity
-        # The ID of the instance.
+        # The ID of the request.
         self.instance_id = instance_id
-        # The time when the resource plan took effect.
+        # The name of the template.
         self.start_time = start_time
         # The status of the data transfer plan. Valid values:
         # 
         # *   **valid**: valid
         # *   **closed**: invalid
         self.status = status
-        # The name of the template.
+        # The details about each resource plan. The details are organized in an array. The array consists of the subparameter values of the ResourcePackageInfo parameter.
         self.template_name = template_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9250,17 +9130,17 @@
 
 class DescribeCdnUserResourcePackageResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_package_infos: DescribeCdnUserResourcePackageResponseBodyResourcePackageInfos = None,
     ):
-        # The ID of the request.
+        # The name of the resource plan.
         self.request_id = request_id
-        # The details about each resource plan. The details are organized in an array. The array consists of the subparameter values of the ResourcePackageInfo parameter.
+        # The time when the resource plan expires.
         self.resource_package_infos = resource_package_infos
 
     def validate(self):
         if self.resource_package_infos:
             self.resource_package_infos.validate()
 
     def to_map(self):
@@ -9332,17 +9212,28 @@
 class DescribeCdnWafDomainRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
-        # The accelerated domain name.
+        # The domain name that you want to query.
+        # 
+        # You can specify only one domain name in each request. You have three options to configure this parameter:
+        # 
+        # *   Specify an exact domain name. For example, if you set this parameter to example.com, configuration information of example.com is queried.
+        # *   Specify a keyword. For example, if you set this parameter to example, configuration information about all domain names that contain example is queried.
+        # *   Leave this parameter empty. If this parameter is left empty, all accelerated domain names for which WAF is configured are queried.
         self.domain_name = domain_name
-        # The ID of the region.
+        # The region where WAF is enabled. Valid values:
+        # 
+        # *   **cn-hangzhou**: inside the Chinese mainland
+        # *   **ap-southeast-1**: outside the Chinese mainland
+        # 
+        # > ap-southeast-1 includes Hong Kong (China), Macao (China), Taiwan (China), and other countries and regions.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
@@ -9376,19 +9267,36 @@
         self,
         acl_status: str = None,
         cc_status: str = None,
         domain: str = None,
         status: str = None,
         waf_status: str = None,
     ):
+        # The status of the access control list (ACL) feature. Valid values:
+        # 
+        # *   **0**: disabled
+        # *   **1**: enabled
         self.acl_status = acl_status
+        # The status of protection against HTTP flood attacks. Valid values:
+        # 
+        # *   **0**: disabled
+        # *   **1**: enabled
         self.cc_status = cc_status
-        # The domain name.
+        # The accelerated domain name.
         self.domain = domain
+        # The WAF status of the domain name. Valid values:
+        # 
+        # *   **1**: The domain name is added to WAF or valid.
+        # *   **10**: The domain name is being added to WAF.
+        # *   **11**: The domain name failed to be added to WAF.
         self.status = status
+        # The status of WAF. Valid values:
+        # 
+        # *   **0**: disabled
+        # *   **1**: enabled
         self.waf_status = waf_status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9426,18 +9334,19 @@
 class DescribeCdnWafDomainResponseBody(TeaModel):
     def __init__(
         self,
         out_put_domains: List[DescribeCdnWafDomainResponseBodyOutPutDomains] = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The information about the accelerated domain name.
         self.out_put_domains = out_put_domains
         # The ID of the request.
         self.request_id = request_id
-        # The total number of entries returned.
+        # The number of accelerated domain names.
         self.total_count = total_count
 
     def validate(self):
         if self.out_put_domains:
             for k in self.out_put_domains:
                 if k:
                     k.validate()
@@ -9766,21 +9675,21 @@
     def __init__(
         self,
         remark: str = None,
         request_id: str = None,
         sample: str = None,
         tag: str = None,
     ):
-        # The format of the log configuration.
+        # The operation that you want to perform. Set the value to **DescribeCustomLogConfig**.
         self.remark = remark
         # The ID of the request.
         self.request_id = request_id
         # A sample log configuration.
         self.sample = sample
-        # The tag information about the log configuration.
+        # The format of the log configuration.
         self.tag = tag
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9863,37 +9772,35 @@
         end_time: str = None,
         interval: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
         time_merge: str = None,
     ):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
-        # 
-        # By default, this operation queries the bandwidth values during back-to-origin routing for all accelerated domain names that belong to your Alibaba Cloud account.
+        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you do not set this parameter, all ISPs are queried.
         self.domain_name = domain_name
-        # The type of the query condition. Valid values: When you set the value to dynamic, this operation queries the average response time of dynamic resources and static resources. If you do not set this parameter, this operation queries the average response time of only static resources. By default, this parameter is not set.
-        self.domain_type = domain_type
-        # The end of the time range queried. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # The end time must be later than the start time.
-        self.end_time = end_time
         # The time interval between the data entries. Unit: seconds. The value varies based on the values of the **StartTime** and **EndTime** parameters. Valid values:
         # 
         # *   If the time span between StartTime and EndTime is less than 3 days (3 days excluded), valid values are **300**, **3600**, and **86400**. Default value: **300**.
         # *   If the time span between StartTime and EndTime is from 3 to 31 days (31 days excluded), valid values are **3600** and **86400**. Default value: **3600**.
         # *   If the time range between StartTime and EndTime is 31 days or longer, the valid value is **86400**. Default value: **86400**.
+        self.domain_type = domain_type
+        # The end of the time range during which data was queried.
+        self.end_time = end_time
+        # The beginning of the time range during which data was queried.
         self.interval = interval
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you do not set this parameter, all ISPs are queried.
+        # The ID of the request.
         self.isp_name_en = isp_name_en
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
+        # The accelerated domain name.
         self.location_name_en = location_name_en
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
         self.start_time = start_time
-        # Specifies whether to automatically set the interval. If you set the value to 1, the value of the Interval parameter is automatically assigned based on the StartTime and EndTime parameters. You can set this parameter or the Interval parameter.
+        # The end of the time range queried. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # The end time must be later than the start time.
         self.time_merge = time_merge
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9942,17 +9849,17 @@
 
 class DescribeDomainAverageResponseTimeResponseBodyAvgRTPerIntervalDataModule(TeaModel):
     def __init__(
         self,
         time_stamp: str = None,
         value: str = None,
     ):
-        # The timestamp of the returned data.
+        # The accelerated domain name.
         self.time_stamp = time_stamp
-        # The average response time.
+        # The type of the query condition. Valid values: When you set the value to dynamic, this operation queries the average response time of dynamic resources and static resources. If you do not set this parameter, this operation queries the average response time of only static resources. By default, this parameter is not set.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10016,25 +9923,29 @@
         avg_rtper_interval: DescribeDomainAverageResponseTimeResponseBodyAvgRTPerInterval = None,
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         request_id: str = None,
         start_time: str = None,
     ):
-        # The average response time collected at each time interval.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
         self.avg_rtper_interval = avg_rtper_interval
-        # The time interval between the data entries returned.
+        # The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.  
+        # 
+        # > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        # - You can call this operation up to 100 times per second per account.
+        # - You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
         self.data_interval = data_interval
-        # The accelerated domain name.
+        # The timestamp of the returned data.
         self.domain_name = domain_name
-        # The end of the time range during which data was queried.
+        # The time interval between the data entries returned.
         self.end_time = end_time
-        # The ID of the request.
+        # The average response time.
         self.request_id = request_id
-        # The beginning of the time range during which data was queried.
+        # The average response time collected at each time interval.
         self.start_time = start_time
 
     def validate(self):
         if self.avg_rtper_interval:
             self.avg_rtper_interval.validate()
 
     def to_map(self):
@@ -10125,35 +10036,19 @@
         domain_name: str = None,
         end_time: str = None,
         interval: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
-        # 
-        # By default, this operation queries bandwidth data for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time granularity of the data entries. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
-        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
-        # 
-        # If you do not set this parameter, data of all ISPs is queried.
         self.isp_name_en = isp_name_en
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
-        # 
-        # If you do not specify a region, data in all regions is queried.
         self.location_name_en = location_name_en
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10199,27 +10094,20 @@
         https_domestic_value: str = None,
         https_overseas_value: str = None,
         https_value: str = None,
         overseas_value: str = None,
         time_stamp: str = None,
         value: str = None,
     ):
-        # The bandwidth value in the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.domestic_value = domestic_value
-        # The bandwidth data for HTTPS requests in the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.https_domestic_value = https_domestic_value
-        # The bandwidth data for HTTPS requests in regions outside the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.https_overseas_value = https_overseas_value
-        # The bandwidth value for HTTPS requests. Unit: bit/s.
         self.https_value = https_value
-        # The bandwidth data in regions outside the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.overseas_value = overseas_value
-        # The timestamp of the data returned.
         self.time_stamp = time_stamp
-        # The bandwidth. Unit: bit/s.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10305,29 +10193,21 @@
         domain_name: str = None,
         end_time: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         request_id: str = None,
         start_time: str = None,
     ):
-        # The list of bandwidth data entries returned at each interval.
         self.bps_data_per_interval = bps_data_per_interval
-        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
-        # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The name of the ISP.
         self.isp_name_en = isp_name_en
-        # The name of the region.
         self.location_name_en = location_name_en
-        # The ID of the request.
         self.request_id = request_id
-        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.bps_data_per_interval:
             self.bps_data_per_interval.validate()
 
     def to_map(self):
@@ -10915,44 +10795,44 @@
         rule_name: str = None,
         start_time: str = None,
         trigger_object: str = None,
         value: str = None,
     ):
         # The accelerated domain name. You can specify multiple domain names and separate them with commas (,).
         # 
-        # If you do not specify a domain name, data of all domain names is queried.
+        # If you do not specify this parameter, data of all accelerated domain names under your account is queried.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # The end time must be later than the start time.
         self.end_time = end_time
-        # The number of the page to return. Default value: **1**.
+        # The page number of the page to return. Default value: **1**.
         self.page_number = page_number
         # The number of entries to return on each page. Default value: **30**.
         self.page_size = page_size
         # A custom rule name. Valid values:
         # 
-        # *   Default mode: default_normal.
-        # *   Emergency mode: default_attack.
+        # *   default_normal: rule for the normal mode
+        # *   default_attack: rule for the emergency mode
         # 
-        # If you do not set this parameter, all events that triggered rate limiting are queried.
+        # If you leave this parameter empty, events that triggered rate limiting based on all rules are queried.
         self.rule_name = rule_name
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # Data is collected every 5 minutes.
+        # The minimum time granularity of data collection is 5 minutes.
         # 
-        # If you do not set this parameter, data within the last 24 hours is queried.
+        # If you leave this parameter empty, the data collected over the last 24 hours is queried.
         self.start_time = start_time
-        # The object that triggered rate limiting.
+        # The trigger of rate limiting by which you want to query data.
         # 
-        # If you do not set this parameter, all events that triggered rate limiting are queried.
+        # If you leave this parameter empty, all events that triggered rate limiting are queried.
         self.trigger_object = trigger_object
-        # The value of the object that triggered rate limiting.
+        # The value of the trigger.
         # 
-        # If you do not set this parameter, the values of all events that triggered rate limiting are queried.
+        # If you leave this parameter empty, all events recorded for the trigger are queried.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11010,23 +10890,23 @@
         ttl: int = None,
         value: str = None,
     ):
         # The action that was triggered.
         self.action = action
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The name of the rule that was triggered
+        # The name of the rule based on which rate limiting was triggered.
         self.rule_name = rule_name
-        # The timestamp of the data.
+        # The timestamp of the data returned.
         self.time_stamp = time_stamp
-        # The object that triggered rate limiting.
+        # The trigger of rate limiting.
         self.trigger_object = trigger_object
-        # The period of time that rate limiting remains effective.
+        # The period of time during which rate limiting remains effective.
         self.ttl = ttl
-        # The value of the object that triggered rate limiting.
+        # The value of the trigger for rate limiting.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11074,15 +10954,15 @@
         self,
         activity_log: List[DescribeDomainCcActivityLogResponseBodyActivityLog] = None,
         page_index: int = None,
         page_size: int = None,
         request_id: str = None,
         total: int = None,
     ):
-        # The log entry of the event that triggered rate limiting.
+        # The list of rate limiting logs.
         self.activity_log = activity_log
         # The page number of the returned page.
         self.page_index = page_index
         # The number of entries returned per page.
         self.page_size = page_size
         # The ID of the request.
         self.request_id = request_id
@@ -11178,15 +11058,15 @@
 
 
 class DescribeDomainCertificateInfoRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name in each query.
+        # The information about the SSL certificate.
         self.domain_name = domain_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11220,68 +11100,70 @@
         cert_update_time: str = None,
         domain_cname_status: str = None,
         domain_name: str = None,
         server_certificate: str = None,
         server_certificate_status: str = None,
         status: str = None,
     ):
-        # The domain name that matches the SSL certificate.
+        # The name of the certificate authority (CA) that issued the SSL certificate.
         self.cert_domain_name = cert_domain_name
-        # The time when the SSL certificate expires.
+        # The status of the SSL certificate.
+        # 
+        # *   **success**: The SSL certificate is effective.
+        # *   **checking**: The system is checking whether the domain name is accelerated by Alibaba Cloud CDN.
+        # *   **cname_error**: The domain name is not accelerated by Alibaba Cloud CDN.
+        # *   **top_domain_cname_error**: The top-level domain name is not an accelerated domain name.
+        # *   **domain_invalid**: The domain name contains invalid characters.
+        # *   **unsupport_wildcard**: Wildcard domain names are not supported.
+        # *   **applying**: The application for a certificate is in progress.
+        # *   **fget_token_timeout**: The application for a certificate timed out.
+        # *   **check_token_timeout**: The verification timed out.
+        # *   **get_cert_timeout**: The request to obtain the certificate timed out.
+        # *   **failed**: The application for a certificate failed.
         self.cert_expire_time = cert_expire_time
+        # The domain name that matches the SSL certificate.
         self.cert_id = cert_id
-        # The unit of the validity period of the SSL certificate.
-        # 
-        # *   **months**: The validity period is measured in months.
-        # *   **years**: The validity period is measured in years.
+        # The time when the certificate was renewed.
         self.cert_life = cert_life
-        # The name of the SSL certificate.
+        # The public key of the SSL certificate.
         self.cert_name = cert_name
-        # The name of the certificate authority (CA) that issued the SSL certificate.
+        # The time when the SSL certificate became effective.
         self.cert_org = cert_org
+        # The status of HTTPS.
+        # 
+        # *   **on**: enabled.
+        # *   **off**: disabled.
         self.cert_region = cert_region
-        # The time when the SSL certificate became effective.
+        # The name of the SSL certificate.
         self.cert_start_time = cert_start_time
-        # The type of the SSL certificate. Valid values:
-        # 
-        # *   **free**: a free SSL certificate.
-        # *   **cas**: an SSL certificate purchased from Alibaba Cloud SSL Certificates Service.
-        # *   **upload**: a user-uploaded SSL certificate.
-        self.cert_type = cert_type
-        # The time when the certificate was renewed.
-        self.cert_update_time = cert_update_time
         # The status of the CNAME of the domain name.
         # 
         # *   **ok**: The domain name points to the CNAME assigned from Alibaba Cloud Content Delivery Network (CDN).
         # *   **cname_error**: An error occurred and the domain name cannot point to the CNAME.
         # *   **top_domain_cname_error**: An error occurred to the CNAME of the top-level domain name. The domain name cannot point to the CNAME.
         # *   **unsupport_wildcard**: Wildcard domain names are not supported.
-        self.domain_cname_status = domain_cname_status
-        # The accelerated domain name.
-        self.domain_name = domain_name
-        # The public key of the SSL certificate.
-        self.server_certificate = server_certificate
+        self.cert_type = cert_type
         # The status of HTTPS.
         # 
         # *   **on**: enabled.
         # *   **off**: disabled.
-        self.server_certificate_status = server_certificate_status
-        # The status of the SSL certificate.
+        self.cert_update_time = cert_update_time
+        # >  The maximum number of times that each user can call this operation per second is 100.
+        self.domain_cname_status = domain_cname_status
+        # The type of the SSL certificate. Valid values:
         # 
-        # *   **success**: The SSL certificate is effective.
-        # *   **checking**: The system is checking whether the domain name is accelerated by Alibaba Cloud CDN.
-        # *   **cname_error**: The domain name is not accelerated by Alibaba Cloud CDN.
-        # *   **top_domain_cname_error**: The top-level domain name is not an accelerated domain name.
-        # *   **domain_invalid**: The domain name contains invalid characters.
-        # *   **unsupport_wildcard**: Wildcard domain names are not supported.
-        # *   **applying**: The application for a certificate is in progress.
-        # *   **fget_token_timeout**: The application for a certificate timed out.
-        # *   **check_token_timeout**: The verification timed out.
-        # *   **get_cert_timeout**: The request to obtain the certificate timed out.
-        # *   **failed**: The application for a certificate failed.
+        # *   **free**: a free SSL certificate.
+        # *   **cas**: an SSL certificate purchased from Alibaba Cloud SSL Certificates Service.
+        # *   **upload**: a user-uploaded SSL certificate.
+        self.domain_name = domain_name
+        # The public key of the SSL certificate.
+        self.server_certificate = server_certificate
+        # The accelerated domain name.
+        self.server_certificate_status = server_certificate_status
+        # The domain name that matches the SSL certificate.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11393,17 +11275,20 @@
 
 class DescribeDomainCertificateInfoResponseBody(TeaModel):
     def __init__(
         self,
         cert_infos: DescribeDomainCertificateInfoResponseBodyCertInfos = None,
         request_id: str = None,
     ):
-        # The information about the SSL certificate.
+        # The unit of the validity period of the SSL certificate.
+        # 
+        # *   **months**: The validity period is measured in months.
+        # *   **years**: The validity period is measured in years.
         self.cert_infos = cert_infos
-        # The ID of the request.
+        # The time when the SSL certificate expires.
         self.request_id = request_id
 
     def validate(self):
         if self.cert_infos:
             self.cert_infos.validate()
 
     def to_map(self):
@@ -11694,23 +11579,23 @@
         self,
         config_id: str = None,
         remark: str = None,
         request_id: str = None,
         sample: str = None,
         tag: str = None,
     ):
-        # The ID of the log configuration.
+        # The sample log configuration.
         self.config_id = config_id
-        # The format of the log configuration.
-        self.remark = remark
         # The ID of the request.
+        self.remark = remark
+        # The format of the log configuration.
         self.request_id = request_id
-        # The sample log configuration.
+        # The operation that you want to perform. Set the value to **DescribeDomainCustomLogConfig**.
         self.sample = sample
-        # The tag information about the log configuration.
+        # The ID of the log configuration.
         self.tag = tag
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11796,35 +11681,35 @@
         end_time: str = None,
         field: str = None,
         isp_name_en: str = None,
         layer: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # The domain name that you want to query. You can specify multiple domain names and separate them with commas (,). You can specify at most 30 domain names in each call.
-        self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # >  The end time must be later than the start time.
-        self.end_time = end_time
-        # The metric that you want to query. You can specify one or more metrics and separate them with commas (,). Valid values: **bps**, **qps**, **traf**, **acc**, **ipv6\_traf**, **ipv6\_bps**, **ipv6\_acc**, **ipv6\_qps**, and **http_code**.
-        self.field = field
         # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
         # 
         # If you do not specify an ISP, data of all ISPs is queried.
-        self.isp_name_en = isp_name_en
+        self.domain_name = domain_name
         # The protocol by which you want to query data. Valid values: **http**, **https**, **quic**, and **all**.
         # 
         # The default value is **all**.
+        self.end_time = end_time
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # >  The end time must be later than the start time.
+        self.field = field
+        # The ID of the request.
+        self.isp_name_en = isp_name_en
+        # The amount of network traffic. Unit: bytes.
         self.layer = layer
+        # The detailed data of the accelerated domain names.
+        self.location_name_en = location_name_en
         # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         # 
         # If you do not specify a region, data in all regions is queried.
-        self.location_name_en = location_name_en
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11878,35 +11763,46 @@
         ipv_6bps: float = None,
         ipv_6qps: float = None,
         ipv_6traf: int = None,
         qps: float = None,
         time_stamp: str = None,
         traf: int = None,
     ):
-        # The number of requests.
+        # The timestamp of the data returned.
         self.acc = acc
-        # The bandwidth. Unit: bit/s.
+        # The bandwidth of IPv6 requests. Unit: bit/s.
         self.bps = bps
-        # The domain name.
+        # The number of requests.
         self.domain_name = domain_name
-        # The proportions of HTTP status codes.
+        # - You can call this operation up to 20 times per second per account.
+        # - If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        # 
+        # **Time granularity**\
+        # 
+        # The following table describes the time granularity, the time period within which historical data is available, and the data delay, which vary with the maximum time range per query. 
+        # 
+        # | Time granularity | Maximum time range per query | Historical data available | Data delay |
+        # | ---------------- | ---------------------------- | ------------------------- | ---------- |
+        # | 5 minutes | 3 days | 93 days | 15 minutes |
+        # | 1 hour | 31 days | 186 days | 4 hours |
+        # | 1 days | 366 days | 366 days | 04:00 on the next day |
         self.http_code = http_code
-        # The number of IPv6 requests.
+        # The bandwidth. Unit: bit/s.
         self.ipv_6acc = ipv_6acc
-        # The bandwidth of IPv6 requests. Unit: bit/s.
+        # The number of IPv6 requests.
         self.ipv_6bps = ipv_6bps
-        # The number of IPv6 requests per second.
-        self.ipv_6qps = ipv_6qps
         # The amount of network traffic generated by IPv6 requests. Unit: bytes.
+        self.ipv_6qps = ipv_6qps
+        # The proportions of HTTP status codes.
         self.ipv_6traf = ipv_6traf
-        # The number of queries per second.
+        # The number of requests.
         self.qps = qps
-        # The timestamp of the data returned.
+        # The domain name.
         self.time_stamp = time_stamp
-        # The amount of network traffic. Unit: bytes.
+        # The bandwidth of IPv6 requests. Unit: bit/s.
         self.traf = traf
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12002,17 +11898,17 @@
 
 class DescribeDomainDetailDataByLayerResponseBody(TeaModel):
     def __init__(
         self,
         data: DescribeDomainDetailDataByLayerResponseBodyData = None,
         request_id: str = None,
     ):
-        # The detailed data of the accelerated domain names.
+        # The number of IPv6 requests per second.
         self.data = data
-        # The ID of the request.
+        # The number of queries per second.
         self.request_id = request_id
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -12085,31 +11981,17 @@
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         interval: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
-        # 
-        # By default, this operation queries the byte hit ratios for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name
-        # The end of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time granularity of the data entries. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
-        # The beginning of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12143,19 +12025,16 @@
 class DescribeDomainHitRateDataResponseBodyHitRateIntervalDataModule(TeaModel):
     def __init__(
         self,
         https_value: str = None,
         time_stamp: str = None,
         value: str = None,
     ):
-        # The byte hit ratio of HTTPS requests.
         self.https_value = https_value
-        # The timestamp of the data returned.
         self.time_stamp = time_stamp
-        # The byte hit ratio.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12223,25 +12102,19 @@
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         hit_rate_interval: DescribeDomainHitRateDataResponseBodyHitRateInterval = None,
         request_id: str = None,
         start_time: str = None,
     ):
-        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
-        # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The byte hit ratio at each time interval. The byte hit ratio is measured in percentage.
         self.hit_rate_interval = hit_rate_interval
-        # The ID of the request.
         self.request_id = request_id
-        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.hit_rate_interval:
             self.hit_rate_interval.validate()
 
     def to_map(self):
@@ -12332,33 +12205,31 @@
         domain_name: str = None,
         end_time: str = None,
         interval: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the total number and proportions of HTTP status codes returned from all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries the number and proportions of HTTP status codes for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name
-        # The end of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
+        # The name of the region. You can call the DescribeCdnRegionAndIsp operation to query regions. If you do not specify this parameter, data in all regions is queried.
         self.isp_name_en = isp_name_en
+        # The name of the Internet service provider (ISP). You can call the DescribeCdnRegionAndIsp operation to query ISPs. If you do not specify this parameter, data of all ISPs is queried.
         self.location_name_en = location_name_en
-        # The start of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12400,17 +12271,17 @@
 class DescribeDomainHttpCodeDataResponseBodyHttpCodeDataUsageDataValueCodeProportionData(TeaModel):
     def __init__(
         self,
         code: str = None,
         count: str = None,
         proportion: str = None,
     ):
-        # The HTTP status code.
+        # The HTTP status code returned.
         self.code = code
-        # The total number of HTTP status code returned.
+        # The count of each HTTP status code.
         self.count = count
         # The proportion of the HTTP status code.
         self.proportion = proportion
 
     def validate(self):
         pass
 
@@ -12476,17 +12347,17 @@
 
 class DescribeDomainHttpCodeDataResponseBodyHttpCodeDataUsageData(TeaModel):
     def __init__(
         self,
         time_stamp: str = None,
         value: DescribeDomainHttpCodeDataResponseBodyHttpCodeDataUsageDataValue = None,
     ):
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
-        # The proportions of HTTP status codes.
+        # The information about the HTTP status codes.
         self.value = value
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -12552,25 +12423,25 @@
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         http_code_data: DescribeDomainHttpCodeDataResponseBodyHttpCodeData = None,
         request_id: str = None,
         start_time: str = None,
     ):
-        # The interval at which the monitoring data is queried.
+        # The time interval.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The proportions of HTTP status codes at each time interval.
         self.http_code_data = http_code_data
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The beginning of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.http_code_data:
             self.http_code_data.validate()
 
     def to_map(self):
@@ -12905,23 +12776,19 @@
 class DescribeDomainISPDataRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name in each call.
-        # 
-        # By default, this operation queries the proportions of data usage for all accelerated domain names.
+        # The beginning of the time range that was queried.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # The end time must be later than the start time.
+        # The accelerated domain name.
         self.end_time = end_time
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The ID of the request.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12960,37 +12827,41 @@
         isp_ename: str = None,
         proportion: str = None,
         qps: str = None,
         req_err_rate: str = None,
         total_bytes: str = None,
         total_query: str = None,
     ):
-        # The average response size. Unit: bytes.
+        # The name of the ISP.
         self.avg_object_size = avg_object_size
-        # The average response speed. Unit: byte/ms.
+        # The bandwidth value.
         self.avg_response_rate = avg_response_rate
-        # The average response time. Unit: milliseconds.
+        # The number of queries per second.
         self.avg_response_time = avg_response_time
-        # The bandwidth value.
+        # The information about the ISP.
         self.bps = bps
-        # The proportion of network traffic.
+        # The total amount of network traffic.
         self.bytes_proportion = bytes_proportion
-        # The information about the ISP.
-        self.isp = isp
         # The name of the ISP.
+        self.isp = isp
+        # The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.  
+        # 
+        # > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        # - This operation queries proportions of data usage of different ISPs only for a specific accelerated domain name, or for all accelerated domain names that belong your Alibaba Cloud account.
+        # - You can call this operation up to 100 times per second per account.
         self.isp_ename = isp_ename
-        # The proportion of the HTTP status code.
+        # The proportion of network traffic.
         self.proportion = proportion
-        # The number of queries per second.
+        # chinanet
         self.qps = qps
-        # The request error rate.
+        # The proportion of the HTTP status code.
         self.req_err_rate = req_err_rate
-        # The total amount of network traffic.
+        # The average response size. Unit: bytes.
         self.total_bytes = total_bytes
-        # The total number of requests.
+        # The request error rate.
         self.total_query = total_query
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13094,25 +12965,25 @@
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         request_id: str = None,
         start_time: str = None,
         value: DescribeDomainISPDataResponseBodyValue = None,
     ):
-        # The time interval between the data entries. Unit: seconds.
+        # The average response speed. Unit: byte/ms.
         self.data_interval = data_interval
-        # The accelerated domain name.
+        # The total amount of network traffic.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The time interval between the data entries. Unit: seconds.
         self.end_time = end_time
-        # The ID of the request.
+        # The total number of requests.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
-        self.start_time = start_time
         # The access statistics by ISP.
+        self.start_time = start_time
+        # The average response time. Unit: milliseconds.
         self.value = value
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -13471,24 +13342,19 @@
 class DescribeDomainMultiUsageDataRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain names. You can specify multiple accelerated domain names and separate domain names with commas (,).
-        # 
-        # > *   You can specify at most 30 accelerated domain names.
-        # *   If you do not set this parameter, the data of all accelerated domain names that belong to your Alibaba Cloud account is queried.
+        # The beginning of the time range that was queried.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # >  The end time must be later than the start time.
+        # The information about requests collected every 5 minutes.
         self.end_time = end_time
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The ID of the request.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13519,23 +13385,27 @@
     def __init__(
         self,
         domain: str = None,
         request: int = None,
         time_stamp: str = None,
         type: str = None,
     ):
-        # The information about the accelerated domain name.
+        # The accelerated domain name.
         self.domain = domain
-        # The number of requests.
-        self.request = request
         # The timestamp of the data returned.
-        self.time_stamp = time_stamp
-        # The type of data returned.
+        self.request = request
+        # The type of data returned. Valid values:
         # 
-        # >  For Alibaba Cloud CDN, the valid value is Simple.
+        # - **StaticHttps**: the number of HTTPS requests for static content.
+        # - **DynamicHttps**: the number of HTTPS requests for dynamic content.
+        # - **DynamicHttp**: the number of HTTP requests for dynamic content.
+        # - **StaticQuic**: the number of QUIC requests for static content.
+        # - **DynamicQuic**: the number of QUIC requests for dynamic content.
+        self.time_stamp = time_stamp
+        # The statistics about data transfer collected every 5 minutes.
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13606,29 +13476,29 @@
         self,
         area: str = None,
         bps: float = None,
         domain: str = None,
         time_stamp: str = None,
         type: str = None,
     ):
-        # The name of the district.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # >  The end time must be later than the start time.
         self.area = area
-        # The bandwidth. Unit: bit/s.
+        # The timestamp of the data returned.
         self.bps = bps
-        # The accelerated domain name.
+        # > *   If you do not set StartTime or EndTime, data collected within the last 10 minutes is queried.
+        # *   The maximum time range between StartTime and EndTime can be 1 hour.
+        # *   You can query data within the last 90 days.
+        # *   You can query the amount of data transfer and the number of requests for accelerated domain names that have been already removed from Alibaba Cloud CDN.
+        # *   The maximum number of times that each user can call this operation per second is 50.
         self.domain = domain
-        # The timestamp of the data returned.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.time_stamp = time_stamp
-        # The type of data returned. Valid values:
-        # 
-        # - **StaticHttps**: the number of HTTPS requests for static content.
-        # - **DynamicHttps**: the number of HTTPS requests for dynamic content.
-        # - **DynamicHttp**: the number of HTTP requests for dynamic content.
-        # - **StaticQuic**: the number of QUIC requests for static content.
-        # - **DynamicQuic**: the number of QUIC requests for dynamic content.
+        # The bandwidth. Unit: bit/s.
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13703,23 +13573,25 @@
         self,
         end_time: str = None,
         request_id: str = None,
         request_per_interval: DescribeDomainMultiUsageDataResponseBodyRequestPerInterval = None,
         start_time: str = None,
         traffic_per_interval: DescribeDomainMultiUsageDataResponseBodyTrafficPerInterval = None,
     ):
-        # The end of the time range that was queried.
+        # The type of data returned.
+        # 
+        # >  For Alibaba Cloud CDN, the valid value is Simple.
         self.end_time = end_time
-        # The ID of the request.
+        # The information about the accelerated domain name.
         self.request_id = request_id
-        # The information about requests collected every 5 minutes.
+        # The number of requests.
         self.request_per_interval = request_per_interval
-        # The beginning of the time range that was queried.
+        # The timestamp of the data returned.
         self.start_time = start_time
-        # The statistics about data transfer collected every 5 minutes.
+        # The name of the district.
         self.traffic_per_interval = traffic_per_interval
 
     def validate(self):
         if self.request_per_interval:
             self.request_per_interval.validate()
         if self.traffic_per_interval:
             self.traffic_per_interval.validate()
@@ -14080,21 +13952,19 @@
 class DescribeDomainPvDataRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name.
+        # The beginning of the time range during which data was queried.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # The end time must be later than the start time.
+        # The accelerated domain name.
         self.end_time = end_time
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The ID of the request.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14123,15 +13993,15 @@
 
 class DescribeDomainPvDataResponseBodyPvDataIntervalUsageData(TeaModel):
     def __init__(
         self,
         time_stamp: str = None,
         value: str = None,
     ):
-        # The timestamp of the returned data.
+        # The accelerated domain name. You can specify only one domain name.
         self.time_stamp = time_stamp
         # The number of PVs.
         self.value = value
 
     def validate(self):
         pass
 
@@ -14197,25 +14067,28 @@
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         pv_data_interval: DescribeDomainPvDataResponseBodyPvDataInterval = None,
         request_id: str = None,
         start_time: str = None,
     ):
-        # The time interval between the data entries. Unit: seconds.
+        # The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.  
+        # 
+        # > - If you do not set StartTime or EndTime, monitoring data within the last 24 hours is queried. If you set both StartTime and EndTime, monitoring data within the specified time range is queried.
+        # - You can call this operation up to 50 times per second per account.
         self.data_interval = data_interval
-        # The accelerated domain name.
+        # The timestamp of the returned data.
         self.domain_name = domain_name
-        # The end of the time range during which data was queried.
+        # The time interval between the data entries. Unit: seconds.
         self.end_time = end_time
-        # The number of PVs at each interval.
+        # The end of the time range during which data was queried.
         self.pv_data_interval = pv_data_interval
-        # The ID of the request.
+        # The number of PVs.
         self.request_id = request_id
-        # The beginning of the time range during which data was queried.
+        # The number of PVs at each interval.
         self.start_time = start_time
 
     def validate(self):
         if self.pv_data_interval:
             self.pv_data_interval.validate()
 
     def to_map(self):
@@ -15352,49 +15225,44 @@
         field: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         merge: str = None,
         merge_loc_isp: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name for which you want to query data. You can specify multiple accelerated domain names and separate them with commas (,).
-        self.domain_name = domain_name
-        # The end of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. Example: 2019-11-30T05:40:00Z.
-        # 
-        # >  The end time must be later than the start time. The time range between the end time and the start time cannot exceed 10 minutes.
-        self.end_time = end_time
         # The metrics that you want to query. You can specify multiple metrics and separate them with commas (,). Valid values:
         # 
         # *   **qps**: the number of queries per second
         # *   **bps**: bandwidth values
         # *   **http_code**: HTTP status codes
-        self.field = field
+        self.domain_name = domain_name
         # The name of the Internet service provider. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs.
-        self.isp_name_en = isp_name_en
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
-        self.location_name_en = location_name_en
+        self.end_time = end_time
         # Specifies whether to merge the results. Valid values:
         # 
         # *   **true**: merges the results.
         # *   **false**: does not merge the results. This is the default value.
         # 
         # Default value: **false**.
-        self.merge = merge
+        self.field = field
+        # The data usage of each ISP and the number of visits in each region.
+        self.isp_name_en = isp_name_en
         # Specifies whether to merge the results. Valid values:
         # 
         # *   **true**: groups the results by domain name and merges the results by region and ISP.
         # *   **false**: groups the results by domain name.
         # 
         # Default value: **false**.
+        self.location_name_en = location_name_en
+        # The ID of the request.
+        self.merge = merge
+        # - You can query data within the last seven days. Data is collected every minute.
+        # - The maximum number of times that each user can call this operation per second is 10.
         self.merge_loc_isp = merge_loc_isp
-        # The beginning of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. Example: 2019-11-30T05:33:00Z.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15443,17 +15311,17 @@
 
 class DescribeDomainRealTimeDetailDataResponseBody(TeaModel):
     def __init__(
         self,
         data: str = None,
         request_id: str = None,
     ):
-        # The data usage of each ISP and the number of visits in each region.
+        # The name of the Internet service provider. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs.
         self.data = data
-        # The ID of the request.
+        # The accelerated domain name for which you want to query data. You can specify multiple accelerated domain names and separate them with commas (,).
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15525,31 +15393,18 @@
         self,
         domain_name: str = None,
         end_time: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. You can specify multiple accelerated domain names and separate them with commas (,).
-        # 
-        # > You can specify up to 100 accelerated domain names in each request.
         self.domain_name = domain_name
-        # The end of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
         self.isp_name_en = isp_name_en
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions. If you do not specify a region, all regions are queried.
         self.location_name_en = location_name_en
-        # The beginning of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15587,19 +15442,16 @@
 class DescribeDomainRealTimeHttpCodeDataResponseBodyRealTimeHttpCodeDataUsageDataValueRealTimeCodeProportionData(TeaModel):
     def __init__(
         self,
         code: str = None,
         count: str = None,
         proportion: str = None,
     ):
-        # The HTTP status code returned.
         self.code = code
-        # The total number of entries.
         self.count = count
-        # The proportion of the HTTP status code.
         self.proportion = proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15663,17 +15515,15 @@
 
 class DescribeDomainRealTimeHttpCodeDataResponseBodyRealTimeHttpCodeDataUsageData(TeaModel):
     def __init__(
         self,
         time_stamp: str = None,
         value: DescribeDomainRealTimeHttpCodeDataResponseBodyRealTimeHttpCodeDataUsageDataValue = None,
     ):
-        # The timestamp of the data returned.
         self.time_stamp = time_stamp
-        # The proportions of the HTTP status codes.
         self.value = value
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -15739,27 +15589,19 @@
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         real_time_http_code_data: DescribeDomainRealTimeHttpCodeDataResponseBodyRealTimeHttpCodeData = None,
         request_id: str = None,
         start_time: str = None,
     ):
-        # The time interval between the data entries returned. Unit: seconds.
-        # 
-        # Depending on the maximum time range per query, the value is 60 (1 minute), 300 (5 minutes), or 3600 (1 hour). For more information, see the "Time granularity" section in Usage notes.
         self.data_interval = data_interval
-        # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The proportions of HTTP status codes at each time interval.
         self.real_time_http_code_data = real_time_http_code_data
-        # The ID of the request.
         self.request_id = request_id
-        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.real_time_http_code_data:
             self.real_time_http_code_data.validate()
 
     def to_map(self):
@@ -16066,21 +15908,19 @@
 class DescribeDomainRealTimeReqHitRateDataRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 100 domain names in each call.
+        # The response parameters.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # >  The end time must be later than the start time.
+        # The timestamp. The time follows the ISO 8601 standard. The time is displayed in UTC.
         self.end_time = end_time
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The request hit ratio.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16109,17 +15949,17 @@
 
 class DescribeDomainRealTimeReqHitRateDataResponseBodyDataReqHitRateDataModel(TeaModel):
     def __init__(
         self,
         req_hit_rate: float = None,
         time_stamp: str = None,
     ):
-        # The request hit ratio.
+        # You can specify multiple domain names and separate them with commas (,). You can specify at most 100 domain names in each call.
         self.req_hit_rate = req_hit_rate
-        # The timestamp. The time follows the ISO 8601 standard. The time is displayed in UTC.
+        # The request hit ratio.
         self.time_stamp = time_stamp
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16179,17 +16019,30 @@
 
 class DescribeDomainRealTimeReqHitRateDataResponseBody(TeaModel):
     def __init__(
         self,
         data: DescribeDomainRealTimeReqHitRateDataResponseBodyData = None,
         request_id: str = None,
     ):
-        # The response parameters.
+        # - The maximum number of times that each user can call this operation per second is 10.
+        # - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        # - By default, requests in the Go programming language use the POST request method. You must manually change the request method to GET by declaring: request.Method="GET".
+        # - The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the request hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
+        # 
+        # **Time granularity**\
+        # 
+        # The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay. 
+        # 
+        # | Time granularity | Time range to query | Historical data available | Data delay |
+        # | ---------------- | ------------------- | ------------------------- | ---------- |
+        # | 1 minute | 1 hour | 7 days | 5 minutes |
+        # | 5 minutes | 3 Days | 93 days | 15 minutes |
+        # | 1 hour | 31 days | 186 days | 4 hours |
         self.data = data
-        # The ID of the request.
+        # 624461
         self.request_id = request_id
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -16261,23 +16114,16 @@
 class DescribeDomainRealTimeSrcBpsDataRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. You can specify up to 100 domain names in each request. Separate multiple domain names with commas (,).
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The beginning of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16306,17 +16152,15 @@
 
 class DescribeDomainRealTimeSrcBpsDataResponseBodyRealTimeSrcBpsDataPerIntervalDataModule(TeaModel):
     def __init__(
         self,
         time_stamp: str = None,
         value: str = None,
     ):
-        # The timestamp of the returned data.
         self.time_stamp = time_stamp
-        # The bandwidth during back-to-origin routing. Unit: bit/s.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16380,27 +16224,19 @@
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         real_time_src_bps_data_per_interval: DescribeDomainRealTimeSrcBpsDataResponseBodyRealTimeSrcBpsDataPerInterval = None,
         request_id: str = None,
         start_time: str = None,
     ):
-        # The time interval between the data entries returned. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 60 (1 minute), 300 (5 minutes), and 3600(1 hour). For more information, see **Usage notes**.
         self.data_interval = data_interval
-        # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The origin bandwidth data at each interval.
         self.real_time_src_bps_data_per_interval = real_time_src_bps_data_per_interval
-        # The ID of the request.
         self.request_id = request_id
-        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.real_time_src_bps_data_per_interval:
             self.real_time_src_bps_data_per_interval.validate()
 
     def to_map(self):
@@ -16490,25 +16326,18 @@
         self,
         domain_name: str = None,
         end_time: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. You can specify up to 100 domain names in each call. Separate multiple domain names with commas (,).
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you leave this parameter empty, all ISPs are queried.
         self.isp_name_en = isp_name_en
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions. If you leave this parameter empty, all regions are queried.
         self.location_name_en = location_name_en
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16546,19 +16375,16 @@
 class DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeDataUsageDataValueRealTimeSrcCodeProportionData(TeaModel):
     def __init__(
         self,
         code: str = None,
         count: str = None,
         proportion: str = None,
     ):
-        # The HTTP status code returned.
         self.code = code
-        # The count of each HTTP status code.
         self.count = count
-        # The proportion of the HTTP status code.
         self.proportion = proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16622,17 +16448,15 @@
 
 class DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeDataUsageData(TeaModel):
     def __init__(
         self,
         time_stamp: str = None,
         value: DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeDataUsageDataValue = None,
     ):
-        # The timestamp of the returned data.
         self.time_stamp = time_stamp
-        # The proportions of the HTTP status codes.
         self.value = value
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -16698,25 +16522,19 @@
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         real_time_src_http_code_data: DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeData = None,
         request_id: str = None,
         start_time: str = None,
     ):
-        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
-        # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The proportions of HTTP status codes at each time interval.
         self.real_time_src_http_code_data = real_time_src_http_code_data
-        # The ID of the request.
         self.request_id = request_id
-        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.real_time_src_http_code_data:
             self.real_time_src_http_code_data.validate()
 
     def to_map(self):
@@ -17278,15 +17096,15 @@
 
 
 class DescribeDomainRealtimeLogDeliveryRequest(TeaModel):
     def __init__(
         self,
         domain: str = None,
     ):
-        # The accelerated domain name for which real-time log delivery is enabled. You can specify only one domain name.
+        # The ID of the request.
         self.domain = domain
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17310,26 +17128,19 @@
         self,
         logstore: str = None,
         project: str = None,
         region: str = None,
         request_id: str = None,
         status: str = None,
     ):
-        # The name of the Logstore where log entries are stored.
         self.logstore = logstore
-        # The name of the Log Service project that is used for real-time log delivery.
         self.project = project
-        # The ID of the region where the Log Service project is deployed.
         self.region = region
-        # The ID of the request.
         self.request_id = request_id
-        # The status of real-time log delivery. Valid values:
-        # 
-        # *   **online**\
-        # *   **offline**\
+        # The ID of the region where the Log Service project is deployed.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17411,23 +17222,19 @@
 class DescribeDomainRegionDataRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).  
-        # 
-        # By default, this operation queries the geographic distribution of users for all accelerated domain names.
+        # The ID of the request.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.  
-        # 
-        # The end time must be later than the start time.
+        # The time interval between the data entries returned. Unit: seconds.
         self.end_time = end_time
-        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The accelerated domain name.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17466,37 +17273,41 @@
         qps: str = None,
         region: str = None,
         region_ename: str = None,
         req_err_rate: str = None,
         total_bytes: str = None,
         total_query: str = None,
     ):
-        # The average response size. Unit: bytes.
+        # cn-shenzhen
         self.avg_object_size = avg_object_size
-        # The average response speed. Unit: bit/s.
+        # The number of queries per second.
         self.avg_response_rate = avg_response_rate
-        # The average response time. Unit: milliseconds.
+        # The name of the region.
         self.avg_response_time = avg_response_time
-        # The bandwidth.
+        # The proportion of visits from each region. For example, a value of 90 indicates that 90% of the visits are from the specified area.
         self.bps = bps
-        # The proportion of bytes transferred from each region. For example, a value of 90 indicates that 90% of the bytes are transferred from the specified area.
+        # The accelerated domain name.
         self.bytes_proportion = bytes_proportion
-        # The proportion of visits from each region. For example, a value of 90 indicates that 90% of the visits are from the specified area.
+        # The request error rate. A value of 90 indicates that 90% of the requests encountered errors.
         self.proportion = proportion
-        # The number of queries per second.
+        # The proportion of bytes transferred from each region. For example, a value of 90 indicates that 90% of the bytes are transferred from the specified area.
         self.qps = qps
-        # The information of the regions.
+        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.region = region
-        # The name of the region.
+        # The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.  
+        # 
+        # > - If you do not set **StartTime** or **EndTime**, data collected within the last **24** hours is queried. If you set both **StartTime** and **EndTime**, data collected within the specified time range is queried.
+        # - You may fail to query the latest data. If you need to query data collected within the last day, we recommend that you query the data on the next day.
+        # - You can call this operation up to 100 times per second per account.
         self.region_ename = region_ename
-        # The request error rate. A value of 90 indicates that 90% of the requests encountered errors.
+        # The information of the regions.
         self.req_err_rate = req_err_rate
-        # The total traffic. Unit: bytes.
+        # The bandwidth.
         self.total_bytes = total_bytes
-        # The total number of requests.
+        # The average response size. Unit: bytes.
         self.total_query = total_query
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17600,25 +17411,25 @@
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         request_id: str = None,
         start_time: str = None,
         value: DescribeDomainRegionDataResponseBodyValue = None,
     ):
-        # The time interval between the data entries returned. Unit: seconds.
+        # The average response time. Unit: milliseconds.
         self.data_interval = data_interval
-        # The accelerated domain name.
+        # The average response speed. Unit: bit/s.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The proportions of requests initiated from each area.
         self.end_time = end_time
-        # The ID of the request.
+        # The total traffic. Unit: bytes.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The total number of requests.
         self.start_time = start_time
-        # The proportions of requests initiated from each area.
+        # The request error rate. A value of 90 indicates that 90% of the requests encountered errors.
         self.value = value
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -18744,28 +18555,21 @@
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         sort_by: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
+        # The number of visits to the URL.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # >  The end time must be later than the start time. The difference between the end time and the start time cannot exceed seven days.
+        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
         self.end_time = end_time
-        # The method that is used to sort the returned URLs.**** Valid values:
-        # 
-        # *   **traf**: by network traffic.
-        # *   **pv**: by the number of page views. This is the default value.
+        # A list of frequently requested URLs.
         self.sort_by = sort_by
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # >  If you do not set the StartTime parameter, the data within the previous day is queried.
+        # The operation that you want to perform. Set the value to **DescribeDomainSrcTopUrlVisit**.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18801,23 +18605,26 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         url_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The amount of network traffic. Unit: bytes.
-        self.flow = flow
         # The proportion of network traffic consumed to access the URL.
-        self.flow_proportion = flow_proportion
+        self.flow = flow
         # The complete URL.
+        self.flow_proportion = flow_proportion
+        # The amount of network traffic. Unit: bytes.
         self.url_detail = url_detail
-        # The number of visits to the URL.
+        # The beginning of the time range that was queried.
         self.visit_data = visit_data
-        # The proportion of visits to the URL.
+        # The method that is used to sort the returned URLs.**** Valid values:
+        # 
+        # *   **traf**: by network traffic.
+        # *   **pv**: by the number of page views. This is the default value.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18892,23 +18699,19 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         url_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The amount of network traffic. Unit: bytes.
+        # Queries frequently requested back-to-origin URLs of one or more accelerated domain names.
         self.flow = flow
-        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion
-        # The complete URL.
         self.url_detail = url_detail
-        # The number of visits to the URL.
         self.visit_data = visit_data
-        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18983,23 +18786,18 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         url_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The amount of network traffic. Unit: bytes.
         self.flow = flow
-        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion
-        # The complete URL.
         self.url_detail = url_detail
-        # The number of visits to the URL.
         self.visit_data = visit_data
-        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19074,23 +18872,18 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         url_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The amount of network traffic. Unit: bytes.
         self.flow = flow
-        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion
-        # The complete URL.
         self.url_detail = url_detail
-        # The number of visits to the URL.
         self.visit_data = visit_data
-        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19165,23 +18958,18 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         url_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The network traffic consumed to visit the URL, in bytes.
         self.flow = flow
-        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion
-        # The complete URL.
         self.url_detail = url_detail
-        # The number of visits to the URL.
         self.visit_data = visit_data
-        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19259,29 +19047,30 @@
         request_id: str = None,
         start_time: str = None,
         url_200list: DescribeDomainSrcTopUrlVisitResponseBodyUrl200List = None,
         url_300list: DescribeDomainSrcTopUrlVisitResponseBodyUrl300List = None,
         url_400list: DescribeDomainSrcTopUrlVisitResponseBodyUrl400List = None,
         url_500list: DescribeDomainSrcTopUrlVisitResponseBodyUrl500List = None,
     ):
-        # A list of frequently requested URLs.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # >  The end time must be later than the start time. The difference between the end time and the start time cannot exceed seven days.
         self.all_url_list = all_url_list
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The ID of the request.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # >  If you do not set the StartTime parameter, the data within the previous day is queried.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The proportion of visits to the URL.
         self.start_time = start_time
-        # A list of URLs for which 2xx status codes were returned.
+        # The ID of the request.
         self.url_200list = url_200list
-        # A list of URLs for which 3xx status codes were returned.
         self.url_300list = url_300list
-        # A list of URLs for which 4xx status codes were returned.
         self.url_400list = url_400list
-        # A list of URLs for which 5xx status codes were returned.
         self.url_500list = url_500list
 
     def validate(self):
         if self.all_url_list:
             self.all_url_list.validate()
         if self.url_200list:
             self.url_200list.validate()
@@ -19637,36 +19426,32 @@
         domain_name: str = None,
         end_time: str = None,
         limit: str = None,
         location_name_en: str = None,
         sort_by: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
-        # 
-        # By default, this operation queries client IP addresses for all accelerated domain names.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # The end time must be later than the start time.
-        self.end_time = end_time
         # The maximum number of entries to return. Maximum value: 100.
         # 
         # Default value: 20. The default value 20 specifies that the top 20 data entries are returned.
+        self.end_time = end_time
+        # A list of client IP addresses.
         self.limit = limit
-        # The name of the region. Separate multiple region names with commas (,).
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
+        # The end time must be later than the start time.
         self.location_name_en = location_name_en
+        # The ID of the request.
+        self.sort_by = sort_by
         # The method that is used to sort the client IP addresses. Valid values:
         # 
         # *   **traf**: by network traffic. This is the default value.
         # *   **acc**: by the number of requests.
-        self.sort_by = sort_by
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19709,21 +19494,25 @@
     def __init__(
         self,
         acc: int = None,
         client_ip: str = None,
         rank: int = None,
         traffic: int = None,
     ):
-        # The total number of requests.
+        # The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.  
+        # 
+        # > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        # - Data is collected every hour.
+        # - You can call this operation up to 10 times per second per account.
         self.acc = acc
-        # The client IP address returned. Only IPv4 addressed are supported.
+        # The total amount of network traffic consumed. Unit: bytes.
         self.client_ip = client_ip
-        # The ranking of the client IP address returned.
+        # The total number of requests.
         self.rank = rank
-        # The total amount of network traffic consumed. Unit: bytes.
+        # The total number of requests.
         self.traffic = traffic
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19756,17 +19545,17 @@
 
 class DescribeDomainTopClientIpVisitResponseBody(TeaModel):
     def __init__(
         self,
         client_ip_list: List[DescribeDomainTopClientIpVisitResponseBodyClientIpList] = None,
         request_id: str = None,
     ):
-        # A list of client IP addresses.
+        # The client IP address returned. Only IPv4 addressed are supported.
         self.client_ip_list = client_ip_list
-        # The ID of the request.
+        # The ranking of the client IP address returned.
         self.request_id = request_id
 
     def validate(self):
         if self.client_ip_list:
             for k in self.client_ip_list:
                 if k:
                     k.validate()
@@ -19845,26 +19634,21 @@
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         sort_by: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain names. Separate multiple accelerated domain names with commas (,).
+        # The beginning of the time range that was queried.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # The end time must be later than the start time.
+        # The accelerated domain name.
         self.end_time = end_time
-        # The sorting method. Valid values:
-        # 
-        # *   **traf**: by network traffic.
-        # *   **pv**: by the number of page views. This is the default value.
+        # The most frequently requested web pages.
         self.sort_by = sort_by
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The ID of the request.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19900,23 +19684,29 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         refer_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The amount of network traffic. Unit: bytes.
+        # The proportion of visits to the web page.
         self.flow = flow
-        # The proportion of the amount of network traffic consumed for visiting the web page.
+        # The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to analyze data.  
+        # 
+        # > - If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
+        # - Data is collected at an interval of five minutes.
+        # - You can call this operation up to 10 times per second per account.
         self.flow_proportion = flow_proportion
-        # The URLs to the most frequently requested web pages.
+        # The accelerated domain name.
         self.refer_detail = refer_detail
-        # The number of visits to the web page.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.visit_data = visit_data
-        # The proportion of visits to the web page.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # The end time must be later than the start time.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19990,21 +19780,21 @@
     def __init__(
         self,
         domain_name: str = None,
         request_id: str = None,
         start_time: str = None,
         top_refer_list: DescribeDomainTopReferVisitResponseBodyTopReferList = None,
     ):
-        # The accelerated domain name.
+        # The number of visits to the web page.
         self.domain_name = domain_name
-        # The ID of the request.
+        # The proportion of the amount of network traffic consumed for visiting the web page.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The amount of network traffic. Unit: bytes.
         self.start_time = start_time
-        # The most frequently requested web pages.
+        # The URLs to the most frequently requested web pages.
         self.top_refer_list = top_refer_list
 
     def validate(self):
         if self.top_refer_list:
             self.top_refer_list.validate()
 
     def to_map(self):
@@ -21026,69 +20816,69 @@
         domain_name: str = None,
         end_time: str = None,
         field: str = None,
         interval: str = None,
         start_time: str = None,
         type: str = None,
     ):
-        # The billable region. Default value: CN. Valid values:
+        # The ID of the billable region. Valid values:
         # 
-        # *   **CN**: Chinese mainland
+        # *   **CN** (default): inside the Chinese mainland
         # *   **OverSeas**: outside the Chinese mainland
         # *   **AP1**: Asia Pacific 1
         # *   **AP2**: Asia Pacific 2
         # *   **AP3**: Asia Pacific 3
         # *   **NA**: North America
         # *   **SA**: South America
         # *   **EU**: Europe
         # *   **MEAA**: Middle East and Africa
         # *   **all**: all the preceding billable regions
         self.area = area
-        # The protocol of the data that you want to query. Default value: all. Valid values:
+        # The protocol of the data that you want to query. Valid values:
         # 
         # *   **http**: HTTP
         # *   **https**: HTTPS
         # *   **quic**: QUIC
-        # *   **all**: HTTP, HTTPS, and QUIC
+        # *   **all** (default): HTTP, HTTPS, and QUIC
         self.data_protocol = data_protocol
         # The accelerated domain name. You can specify up to 100 domain names in each request. Separate multiple domain names with commas (,).
         # 
         # > If you leave this parameter empty, the usage data of all accelerated domain names in your Alibaba Cloud account is returned.
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # > The end time must be later than the start time. The maximum time range that can be specified is 31 days.
         self.end_time = end_time
-        # The type of data that you want to query. Valid values:
+        # The type of the data that you want to query. Valid values:
         # 
         # *   **bps**: bandwidth
         # *   **traf**: traffic
         # *   **acc**: requests
         # 
         # > If you set this parameter to **acc**, the **Area** parameter is not supported.
         self.field = field
-        # The time interval between the data entries to return. Unit: seconds. Valid values: **300** (5 minutes), **3600** (1 hour), and **86400** (1 day).
+        # The time granularity of the data entries. Unit: seconds. Valid values: **300** (5 minutes), **3600** (1 hour), and **86400** (1 day).
         # 
-        # *   If **Interval** is set to **300**, you can query usage data in the last six months. The maximum time range per query that can be specified is three days.
+        # *   If **Interval** is set to **300**, you can query usage data in the last 6 months. The maximum time range per query that can be specified is 3 days.
         # *   If **Interval** is set to **3600** or **86400**, you can query usage data of the previous year.
-        # *   If you do not set the **Interval** parameter, the maximum time range that you can query is one month. If you specify a time range of 1 to 3 days, the time interval between the entries that are returned is 1 hour. If you specify a time range of at least 4 days, the time interval between the entries that are returned is 1 day.
+        # *   If you leave the **Interval** parameter empty, the maximum time range that you can query is 1 month. If you specify a time range of 1 to 3 days, the time interval between the entries that are returned is 1 hour. If you specify a time range of at least 4 days, the time interval between the entries that are returned is 1 day.
         self.interval = interval
         # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # > Data is collected every 5 minutes.
         self.start_time = start_time
-        # The type of content that you want to query. Default value: all. Valid values:
+        # The type of content that you want to query. Valid values:
         # 
         # *   **static**: static content
         # *   **dynamic**: dynamic content
-        # *   **all**: both static and dynamic content
+        # *   **all** (default): both static and dynamic content
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -21141,21 +20931,21 @@
         peak_time: str = None,
         special_value: str = None,
         time_stamp: str = None,
         value: str = None,
     ):
         # The time of the peak bandwidth value if the **Field** parameter in the request is set to **bps**. Otherwise, this parameter returns the same value as the **TimeStamp** parameter.
         self.peak_time = peak_time
-        # The data usage in a specific scenario.
+        # The resource usage in a specific scenario.
         # 
         # > SpecialValue indicates the data usage in a specific scenario. If no special billable item is specified, ignore this parameter.
         self.special_value = special_value
         # The timestamp of the data returned.
         # 
-        # > **TimeStamp** indicates the timestamp of the returned data at each interval.
+        # > **TimeStamp** indicates the timestamp of the data returned at each interval.
         self.time_stamp = time_stamp
         # The amount of resource usage.
         self.value = value
 
     def validate(self):
         pass
 
@@ -21231,25 +21021,25 @@
         domain_name: str = None,
         end_time: str = None,
         request_id: str = None,
         start_time: str = None,
         type: str = None,
         usage_data_per_interval: DescribeDomainUsageDataResponseBodyUsageDataPerInterval = None,
     ):
-        # The billable region where the data was collected.
+        # The ID of the billable region where the data was collected.
         self.area = area
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
         # The end of the time range during which data was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
-        # The start of the time range during which data was queried.
+        # The beginning of the time range during which data was queried.
         self.start_time = start_time
         # The type of content.
         self.type = type
         # The resource usage that was collected at each interval.
         self.usage_data_per_interval = usage_data_per_interval
 
     def validate(self):
@@ -21574,15 +21364,15 @@
         self,
         owner_id: int = None,
         security_token: str = None,
         sources: str = None,
     ):
         self.owner_id = owner_id
         self.security_token = security_token
-        # The origin servers. Separate origin servers with commas (,). Fuzzy match is not supported.
+        # The origin servers. Separate multiple origin servers with commas (,). Fuzzy match is not supported.
         self.sources = sources
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -21617,35 +21407,34 @@
         domain_cname: str = None,
         domain_name: str = None,
         status: str = None,
         update_time: str = None,
     ):
         # The workload type of the accelerated domain name. Valid values:
         # 
-        # *   **web**: images and small files.
-        # *   **download**: large files.
-        # *   **video**: on-demand video and audio streaming.
+        # *   **web**: images and small files
+        # *   **download**: large files
+        # *   **video**: on-demand video and audio streaming
         self.cdn_type = cdn_type
-        # The time when the domain name was added to Alibaba Cloud CDN.
+        # The creation time.
         self.create_time = create_time
-        # The CNAME assigned to the domain name.
+        # The CNAME record assigned to the domain name.
         self.domain_cname = domain_cname
         # The domain name.
         self.domain_name = domain_name
-        # The status of the accelerated domain name. Valid values:
+        # The status of the domain name. Valid values:
         # 
         # *   **applying**: The domain name is under review.
-        # *   **configure_failed**: The domain name failed the review.
         # *   **configuring**: The domain name is being configured.
         # *   **online**: The domain name is working as expected.
         # *   **stopping**: The domain name is being stopped.
         # *   **offline**: The domain name is disabled.
-        # *   **disabling**: The domain name is being disabled.
+        # *   **disabling**: The domain name is being removed.
         self.status = status
-        # The time when the configuration was updated.
+        # The update time.
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -21749,19 +21538,19 @@
 class DescribeDomainsBySourceResponseBodyDomainsListDomainsData(TeaModel):
     def __init__(
         self,
         domain_infos: DescribeDomainsBySourceResponseBodyDomainsListDomainsDataDomainInfos = None,
         domains: DescribeDomainsBySourceResponseBodyDomainsListDomainsDataDomains = None,
         source: str = None,
     ):
-        # The detailed information about the domain name. The data is indicated by the domainInfo parameter. Data type: array.
+        # Information about the domain name.
         self.domain_infos = domain_infos
-        # The domain names that correspond to each origin server. The domain name is indicated by the domainNames parameter.
+        # The domain names that correspond to each origin server.
         self.domains = domains
-        # An origin server.
+        # The origin server.
         self.source = source
 
     def validate(self):
         if self.domain_infos:
             self.domain_infos.validate()
         if self.domains:
             self.domains.validate()
@@ -21831,15 +21620,15 @@
 class DescribeDomainsBySourceResponseBody(TeaModel):
     def __init__(
         self,
         domains_list: DescribeDomainsBySourceResponseBodyDomainsList = None,
         request_id: str = None,
         sources: str = None,
     ):
-        # The domain names corresponding to each origin server. The data is indicated by the DomainsData parameter. Data type: array.
+        # The domain names corresponding to each origin server.
         self.domains_list = domains_list
         # The ID of the request.
         self.request_id = request_id
         # The origin servers.
         self.sources = sources
 
     def validate(self):
@@ -22291,21 +22080,25 @@
 class DescribeEsExceptionDataRequest(TeaModel):
     def __init__(
         self,
         end_time: str = None,
         rule_id: str = None,
         start_time: str = None,
     ):
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end of the time range to query.
         # 
-        # >  The end time must be later than the start time.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The ID of the script that you want to query. You can call the [DescribeCdnDomainConfigs](~~90924~~) operation to query script IDs.
+        # The script ID. You can call the [DescribeCdnDomainConfigs](~~90924~~) operation to query script IDs.
         self.rule_id = rule_id
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The beginning of the time range to query.
+        # 
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22333,14 +22126,15 @@
 
 
 class DescribeEsExceptionDataResponseBodyContentsPoints(TeaModel):
     def __init__(
         self,
         points: List[str] = None,
     ):
+        # The data points.
         self.points = points
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22362,19 +22156,19 @@
 class DescribeEsExceptionDataResponseBodyContents(TeaModel):
     def __init__(
         self,
         columns: List[str] = None,
         name: str = None,
         points: List[DescribeEsExceptionDataResponseBodyContentsPoints] = None,
     ):
-        # The column names of the chart that shows the errors of the script and the time of each data entry.
+        # Information about the time column and the error column name.
         self.columns = columns
-        # The name of the chart that shows the errors of the script.
+        # The name of the table that shows the errors of the script.
         self.name = name
-        # The value of each time and the column of each data entry.
+        # The time columns and error column names.
         self.points = points
 
     def validate(self):
         if self.points:
             for k in self.points:
                 if k:
                     k.validate()
@@ -22411,15 +22205,15 @@
 
 class DescribeEsExceptionDataResponseBody(TeaModel):
     def __init__(
         self,
         contents: List[DescribeEsExceptionDataResponseBodyContents] = None,
         request_id: str = None,
     ):
-        # The content of the script.
+        # The content of the script for which an error was reported.
         self.contents = contents
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.contents:
             for k in self.contents:
@@ -22499,21 +22293,21 @@
 class DescribeEsExecuteDataRequest(TeaModel):
     def __init__(
         self,
         end_time: str = None,
         rule_id: str = None,
         start_time: str = None,
     ):
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The ID of the script that you want to query. You can call the [DescribeCdnDomainConfigs](~~90924~~) operation to query script IDs.
+        # The ID of the rule. You can call the [DescribeCdnDomainConfigs](~~90924~~) operation to query script IDs.
         self.rule_id = rule_id
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22543,19 +22337,19 @@
 class DescribeEsExecuteDataResponseBodyContents(TeaModel):
     def __init__(
         self,
         columns: List[str] = None,
         name: str = None,
         points: List[str] = None,
     ):
-        # The column names of the chart that shows the status of the script and the time of each data entry.
+        # The time and column names in the table that shows the status of the script.
         self.columns = columns
-        # The name of the chart that shows the status of the script.
+        # The name of the table that shows the status of the script.
         self.name = name
-        # The value of each time and the column of each data entry.
+        # The list of timestamps and values in the corresponding columns of the table that shows the status of the script.
         self.points = points
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22707,15 +22501,15 @@
         source_arn: str = None,
         trigger_arn: str = None,
     ):
         # The name of the event.
         self.event_meta_name = event_meta_name
         # The version of the event.
         self.event_meta_version = event_meta_version
-        # The remarks.
+        # The remarks of the Function Compute trigger.
         self.notes = notes
         # The assigned Resource Access Management (RAM) role.
         self.role_arn = role_arn
         # The resources and filters for event listening.
         self.source_arn = source_arn
         # The trigger that corresponds to the Function Compute service.
         self.trigger_arn = trigger_arn
@@ -22874,17 +22668,17 @@
         self,
         download_url: str = None,
         request_id: str = None,
         status: str = None,
     ):
         # The URL where you can download the file that contains invalid URLs. This parameter is valid only if the export task is successful.
         self.download_url = download_url
-        # The ID of the request.
+        # The operation that you want to perform. Set the value to **DescribeIllegalUrlExportTask**.
         self.request_id = request_id
-        # The status of the export task. A value of **complete** indicates that the task is successful.
+        # The ID of the request.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22989,22 +22783,22 @@
         cdn_ip: str = None,
         isp: str = None,
         isp_ename: str = None,
         region: str = None,
         region_ename: str = None,
         request_id: str = None,
     ):
-        # Indicates whether the specified IP address is assigned to an Alibaba Cloud CDN node.
+        # Indicates whether the IP address belongs to an Alibaba Cloud CDN POP.
         # 
-        # *   **True**: Yes
-        # *   **False**: No
+        # *   **True**\
+        # *   **False**\
         self.cdn_ip = cdn_ip
-        # The Chinese name of the Internet service provider (ISP).
+        # The Chinese name of the ISP.
         self.isp = isp
-        # The English name of the ISP.
+        # The English name of the Internet service provider (ISP).
         self.isp_ename = isp_ename
         # The Chinese name of the region.
         self.region = region
         # The English name of the region.
         self.region_ename = region_ename
         # The ID of the request.
         self.request_id = request_id
@@ -23123,21 +22917,21 @@
 
 class DescribeIpStatusResponseBodyIpStatus(TeaModel):
     def __init__(
         self,
         ip: str = None,
         status: str = None,
     ):
-        # The IP address of the node.
+        # The IP address of the POP.
         self.ip = ip
-        # The status. Valid values:
+        # The status.
         # 
-        # *   **nonali**: The node is not an Alibaba Cloud CDN edge node.
-        # *   **normal**: The node is an available Alibaba Cloud CDN edge node.
-        # *   **abnormal**: The node is an unavailable Alibaba Cloud CDN edge node.
+        # *   **nonali**: not an Alibaba Cloud CDN POP
+        # *   **normal**: an available Alibaba Cloud CDN POP
+        # *   **abnormal**: an unavailable Alibaba Cloud CDN POP
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -23162,15 +22956,15 @@
 
 class DescribeIpStatusResponseBody(TeaModel):
     def __init__(
         self,
         ip_status: List[DescribeIpStatusResponseBodyIpStatus] = None,
         request_id: str = None,
     ):
-        # The status of the node IP addresses.
+        # The status of the IP addresses of the POPs.
         self.ip_status = ip_status
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.ip_status:
             for k in self.ip_status:
@@ -23786,29 +23580,29 @@
         self,
         end_time: str = None,
         interval: str = None,
         log_store: str = None,
         project: str = None,
         start_time: str = None,
     ):
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # The end of the time range to query. The end time must be later than the start time.
+        # The end time must be later than the start time.
         self.end_time = end_time
-        # The time interval between the data entries. Unit: seconds. The value varies based on the values of the **StartTime** and **EndTime** parameters. Valid values:
+        # The time granularity of the data entries. Unit: seconds. The value varies based on the values of the **StartTime** and **EndTime** parameters. Valid values:
         # 
         # *   If the time span between StartTime and EndTime is less than 3 days, valid values are **300**, **3600**, and **86400**. Default value: **300**.
-        # *   If the time span between StartTime and EndTime is from 3 to 31 days (31 days excluded), valid values are **3600** and **86400**. Default value: **3600**.
+        # *   If the time span between StartTime and EndTime is greater than or equal to 3 days and less than 31 days, valid values are **3600** and **86400**. Default value: **3600**.
         # *   If the time span between StartTime and EndTime is 31 days or longer, the valid value is **86400**. Default value: **86400**.
         self.interval = interval
-        # The name of the Logstore that collects log data from Alibaba Cloud Content Delivery Network (CDN) in real time. By default, all Logstores are queried.
+        # The name of the Logstore that stores log data. If you do leave this parameter empty, real-time log deliveries of all Logstores are queried.
         self.log_store = log_store
-        # The name of the Log Service project that is used for real-time log delivery. By default, all projects are queried.
+        # The name of the Log Service project that is used for real-time log delivery. If you do leave this parameter empty, real-time log deliveries of all projects are queried.
         self.project = project
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -23850,15 +23644,15 @@
         success_num: int = None,
         time_stamp: str = None,
     ):
         # The number of failed attempts to deliver log data to Log Service.
         self.failed_num = failed_num
         # The number of successful deliveries of log data to Log Service.
         self.success_num = success_num
-        # The timestamp of the data.
+        # The timestamp of the data returned.
         self.time_stamp = time_stamp
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -23922,15 +23716,15 @@
 
 class DescribeRealtimeDeliveryAccResponseBody(TeaModel):
     def __init__(
         self,
         reat_time_delivery_acc_data: DescribeRealtimeDeliveryAccResponseBodyReatTimeDeliveryAccData = None,
         request_id: str = None,
     ):
-        # The information about real-time log delivery.
+        # The statistics about real-time log deliveries.
         self.reat_time_delivery_acc_data = reat_time_delivery_acc_data
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.reat_time_delivery_acc_data:
             self.reat_time_delivery_acc_data.validate()
@@ -24051,35 +23845,35 @@
         regex_remain: str = None,
         request_id: str = None,
         url_quota: str = None,
         url_remain: str = None,
     ):
         # The maximum number of URLs and directories that can be blocked on the current day.
         self.block_quota = block_quota
-        # The remaining number of URLs and directories that can be blocked on the current day.
+        # The remaining number of URLs that can be blocked on the current day.
         self.block_remain = block_remain
         # The maximum number of directories that can be refreshed on the current day.
         self.dir_quota = dir_quota
         # The remaining number of directories that can be refreshed on the current day.
         self.dir_remain = dir_remain
         self.ignore_params_quota = ignore_params_quota
         self.ignore_params_remain = ignore_params_remain
-        # The maximum number of times that you can prefetch content to L1 nodes on the current day.
+        # The maximum number of times that you can prefetch content to L1 POPs on the current day.
         self.preload_edge_quota = preload_edge_quota
-        # The remaining number of times that you can prefetch content to L1 nodes on the current day.
+        # The remaining number of times that you can prefetch content to L1 POPs on the current day.
         self.preload_edge_remain = preload_edge_remain
-        # The maximum number of times that you can prefetch content to L2 nodes on the current day.
+        # The maximum number of times that you can prefetch content to L2 POPs on the current day.
         self.preload_quota = preload_quota
-        # The remaining number of times that you can prefetch content to L2 nodes on the current day.
+        # The remaining number of times that you can prefetch content to L2 points of presence (POPs) on the current day.
         self.preload_remain = preload_remain
-        # The maximum number of times that you can use regular expressions to refresh directories or URLs on the current day.
+        # The maximum number of URLs or directories that can be refreshed by using regular expressions on the current day.
         self.regex_quota = regex_quota
-        # The remaining number of times that you can use regular expressions to refresh directories or URLs on the current day.
+        # The remaining number of URLs or directories that can be refreshed by using regular expressions on the current day.
         self.regex_remain = regex_remain
-        # The ID of the request
+        # The ID of the request.
         self.request_id = request_id
         # The maximum number of URLs that can be refreshed on the current day.
         self.url_quota = url_quota
         # The remaining number of URLs that can be refreshed on the current day.
         self.url_remain = url_remain
 
     def validate(self):
@@ -24203,19 +23997,20 @@
 
 
 class DescribeRefreshTaskByIdRequest(TeaModel):
     def __init__(
         self,
         task_id: str = None,
     ):
-        # The ID of the task that you want to query.
-        # 
-        # You can call the [RefreshObjectCaches](~~91164~~) operation to query task IDs. Then, you can use the task IDs to query task status.
+        # The status of the task. Valid values:
         # 
-        # You can specify up to 10 task IDs. Separate task IDs with commas (,).
+        # *   **Complete**: The task is complete.
+        # *   **Pending**: The task is pending.
+        # *   **Refreshing**: The task is running.
+        # *   **Failed**: The task failed.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -24241,41 +24036,42 @@
         description: str = None,
         object_path: str = None,
         object_type: str = None,
         process: str = None,
         status: str = None,
         task_id: str = None,
     ):
-        # The time when the task was created. The time is displayed in UTC.
+        # The path of the object refreshed by the refresh task.
         self.creation_time = creation_time
-        # The error returned when the refresh or prefetch task failed. Valid values:
-        # 
-        # *   **Internal Error**: An internal error occurred.
-        # *   **Origin Timeout**: The response from the origin server timed out.
-        # *   **Origin Return StatusCode 5XX**: The origin server returned a 5XX error.
+        # The tasks.
         self.description = description
-        # The path of the object refreshed by the refresh task.
-        self.object_path = object_path
         # The type of the task. Valid values:
         # 
         # *   **file**: refreshes an individual file.
         # *   **directory**: refreshes files under the specified directory.
         # *   **preload**: prefetches an individual file.
         # *   **regex**: refreshes content based on a regular expression.
+        self.object_path = object_path
+        # The ID of the task.
         self.object_type = object_type
-        # The progress of the task, in percentage.
+        # > - You can query data within the last three days.
+        # - You can call this operation up to 30 times per second per account.
         self.process = process
+        # The error returned when the refresh or prefetch task failed. Valid values:
+        # 
+        # *   **Internal Error**: An internal error occurred.
+        # *   **Origin Timeout**: The response from the origin server timed out.
+        # *   **Origin Return StatusCode 5XX**: The origin server returned a 5XX error.
+        self.status = status
         # The status of the task. Valid values:
         # 
         # *   **Complete**: The task is complete.
         # *   **Pending**: The task is pending.
         # *   **Refreshing**: The task is running.
         # *   **Failed**: The task failed.
-        self.status = status
-        # The ID of the task.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -24321,19 +24117,24 @@
 class DescribeRefreshTaskByIdResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tasks: List[DescribeRefreshTaskByIdResponseBodyTasks] = None,
         total_count: int = None,
     ):
-        # The ID of the request.
+        # The type of the task. Valid values:
+        # 
+        # *   **file**: refreshes an individual file.
+        # *   **directory**: refreshes files under the specified directory.
+        # *   **preload**: prefetches an individual file.
+        # *   **regex**: refreshes content based on a regular expression.
         self.request_id = request_id
-        # The tasks.
+        # The progress of the task, in percentage.
         self.tasks = tasks
-        # The total number of tasks.
+        # The time when the task was created. The time is displayed in UTC.
         self.total_count = total_count
 
     def validate(self):
         if self.tasks:
             for k in self.tasks:
                 if k:
                     k.validate()
@@ -24424,48 +24225,25 @@
         page_size: int = None,
         resource_group_id: str = None,
         security_token: str = None,
         start_time: str = None,
         status: str = None,
         task_id: str = None,
     ):
-        # The accelerated domain name. You can specify only one accelerated domain name in each call. By default, this operation queries the status of tasks for all accelerated domain names.
         self.domain_name = domain_name
-        # The end time. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The path of the object. The path is used as a condition for exact matching.
         self.object_path = object_path
-        # The type of the task. Valid values:
-        # 
-        # *   **file**: refreshes one or more files.
-        # *   **directory**: refreshes files in the specified directories.
-        # *   **regex**: refreshes content based on a regular expression.
-        # *   **preload**: prefetches one or more files.
-        # 
-        # > If you set the **DomainName** or **Status** parameter, you must also set the **ObjectType** parameter.
         self.object_type = object_type
         self.owner_id = owner_id
-        # The number of the page to return. Valid values: **1** to **100000**.
         self.page_number = page_number
-        # The number of entries to return on each page. Default value: **20**. Maximum value: **100**. Valid values: **1** to **100**.
         self.page_size = page_size
-        # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.security_token = security_token
-        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
-        # The status of the task. Valid values:
-        # 
-        # *   **Complete**: The task has completed.
-        # *   **Refreshing**: The task is in progress.
-        # *   **Failed**: The task failed.
         self.status = status
-        # The ID of the task that you want to query.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -24535,40 +24313,20 @@
         description: str = None,
         object_path: str = None,
         object_type: str = None,
         process: str = None,
         status: str = None,
         task_id: str = None,
     ):
-        # The time when the task was created. The time is displayed in UTC.
         self.creation_time = creation_time
-        # The type of the error returned when the refresh or prefetch task failed. Valid values:
-        # 
-        # *   **InternalError**: An internal error occurred.
-        # *   **OriginTimeout**: The response from the origin server timed out.
-        # *   **OriginReturnStatusCode 5XX**: The origin server returned a 5XX error.
         self.description = description
-        # The URL of the object refreshed.
         self.object_path = object_path
-        # The type of the task.
-        # 
-        # *   **file**: refreshes one or more files.
-        # *   **directory**: refreshes files in the specified directories.
-        # *   **regex**: refreshes content based on a regular expression.
-        # *   **preload**: prefetches one or more files.
         self.object_type = object_type
-        # The progress of the task, in percentage.
         self.process = process
-        # The status of the task. Valid values:
-        # 
-        # *   **Complete**: The task has completed.
-        # *   **Refreshing**: The task is in progress.
-        # *   **Failed**: The task failed.
         self.status = status
-        # The ID of the task.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -24651,23 +24409,18 @@
         self,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         tasks: DescribeRefreshTasksResponseBodyTasks = None,
         total_count: int = None,
     ):
-        # The page number of the returned page.
         self.page_number = page_number
-        # The number of entries returned per page.
         self.page_size = page_size
-        # The ID of the request.
         self.request_id = request_id
-        # Details about tasks.
         self.tasks = tasks
-        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.tasks:
             self.tasks.validate()
 
     def to_map(self):
@@ -24777,17 +24530,17 @@
 
 class DescribeStagingIpResponseBody(TeaModel):
     def __init__(
         self,
         ipv4s: DescribeStagingIpResponseBodyIPV4s = None,
         request_id: str = None,
     ):
-        # The IPv4 addresses of the nodes.
-        self.ipv4s = ipv4s
         # The ID of the request.
+        self.ipv4s = ipv4s
+        # The IPv4 addresses of the nodes.
         self.request_id = request_id
 
     def validate(self):
         if self.ipv4s:
             self.ipv4s.validate()
 
     def to_map(self):
@@ -24858,17 +24611,15 @@
 
 class DescribeTagResourcesRequestTag(TeaModel):
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
@@ -24894,19 +24645,16 @@
 class DescribeTagResourcesRequest(TeaModel):
     def __init__(
         self,
         resource_id: List[str] = None,
         resource_type: str = None,
         tag: List[DescribeTagResourcesRequestTag] = None,
     ):
-        # The IDs of the resources. You can specify up to 50 IDs in each request.
         self.resource_id = resource_id
-        # The type of the resource. Set this value to **DOMAIN**.
         self.resource_type = resource_type
-        # The tags. You can specify up to 20 tags in each request.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -24943,17 +24691,15 @@
 
 class DescribeTagResourcesResponseBodyTagResourcesTag(TeaModel):
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
@@ -24978,17 +24724,15 @@
 
 class DescribeTagResourcesResponseBodyTagResources(TeaModel):
     def __init__(
         self,
         resource_id: str = None,
         tag: List[DescribeTagResourcesResponseBodyTagResourcesTag] = None,
     ):
-        # The ID of the resource.
         self.resource_id = resource_id
-        # The tags.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -25021,17 +24765,15 @@
 
 class DescribeTagResourcesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tag_resources: List[DescribeTagResourcesResponseBodyTagResources] = None,
     ):
-        # The ID of the request.
         self.request_id = request_id
-        # Details about the tag.
         self.tag_resources = tag_resources
 
     def validate(self):
         if self.tag_resources:
             for k in self.tag_resources:
                 if k:
                     k.validate()
@@ -25111,21 +24853,21 @@
         self,
         end_time: str = None,
         limit: int = None,
         start_time: str = None,
     ):
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
         # The maximum number of domain names to query. Valid values: **1** to **100**. Default value: **20**.
         self.limit = limit
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  Set StartTime to UTC time in the yyyy-MM-ddTHH:mm:ssZ format. For example, if the local time is 00:00, June 1, 2021, set StartTime to 2021-05-31T16:00:00Z.
+        # > The value of StartTime must be in UTC. For example, if the local time is 00:00 on June 1, 2021, set StartTime to 2021-05-31T16:00:00Z.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25167,19 +24909,19 @@
         self.domain_name = domain_name
         # The peak bandwidth value.
         self.max_bps = max_bps
         # The time when the bandwidth reached the peak value.
         self.max_bps_time = max_bps_time
         # The ranking of the accelerated domain name.
         self.rank = rank
-        # The number of visits to the accelerated domain name.
+        # The number of visits to the domain name.
         self.total_access = total_access
-        # The total amount of network traffic.
+        # The total volume of traffic.
         self.total_traffic = total_traffic
-        # The proportion of the amount of network traffic consumed for visiting the web page.
+        # The proportion of network traffic consumed to access the domain name.
         self.traffic_percent = traffic_percent
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25271,15 +25013,15 @@
         self.domain_count = domain_count
         # The total number of accelerated domain names that are in the **Enabled** state within the current Alibaba Cloud account.
         self.domain_online_count = domain_online_count
         # The end of the time range during which data was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range during which data was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
         # The top N domain names ranked by network traffic.
         self.top_domains = top_domains
 
     def validate(self):
         if self.top_domains:
             self.top_domains.validate()
@@ -25369,19 +25111,18 @@
 class DescribeUserCertificateExpireCountResponseBody(TeaModel):
     def __init__(
         self,
         expire_within_30days_count: int = None,
         expired_count: int = None,
         request_id: str = None,
     ):
-        # The number of domain names whose SSL certificates are about to expire within 30 days.
+        # The ID of the request.
         self.expire_within_30days_count = expire_within_30days_count
-        # The number of domain names whose SSL certificates have already expired.
         self.expired_count = expired_count
-        # The ID of the request.
+        # The number of domain names whose SSL certificates have already expired.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25455,14 +25196,15 @@
 class DescribeUserConfigsRequest(TeaModel):
     def __init__(
         self,
         config: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
+        # The feature whose configurations you want to query. You can specify only one feature in each request. Valid values: oss, green_manager, waf, cc_rule, ddos_dispatch, edge_safe, blocked_regions, http_acl_policy, bot_manager, and ip_reputation.
         self.config = config
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
@@ -25494,16 +25236,19 @@
 class DescribeUserConfigsResponseBodyConfigsOssLogConfig(TeaModel):
     def __init__(
         self,
         bucket: str = None,
         enable: str = None,
         prefix: str = None,
     ):
+        # The name of the bucket.
         self.bucket = bucket
+        # Indicates whether the OSS bucket is enabled.
         self.enable = enable
+        # The prefix.
         self.prefix = prefix
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25531,14 +25276,15 @@
 
 
 class DescribeUserConfigsResponseBodyConfigsWafConfig(TeaModel):
     def __init__(
         self,
         enable: str = None,
     ):
+        # Indicates whether WAF is enabled.
         self.enable = enable
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25559,15 +25305,17 @@
 
 class DescribeUserConfigsResponseBodyConfigs(TeaModel):
     def __init__(
         self,
         oss_log_config: DescribeUserConfigsResponseBodyConfigsOssLogConfig = None,
         waf_config: DescribeUserConfigsResponseBodyConfigsWafConfig = None,
     ):
+        # The configurations of Object Storage Service (OSS).
         self.oss_log_config = oss_log_config
+        # The configurations of Web Application Firewall (WAF).
         self.waf_config = waf_config
 
     def validate(self):
         if self.oss_log_config:
             self.oss_log_config.validate()
         if self.waf_config:
             self.waf_config.validate()
@@ -25597,14 +25345,15 @@
 
 class DescribeUserConfigsResponseBody(TeaModel):
     def __init__(
         self,
         configs: DescribeUserConfigsResponseBodyConfigs = None,
         request_id: str = None,
     ):
+        # The configurations of the specified feature.
         self.configs = configs
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.configs:
             self.configs.validate()
@@ -25677,19 +25426,19 @@
 
 class DescribeUserDomainsRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # The key of the tag. Valid values of N: **1** to **20**.
+        # The key of a tag.
         # 
         # By default, all tag keys are queried.
         self.key = key
-        # The value of the tag. Valid values of N: **1** to **20**.
+        # The value of the tag.
         # 
         # By default, all tag values are queried.
         self.value = value
 
     def validate(self):
         pass
 
@@ -25739,64 +25488,64 @@
         # *   **download**: large files
         # *   **video**: on-demand video and audio streaming
         # 
         # If you do not set this parameter, all service types are queried.
         self.cdn_type = cdn_type
         # The end of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.change_end_time = change_end_time
         # The beginning of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.change_start_time = change_start_time
         # Specifies whether to display domain names that are under review, failed the review, or failed to be configured. Valid values:
         # 
-        # *   **true**: yes
-        # *   **false**: no
+        # *   **true**\
+        # *   **false**\
         self.check_domain_show = check_domain_show
-        # The accelerated region. By default, all accelerated regions are queried. Valid values:
+        # The acceleration region. By default, all acceleration regions are queried. Valid values:
         # 
         # *   **domestic**: Chinese mainland
-        # *   **global**\
-        # *   **overseas**: global (excluding the Chinese mainland)
+        # *   **global**: global
+        # *   **overseas**: outside the Chinese mainland
         self.coverage = coverage
-        # The accelerated domain names. If you do not set this parameter, configurations of all domain names that match the conditions are returned.
+        # The accelerated domain. If you do not set this parameter, all domain names that match the conditions are returned.
         self.domain_name = domain_name
         # The search mode. Valid values:
         # 
         # *   **fuzzy_match**: fuzzy match
         # *   **pre_match**: prefix match
         # *   **suf_match**: suffix match
         # *   **full_match** (default): exact match
         # 
-        # >  If you specify the domain names to query but do not set the DomainSearchType parameter, the exact match mode is used.
+        # > If you specify the domain names to query but do not set the DomainSearchType parameter, the exact match mode is used.
         self.domain_search_type = domain_search_type
-        # The status of the domain name. You can filter domain names by status. Valid values:
+        # The status of the domain name. Valid values:
         # 
-        # *   **online**: enabled
-        # *   **offline**: disabled
-        # *   **configuring**: being configured
-        # *   **configure_failed**: failed to be configured
-        # *   **checking**: under review
-        # *   **check_failed**: failed the review
-        # *   **stopping**: being disabled
-        # *   **deleting**: deleting
+        # *   **online**\
+        # *   **offline**\
+        # *   **configuring**\
+        # *   **configure_failed**\
+        # *   **checking**\
+        # *   **check_failed**\
+        # *   **stopping**\
+        # *   **deleting**\
         # 
-        # If you do not set this parameter, all states are queried.
+        # If you do not set this parameter, domain names in all states are queried.
         self.domain_status = domain_status
         self.owner_id = owner_id
         # The number of the page to return. Valid values: **1** to **100000**.
         self.page_number = page_number
         # The number of entries to return on each page. Valid values: **1 to 50**. Default value: **20**. Maximum value: **50**.
         self.page_size = page_size
         # The ID of the resource group. By default, all IDs are queried.
         self.resource_group_id = resource_group_id
         self.security_token = security_token
         # The information about the origin server.
         self.source = source
-        # The tags.
+        # The list of tags. Maximum number of elements in the list: 20
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -25888,19 +25637,19 @@
         type: str = None,
         weight: str = None,
     ):
         # The address of the origin server.
         self.content = content
         # The port of the origin server.
         self.port = port
-        # The priority of the origin server.
+        # The priority.
         self.priority = priority
         # The type of the origin server.
         self.type = type
-        # The weight of the origin server if multiple origin servers are specified.
+        # The weight of the origin server if multiple origin servers have been specified.
         self.weight = weight
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25983,59 +25732,59 @@
         gmt_created: str = None,
         gmt_modified: str = None,
         resource_group_id: str = None,
         sandbox: str = None,
         sources: DescribeUserDomainsResponseBodyDomainsPageDataSources = None,
         ssl_protocol: str = None,
     ):
-        # The type of workload accelerated by Alibaba Cloud CDN. Valid values:
+        # The type of the workload accelerated by Alibaba Cloud CDN. Valid values:
         # 
         # *   **web**: images and small files
         # *   **download**: large files
         # *   **video**: on-demand video and audio streaming
         self.cdn_type = cdn_type
         # The CNAME assigned to the accelerated domain name.
         self.cname = cname
         # The acceleration region. Valid values:
         # 
         # *   **domestic**: Chinese mainland
-        # *   **global**\
-        # *   **overseas**: global (excluding the Chinese mainland)
+        # *   **global**: global
+        # *   **overseas**: outside the Chinese mainland
         self.coverage = coverage
-        # The information about the Internet Content Provider (ICP) number.
+        # The information about Internet Content Provider (ICP) filing.
         self.description = description
         # The ID of the accelerated domain name.
         self.domain_id = domain_id
-        # The accelerated domain names.
+        # The accelerated domain.
         self.domain_name = domain_name
         # The status of the accelerated domain name. Valid values:
         # 
-        # *   **online**: enabled
-        # *   **offline**: disabled
-        # *   **configuring**: being configured
-        # *   **configure_failed**: failed to be configured
-        # *   **checking**: under review
-        # *   **check_failed**: failed the review
-        # *   **stopping**: being disabled
-        # *   **deleting**: deleting
+        # *   **online**\
+        # *   **offline**\
+        # *   **configuring**\
+        # *   **configure_failed**\
+        # *   **checking**\
+        # *   **check_failed**\
+        # *   **stopping**\
+        # *   **deleting**\
         self.domain_status = domain_status
-        # The time when the accelerated domain name was added to Alibaba Cloud CDN.
+        # The time when the accelerated domain name was added.
         self.gmt_created = gmt_created
-        # The time when the accelerated domain name was last modified.
+        # The time when the accelerated domain name was modified.
         self.gmt_modified = gmt_modified
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         # Indicates whether the accelerated domain name is in a sandbox.
         self.sandbox = sandbox
         # The information about the origin server.
         self.sources = sources
         # Indicates whether HTTPS is enabled. Valid values:
         # 
-        # *   **on**: enabled
-        # *   **off**: disabled
+        # *   **on**\
+        # *   **off**\
         self.ssl_protocol = ssl_protocol
 
     def validate(self):
         if self.sources:
             self.sources.validate()
 
     def to_map(self):
@@ -26144,23 +25893,23 @@
         self,
         domains: DescribeUserDomainsResponseBodyDomains = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The information about the accelerated domain name.
+        # The list of the accelerated domain names returned.
         self.domains = domains
         # The page number of the returned page.
         self.page_number = page_number
         # The number of entries returned per page.
         self.page_size = page_size
         # The ID of the request.
         self.request_id = request_id
-        # Indicates the total number of entries returned.
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.domains:
             self.domains.validate()
 
     def to_map(self):
@@ -26243,17 +25992,17 @@
 
 class DescribeUserTagsResponseBodyTags(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: List[str] = None,
     ):
-        # The key of the tag.
+        # The value of the tag.
         self.key = key
-        # The list of tag value.
+        # The ID of the request.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -26278,17 +26027,17 @@
 
 class DescribeUserTagsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tags: List[DescribeUserTagsResponseBodyTags] = None,
     ):
-        # The ID of the request.
-        self.request_id = request_id
         # The list of tags returned.
+        self.request_id = request_id
+        # The key of the tag.
         self.tags = tags
 
     def validate(self):
         if self.tags:
             for k in self.tags:
                 if k:
                     k.validate()
@@ -26365,19 +26114,17 @@
 
 class DescribeUserUsageDataExportTaskRequest(TeaModel):
     def __init__(
         self,
         page_number: str = None,
         page_size: str = None,
     ):
-        # The number of the page to return. Valid values: **1** to **100000**.
+        # The name of the task.
         self.page_number = page_number
-        # The number of entries to return on each page. Default value: **20**. Maximum value: **50**.
-        # 
-        # Valid values: **1** to **50**.
+        # The usage details returned per page.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -26402,17 +26149,17 @@
 
 class DescribeUserUsageDataExportTaskResponseBodyUsageDataPerPageDataDataItemTaskConfig(TeaModel):
     def __init__(
         self,
         end_time: str = None,
         start_time: str = None,
     ):
-        # The end of the time range that was queried.
+        # The ID of the request.
         self.end_time = end_time
-        # The start of the time range that was queried.
+        # The last time when the task was modified.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -26442,31 +26189,29 @@
         download_url: str = None,
         status: str = None,
         task_config: DescribeUserUsageDataExportTaskResponseBodyUsageDataPerPageDataDataItemTaskConfig = None,
         task_id: str = None,
         task_name: str = None,
         update_time: str = None,
     ):
-        # The time when the task was created.
-        self.create_time = create_time
         # The download URL.
+        self.create_time = create_time
+        # The configurations of the task.
         self.download_url = download_url
-        # The status of the task.
-        # 
-        # *   created: The task is being created.
-        # *   success: The task has been created.
-        # *   failed: The creation of the task failed.
+        # The time when the task was created.
         self.status = status
-        # The configurations of the task.
+        # The total number of entries returned.
         self.task_config = task_config
-        # The ID of the task.
+        # The number of the current page.
         self.task_id = task_id
-        # The name of the task.
+        # The number of entries to return on each page. Default value: **20**. Maximum value: **50**.
+        # 
+        # Valid values: **1** to **50**.
         self.task_name = task_name
-        # The last time when the task was modified.
+        # The operation that you want to perform. Set the value to **DescribeUserUsageDataExportTask**.
         self.update_time = update_time
 
     def validate(self):
         if self.task_config:
             self.task_config.validate()
 
     def to_map(self):
@@ -26550,21 +26295,25 @@
     def __init__(
         self,
         data: DescribeUserUsageDataExportTaskResponseBodyUsageDataPerPageData = None,
         page_number: int = None,
         page_size: int = None,
         total_count: int = None,
     ):
-        # The description of the task.
+        # The status of the task.
+        # 
+        # *   created: The task is being created.
+        # *   success: The task has been created.
+        # *   failed: The creation of the task failed.
         self.data = data
-        # The number of the current page.
+        # The number of the page to return. Valid values: **1** to **100000**.
         self.page_number = page_number
-        # The number of entries returned per page.
+        # The description of the task.
         self.page_size = page_size
-        # The total number of entries returned.
+        # The start of the time range that was queried.
         self.total_count = total_count
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -26599,17 +26348,17 @@
 
 class DescribeUserUsageDataExportTaskResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         usage_data_per_page: DescribeUserUsageDataExportTaskResponseBodyUsageDataPerPage = None,
     ):
-        # The ID of the request.
+        # The ID of the task.
         self.request_id = request_id
-        # The usage details returned per page.
+        # The end of the time range that was queried.
         self.usage_data_per_page = usage_data_per_page
 
     def validate(self):
         if self.usage_data_per_page:
             self.usage_data_per_page.validate()
 
     def to_map(self):
@@ -26680,19 +26429,17 @@
 
 class DescribeUserUsageDetailDataExportTaskRequest(TeaModel):
     def __init__(
         self,
         page_number: str = None,
         page_size: str = None,
     ):
-        # The number of the page to return. Valid values: **1** to **100000**.
+        # The name of the task.
         self.page_number = page_number
-        # The number of entries to return on each page. Default value: **20**. Maximum value: **50**.
-        # 
-        # Valid values: **1** to **50**.
+        # The usage details returned per page.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -26717,17 +26464,17 @@
 
 class DescribeUserUsageDetailDataExportTaskResponseBodyUsageDataPerPageDataDataItemTaskConfig(TeaModel):
     def __init__(
         self,
         end_time: str = None,
         start_time: str = None,
     ):
-        # The end of the time range that was queried.
+        # refresh
         self.end_time = end_time
-        # The start of the time range that was queried.
+        # The ID of the request.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -26757,27 +26504,29 @@
         download_url: str = None,
         status: str = None,
         task_config: DescribeUserUsageDetailDataExportTaskResponseBodyUsageDataPerPageDataDataItemTaskConfig = None,
         task_id: str = None,
         task_name: str = None,
         update_time: str = None,
     ):
-        # The time when the task was created.
-        self.create_time = create_time
         # The download URL.
+        self.create_time = create_time
+        # The configurations of the task.
         self.download_url = download_url
-        # The status of the task.
+        # The time when the task was created.
         self.status = status
-        # The configurations of the task.
+        # The total number of entries returned.
         self.task_config = task_config
-        # The ID of the task.
+        # The number of the page returned.
         self.task_id = task_id
-        # The name of the task.
+        # The number of entries to return on each page. Default value: **20**. Maximum value: **50**.
+        # 
+        # Valid values: **1** to **50**.
         self.task_name = task_name
-        # The last time when the task was modified.
+        # The operation that you want to perform. Set the value to **DescribeUserUsageDetailDataExportTask**.
         self.update_time = update_time
 
     def validate(self):
         if self.task_config:
             self.task_config.validate()
 
     def to_map(self):
@@ -26861,21 +26610,21 @@
     def __init__(
         self,
         data: DescribeUserUsageDetailDataExportTaskResponseBodyUsageDataPerPageData = None,
         page_number: int = None,
         page_size: int = None,
         total_count: int = None,
     ):
-        # The description of the task.
+        # The status of the task.
         self.data = data
-        # The number of the page returned.
+        # The number of the page to return. Valid values: **1** to **100000**.
         self.page_number = page_number
-        # The number of the entries returned per page.
+        # The description of the task.
         self.page_size = page_size
-        # The total number of entries returned.
+        # The start of the time range that was queried.
         self.total_count = total_count
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -26910,17 +26659,17 @@
 
 class DescribeUserUsageDetailDataExportTaskResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         usage_data_per_page: DescribeUserUsageDetailDataExportTaskResponseBodyUsageDataPerPage = None,
     ):
-        # The ID of the request.
+        # The ID of the task.
         self.request_id = request_id
-        # The usage details returned per page.
+        # The end of the time range that was queried.
         self.usage_data_per_page = usage_data_per_page
 
     def validate(self):
         if self.usage_data_per_page:
             self.usage_data_per_page.validate()
 
     def to_map(self):
@@ -26991,20 +26740,17 @@
 
 class DescribeUserVipsByDomainRequest(TeaModel):
     def __init__(
         self,
         available: str = None,
         domain_name: str = None,
     ):
-        # Specifies whether to query the virtual IP addresses of only healthy CDN edge nodes. Valid values: Valid values:
-        # 
-        # *   **on**: healthy CDN edge nodes
-        # *   **off**: all CDN edge nodes
+        # The virtual IP address.
         self.available = available
-        # The accelerated domain name. You can specify only one domain name.
+        # A list of virtual IP addresses.
         self.domain_name = domain_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -27057,19 +26803,19 @@
 class DescribeUserVipsByDomainResponseBody(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         request_id: str = None,
         vips: DescribeUserVipsByDomainResponseBodyVips = None,
     ):
-        # The domain name.
+        # >  The maximum number of times that each user can call this operation per second is 30.
         self.domain_name = domain_name
-        # The ID of the request.
-        self.request_id = request_id
         # A list of virtual IP addresses.
+        self.request_id = request_id
+        # The accelerated domain name. You can specify only one domain name.
         self.vips = vips
 
     def validate(self):
         if self.vips:
             self.vips.validate()
 
     def to_map(self):
@@ -27143,15 +26889,14 @@
 
 
 class DescribeVerifyContentRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
     ):
-        # The domain name of which you want to verify the ownership. You can specify only one domain name.
         self.domain_name = domain_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -27172,17 +26917,15 @@
 
 class DescribeVerifyContentResponseBody(TeaModel):
     def __init__(
         self,
         content: str = None,
         request_id: str = None,
     ):
-        # The verification result.
         self.content = content
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -27506,15 +27249,15 @@
 
 class ListDomainsByLogConfigIdResponseBody(TeaModel):
     def __init__(
         self,
         domains: ListDomainsByLogConfigIdResponseBodyDomains = None,
         request_id: str = None,
     ):
-        # The list of domain names.
+        # The domain names.
         self.domains = domains
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.domains:
             self.domains.validate()
@@ -27587,15 +27330,15 @@
 
 class ListFCTriggerRequest(TeaModel):
     def __init__(
         self,
         event_meta_name: str = None,
         event_meta_version: str = None,
     ):
-        # The name of the event for which the Function Compute trigger is set. You can specify only one name.
+        # The name of the event. You can specify only one name.
         self.event_meta_name = event_meta_name
         # The version number of the event. You can specify only one version number.
         self.event_meta_version = event_meta_version
 
     def validate(self):
         pass
 
@@ -27626,25 +27369,25 @@
         event_meta_name: str = None,
         event_meta_version: str = None,
         notes: str = None,
         role_arn: str = None,
         source_arn: str = None,
         trigger_arn: str = None,
     ):
-        # The name of the event for which the Function Compute trigger is set.
+        # The name of the event.
         self.event_meta_name = event_meta_name
-        # The version of the event for which the Function Compute trigger is set.
+        # The version of the event.
         self.event_meta_version = event_meta_version
-        # The remarks for the event.
+        # The remarks.
         self.notes = notes
         # The Resource Access Management (RAM) role.
         self.role_arn = role_arn
         # The resources and filters for event listening.
         self.source_arn = source_arn
-        # The trigger corresponding to the Function Compute service.
+        # The trigger that corresponds to the Function Compute service.
         self.trigger_arn = trigger_arn
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -27685,15 +27428,15 @@
 
 class ListFCTriggerResponseBody(TeaModel):
     def __init__(
         self,
         fctriggers: List[ListFCTriggerResponseBodyFCTriggers] = None,
         request_id: str = None,
     ):
-        # The information about the Function Compute trigger returned.
+        # The Function Compute triggers that are set for Alibaba Cloud CDN events.
         self.fctriggers = fctriggers
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.fctriggers:
             for k in self.fctriggers:
@@ -27773,15 +27516,15 @@
 class ListRealtimeLogDeliveryDomainsRequest(TeaModel):
     def __init__(
         self,
         logstore: str = None,
         project: str = None,
         region: str = None,
     ):
-        # The name of the Logstore that collects log data from Alibaba Cloud Content Delivery Network (CDN) in real time. You can specify multiple Logstore names and separate them with commas (,).
+        # The name of the Logstore that collects log data from Alibaba Cloud CDN in real time. You can specify multiple Logstore names and separate them with commas (,).
         self.logstore = logstore
         # The name of the Log Service project that is used for real-time log delivery. You can specify multiple project names and separate them with commas (,).
         self.project = project
         # The ID of the region where the Log Service project is deployed. You can specify multiple region IDs and separate them with commas (,).
         # 
         # For more information about regions, see [Regions that support real-time log delivery](~~144883~~).
         self.region = region
@@ -27816,20 +27559,20 @@
 
 class ListRealtimeLogDeliveryDomainsResponseBodyContentDomains(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         status: str = None,
     ):
-        # The accelerated domain name.
+        # The domain name.
         self.domain_name = domain_name
-        # The status of the real-time log delivery feature. Valid values:
+        # The status. Valid values:
         # 
-        # *   **online**: The feature is enabled.
-        # *   **offline**: The feature is disabled.
+        # *   **online**: enabled
+        # *   **offline**: disabled
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -27971,15 +27714,15 @@
 class ListRealtimeLogDeliveryInfosResponseBodyContentRealtimeLogDeliveryInfos(TeaModel):
     def __init__(
         self,
         logstore: str = None,
         project: str = None,
         region: str = None,
     ):
-        # The name of the Logstore that collects log data from Alibaba Cloud Content Delivery Network (CDN) in real time.
+        # The name of the Logstore that collects log data from Alibaba Cloud CDN in real time.
         self.logstore = logstore
         # The name of the Log Service project that is used for real-time log delivery.
         self.project = project
         # The ID of the region where the Log Service project is deployed. For more information, see [Regions that support real-time log delivery](~~144883~~).
         self.region = region
 
     def validate(self):
@@ -28047,15 +27790,15 @@
 
 class ListRealtimeLogDeliveryInfosResponseBody(TeaModel):
     def __init__(
         self,
         content: ListRealtimeLogDeliveryInfosResponseBodyContent = None,
         request_id: str = None,
     ):
-        # The content of the log entry.
+        # The information about real-time log delivery.
         self.content = content
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.content:
             self.content.validate()
@@ -28155,17 +27898,17 @@
 
 class ListUserCustomLogConfigResponseBody(TeaModel):
     def __init__(
         self,
         config_ids: ListUserCustomLogConfigResponseBodyConfigIds = None,
         request_id: str = None,
     ):
-        # The list of configuration ID.
-        self.config_ids = config_ids
         # The ID of the request.
+        self.config_ids = config_ids
+        # The ID of the log configuration.
         self.request_id = request_id
 
     def validate(self):
         if self.config_ids:
             self.config_ids.validate()
 
     def to_map(self):
@@ -28240,27 +27983,27 @@
         domain_name: str = None,
         owner_id: int = None,
         resource_group_id: str = None,
         security_token: str = None,
         sources: str = None,
         top_level_domain: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name
         self.owner_id = owner_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.security_token = security_token
-        # The list of origin URLs.
+        # The information about the addresses of origin servers.
         # 
-        # >  You cannot set both the **Sources** and **TopLevelDomain** parameters in the same request. Otherwise, ********the **TopLevelDomain** parameter cannot take effect.
+        # > Do not set **Sources** and **TopLevelDomain** at the same time. If you set **Sources** and **TopLevelDomain** at the same time, **TopLevelDomain** does not take effect.
         self.sources = sources
-        # The top-level domain name. To add a top-level domain name, set the parameter CDN_TOP_LEVEL_DOMAIN_GREY_USER_LIST. This feature is available to only selected users.
+        # The root domain. To add a root domain name, you must be added to the whitelist specified by the CDN_TOP_LEVEL_DOMAIN_GREY_USER_LIST parameter.
         # 
-        # >  You cannot set both the **Sources** and **TopLevelDomain** parameters in the same request. Otherwise, ****the **TopLevelDomain** parameter cannot take effect.
+        # > Do not set **Sources** and **TopLevelDomain** at the same time. If you set **Sources** and **TopLevelDomain** at the same time, **TopLevelDomain** does not take effect.
         self.top_level_domain = top_level_domain
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -28373,15 +28116,15 @@
 
 class ModifyCdnDomainSchdmByPropertyRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         property: str = None,
     ):
-        # The accelerated domain name for which you want to change the accelerated region. You can specify only one domain name.
+        # The operation that you want to perform. Set the value to **ModifyCdnDomainSchdmByProperty**.
         self.domain_name = domain_name
         # The accelerated region. Valid values for coverage:
         # 
         # *   **domestic**: Chinese mainland
         # *   **overseas**: global (excluding the Chinese mainland)
         # *   **global**: global
         self.property = property
@@ -28411,15 +28154,14 @@
 
 
 class ModifyCdnDomainSchdmByPropertyResponseBody(TeaModel):
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
@@ -28486,21 +28228,21 @@
     def __init__(
         self,
         domain: str = None,
         logstore: str = None,
         project: str = None,
         region: str = None,
     ):
-        # The accelerated domain name for which you want to modify the configurations of real-time log delivery. Only one domain name is supported.
+        # The ID of the request.
         self.domain = domain
-        # The name of the Logstore.
+        # The accelerated domain name for which you want to modify the configurations of real-time log delivery. Only one domain name is supported.
         self.logstore = logstore
-        # The name of the Log Service project that is used for real-time log delivery.
-        self.project = project
         # The ID of the region where the Log Service project is deployed. For more information, see [Regions that support real-time log delivery](~~144883~~).
+        self.project = project
+        # The name of the Log Service project that is used for real-time log delivery.
         self.region = region
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -28532,15 +28274,15 @@
 
 
 class ModifyRealtimeLogDeliveryResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
+        # The operation that you want to perform. Set the value to **ModifyRealtimeLogDelivery**.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -28977,23 +28719,24 @@
         self,
         object_path: str = None,
         object_type: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
         self.object_path = object_path
-        # The type of the object that you want to refresh. Default value: File. Valid values:
+        # The type of the object that you want to refresh. Valid values:
         # 
-        # *   **File**: refreshes one or more files.
+        # *   **File** (default): refreshes one or more files.
         # *   **Directory**: refreshes the files in one or more directories.
         # *   **Regex**: refreshes content based on regular expressions.
+        # *   **ExQuery**: omits parameters after the question mark in the URL and refreshes content.
         # 
         # If you set the ObjectType parameter to File or Directory, you can view [Refresh and prefetch resources](~~27140~~) to obtain more information. If you set the ObjectType parameter to Regex, you can view [Configure URL refresh rules that contain regular expressions](~~146195~~) to obtain more information.
         # 
-        # If you set the ObjectType parameter to Directory, the resources in the directory that you want to refresh are marked as expired. You cannot delete the directory. If clients request resources on POPs that are marked as expired, Alibaba Cloud CDN checks whether the resources on your origin server are updated. If resources are updated, Alibaba Cloud CDN retrieves the most recent version of the resources and returns the resources to the clients. Otherwise, the origin server returns the 304 status code.
+        # If you set the ObjectType parameter to Directory, the resources in the directory that you want to refresh are marked as expired. You cannot delete the directory. If clients request resources on POPs that are marked as expired, Alibaba Cloud CDN checks whether the resources on your origin server are updated. If resources are updated, Alibaba Cloud CDN retrieves the latest version of the resources and returns the resources to the clients. Otherwise, the origin server returns the 304 status code.
         self.object_type = object_type
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
@@ -29028,20 +28771,20 @@
 
 class RefreshObjectCachesResponseBody(TeaModel):
     def __init__(
         self,
         refresh_task_id: str = None,
         request_id: str = None,
     ):
-        # The ID of the refresh task. If multiple tasks are returned, the IDs are separated by commas (,). The task IDs are merged based on the following rules:
+        # The refresh task ID. If multiple tasks are returned, the IDs are separated by commas (,). The task IDs are merged based on the following rules:
         # 
         # *   If the tasks are specified for the same accelerated domain name, submitted within the same second, and run to refresh content based on URLs instead of directories, the task IDs are merged into one task ID.
         # *   If the number of tasks that are specified for the same accelerated domain name, submitted within the same second, and run to refresh content based on URLs instead of directories exceeds 2,000, every 2,000 task IDs are merged into one task ID.
         self.refresh_task_id = refresh_task_id
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -29109,15 +28852,15 @@
 
 
 class RollbackStagingConfigRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -29210,15 +28953,15 @@
 
 class SetCdnDomainCSRCertificateRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         server_certificate: str = None,
     ):
-        # The accelerated domain name for which you want to configure an SSL certificate. The domain name must have HTTPS secure acceleration enabled.
+        # The ID of the request.
         self.domain_name = domain_name
         # The content of the certificate. The certificate must match the certificate signing request (CSR) created by calling the [CreateCdnCertificateSigningRequest](~~144478~~) operation. Make sure that the certificate is in the PEM format, and the content of the certificate is encoded in Base64 and then encoded by encodeURIComponent.
         self.server_certificate = server_certificate
 
     def validate(self):
         pass
 
@@ -29244,15 +28987,15 @@
 
 
 class SetCdnDomainCSRCertificateResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
+        # The operation that you want to perform. Set the value to **SetCdnDomainCSRCertificate**.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -29320,25 +29063,25 @@
         self,
         cert_identifier: str = None,
         domain_name: str = None,
         owner_id: int = None,
         sslprotocol: str = None,
         security_token: str = None,
     ):
-        # The ID of the SM certificate that you want to configure.
+        # The ID of the SM certificate that you want to configure. The identifier of the certificate. The value is Certificate ID-cn-hangzhou. For example, if the certificate ID is 123, set the value of this parameter to 123-cn-hangzhou.
         self.cert_identifier = cert_identifier
         # The accelerated domain name for which you want to configure the SM certificate.
         # 
-        # >  The domain name uses HTTPS secure acceleration.
+        # > The domain name must use HTTPS acceleration.
         self.domain_name = domain_name
         self.owner_id = owner_id
         # Specifies whether to enable the SSL certificate. Valid values:
         # 
-        # *   **on**: enables the SSL certificate.
-        # *   **off**: disables the SSL certificate.
+        # *   **on**\
+        # *   **off**\
         self.sslprotocol = sslprotocol
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -29442,45 +29185,173 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SetCdnDomainSMCertificateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SetCdnDomainSSLCertificateRequest(TeaModel):
+    def __init__(
+        self,
+        cert_id: int = None,
+        cert_name: str = None,
+        cert_region: str = None,
+        cert_type: str = None,
+        domain_name: str = None,
+        owner_id: int = None,
+        sslpri: str = None,
+        sslprotocol: str = None,
+        sslpub: str = None,
+        security_token: str = None,
+    ):
+        self.cert_id = cert_id
+        self.cert_name = cert_name
+        self.cert_region = cert_region
+        self.cert_type = cert_type
+        self.domain_name = domain_name
+        self.owner_id = owner_id
+        self.sslpri = sslpri
+        self.sslprotocol = sslprotocol
+        self.sslpub = sslpub
+        self.security_token = security_token
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
+        if self.cert_id is not None:
+            result['CertId'] = self.cert_id
+        if self.cert_name is not None:
+            result['CertName'] = self.cert_name
+        if self.cert_region is not None:
+            result['CertRegion'] = self.cert_region
+        if self.cert_type is not None:
+            result['CertType'] = self.cert_type
+        if self.domain_name is not None:
+            result['DomainName'] = self.domain_name
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.sslpri is not None:
+            result['SSLPri'] = self.sslpri
+        if self.sslprotocol is not None:
+            result['SSLProtocol'] = self.sslprotocol
+        if self.sslpub is not None:
+            result['SSLPub'] = self.sslpub
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CertId') is not None:
+            self.cert_id = m.get('CertId')
+        if m.get('CertName') is not None:
+            self.cert_name = m.get('CertName')
+        if m.get('CertRegion') is not None:
+            self.cert_region = m.get('CertRegion')
+        if m.get('CertType') is not None:
+            self.cert_type = m.get('CertType')
+        if m.get('DomainName') is not None:
+            self.domain_name = m.get('DomainName')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('SSLPri') is not None:
+            self.sslpri = m.get('SSLPri')
+        if m.get('SSLProtocol') is not None:
+            self.sslprotocol = m.get('SSLProtocol')
+        if m.get('SSLPub') is not None:
+            self.sslpub = m.get('SSLPub')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class SetCdnDomainSSLCertificateResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetCdnDomainSSLCertificateResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SetCdnDomainSSLCertificateResponseBody = None,
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
+            temp_model = SetCdnDomainSSLCertificateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SetCdnDomainStagingConfigRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         functions: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name.
         self.domain_name = domain_name
-        # The features that you want to configure. Format:
-        # 
-        # > - **functionName**: The name of the feature. Separate multiple values with commas (,).
-        # > - **argName**: The feature parameters for **functionName**.
-        # > - **argValue**: The parameter values set for **functionName**.
-        # 
-        # ```
-        #         [
-        #          {
-        #            "functionArgs": [
-        #             {
-        #              "argName": "Parameter A", 
-        #              "argValue": "Parameter value"
-        #             }, 
-        #           {
-        #             "argName": "Parameter B", 
-        #             "argValue": "Parameter value"
-        #              }
-        #          ], 
-        #          "functionName": "Feature name"
-        #             }
-        #         ]
-        #  ```
         self.functions = functions
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -29506,19 +29377,16 @@
 class SetCdnDomainStagingConfigResponseBodyDomainConfigList(TeaModel):
     def __init__(
         self,
         config_id: int = None,
         domain_name: str = None,
         function_name: str = None,
     ):
-        # The ID of the configuration.
         self.config_id = config_id
-        # The accelerated domain name.
         self.domain_name = domain_name
-        # The function name.
         self.function_name = function_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -29547,17 +29415,15 @@
 
 class SetCdnDomainStagingConfigResponseBody(TeaModel):
     def __init__(
         self,
         domain_config_list: List[SetCdnDomainStagingConfigResponseBodyDomainConfigList] = None,
         request_id: str = None,
     ):
-        # The list of the domain configuration.
         self.domain_config_list = domain_config_list
-        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.domain_config_list:
             for k in self.domain_config_list:
                 if k:
                     k.validate()
@@ -29641,40 +29507,38 @@
         force_set: str = None,
         owner_id: int = None,
         private_key: str = None,
         security_token: str = None,
         server_certificate: str = None,
         server_certificate_status: str = None,
     ):
-        # The name of the SSL certificate. You can specify only one name.
+        # Specifies whether to check the certificate name for duplicates. If you set the value to 1, the system does not perform the check and overwrites the information of the existing certificate that uses the same name.
         self.cert_name = cert_name
+        # The ID of the request.
+        self.cert_type = cert_type
+        # The private key. Specify the private key only if you want to enable the SSL certificate.
+        self.domain_name = domain_name
+        # Specifies whether to enable the SSL certificate. Valid values:
+        # 
+        # *   **on**: enables the SSL certificate.
+        # *   **off**: disables the SSL certificate. This is the default value.
+        self.force_set = force_set
+        self.owner_id = owner_id
+        # Specifies whether to check the certificate name for duplicates. If you set the value to 1, the system does not perform the check and overwrites the information of the existing certificate that uses the same name.
+        self.private_key = private_key
+        self.security_token = security_token
         # The type of the SSL certificate. Valid values:
         # 
         # *   **upload**: a user-uploaded SSL certificate.
         # *   **cas**: an SSL certificate that is issued by Alibaba Cloud SSL Certificates Service.
         # *   **free**: a free SSL certificate.
         # 
         # >  If this parameter is set to **cas**, the **PrivateKey** parameter is optional.
-        self.cert_type = cert_type
-        # The accelerated domain name for which you want to configure the SSL certificate. The type of request supported by the domain name must be HTTPS.
-        # 
-        # You can specify one domain name in each call.
-        self.domain_name = domain_name
-        # Specifies whether to check the certificate name for duplicates. If you set the value to 1, the system does not perform the check and overwrites the information of the existing certificate that uses the same name.
-        self.force_set = force_set
-        self.owner_id = owner_id
-        # The private key. Specify the private key only if you want to enable the SSL certificate.
-        self.private_key = private_key
-        self.security_token = security_token
-        # The content of the SSL certificate. Specify the content of the SSL certificate only if you want to enable the SSL certificate.
         self.server_certificate = server_certificate
-        # Specifies whether to enable the SSL certificate. Valid values:
-        # 
-        # *   **on**: enables the SSL certificate.
-        # *   **off**: disables the SSL certificate. This is the default value.
+        # The name of the SSL certificate. You can specify only one name.
         self.server_certificate_status = server_certificate_status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -29805,21 +29669,21 @@
         key: str = None,
         owner_id: int = None,
         security_token: str = None,
         value: str = None,
     ):
         # The ID of the configuration.
         self.config_id = config_id
-        # The accelerated domain names. You can specify one or more domain names and separate them with commas (,).
+        # The accelerated domain name. Separate multiple domain names with commas (,).
         self.domain_name = domain_name
-        # The parameter of the custom header.
+        # The name of the custom header.
         self.key = key
         self.owner_id = owner_id
         self.security_token = security_token
-        # The value of the custom parameter.
+        # The value of the custom header.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -29940,17 +29804,17 @@
         wait_uri: str = None,
         wait_url: str = None,
     ):
         # The percentage of requests that are allowed to be redirected to the origin server. Valid values: **0** to **100**.
         self.allow_pct = allow_pct
         # The accelerated domain name. You can specify only one domain name.
         self.domain_name = domain_name
-        # The length of waiting time to skip after users exit the queue. Unit: seconds.
+        # The length of waiting time to skip after an exit from the queue. Unit: seconds.
         self.gap_time = gap_time
-        # The maximum length of time that users need to wait in the queue. Unit: seconds.
+        # The maximum length of waiting time in the queue. Unit: seconds.
         self.max_time_wait = max_time_wait
         # The regular expression that is used to match URI strings for which the virtual waiting room feature is enabled.
         self.wait_uri = wait_uri
         # The URL of the waiting page.
         self.wait_url = wait_url
 
     def validate(self):
@@ -30068,15 +29932,15 @@
 class StartCdnDomainRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
-        # The domain name that you want to enable. You can specify only one domain name.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
@@ -30180,15 +30044,15 @@
 class StopCdnDomainRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
-        # The accelerated domain name that you want to disable. You can specify only one domain name.
+        # The accelerated domain name that you want to disable. You can specify only one domain name in each request.
         self.domain_name = domain_name
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
@@ -30291,17 +30155,17 @@
 
 class TagResourcesRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # The key of the tag. Valid values of N: **1** to **20**.
+        # The ID of the request.
         self.key = key
-        # The value of the tag. Valid values of N: **1** to **20**.
+        # The operation that you want to perform. Set the value to **TagResources**.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30327,19 +30191,19 @@
 class TagResourcesRequest(TeaModel):
     def __init__(
         self,
         resource_id: List[str] = None,
         resource_type: str = None,
         tag: List[TagResourcesRequestTag] = None,
     ):
-        # The list of resource ID.
+        # The ID of the resource. Valid values of N: **1** to **50**.
         self.resource_id = resource_id
-        # The type of resource. The resource type. Set the value to **DOMAIN**.
+        # >  The maximum number of times that each user can call this operation per second is 100.
         self.resource_type = resource_type
-        # The tags.
+        # The type of resource. The resource type. Set the value to **DOMAIN**.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -30375,15 +30239,15 @@
 
 
 class TagResourcesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
+        # Adds tags to a resource.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30450,26 +30314,26 @@
     def __init__(
         self,
         all: bool = None,
         resource_id: List[str] = None,
         resource_type: str = None,
         tag_key: List[str] = None,
     ):
-        # Specifies whether to delete all tags. Valid values:
+        # Specifies whether to remove all tags. Valid values:
         # 
         # *   **true**: yes.
         # *   **false**: no.
         # 
         # Default value: **false**.
         self.all = all
-        # The list of resource ID. The max items count is up to 20.
+        # The list of resource IDs. You can specify up to 50 resource IDs in the list.
         self.resource_id = resource_id
-        # The type of resource. The resource type. Set the value to **DOMAIN**.
+        # The type of the resources from which you want to remove tags. Set this parameter to **DOMAIN**.
         self.resource_type = resource_type
-        # The list of tag key.
+        # The list of tag keys. You can specify up to 20 tag keys in the list.
         self.tag_key = tag_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30582,17 +30446,15 @@
         reports: str = None,
         schedule: str = None,
     ):
         # The method that is used to send operations reports. Operations reports are sent to you only by email. The settings must be escaped in JSON.
         self.deliver = deliver
         # The ID of the tracking task that you want to update.
         self.deliver_id = deliver_id
-        # The domain name that you want to track. You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
-        # 
-        # If you do not specify a domain name, the task collects data from all domain names that belong to your Alibaba Cloud account.
+        # The domain name that you want to track. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,). If you do not specify a domain name, the task collects data from all domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name
         # The name of the tracking task.
         self.name = name
         # The operations reports that are tracked by the task. The data must be escaped in JSON.
         self.reports = reports
         # The parameters that specify the time interval at which the tracking task sends operations reports. The settings must be escaped in JSON.
         self.schedule = schedule
@@ -30713,23 +30575,21 @@
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         report_ids: str = None,
         start_time: str = None,
     ):
-        # The domain names that you want to track. You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
-        # 
-        # If you do not specify a domain name, the task collects data from all domain names that belong to your Alibaba Cloud account.
+        # The domain name that you want to track. You can specify up to 500 domain names in each request. If you specify multiple domain names, separate them with commas (,). If you do not specify a domain name, operations reports are updated for all domain names in your Alibaba Cloud account.
         self.domain_name = domain_name
-        # The end time of the operations report. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end time of the operations report. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time
         # The IDs of operations reports that you want to update. Separate IDs with commas (,).
         self.report_ids = report_ids
-        # The start time of the operations report. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The start time of the operations report. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30841,15 +30701,15 @@
         source_arn: str = None,
         trigger_arn: str = None,
     ):
         # The feature trigger.
         self.function_arn = function_arn
         # The remarks.
         self.notes = notes
-        # The assigned Resource Access Management (RAM) role.
+        # The assigned RAM role.
         self.role_arn = role_arn
         # The resources and filters for event listening.
         self.source_arn = source_arn
         # The trigger that corresponds to the Function Compute service.
         self.trigger_arn = trigger_arn
 
     def validate(self):
@@ -31004,15 +30864,15 @@
         content: str = None,
         request_id: str = None,
     ):
         # The verification result.
         # 
         # > This parameter is returned only if the operation fails.
         self.content = content
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510.egg-info/PKG-INFO` & `alibabacloud_cdn20180510-1.2.8/alibabacloud_cdn20180510.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cdn20180510
-Version: 1.2.7
+Version: 1.2.8
 Summary: Alibaba Cloud Alibaba Cloud CDN (20180510) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cdn20180510-1.2.7/setup.py` & `alibabacloud_cdn20180510-1.2.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cdn20180510.
 
-Created on 25/04/2023
+Created on 04/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cdn20180510"
 NAME = "alibabacloud_cdn20180510" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Alibaba Cloud CDN (20180510) SDK Library for Python"
```

