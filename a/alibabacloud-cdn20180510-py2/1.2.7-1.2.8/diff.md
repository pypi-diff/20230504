# Comparing `tmp/alibabacloud_cdn20180510_py2-1.2.7.tar.gz` & `tmp/alibabacloud_cdn20180510_py2-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cdn20180510_py2-1.2.7.tar", last modified: Tue Apr 25 07:16:42 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cdn20180510_py2-1.2.8.tar", last modified: Thu May  4 07:55:17 2023, max compression
```

## Comparing `alibabacloud_cdn20180510_py2-1.2.7.tar` & `alibabacloud_cdn20180510_py2-1.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/
--rw-r--r--   0 root         (0) root         (0)     1417 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2486 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510/__init__.py
--rw-r--r--   0 root         (0) root         (0)   354806 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510/client.py
--rw-r--r--   0 root         (0) root         (0)  1077740 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2486 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2917 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/alibabacloud_cdn20180510/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/alibabacloud_cdn20180510/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   333869 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/alibabacloud_cdn20180510/client.py
+-rw-r--r--   0 root         (0) root         (0)  1068203 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/alibabacloud_cdn20180510/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/alibabacloud_cdn20180510_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/alibabacloud_cdn20180510_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/alibabacloud_cdn20180510_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/alibabacloud_cdn20180510_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/alibabacloud_cdn20180510_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/alibabacloud_cdn20180510_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-05-04 07:55:17.000000 alibabacloud_cdn20180510_py2-1.2.8/setup.py
```

### Comparing `alibabacloud_cdn20180510_py2-1.2.7/ChangeLog.md` & `alibabacloud_cdn20180510_py2-1.2.8/ChangeLog.md`

 * *Files 2% similar despite different names*

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

### Comparing `alibabacloud_cdn20180510_py2-1.2.7/LICENSE` & `alibabacloud_cdn20180510_py2-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cdn20180510_py2-1.2.7/PKG-INFO` & `alibabacloud_cdn20180510_py2-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cdn20180510_py2
-Version: 1.2.7
+Version: 1.2.8
 Summary: Alibaba Cloud Alibaba Cloud CDN (20180510) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cdn20180510_py2-1.2.7/README-CN.md` & `alibabacloud_cdn20180510_py2-1.2.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cdn20180510_py2-1.2.7/README.md` & `alibabacloud_cdn20180510_py2-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510/client.py` & `alibabacloud_cdn20180510_py2-1.2.8/alibabacloud_cdn20180510/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,28 +40,14 @@
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def add_cdn_domain_with_options(self, request, runtime):
-        """
-        You must activate Alibaba Cloud CDN before you can add a domain name to it. For more information, see [Activate Alibaba Cloud CDN](~~27272~~).
-        *   If the acceleration region is Chinese Mainland Only or Global, you must apply for an ICP filing for the domain name.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
-        *   For more information, see [Add a domain name](~~122181~~).
-        *   You can call this operation up to 30 times per second per account.
-        
-
-        @param request: AddCdnDomainRequest
-
-        @param runtime: runtime options for this request RuntimeOptions
-
-        @return: AddCdnDomainResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cdn_type):
             query['CdnType'] = request.cdn_type
         if not UtilClient.is_unset(request.check_url):
             query['CheckUrl'] = request.check_url
         if not UtilClient.is_unset(request.domain_name):
@@ -98,26 +84,14 @@
         )
         return TeaCore.from_map(
             cdn_20180510_models.AddCdnDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def add_cdn_domain(self, request):
-        """
-        You must activate Alibaba Cloud CDN before you can add a domain name to it. For more information, see [Activate Alibaba Cloud CDN](~~27272~~).
-        *   If the acceleration region is Chinese Mainland Only or Global, you must apply for an ICP filing for the domain name.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
-        *   For more information, see [Add a domain name](~~122181~~).
-        *   You can call this operation up to 30 times per second per account.
-        
-
-        @param request: AddCdnDomainRequest
-
-        @return: AddCdnDomainResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.add_cdn_domain_with_options(request, runtime)
 
     def add_fctrigger_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.trigger_arn):
@@ -157,19 +131,15 @@
 
     def add_fctrigger(self, request):
         runtime = util_models.RuntimeOptions()
         return self.add_fctrigger_with_options(request, runtime)
 
     def batch_add_cdn_domain_with_options(self, request, runtime):
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
@@ -213,32 +183,28 @@
         return TeaCore.from_map(
             cdn_20180510_models.BatchAddCdnDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def batch_add_cdn_domain(self, request):
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
 
     def batch_delete_cdn_domain_config_with_options(self, request, runtime):
         """
-        > - You can configure features for at most 50 domain names in each API call.
-        - The maximum number of times that each user can call this operation per second is 30.
+        You can specify up to 50 domain names in each request.
+        *   You can call this operation up to 30 times per second per account.
         
 
         @param request: BatchDeleteCdnDomainConfigRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: BatchDeleteCdnDomainConfigResponse
@@ -272,30 +238,82 @@
         return TeaCore.from_map(
             cdn_20180510_models.BatchDeleteCdnDomainConfigResponse(),
             self.call_api(params, req, runtime)
         )
 
     def batch_delete_cdn_domain_config(self, request):
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
 
     def batch_set_cdn_domain_config_with_options(self, request, runtime):
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
@@ -329,30 +347,81 @@
         return TeaCore.from_map(
             cdn_20180510_models.BatchSetCdnDomainConfigResponse(),
             self.call_api(params, req, runtime)
         )
 
     def batch_set_cdn_domain_config(self, request):
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
 
     def batch_set_cdn_domain_server_certificate_with_options(self, request, runtime):
         """
-        >    The maximum number of times that each user can call this operation per second is 10.
-        *   You can specify multiple domain names (no more than 50) and separate them with commas (,).
+        The content of the SSL certificate. Specify the content of the certificate only if you want to enable the SSL certificate.
         
 
         @param request: BatchSetCdnDomainServerCertificateRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: BatchSetCdnDomainServerCertificateResponse
@@ -396,30 +465,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.BatchSetCdnDomainServerCertificateResponse(),
             self.call_api(params, req, runtime)
         )
 
     def batch_set_cdn_domain_server_certificate(self, request):
         """
-        >    The maximum number of times that each user can call this operation per second is 10.
-        *   You can specify multiple domain names (no more than 50) and separate them with commas (,).
+        The content of the SSL certificate. Specify the content of the certificate only if you want to enable the SSL certificate.
         
 
         @param request: BatchSetCdnDomainServerCertificateRequest
 
         @return: BatchSetCdnDomainServerCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_set_cdn_domain_server_certificate_with_options(request, runtime)
 
     def batch_start_cdn_domain_with_options(self, request, runtime):
         """
-        - If the domain name is in an invalid state or your have an overdue payment in your account, the domain name cannot be enabled.
-        - The maximum number of times that each user can call this operation per second is 30.
-        - The maximum number of domain names configured at a time is 50.
+        The domain names that you want to enable. Separate multiple domain names with commas (,).
         
 
         @param request: BatchStartCdnDomainRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: BatchStartCdnDomainResponse
@@ -449,17 +515,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.BatchStartCdnDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def batch_start_cdn_domain(self, request):
         """
-        - If the domain name is in an invalid state or your have an overdue payment in your account, the domain name cannot be enabled.
-        - The maximum number of times that each user can call this operation per second is 30.
-        - The maximum number of domain names configured at a time is 50.
+        The domain names that you want to enable. Separate multiple domain names with commas (,).
         
 
         @param request: BatchStartCdnDomainRequest
 
         @return: BatchStartCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -637,15 +701,15 @@
         @return: CreateCdnCertificateSigningRequestResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_cdn_certificate_signing_request_with_options(request, runtime)
 
     def create_cdn_deliver_task_with_options(self, request, runtime):
         """
-        > You can call this operation up to three times per second per account.
+        The ID of the tracking task.
         
 
         @param request: CreateCdnDeliverTaskRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateCdnDeliverTaskResponse
@@ -679,15 +743,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.CreateCdnDeliverTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_cdn_deliver_task(self, request):
         """
-        > You can call this operation up to three times per second per account.
+        The ID of the tracking task.
         
 
         @param request: CreateCdnDeliverTaskRequest
 
         @return: CreateCdnDeliverTaskResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -741,17 +805,17 @@
         @return: CreateCdnSubTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_cdn_sub_task_with_options(request, runtime)
 
     def create_illegal_url_export_task_with_options(self, request, runtime):
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
@@ -779,29 +843,29 @@
         return TeaCore.from_map(
             cdn_20180510_models.CreateIllegalUrlExportTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_illegal_url_export_task(self, request):
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
 
     def create_real_time_log_delivery_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        >  You can call this API operation up to 100 times per second per account.
         
 
         @param request: CreateRealTimeLogDeliveryRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateRealTimeLogDeliveryResponse
@@ -825,15 +889,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.CreateRealTimeLogDeliveryResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_real_time_log_delivery(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        >  You can call this API operation up to 100 times per second per account.
         
 
         @param request: CreateRealTimeLogDeliveryRequest
 
         @return: CreateRealTimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -997,17 +1061,15 @@
         @return: DeleteCdnDeliverTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_cdn_deliver_task_with_options(request, runtime)
 
     def delete_cdn_domain_with_options(self, request, runtime):
         """
-        - We recommend that you add an A record for the domain name in the system of your DNS service provider before you delete the domain name from Alibaba Cloud CDN. Otherwise, the domain name may become inaccessible. Proceed with caution.
-        - After you successfully call the DeleteCdnDomain operation, all records of the deleted domain name are removed. If you need to only disable the domain name, we recommend that you call the StopCdnDomain operation.
-        - The maximum number of times that each user can call this operation per second is 10.
+        The accelerated domain name that you want to delete. You can specify only one domain name in each call.
         
 
         @param request: DeleteCdnDomainRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DeleteCdnDomainResponse
@@ -1037,17 +1099,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DeleteCdnDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_cdn_domain(self, request):
         """
-        - We recommend that you add an A record for the domain name in the system of your DNS service provider before you delete the domain name from Alibaba Cloud CDN. Otherwise, the domain name may become inaccessible. Proceed with caution.
-        - After you successfully call the DeleteCdnDomain operation, all records of the deleted domain name are removed. If you need to only disable the domain name, we recommend that you call the StopCdnDomain operation.
-        - The maximum number of times that each user can call this operation per second is 10.
+        The accelerated domain name that you want to delete. You can specify only one domain name in each call.
         
 
         @param request: DeleteCdnDomainRequest
 
         @return: DeleteCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -1161,15 +1221,15 @@
         @return: DeleteRealTimeLogLogstoreResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_real_time_log_logstore_with_options(request, runtime)
 
     def delete_realtime_log_delivery_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DeleteRealtimeLogDeliveryRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DeleteRealtimeLogDeliveryResponse
@@ -1193,27 +1253,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DeleteRealtimeLogDeliveryResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_realtime_log_delivery(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DeleteRealtimeLogDeliveryRequest
 
         @return: DeleteRealtimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_realtime_log_delivery_with_options(request, runtime)
 
     def delete_specific_config_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DeleteSpecificConfigRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DeleteSpecificConfigResponse
@@ -1245,15 +1305,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DeleteSpecificConfigResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_specific_config(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DeleteSpecificConfigRequest
 
         @return: DeleteSpecificConfigResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -1401,15 +1461,15 @@
         @return: DeleteUserUsageDataExportTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_user_usage_data_export_task_with_options(request, runtime)
 
     def describe_blocked_regions_with_options(self, request, runtime):
         """
-        >  You can call this operation up to 50 times per second.
+        > You can call this operation up to 50 times per second per account.
         
 
         @param request: DescribeBlockedRegionsRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeBlockedRegionsResponse
@@ -1433,27 +1493,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeBlockedRegionsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_blocked_regions(self, request):
         """
-        >  You can call this operation up to 50 times per second.
+        > You can call this operation up to 50 times per second per account.
         
 
         @param request: DescribeBlockedRegionsRequest
 
         @return: DescribeBlockedRegionsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_blocked_regions_with_options(request, runtime)
 
     def describe_cdn_certificate_detail_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
 
         @param request: DescribeCdnCertificateDetailRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnCertificateDetailResponse
@@ -1483,27 +1543,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnCertificateDetailResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_certificate_detail(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 20.
+        > You can call this operation up to 20 times per second per account.
         
 
         @param request: DescribeCdnCertificateDetailRequest
 
         @return: DescribeCdnCertificateDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_certificate_detail_with_options(request, runtime)
 
     def describe_cdn_certificate_list_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeCdnCertificateListRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnCertificateListResponse
@@ -1533,27 +1593,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnCertificateListResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_certificate_list(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeCdnCertificateListRequest
 
         @return: DescribeCdnCertificateListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_certificate_list_with_options(request, runtime)
 
     def describe_cdn_deleted_domains_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 10.
+        > You can call this operation up to 10 times per second per account.
         
 
         @param request: DescribeCdnDeletedDomainsRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnDeletedDomainsResponse
@@ -1581,15 +1641,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnDeletedDomainsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_deleted_domains(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 10.
+        > You can call this operation up to 10 times per second per account.
         
 
         @param request: DescribeCdnDeletedDomainsRequest
 
         @return: DescribeCdnDeletedDomainsResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -1687,15 +1747,15 @@
         @return: DescribeCdnDomainByCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_domain_by_certificate_with_options(request, runtime)
 
     def describe_cdn_domain_configs_with_options(self, request, runtime):
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeCdnDomainConfigsRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnDomainConfigsResponse
@@ -1729,27 +1789,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnDomainConfigsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_domain_configs(self, request):
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeCdnDomainConfigsRequest
 
         @return: DescribeCdnDomainConfigsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_domain_configs_with_options(request, runtime)
 
     def describe_cdn_domain_detail_with_options(self, request, runtime):
         """
-        The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeCdnDomainDetailRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnDomainDetailResponse
@@ -1779,15 +1839,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnDomainDetailResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_domain_detail(self, request):
         """
-        The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeCdnDomainDetailRequest
 
         @return: DescribeCdnDomainDetailResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -1851,15 +1911,15 @@
         @return: DescribeCdnDomainLogsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_domain_logs_with_options(request, runtime)
 
     def describe_cdn_domain_staging_config_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeCdnDomainStagingConfigRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnDomainStagingConfigResponse
@@ -1887,15 +1947,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnDomainStagingConfigResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_domain_staging_config(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeCdnDomainStagingConfigRequest
 
         @return: DescribeCdnDomainStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -1981,16 +2041,16 @@
 
     def describe_cdn_order_commodity_code(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_order_commodity_code_with_options(request, runtime)
 
     def describe_cdn_region_and_isp_with_options(self, request, runtime):
         """
-        >    The lists of ISPs and regions that are supported by Alibaba Cloud CDN are updated and published on the Alibaba Cloud International site.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        The lists of ISPs and regions that are supported by Alibaba Cloud CDN are updated and published on the Alibaba Cloud International site.
+        *   You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeCdnRegionAndIspRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnRegionAndIspResponse
@@ -2018,16 +2078,16 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnRegionAndIspResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_region_and_isp(self, request):
         """
-        >    The lists of ISPs and regions that are supported by Alibaba Cloud CDN are updated and published on the Alibaba Cloud International site.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        The lists of ISPs and regions that are supported by Alibaba Cloud CDN are updated and published on the Alibaba Cloud International site.
+        *   You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeCdnRegionAndIspRequest
 
         @return: DescribeCdnRegionAndIspResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -2089,16 +2149,16 @@
         @return: DescribeCdnReportResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_report_with_options(request, runtime)
 
     def describe_cdn_report_list_with_options(self, request, runtime):
         """
-        > - This operation queries the metadata of all operations reports. The statistics in the reports are not returned.
-        - You can call this API operation up to three times per second per account.
+        This operation queries the metadata of all operations reports. The statistics in the reports are not returned.
+        *   You can call this operation up to three times per second per account.
         
 
         @param request: DescribeCdnReportListRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnReportListResponse
@@ -2124,16 +2184,16 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnReportListResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_report_list(self, request):
         """
-        > - This operation queries the metadata of all operations reports. The statistics in the reports are not returned.
-        - You can call this API operation up to three times per second per account.
+        This operation queries the metadata of all operations reports. The statistics in the reports are not returned.
+        *   You can call this operation up to three times per second per account.
         
 
         @param request: DescribeCdnReportListRequest
 
         @return: DescribeCdnReportListResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -2187,15 +2247,15 @@
         @return: DescribeCdnSMCertificateDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_smcertificate_detail_with_options(request, runtime)
 
     def describe_cdn_smcertificate_list_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeCdnSMCertificateListRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnSMCertificateListResponse
@@ -2225,27 +2285,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnSMCertificateListResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_smcertificate_list(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeCdnSMCertificateListRequest
 
         @return: DescribeCdnSMCertificateListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_smcertificate_list_with_options(request, runtime)
 
     def describe_cdn_service_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeCdnServiceRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnServiceResponse
@@ -2273,28 +2333,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnServiceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_service(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeCdnServiceRequest
 
         @return: DescribeCdnServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_service_with_options(request, runtime)
 
     def describe_cdn_sub_list_with_options(self, runtime):
         """
-        By default, this operation queries all custom operations reports. However, only one operations report can be displayed. Therefore, only one operations report is returned.
-        *   You can call this operation up to three times per second per account.
+        {"RequestId":"3250A51D-C11D-46BA-B6B3-95348EEDE652","Description":"Successful","Content":{"data":\\[{"subId":5,"reportId":\\[1,2,3],"createTime":"2020-09-25T09:39:33Z","domains"\\["www.example.com","www.example.com"],"effectiveFrom":"2020-09-17T00:00:00Z","effectiveEnd":"2020-11-17T00:00:00Z","status":"enable"}]}}
         
 
         @param request: DescribeCdnSubListRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnSubListResponse
@@ -2314,16 +2373,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnSubListResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_sub_list(self):
         """
-        By default, this operation queries all custom operations reports. However, only one operations report can be displayed. Therefore, only one operations report is returned.
-        *   You can call this operation up to three times per second per account.
+        {"RequestId":"3250A51D-C11D-46BA-B6B3-95348EEDE652","Description":"Successful","Content":{"data":\\[{"subId":5,"reportId":\\[1,2,3],"createTime":"2020-09-25T09:39:33Z","domains"\\["www.example.com","www.example.com"],"effectiveFrom":"2020-09-17T00:00:00Z","effectiveEnd":"2020-11-17T00:00:00Z","status":"enable"}]}}
         
 
         @return: DescribeCdnSubListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_sub_list_with_options(runtime)
 
@@ -2375,21 +2433,21 @@
         @return: DescribeCdnUserBillHistoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_user_bill_history_with_options(request, runtime)
 
     def describe_cdn_user_bill_prediction_with_options(self, request, runtime):
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
@@ -2421,21 +2479,21 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnUserBillPredictionResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_user_bill_prediction(self, request):
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
@@ -2487,15 +2545,22 @@
         @return: DescribeCdnUserBillTypeResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_user_bill_type_with_options(request, runtime)
 
     def describe_cdn_user_configs_with_options(self, request, runtime):
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
@@ -2521,35 +2586,32 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnUserConfigsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_user_configs(self, request):
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
 
     def describe_cdn_user_domains_by_func_with_options(self, request, runtime):
-        """
-        > You can call this operation up to 100 times per second per account.
-        
-
-        @param request: DescribeCdnUserDomainsByFuncRequest
-
-        @param runtime: runtime options for this request RuntimeOptions
-
-        @return: DescribeCdnUserDomainsByFuncResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.func_id):
             query['FuncId'] = request.func_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -2572,28 +2634,20 @@
         )
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnUserDomainsByFuncResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_user_domains_by_func(self, request):
-        """
-        > You can call this operation up to 100 times per second per account.
-        
-
-        @param request: DescribeCdnUserDomainsByFuncRequest
-
-        @return: DescribeCdnUserDomainsByFuncResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_user_domains_by_func_with_options(request, runtime)
 
     def describe_cdn_user_quota_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeCdnUserQuotaRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnUserQuotaResponse
@@ -2621,15 +2675,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnUserQuotaResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_user_quota(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeCdnUserQuotaRequest
 
         @return: DescribeCdnUserQuotaResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -2682,14 +2736,24 @@
 
         @return: DescribeCdnUserResourcePackageResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_user_resource_package_with_options(request, runtime)
 
     def describe_cdn_waf_domain_with_options(self, request, runtime):
+        """
+        > You can call this operation up to 150 times per second per account.
+        
+
+        @param request: DescribeCdnWafDomainRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeCdnWafDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -2710,14 +2774,22 @@
         )
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnWafDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_waf_domain(self, request):
+        """
+        > You can call this operation up to 150 times per second per account.
+        
+
+        @param request: DescribeCdnWafDomainRequest
+
+        @return: DescribeCdnWafDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_waf_domain_with_options(request, runtime)
 
     def describe_certificate_info_by_idwith_options(self, request, runtime):
         """
         You can call this operation up to 100 times per second per account.
         *   If a certificate is associated with a domain name but the certificate is not enabled, the result of this operation shows that the certificate does not exist.
@@ -2805,18 +2877,15 @@
         @return: DescribeCustomLogConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_custom_log_config_with_options(request, runtime)
 
     def describe_domain_average_response_time_with_options(self, request, runtime):
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - You can call this operation up to 100 times per second per account.
-        - You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
+        The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         
 
         @param request: DescribeDomainAverageResponseTimeRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDomainAverageResponseTimeResponse
@@ -2856,38 +2925,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainAverageResponseTimeResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_average_response_time(self, request):
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
 
     def describe_domain_bps_data_with_options(self, request, runtime):
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
@@ -2923,23 +2981,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainBpsDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_bps_data(self, request):
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
@@ -3075,18 +3125,18 @@
         @return: DescribeDomainBpsDataByTimeStampResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_bps_data_by_time_stamp_with_options(request, runtime)
 
     def describe_domain_cc_activity_log_with_options(self, request, runtime):
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
@@ -3126,30 +3176,30 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainCcActivityLogResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_cc_activity_log(self, request):
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
 
     def describe_domain_certificate_info_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
 
         @param request: DescribeDomainCertificateInfoRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDomainCertificateInfoResponse
@@ -3175,15 +3225,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainCertificateInfoResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_certificate_info(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
 
         @param request: DescribeDomainCertificateInfoRequest
 
         @return: DescribeDomainCertificateInfoResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -3259,23 +3309,15 @@
         @return: DescribeDomainCustomLogConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_custom_log_config_with_options(request, runtime)
 
     def describe_domain_detail_data_by_layer_with_options(self, request, runtime):
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
@@ -3299,43 +3341,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainDetailDataByLayerResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_detail_data_by_layer(self, request):
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
 
     def describe_domain_hit_rate_data_with_options(self, request, runtime):
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
@@ -3367,43 +3393,35 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainHitRateDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_hit_rate_data(self, request):
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
 
     def describe_domain_http_code_data_with_options(self, request, runtime):
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
@@ -3439,23 +3457,23 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainHttpCodeDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_http_code_data(self, request):
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
@@ -3533,18 +3551,15 @@
         @return: DescribeDomainHttpCodeDataByLayerResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_http_code_data_by_layer_with_options(request, runtime)
 
     def describe_domain_ispdata_with_options(self, request, runtime):
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - This operation queries proportions of data usage of different ISPs only for a specific accelerated domain name, or for all accelerated domain names that belong your Alibaba Cloud account.
-        - You can call this operation up to 100 times per second per account.
+        The end of the time range that was queried.
         
 
         @param request: DescribeDomainISPDataRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDomainISPDataResponse
@@ -3574,18 +3589,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainISPDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_ispdata(self, request):
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
@@ -3651,19 +3663,15 @@
         @return: DescribeDomainMax95BpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_max_95bps_data_with_options(request, runtime)
 
     def describe_domain_multi_usage_data_with_options(self, request, runtime):
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
@@ -3693,19 +3701,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainMultiUsageDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_multi_usage_data(self, request):
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
@@ -3765,17 +3769,15 @@
         @return: DescribeDomainPathDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_path_data_with_options(request, runtime)
 
     def describe_domain_pv_data_with_options(self, request, runtime):
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, monitoring data within the last 24 hours is queried. If you set both StartTime and EndTime, monitoring data within the specified time range is queried.
-        - You can call this operation up to 50 times per second per account.
+        The end of the time range during which data was queried.
         
 
         @param request: DescribeDomainPvDataRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDomainPvDataResponse
@@ -3805,17 +3807,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainPvDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_pv_data(self, request):
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, monitoring data within the last 24 hours is queried. If you set both StartTime and EndTime, monitoring data within the specified time range is queried.
-        - You can call this operation up to 50 times per second per account.
+        The end of the time range during which data was queried.
         
 
         @param request: DescribeDomainPvDataRequest
 
         @return: DescribeDomainPvDataResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -4085,16 +4085,16 @@
         @return: DescribeDomainRealTimeByteHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_byte_hit_rate_data_with_options(request, runtime)
 
     def describe_domain_real_time_detail_data_with_options(self, request, runtime):
         """
-        - You can query data within the last seven days. Data is collected every minute.
-        - The maximum number of times that each user can call this operation per second is 10.
+        The beginning of the time range to query.
+        Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. Example: 2019-11-30T05:33:00Z.
         
 
         @param request: DescribeDomainRealTimeDetailDataRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDomainRealTimeDetailDataResponse
@@ -4118,36 +4118,28 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainRealTimeDetailDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_real_time_detail_data(self, request):
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
 
     def describe_domain_real_time_http_code_data_with_options(self, request, runtime):
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
@@ -4181,23 +4173,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_real_time_http_code_data(self, request):
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
@@ -4261,25 +4245,15 @@
         @return: DescribeDomainRealTimeQpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_qps_data_with_options(request, runtime)
 
     def describe_domain_real_time_req_hit_rate_data_with_options(self, request, runtime):
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
@@ -4303,45 +4277,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainRealTimeReqHitRateDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_real_time_req_hit_rate_data(self, request):
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
 
     def describe_domain_real_time_src_bps_data_with_options(self, request, runtime):
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
@@ -4371,43 +4327,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_real_time_src_bps_data(self, request):
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
 
     def describe_domain_real_time_src_http_code_data_with_options(self, request, runtime):
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
@@ -4441,23 +4381,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_real_time_src_http_code_data(self, request):
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
@@ -4597,15 +4529,15 @@
         @return: DescribeDomainRealTimeTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_traffic_data_with_options(request, runtime)
 
     def describe_domain_realtime_log_delivery_with_options(self, request, runtime):
         """
-        > You can call this operation up to 100 times per second per account.
+        The name of the Log Service project that is used for real-time log delivery.
         
 
         @param request: DescribeDomainRealtimeLogDeliveryRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDomainRealtimeLogDeliveryResponse
@@ -4629,30 +4561,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainRealtimeLogDeliveryResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_realtime_log_delivery(self, request):
         """
-        > You can call this operation up to 100 times per second per account.
+        The name of the Log Service project that is used for real-time log delivery.
         
 
         @param request: DescribeDomainRealtimeLogDeliveryRequest
 
         @return: DescribeDomainRealtimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_realtime_log_delivery_with_options(request, runtime)
 
     def describe_domain_region_data_with_options(self, request, runtime):
         """
-        The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set **StartTime** or **EndTime**, data collected within the last **24** hours is queried. If you set both **StartTime** and **EndTime**, data collected within the specified time range is queried.
-        - You may fail to query the latest data. If you need to query data collected within the last day, we recommend that you query the data on the next day.
-        - You can call this operation up to 100 times per second per account.
+        The beginning of the time range that was queried.
         
 
         @param request: DescribeDomainRegionDataRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDomainRegionDataResponse
@@ -4682,18 +4611,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainRegionDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_region_data(self, request):
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
@@ -5093,18 +5019,16 @@
         @return: DescribeDomainSrcTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_src_traffic_data_with_options(request, runtime)
 
     def describe_domain_top_client_ip_visit_with_options(self, request, runtime):
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
@@ -5140,33 +5064,30 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainTopClientIpVisitResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_top_client_ip_visit(self, request):
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
 
     def describe_domain_top_refer_visit_with_options(self, request, runtime):
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
@@ -5198,18 +5119,17 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainTopReferVisitResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_top_refer_visit(self, request):
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
@@ -5348,15 +5268,15 @@
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_traffic_data_with_options(request, runtime)
 
     def describe_domain_usage_data_with_options(self, request, runtime):
         """
         You can call this operation up to 10 times per second per account.
-        * The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        * The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
         |Time granularity|Maximum time range per query|Historical data available|Data delay|
         |---|---|---|---|
         |5 minutes|3 days|93 days|15 minutes|
         |1 hour|31 days|186 days|4 hours|
         |1 day|90 days|366 days|04:00 on the next day|
         
 
@@ -5402,15 +5322,15 @@
             cdn_20180510_models.DescribeDomainUsageDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_usage_data(self, request):
         """
         You can call this operation up to 10 times per second per account.
-        * The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        * The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
         |Time granularity|Maximum time range per query|Historical data available|Data delay|
         |---|---|---|---|
         |5 minutes|3 days|93 days|15 minutes|
         |1 hour|31 days|186 days|4 hours|
         |1 day|90 days|366 days|04:00 on the next day|
         
 
@@ -5477,15 +5397,15 @@
         @return: DescribeDomainUvDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_uv_data_with_options(request, runtime)
 
     def describe_domains_by_source_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeDomainsBySourceRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDomainsBySourceResponse
@@ -5515,15 +5435,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainsBySourceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domains_by_source(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeDomainsBySourceRequest
 
         @return: DescribeDomainsBySourceResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -5581,15 +5501,15 @@
         @return: DescribeDomainsUsageByDayResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domains_usage_by_day_with_options(request, runtime)
 
     def describe_es_exception_data_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeEsExceptionDataRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeEsExceptionDataResponse
@@ -5619,27 +5539,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeEsExceptionDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_es_exception_data(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeEsExceptionDataRequest
 
         @return: DescribeEsExceptionDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_es_exception_data_with_options(request, runtime)
 
     def describe_es_execute_data_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeEsExecuteDataRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeEsExecuteDataResponse
@@ -5669,15 +5589,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeEsExecuteDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_es_execute_data(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeEsExecuteDataRequest
 
         @return: DescribeEsExecuteDataResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -5707,16 +5627,15 @@
 
     def describe_fctrigger(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_fctrigger_with_options(request, runtime)
 
     def describe_illegal_url_export_task_with_options(self, request, runtime):
         """
-        >    Invalid URLs are exported to a CSV file.
-        *   The maximum number of times that each user can call this operation per second is 1.
+        The URL where you can download the file that contains invalid URLs. This parameter is valid only if the export task is successful.
         
 
         @param request: DescribeIllegalUrlExportTaskRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeIllegalUrlExportTaskResponse
@@ -5742,28 +5661,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeIllegalUrlExportTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_illegal_url_export_task(self, request):
         """
-        >    Invalid URLs are exported to a CSV file.
-        *   The maximum number of times that each user can call this operation per second is 1.
+        The URL where you can download the file that contains invalid URLs. This parameter is valid only if the export task is successful.
         
 
         @param request: DescribeIllegalUrlExportTaskRequest
 
         @return: DescribeIllegalUrlExportTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_illegal_url_export_task_with_options(request, runtime)
 
     def describe_ip_info_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
 
         @param request: DescribeIpInfoRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeIpInfoResponse
@@ -5789,27 +5707,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeIpInfoResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_ip_info(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
 
         @param request: DescribeIpInfoRequest
 
         @return: DescribeIpInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_ip_info_with_options(request, runtime)
 
     def describe_ip_status_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
 
         @param request: DescribeIpStatusRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeIpStatusResponse
@@ -5833,15 +5751,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeIpStatusResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_ip_status(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 50.
+        > You can call this operation up to 50 times per second per account.
         
 
         @param request: DescribeIpStatusRequest
 
         @return: DescribeIpStatusResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -5981,15 +5899,15 @@
         @return: DescribeRangeDataByLocateAndIspServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_range_data_by_locate_and_isp_service_with_options(request, runtime)
 
     def describe_realtime_delivery_acc_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeRealtimeDeliveryAccRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeRealtimeDeliveryAccResponse
@@ -6023,28 +5941,28 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeRealtimeDeliveryAccResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_realtime_delivery_acc(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeRealtimeDeliveryAccRequest
 
         @return: DescribeRealtimeDeliveryAccResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_realtime_delivery_acc_with_options(request, runtime)
 
     def describe_refresh_quota_with_options(self, request, runtime):
         """
-        > - You can call the RefreshObjectCaches operation to refresh content and call the PushObjectCache operation to prefetch content.
-        - The maximum number of times that each user can call this operation per second is 20.
+        You can call the [RefreshObjectCaches](~~448057~~) operation to refresh content and call the [PushObjectCache](~~448058~~) operation to prefetch content.
+        *   You can call this operation up to 20 times per second per account.
         
 
         @param request: DescribeRefreshQuotaRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeRefreshQuotaResponse
@@ -6072,29 +5990,28 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeRefreshQuotaResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_refresh_quota(self, request):
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
 
     def describe_refresh_task_by_id_with_options(self, request, runtime):
         """
-        > - You can query data within the last three days.
-        - You can call this operation up to 30 times per second per account.
+        The tasks.
         
 
         @param request: DescribeRefreshTaskByIdRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeRefreshTaskByIdResponse
@@ -6120,32 +6037,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeRefreshTaskByIdResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_refresh_task_by_id(self, request):
         """
-        > - You can query data within the last three days.
-        - You can call this operation up to 30 times per second per account.
+        The tasks.
         
 
         @param request: DescribeRefreshTaskByIdRequest
 
         @return: DescribeRefreshTaskByIdResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_refresh_task_by_id_with_options(request, runtime)
 
     def describe_refresh_tasks_with_options(self, request, runtime):
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
@@ -6193,19 +6105,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeRefreshTasksResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_refresh_tasks(self, request):
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
@@ -6246,24 +6154,14 @@
 
         @return: DescribeStagingIpResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_staging_ip_with_options(runtime)
 
     def describe_tag_resources_with_options(self, request, runtime):
-        """
-        > You can call this operation up to 10 times per second per account.
-        
-
-        @param request: DescribeTagResourcesRequest
-
-        @param runtime: runtime options for this request RuntimeOptions
-
-        @return: DescribeTagResourcesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.tag):
@@ -6284,30 +6182,23 @@
         )
         return TeaCore.from_map(
             cdn_20180510_models.DescribeTagResourcesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_tag_resources(self, request):
-        """
-        > You can call this operation up to 10 times per second per account.
-        
-
-        @param request: DescribeTagResourcesRequest
-
-        @return: DescribeTagResourcesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_tag_resources_with_options(request, runtime)
 
     def describe_top_domains_by_flow_with_options(self, request, runtime):
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
@@ -6337,29 +6228,30 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeTopDomainsByFlowResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_top_domains_by_flow(self, request):
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
 
     def describe_user_certificate_expire_count_with_options(self, runtime):
         """
-        > You can call this operation up to 100 times per second per account.
+        The number of domain names whose SSL certificates are about to expire within 30 days.
         
 
         @param request: DescribeUserCertificateExpireCountRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeUserCertificateExpireCountResponse
@@ -6379,15 +6271,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeUserCertificateExpireCountResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_user_certificate_expire_count(self):
         """
-        > You can call this operation up to 100 times per second per account.
+        The number of domain names whose SSL certificates are about to expire within 30 days.
         
 
         @return: DescribeUserCertificateExpireCountResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_certificate_expire_count_with_options(runtime)
 
@@ -6442,15 +6334,15 @@
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_configs_with_options(request, runtime)
 
     def describe_user_domains_with_options(self, request, runtime):
         """
         You can call this operation up to 100 times per second per account.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
+        *   You can specify up to 50 domain names in each request. Separate multiple domain names with commas (,).
         
 
         @param request: DescribeUserDomainsRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeUserDomainsResponse
@@ -6505,15 +6397,15 @@
             cdn_20180510_models.DescribeUserDomainsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_user_domains(self, request):
         """
         You can call this operation up to 100 times per second per account.
-        *   You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
+        *   You can specify up to 50 domain names in each request. Separate multiple domain names with commas (,).
         
 
         @param request: DescribeUserDomainsRequest
 
         @return: DescribeUserDomainsResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -6653,15 +6545,15 @@
         @return: DescribeUserUsageDetailDataExportTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_usage_detail_data_export_task_with_options(request, runtime)
 
     def describe_user_vips_by_domain_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        The ID of the request.
         
 
         @param request: DescribeUserVipsByDomainRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeUserVipsByDomainResponse
@@ -6685,35 +6577,25 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeUserVipsByDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_user_vips_by_domain(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        The ID of the request.
         
 
         @param request: DescribeUserVipsByDomainRequest
 
         @return: DescribeUserVipsByDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_vips_by_domain_with_options(request, runtime)
 
     def describe_verify_content_with_options(self, request, runtime):
-        """
-        > You can call this operation up to 100 times per second per account.
-        
-
-        @param request: DescribeVerifyContentRequest
-
-        @param runtime: runtime options for this request RuntimeOptions
-
-        @return: DescribeVerifyContentResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -6730,22 +6612,14 @@
         )
         return TeaCore.from_map(
             cdn_20180510_models.DescribeVerifyContentResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_verify_content(self, request):
-        """
-        > You can call this operation up to 100 times per second per account.
-        
-
-        @param request: DescribeVerifyContentRequest
-
-        @return: DescribeVerifyContentResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_verify_content_with_options(request, runtime)
 
     def disable_realtime_log_delivery_with_options(self, request, runtime):
         """
         >  The maximum number of times that each user can call this operation per second is 100.
         
@@ -6831,15 +6705,15 @@
         @return: EnableRealtimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.enable_realtime_log_delivery_with_options(request, runtime)
 
     def list_domains_by_log_config_id_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: ListDomainsByLogConfigIdRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: ListDomainsByLogConfigIdResponse
@@ -6863,27 +6737,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.ListDomainsByLogConfigIdResponse(),
             self.call_api(params, req, runtime)
         )
 
     def list_domains_by_log_config_id(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: ListDomainsByLogConfigIdRequest
 
         @return: ListDomainsByLogConfigIdResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_domains_by_log_config_id_with_options(request, runtime)
 
     def list_fctrigger_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: ListFCTriggerRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: ListFCTriggerResponse
@@ -6907,27 +6781,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.ListFCTriggerResponse(),
             self.call_api(params, req, runtime)
         )
 
     def list_fctrigger(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: ListFCTriggerRequest
 
         @return: ListFCTriggerResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_fctrigger_with_options(request, runtime)
 
     def list_realtime_log_delivery_domains_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: ListRealtimeLogDeliveryDomainsRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: ListRealtimeLogDeliveryDomainsResponse
@@ -6951,27 +6825,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.ListRealtimeLogDeliveryDomainsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def list_realtime_log_delivery_domains(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: ListRealtimeLogDeliveryDomainsRequest
 
         @return: ListRealtimeLogDeliveryDomainsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_realtime_log_delivery_domains_with_options(request, runtime)
 
     def list_realtime_log_delivery_infos_with_options(self, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: ListRealtimeLogDeliveryInfosRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: ListRealtimeLogDeliveryInfosResponse
@@ -6991,15 +6865,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.ListRealtimeLogDeliveryInfosResponse(),
             self.call_api(params, req, runtime)
         )
 
     def list_realtime_log_delivery_infos(self):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @return: ListRealtimeLogDeliveryInfosResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_realtime_log_delivery_infos_with_options(runtime)
 
@@ -7039,15 +6913,15 @@
         @return: ListUserCustomLogConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_user_custom_log_config_with_options(runtime)
 
     def modify_cdn_domain_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: ModifyCdnDomainRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: ModifyCdnDomainResponse
@@ -7083,27 +6957,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.ModifyCdnDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_cdn_domain(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: ModifyCdnDomainRequest
 
         @return: ModifyCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_cdn_domain_with_options(request, runtime)
 
     def modify_cdn_domain_schdm_by_property_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
 
         @param request: ModifyCdnDomainSchdmByPropertyRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: ModifyCdnDomainSchdmByPropertyResponse
@@ -7131,15 +7005,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.ModifyCdnDomainSchdmByPropertyResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_cdn_domain_schdm_by_property(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
 
         @param request: ModifyCdnDomainSchdmByPropertyRequest
 
         @return: ModifyCdnDomainSchdmByPropertyResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -7187,16 +7061,16 @@
         @return: ModifyRealtimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_realtime_log_delivery_with_options(request, runtime)
 
     def open_cdn_service_with_options(self, request, runtime):
         """
-        > - Alibaba Cloud CDN can be activated only once per Alibaba Cloud account. The Alibaba Cloud account must pass real-name verification.
-        > - The maximum number of times that each user can call this operation per second is 5.
+        Alibaba Cloud CDN can be activated only once per Alibaba Cloud account. The Alibaba Cloud account must complete real-name verification to activate Alibaba Cloud CDN.
+        *   You can call this operation up to five times per second per user.
         
 
         @param request: OpenCdnServiceRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: OpenCdnServiceResponse
@@ -7226,16 +7100,16 @@
         return TeaCore.from_map(
             cdn_20180510_models.OpenCdnServiceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def open_cdn_service(self, request):
         """
-        > - Alibaba Cloud CDN can be activated only once per Alibaba Cloud account. The Alibaba Cloud account must pass real-name verification.
-        > - The maximum number of times that each user can call this operation per second is 5.
+        Alibaba Cloud CDN can be activated only once per Alibaba Cloud account. The Alibaba Cloud account must complete real-name verification to activate Alibaba Cloud CDN.
+        *   You can call this operation up to five times per second per user.
         
 
         @param request: OpenCdnServiceRequest
 
         @return: OpenCdnServiceResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -7365,17 +7239,17 @@
 
     def refresh_object_caches_with_options(self, request, runtime):
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
         
@@ -7417,17 +7291,17 @@
 
     def refresh_object_caches(self, request):
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
         
@@ -7437,15 +7311,15 @@
         @return: RefreshObjectCachesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.refresh_object_caches_with_options(request, runtime)
 
     def rollback_staging_config_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: RollbackStagingConfigRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: RollbackStagingConfigResponse
@@ -7471,15 +7345,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.RollbackStagingConfigResponse(),
             self.call_api(params, req, runtime)
         )
 
     def rollback_staging_config(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: RollbackStagingConfigRequest
 
         @return: RollbackStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -7531,15 +7405,15 @@
         @return: SetCdnDomainCSRCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.set_cdn_domain_csrcertificate_with_options(request, runtime)
 
     def set_cdn_domain_smcertificate_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: SetCdnDomainSMCertificateRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: SetCdnDomainSMCertificateResponse
@@ -7573,27 +7447,93 @@
         return TeaCore.from_map(
             cdn_20180510_models.SetCdnDomainSMCertificateResponse(),
             self.call_api(params, req, runtime)
         )
 
     def set_cdn_domain_smcertificate(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: SetCdnDomainSMCertificateRequest
 
         @return: SetCdnDomainSMCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.set_cdn_domain_smcertificate_with_options(request, runtime)
 
+    def set_cdn_domain_sslcertificate_with_options(self, request, runtime):
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
+    def set_cdn_domain_sslcertificate(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.set_cdn_domain_sslcertificate_with_options(request, runtime)
+
     def set_cdn_domain_staging_config_with_options(self, request, runtime):
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
@@ -7621,28 +7561,47 @@
         return TeaCore.from_map(
             cdn_20180510_models.SetCdnDomainStagingConfigResponse(),
             self.call_api(params, req, runtime)
         )
 
     def set_cdn_domain_staging_config(self, request):
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
 
     def set_domain_server_certificate_with_options(self, request, runtime):
         """
-        >    The maximum number of times that each user can call this operation per second is 10.
-        *   Method: POST.
+        The content of the SSL certificate. Specify the content of the SSL certificate only if you want to enable the SSL certificate.
         
 
         @param request: SetDomainServerCertificateRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: SetDomainServerCertificateResponse
@@ -7684,16 +7643,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.SetDomainServerCertificateResponse(),
             self.call_api(params, req, runtime)
         )
 
     def set_domain_server_certificate(self, request):
         """
-        >    The maximum number of times that each user can call this operation per second is 10.
-        *   Method: POST.
+        The content of the SSL certificate. Specify the content of the SSL certificate only if you want to enable the SSL certificate.
         
 
         @param request: SetDomainServerCertificateRequest
 
         @return: SetDomainServerCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -7735,15 +7693,15 @@
 
     def set_req_header_config(self, request):
         runtime = util_models.RuntimeOptions()
         return self.set_req_header_config_with_options(request, runtime)
 
     def set_waiting_room_config_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: SetWaitingRoomConfigRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: SetWaitingRoomConfigResponse
@@ -7779,28 +7737,28 @@
         return TeaCore.from_map(
             cdn_20180510_models.SetWaitingRoomConfigResponse(),
             self.call_api(params, req, runtime)
         )
 
     def set_waiting_room_config(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 30.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: SetWaitingRoomConfigRequest
 
         @return: SetWaitingRoomConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.set_waiting_room_config_with_options(request, runtime)
 
     def start_cdn_domain_with_options(self, request, runtime):
         """
-        - If the domain name is in an invalid state or your have an overdue payment in your account, the domain name cannot be enabled.
-        - The maximum number of times that each user can call this operation per second is 100.
+        If the domain name is in an invalid state or you have an overdue payment in your account, the domain name cannot be enabled.
+        *   You can call this operation up to 100 times per second per account.
         
 
         @param request: StartCdnDomainRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: StartCdnDomainResponse
@@ -7830,29 +7788,29 @@
         return TeaCore.from_map(
             cdn_20180510_models.StartCdnDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def start_cdn_domain(self, request):
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
 
     def stop_cdn_domain_with_options(self, request, runtime):
         """
-        - After an accelerated domain is disabled, the information about the domain name is retained. Requests destined for the domain name are automatically redirected to the origin server.
-        - The maximum number of times that each user can call this operation per second is 40.
+        After an accelerated domain is disabled, Alibaba Cloud CDN retains its information and routes all the requests that are destined for the accelerated domain to the origin server.
+        *   You can call this operation up to 40 times per second per account.
         
 
         @param request: StopCdnDomainRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: StopCdnDomainResponse
@@ -7882,28 +7840,28 @@
         return TeaCore.from_map(
             cdn_20180510_models.StopCdnDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def stop_cdn_domain(self, request):
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
 
     def tag_resources_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
 
         @param request: TagResourcesRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: TagResourcesResponse
@@ -7933,27 +7891,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.TagResourcesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def tag_resources(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        The ID of the request.
         
 
         @param request: TagResourcesRequest
 
         @return: TagResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.tag_resources_with_options(request, runtime)
 
     def untag_resources_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: UntagResourcesRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: UntagResourcesResponse
@@ -7985,27 +7943,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.UntagResourcesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def untag_resources(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: UntagResourcesRequest
 
         @return: UntagResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.untag_resources_with_options(request, runtime)
 
     def update_cdn_deliver_task_with_options(self, request, runtime):
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
 
         @param request: UpdateCdnDeliverTaskRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: UpdateCdnDeliverTaskResponse
@@ -8041,27 +7999,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.UpdateCdnDeliverTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def update_cdn_deliver_task(self, request):
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
 
         @param request: UpdateCdnDeliverTaskRequest
 
         @return: UpdateCdnDeliverTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_cdn_deliver_task_with_options(request, runtime)
 
     def update_cdn_sub_task_with_options(self, request, runtime):
         """
-        >  You can call this API operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
 
         @param request: UpdateCdnSubTaskRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: UpdateCdnSubTaskResponse
@@ -8093,15 +8051,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.UpdateCdnSubTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def update_cdn_sub_task(self, request):
         """
-        >  You can call this API operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
 
         @param request: UpdateCdnSubTaskRequest
 
         @return: UpdateCdnSubTaskResponse
         """
         runtime = util_models.RuntimeOptions()
```

### Comparing `alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510/models.py` & `alibabacloud_cdn20180510_py2-1.2.8/alibabacloud_cdn20180510/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 
 
 class AddCdnDomainRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
-        # The key of a tag.
         self.key = key  # type: str
-        # The value of a tag.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AddCdnDomainRequestTag, self).to_map()
@@ -33,44 +31,24 @@
             self.value = m.get('Value')
         return self
 
 
 class AddCdnDomainRequest(TeaModel):
     def __init__(self, cdn_type=None, check_url=None, domain_name=None, owner_account=None, owner_id=None,
                  resource_group_id=None, scope=None, security_token=None, sources=None, tag=None, top_level_domain=None):
-        # The workload type of the domain name to accelerate. Valid values:
-        # 
-        # *   **web**: images and small files
-        # *   **download**: large files
-        # *   **video**: on-demand video and audio streaming
         self.cdn_type = cdn_type  # type: str
-        # The URL that is used for health checks.
         self.check_url = check_url  # type: str
-        # The domain name that you want to add to Alibaba Cloud CDN.
-        # 
-        # A wildcard domain that starts with a period (.) is supported, such as .example.com.
         self.domain_name = domain_name  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
-        # The ID of the resource group.
-        # 
-        # If you do not set this parameter, the system uses the ID of the default resource group.
         self.resource_group_id = resource_group_id  # type: str
-        # The acceleration region. Default value: domestic. Valid values:
-        # 
-        # *   **domestic**: Chinese mainland
-        # *   **overseas**: global (excluding the Chinese mainland)
-        # *   **global**: global
         self.scope = scope  # type: str
         self.security_token = security_token  # type: str
-        # The information about the addresses of origin servers.
         self.sources = sources  # type: str
-        # Details about the tags. You can specify up to 20 tags.
         self.tag = tag  # type: list[AddCdnDomainRequestTag]
-        # The top-level domain.
         self.top_level_domain = top_level_domain  # type: str
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -135,15 +113,14 @@
         if m.get('TopLevelDomain') is not None:
             self.top_level_domain = m.get('TopLevelDomain')
         return self
 
 
 class AddCdnDomainResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AddCdnDomainResponseBody, self).to_map()
@@ -326,38 +303,23 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class BatchAddCdnDomainRequest(TeaModel):
     def __init__(self, cdn_type=None, check_url=None, domain_name=None, owner_account=None, owner_id=None,
                  resource_group_id=None, scope=None, security_token=None, sources=None, top_level_domain=None):
-        # The workload type of the domain name to accelerate. Valid values:
-        # 
-        # *   **web**: images and small files
-        # *   **download**: large files
-        # *   **video**: on-demand video and audio streaming
         self.cdn_type = cdn_type  # type: str
-        # The URL that is used for health checks.
         self.check_url = check_url  # type: str
-        # The domain names that you want to add to Alibaba Cloud CDN. Separate domain names with commas (,).
         self.domain_name = domain_name  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
-        # The ID of the resource group. If you do not specify a value for this parameter, the system uses the ID of the default resource group.
         self.resource_group_id = resource_group_id  # type: str
-        # The acceleration region. Default value: domestic. Valid values:
-        # 
-        # *   **domestic**: Chinese mainland
-        # *   **overseas**: global (excluding the Chinese mainland)
-        # *   **global**: global
         self.scope = scope  # type: str
         self.security_token = security_token  # type: str
-        # The information about the addresses of origin servers.
         self.sources = sources  # type: str
-        # The top-level domain.
         self.top_level_domain = top_level_domain  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(BatchAddCdnDomainRequest, self).to_map()
@@ -410,15 +372,14 @@
         if m.get('TopLevelDomain') is not None:
             self.top_level_domain = m.get('TopLevelDomain')
         return self
 
 
 class BatchAddCdnDomainResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(BatchAddCdnDomainResponseBody, self).to_map()
@@ -475,17 +436,17 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class BatchDeleteCdnDomainConfigRequest(TeaModel):
     def __init__(self, domain_names=None, function_names=None, owner_account=None, owner_id=None,
                  security_token=None):
-        # The accelerated domain names whose configurations you want to delete. Separate accelerated domain names with commas (,).
+        # The accelerated domain names whose configurations you want to delete. Separate multiple accelerated domain names with commas (,).
         self.domain_names = domain_names  # type: str
-        # The names of the features that you want to manage. Separate feature names with commas (,).
+        # The names of the features that you want to delete. Separate multiple feature names with commas (,). For more information about feature names, see [Parameters for configuring features for domain names](~~388460~~).
         self.function_names = function_names  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
@@ -585,80 +546,17 @@
             temp_model = BatchDeleteCdnDomainConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class BatchSetCdnDomainConfigRequest(TeaModel):
     def __init__(self, domain_names=None, functions=None, owner_account=None, owner_id=None, security_token=None):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
+        # The ID of the request.
         self.domain_names = domain_names  # type: str
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
         self.functions = functions  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
@@ -694,19 +592,21 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class BatchSetCdnDomainConfigResponseBodyDomainConfigListDomainConfigModel(TeaModel):
     def __init__(self, config_id=None, domain_name=None, function_name=None):
-        # The ID of the configuration.
+        # The name of the feature.
         self.config_id = config_id  # type: long
-        # The domain name.
+        # > *   You can call this operation up to 30 times per second per account.
+        # *   You can specify multiple domain names and must separate them with commas (,). You can specify up to 50 domain names in each call.
+        # *   If the BatchSetCdnDomainConfig operation is successful, a unique configuration ID (ConfigId) is generated. You can use configuration IDs to update or delete configurations. For more information, see [Usage notes on ConfigId](~~388994~~).
         self.domain_name = domain_name  # type: str
-        # The name of the feature.
+        # The list of domain configurations.
         self.function_name = function_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(BatchSetCdnDomainConfigResponseBodyDomainConfigListDomainConfigModel, self).to_map()
@@ -763,17 +663,17 @@
                 temp_model = BatchSetCdnDomainConfigResponseBodyDomainConfigListDomainConfigModel()
                 self.domain_config_model.append(temp_model.from_map(k))
         return self
 
 
 class BatchSetCdnDomainConfigResponseBody(TeaModel):
     def __init__(self, domain_config_list=None, request_id=None):
-        # The list of domain configurations.
+        # The domain name.
         self.domain_config_list = domain_config_list  # type: BatchSetCdnDomainConfigResponseBodyDomainConfigList
-        # The ID of the request.
+        # The ID of the configuration.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.domain_config_list:
             self.domain_config_list.validate()
 
     def to_map(self):
@@ -836,38 +736,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class BatchSetCdnDomainServerCertificateRequest(TeaModel):
     def __init__(self, cert_name=None, cert_type=None, domain_name=None, force_set=None, owner_id=None, region=None,
                  sslpri=None, sslprotocol=None, sslpub=None, security_token=None):
-        # The name of the certificate.
+        # The region.
         self.cert_name = cert_name  # type: str
-        # The type of the SSL certificate. Valid values:
-        # 
-        # *   **upload**: a user-uploaded SSL certificate.
-        # *   **cas**: a certificate that is issued by SSL Certificates Service.
+        # Specifies whether to check the certificate name for duplicates. If you set the value to 1, the system does not perform the check and overwrites the information about the existing certificate that uses the same name.
         self.cert_type = cert_type  # type: str
-        # The accelerated domain name to which the SSL certificate belongs. The type of request supported by the accelerated domain name must be HTTPS. You can specify multiple accelerated domain names and separate them with commas (,).
-        # 
-        # >  You can manage the SSL certificates of up to 50 accelerated domain names in each call.
+        # The private key. Specify the private key only if you enable the SSL certificate.
         self.domain_name = domain_name  # type: str
         # Specifies whether to check the certificate name for duplicates. If you set the value to 1, the system does not perform the check and overwrites the information about the existing certificate that uses the same name.
         self.force_set = force_set  # type: str
         self.owner_id = owner_id  # type: long
-        # The region.
+        # The accelerated domain name to which the SSL certificate belongs. The type of request supported by the accelerated domain name must be HTTPS. You can specify multiple accelerated domain names and separate them with commas (,).
+        # 
+        # >  You can manage the SSL certificates of up to 50 accelerated domain names in each call.
         self.region = region  # type: str
         # The private key. Specify the private key only if you enable the SSL certificate.
         self.sslpri = sslpri  # type: str
-        # Specifies whether to enable the SSL certificate. Valid values:
-        # 
-        # *   **on**: enables the SSL certificate.
-        # *   **off**: disables the SSL certificate. This is the default value.
+        # The ID of the request.
         self.sslprotocol = sslprotocol  # type: str
-        # The content of the SSL certificate. Specify the content of the certificate only if you want to enable the SSL certificate.
+        # > *   The maximum number of times that each user can call this operation per second is 10.
+        # *   You can specify multiple domain names (no more than 50) and separate them with commas (,).
         self.sslpub = sslpub  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -921,15 +816,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class BatchSetCdnDomainServerCertificateResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
+        # The name of the certificate.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(BatchSetCdnDomainServerCertificateResponseBody, self).to_map()
@@ -985,15 +880,15 @@
             temp_model = BatchSetCdnDomainServerCertificateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class BatchStartCdnDomainRequest(TeaModel):
     def __init__(self, domain_names=None, owner_id=None, security_token=None):
-        # The domain names that you want to enable. Separate multiple domain names with commas (,).
+        # The ID of the request.
         self.domain_names = domain_names  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
@@ -1020,15 +915,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class BatchStartCdnDomainResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
+        # 1.0.0
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(BatchStartCdnDomainResponseBody, self).to_map()
@@ -1184,27 +1079,25 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class BatchUpdateCdnDomainRequest(TeaModel):
     def __init__(self, domain_name=None, owner_id=None, resource_group_id=None, security_token=None, sources=None,
                  top_level_domain=None):
-        # The accelerated domain names. You can specify one or more accelerated domain names. Separate domain names with commas (,).
+        # The top-level domain name.
+        # 
+        # >  You can set only one of **Sources** and **TopLevelDomain**. If you set both **Sources** and **TopLevelDomain**, **TopLevelDomain** does not take effect.
         self.domain_name = domain_name  # type: str
         self.owner_id = owner_id  # type: long
-        # The ID of the resource group.
+        # The ID of the request.
         self.resource_group_id = resource_group_id  # type: str
         self.security_token = security_token  # type: str
-        # The information about the addresses of origin servers.
-        # 
-        # >  You can set only one of **Sources** and **TopLevelDomain**. If you set both **Sources** and **TopLevelDomain**, **TopLevelDomain** does not take effect.
+        # The accelerated domain names. You can specify one or more accelerated domain names. Separate domain names with commas (,).
         self.sources = sources  # type: str
-        # The top-level domain name.
-        # 
-        # >  You can set only one of **Sources** and **TopLevelDomain**. If you set both **Sources** and **TopLevelDomain**, **TopLevelDomain** does not take effect.
+        # The operation that you want to perform. Set the value to **BatchUpdateCdnDomain**.
         self.top_level_domain = top_level_domain  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(BatchUpdateCdnDomainRequest, self).to_map()
@@ -1241,15 +1134,17 @@
         if m.get('TopLevelDomain') is not None:
             self.top_level_domain = m.get('TopLevelDomain')
         return self
 
 
 class BatchUpdateCdnDomainResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
+        # The information about the addresses of origin servers.
+        # 
+        # >  You can set only one of **Sources** and **TopLevelDomain**. If you set both **Sources** and **TopLevelDomain**, **TopLevelDomain** does not take effect.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(BatchUpdateCdnDomainResponseBody, self).to_map()
@@ -1308,27 +1203,27 @@
 
 
 class CreateCdnCertificateSigningRequestRequest(TeaModel):
     def __init__(self, city=None, common_name=None, country=None, email=None, organization=None,
                  organization_unit=None, sans=None, state=None):
         # The city to which the organization belongs. Default value: Hangzhou.
         self.city = city  # type: str
-        # The Common Name of the SSL certificate.
+        # The email address that can be used to contact the organization.
         self.common_name = common_name  # type: str
-        # The country to which the organization belongs. Default value: CN.
+        # The content of the CSR.
         self.country = country  # type: str
-        # The email address that can be used to contact the organization.
+        # The operation that you want to perform. Set the value to **CreateCdnCertificateSigningRequest**.
         self.email = email  # type: str
-        # The name of the organization. Default value: Alibaba Inc.
+        # The Subject Alternative Name (SAN) extension of the SSL certificate. This extension is used to add domain names to the certificate. Separate multiple domain names with commas (,).
         self.organization = organization  # type: str
-        # The name of the organization unit. Default value: Aliyun CDN.
+        # The MD5 value of the certificate public key.
         self.organization_unit = organization_unit  # type: str
-        # The Subject Alternative Name (SAN) extension of the SSL certificate. This extension is used to add domain names to the certificate. Separate multiple domain names with commas (,).
+        # The Common Name of the certificate.
         self.sans = sans  # type: str
-        # The provincial district to which the organization belongs. Default value: Zhejiang.
+        # The name of the organization. Default value: Alibaba Inc.
         self.state = state  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateCdnCertificateSigningRequestRequest, self).to_map()
@@ -1373,21 +1268,21 @@
         if m.get('State') is not None:
             self.state = m.get('State')
         return self
 
 
 class CreateCdnCertificateSigningRequestResponseBody(TeaModel):
     def __init__(self, common_name=None, csr=None, pub_md_5=None, request_id=None):
-        # The Common Name of the certificate.
+        # The name of the organization unit. Default value: Aliyun CDN.
         self.common_name = common_name  # type: str
-        # The content of the CSR.
+        # The Common Name of the SSL certificate.
         self.csr = csr  # type: str
-        # The MD5 value of the certificate public key.
+        # The provincial district to which the organization belongs. Default value: Zhejiang.
         self.pub_md_5 = pub_md_5  # type: str
-        # The ID of the request.
+        # The country to which the organization belongs. Default value: CN.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateCdnCertificateSigningRequestResponseBody, self).to_map()
@@ -1455,21 +1350,19 @@
             temp_model = CreateCdnCertificateSigningRequestResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateCdnDeliverTaskRequest(TeaModel):
     def __init__(self, deliver=None, domain_name=None, name=None, reports=None, schedule=None):
-        # The method that is used to send operations reports. Operations reports are sent to you only by email. The settings must be escaped in JSON.
+        # The ID of the tracking task.
         self.deliver = deliver  # type: str
-        # The domain names to be tracked. Separate multiple domain names with commas (,). You can specify up to 500 domain names. If you want to specify more than 500 domain names, [submit a ticket](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex).  
-        # 
-        # >  If you do not specify a domain name, the custom operations reports are created for all domain names that belong to your Alibaba Cloud account.
+        # The method that is used to send operations reports. Operations reports are sent to you only by email. The settings must be escaped in JSON.
         self.domain_name = domain_name  # type: str
-        # The name of the tracking task.
+        # > You can call this operation up to three times per second per account.
         self.name = name  # type: str
         # The operations reports that are tracked by the task. The data must be escaped in JSON.
         self.reports = reports  # type: str
         # The parameters that specify the time interval at which the tracking task sends operations reports. The settings must be escaped in JSON.
         self.schedule = schedule  # type: str
 
     def validate(self):
@@ -1506,17 +1399,56 @@
         if m.get('Schedule') is not None:
             self.schedule = m.get('Schedule')
         return self
 
 
 class CreateCdnDeliverTaskResponseBody(TeaModel):
     def __init__(self, deliver_id=None, request_id=None):
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
         self.deliver_id = deliver_id  # type: str
-        # The ID of the request.
+        # Creates a tracking task that generates operations reports. The tracking task sends operations reports to a specified email address based on a specified schedule.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateCdnDeliverTaskResponseBody, self).to_map()
@@ -1688,15 +1620,15 @@
         return self
 
 
 class CreateIllegalUrlExportTaskRequest(TeaModel):
     def __init__(self, task_name=None, time_point=None):
         # The name of the export task.
         self.task_name = task_name  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-DDThh:mm:ssZ format. The finest granularity is one day.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. The minimum time granularity is 1 day.
         self.time_point = time_point  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateIllegalUrlExportTaskRequest, self).to_map()
@@ -1787,17 +1719,17 @@
             temp_model = CreateIllegalUrlExportTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateRealTimeLogDeliveryRequest(TeaModel):
     def __init__(self, domain=None, logstore=None, project=None, region=None):
-        # The accelerated domain name for which you want to configure real-time log delivery. You can specify multiple domain names and separate them with commas (,).
+        # The accelerated domain name for which you want to configure real-time log delivery.
         self.domain = domain  # type: str
-        # The name of the Logstore that collects log data from Alibaba Cloud Content Delivery Network (CDN) in real time.
+        # The name of the Logstore where log entries are stored.
         self.logstore = logstore  # type: str
         # The name of the Log Service project that is used for real-time log delivery.
         self.project = project  # type: str
         # The ID of the region where the Log Service project is deployed. For more information, see [Regions that support real-time log delivery](~~144883~~).
         self.region = region  # type: str
 
     def validate(self):
@@ -2273,15 +2205,15 @@
             temp_model = DeleteCdnDeliverTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteCdnDomainRequest(TeaModel):
     def __init__(self, domain_name=None, owner_account=None, owner_id=None):
-        # The accelerated domain name that you want to delete. You can specify only one domain name in each call.
+        # The ID of the request.
         self.domain_name = domain_name  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
 
     def validate(self):
         pass
 
@@ -2308,15 +2240,15 @@
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         return self
 
 
 class DeleteCdnDomainResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
+        # 1.0.0
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteCdnDomainResponseBody, self).to_map()
@@ -2525,19 +2457,20 @@
             temp_model = DeleteFCTriggerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteRealTimeLogLogstoreRequest(TeaModel):
     def __init__(self, logstore=None, project=None, region=None):
-        # The name of the Logstore to which log entries are delivered.
+        # The ID of the region where the Log Service project is deployed. For more information, see [Regions that support real-time log delivery](~~144883~~).
         self.logstore = logstore  # type: str
-        # The name of the Log Service project that is used for real-time log delivery.
+        # Deletes the Logstore that is used by a specified configuration record of real-time
+        #                   log delivery.
         self.project = project  # type: str
-        # The ID of the region where the Log Service project is deployed. For more information, see [Regions that support real-time log delivery](~~144883~~).
+        # The name of the Log Service project that is used for real-time log delivery.
         self.region = region  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteRealTimeLogLogstoreRequest, self).to_map()
@@ -2628,15 +2561,15 @@
         return self
 
 
 class DeleteRealtimeLogDeliveryRequest(TeaModel):
     def __init__(self, domain=None, logstore=None, project=None, region=None):
         # The acceleration domain name for which you want to disable real-time log delivery. You can specify multiple domain names and separate them with commas (,).
         self.domain = domain  # type: str
-        # The name of the Logstore that collects log data from Alibaba Cloud Content Delivery Network (CDN) in real time.
+        # The name of the Logstore where log entries are stored.
         self.logstore = logstore  # type: str
         # The name of the Log Service project that is used for real-time log delivery.
         self.project = project  # type: str
         # The ID of the region where the Log Service project is deployed. For more information, see [Regions that support real-time log delivery](~~144883~~).
         self.region = region  # type: str
 
     def validate(self):
@@ -2733,15 +2666,15 @@
             temp_model = DeleteRealtimeLogDeliveryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteSpecificConfigRequest(TeaModel):
     def __init__(self, config_id=None, domain_name=None, owner_id=None, security_token=None):
-        # The configuration IDs. Separate configuration IDs with commas (,). For more information about ConfigId, see [Usage notes on ConfigId](~~388994~~).
+        # The ID of the configuration. Separate multiple configuration IDs with commas (,). For more information about ConfigId, see [Usage notes on ConfigId](~~388994~~).
         self.config_id = config_id  # type: str
         # The accelerated domain name. You can specify only one domain name.
         self.domain_name = domain_name  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
@@ -2838,15 +2771,15 @@
             temp_model = DeleteSpecificConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteSpecificStagingConfigRequest(TeaModel):
     def __init__(self, config_id=None, domain_name=None, owner_id=None, security_token=None):
-        # The configuration IDs. Separate configuration IDs with commas (,). For more information about ConfigId, see [Usage notes on ConfigId](~~388994~~).
+        # The ID of the request.
         self.config_id = config_id  # type: str
         # The accelerated domain names (no more than 50). Separate domain names with commas (,).
         self.domain_name = domain_name  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
@@ -2879,15 +2812,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DeleteSpecificStagingConfigResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
+        # The operation that you want to perform. Set the value to **DeleteSpecificStagingConfig**.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteSpecificStagingConfigResponseBody, self).to_map()
@@ -3123,17 +3056,17 @@
         return self
 
 
 class DescribeBlockedRegionsRequest(TeaModel):
     def __init__(self, language=None):
         # The language. Valid values:
         # 
-        # - **zh**: simplified Chinese
-        # - **en**: English
-        # - **jp**: Japanese
+        # *   **zh**: simplified Chinese
+        # *   **en**: English
+        # *   **jp**: Japanese
         self.language = language  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeBlockedRegionsRequest, self).to_map()
@@ -3219,15 +3152,15 @@
                 temp_model = DescribeBlockedRegionsResponseBodyInfoListInfoItem()
                 self.info_item.append(temp_model.from_map(k))
         return self
 
 
 class DescribeBlockedRegionsResponseBody(TeaModel):
     def __init__(self, info_list=None, request_id=None):
-        # A list of countries and regions.
+        # The information returned.
         self.info_list = info_list  # type: DescribeBlockedRegionsResponseBodyInfoList
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.info_list:
             self.info_list.validate()
@@ -3326,19 +3259,19 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeCdnCertificateDetailResponseBody(TeaModel):
     def __init__(self, cert=None, cert_id=None, cert_name=None, key=None, request_id=None):
-        # The content of the SSL certificate.
+        # The certificate.
         self.cert = cert  # type: str
-        # The ID of the SSL certificate.
+        # The ID of the certificate.
         self.cert_id = cert_id  # type: long
-        # The name of the SSL certificate.
+        # The name of the certificate.
         self.cert_name = cert_name  # type: str
         # The key of the SSL certificate.
         self.key = key  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
@@ -3414,17 +3347,17 @@
             temp_model = DescribeCdnCertificateDetailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCdnCertificateListRequest(TeaModel):
     def __init__(self, domain_name=None, owner_id=None, security_token=None):
-        # The accelerated domain names. Separate multiple accelerated domain names with commas (,).
+        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
         # 
-        # If you do not specify an ID, SSL certificates of all your accelerated domain names are queried.
+        # If you do not specify an accelerated domain name, SSL certificates of all your accelerated domain names are queried.
         self.domain_name = domain_name  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
@@ -3451,25 +3384,25 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeCdnCertificateListResponseBodyCertificateListModelCertListCert(TeaModel):
     def __init__(self, cert_id=None, cert_name=None, common=None, fingerprint=None, issuer=None, last_time=None):
-        # The ID of the SSL certificate.
+        # The ID of the certificate.
         self.cert_id = cert_id  # type: long
-        # The name of the SSL certificate.
+        # The name of the certificate.
         self.cert_name = cert_name  # type: str
-        # The Common Name (CN) attribute of the SSL certificate. In most cases, the value is a domain name.
+        # The Common Name (CN) attribute of the certificate. In most cases, the CN is a domain name.
         self.common = common  # type: str
-        # The fingerprint of the SSL certificate.
+        # The fingerprint of the certificate.
         self.fingerprint = fingerprint  # type: str
-        # The certificate authority (CA) that issued the SSL certificate.
+        # The certificate authority (CA) that issued the certificate.
         self.issuer = issuer  # type: str
-        # The timestamp when the SSL certificate was issued.
+        # The timestamp.
         self.last_time = last_time  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnCertificateListResponseBodyCertificateListModelCertListCert, self).to_map()
@@ -3538,17 +3471,17 @@
                 temp_model = DescribeCdnCertificateListResponseBodyCertificateListModelCertListCert()
                 self.cert.append(temp_model.from_map(k))
         return self
 
 
 class DescribeCdnCertificateListResponseBodyCertificateListModel(TeaModel):
     def __init__(self, cert_list=None, count=None):
-        # The details about each SSL certificate.
+        # The list of certificates.
         self.cert_list = cert_list  # type: DescribeCdnCertificateListResponseBodyCertificateListModelCertList
-        # The number of SSL certificates returned.
+        # The number of certificates that are returned.
         self.count = count  # type: int
 
     def validate(self):
         if self.cert_list:
             self.cert_list.validate()
 
     def to_map(self):
@@ -3571,15 +3504,15 @@
         if m.get('Count') is not None:
             self.count = m.get('Count')
         return self
 
 
 class DescribeCdnCertificateListResponseBody(TeaModel):
     def __init__(self, certificate_list_model=None, request_id=None):
-        # The data type of the SSL certificate information.
+        # Details about certificates.
         self.certificate_list_model = certificate_list_model  # type: DescribeCdnCertificateListResponseBodyCertificateListModel
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.certificate_list_model:
             self.certificate_list_model.validate()
@@ -3643,17 +3576,17 @@
             temp_model = DescribeCdnCertificateListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCdnDeletedDomainsRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None):
-        # The number of the page to return. Pages start from page **1**. Valid values: **1** to **100000**.
+        # The number of the page to return. Valid values: **1** to **100000**. Default value: **1**.
         self.page_number = page_number  # type: int
-        # The number of entries to return on each page. Default value: **20**. Valid values: **1** to **500**. The value must be an integer.
+        # The number of domain names to return per page. Valid values: an integer between **1** and **500**. Default value: **20**.
         self.page_size = page_size  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnDeletedDomainsRequest, self).to_map()
@@ -3676,15 +3609,15 @@
         return self
 
 
 class DescribeCdnDeletedDomainsResponseBodyDomainsPageData(TeaModel):
     def __init__(self, domain_name=None, gmt_modified=None):
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The last time when the accelerated domain name was modified. The time is in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC+0.
+        # The time when the accelerated domain name was modified. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.gmt_modified = gmt_modified  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnDeletedDomainsResponseBodyDomainsPageData, self).to_map()
@@ -3737,21 +3670,21 @@
                 temp_model = DescribeCdnDeletedDomainsResponseBodyDomainsPageData()
                 self.page_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeCdnDeletedDomainsResponseBody(TeaModel):
     def __init__(self, domains=None, page_number=None, page_size=None, request_id=None, total_count=None):
-        # The information about the accelerated domain names.
+        # The list of accelerated domain names and the time each domain name was last modified.
         self.domains = domains  # type: DescribeCdnDeletedDomainsResponseBodyDomains
-        # The page number of the returned page. It corresponds to the request parameter **PageNumber**.
+        # The page number of the returned page, which is the same as the **PageNumber** parameter in request parameters.
         self.page_number = page_number  # type: long
-        # The number of entries returned per page. It corresponds to the request parameter **PageSize**.
+        # The number of domain names returned per page, which is the same as the **PageSize** parameter in request parameters.
         self.page_size = page_size  # type: long
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id  # type: str
         # The total number of domain names returned.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.domains:
             self.domains.validate()
@@ -3922,22 +3855,22 @@
             temp_model = DescribeCdnDeliverListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCdnDomainByCertificateRequest(TeaModel):
     def __init__(self, sslpub=None, sslstatus=None):
-        # The public key of the SSL certificate. You must encode the public key in Base64 and then call the encodeURIComponent function to encode the public key again.
+        # The public key of the SSL certificate. You must encode the public key in Base64 before you invoke the encodeURIComponent function to encode a URI component.
         # 
-        # The public key must be in the Privacy-Enhanced Mail (PEM) format.
+        # A public key in the Privacy Enhanced Mail (PEM) format is supported.
         self.sslpub = sslpub  # type: str
-        # Specifies whether the domain name list to return contains only domain names with HTTPS enabled or disabled.
+        # Specifies whether to return only domain names with HTTPS enabled or disabled.
         # 
-        # *   true: The list contains only domain names with HTTPS enabled.
-        # *   false: The list contains only domain names with HTTPS disabled.
+        # *   true: returns only domain names with HTTPS enabled.
+        # *   false: returns only domain names with HTTPS disabled.
         self.sslstatus = sslstatus  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnDomainByCertificateRequest, self).to_map()
@@ -3961,31 +3894,31 @@
 
 
 class DescribeCdnDomainByCertificateResponseBodyCertInfosCertInfo(TeaModel):
     def __init__(self, cert_ca_is_legacy=None, cert_expire_time=None, cert_expired=None, cert_start_time=None,
                  cert_subject_common_name=None, cert_type=None, domain_list=None, domain_names=None, issuer=None):
         # Indicates whether the SSL certificate is obsolete. Valid values:
         # 
-        # *   **yes**: The SSL certificate is obsolete.
-        # *   **no**: The SSL certificate is working as expected.
+        # *   **yes**\
+        # *   **no**\
         self.cert_ca_is_legacy = cert_ca_is_legacy  # type: str
-        # The time at which the certificate expires.
+        # The expiration time of the certificate.
         self.cert_expire_time = cert_expire_time  # type: str
         # Indicates whether the SSL certificate is expired. Valid values:
         # 
-        # *   **yes**: The SSL certificate is expired.
-        # *   **no**: The SSL certificate is not expired.
+        # *   **yes**\
+        # *   **no**\
         self.cert_expired = cert_expired  # type: str
-        # The time at which the certificate became effective.
+        # The effective time of the certificate.
         self.cert_start_time = cert_start_time  # type: str
         # The name of the SSL certificate owner.
         self.cert_subject_common_name = cert_subject_common_name  # type: str
         # The type of the certificate. Valid values: **RSA**, **DSA**, and **ECDSA**.
         self.cert_type = cert_type  # type: str
-        # If a value is returned, the value matches the SSL certificate. Multiple domain names are separated by commas (,).
+        # The list of domain names. If a value is returned, the value matches the SSL certificate. Multiple domain names are separated by commas (,).
         self.domain_list = domain_list  # type: str
         # The domain names (DNS fields) that match the SSL certificate. Multiple domain names are separated by commas (,).
         self.domain_names = domain_names  # type: str
         # The certificate authority (CA) that issued the certificate.
         self.issuer = issuer  # type: str
 
     def validate(self):
@@ -4144,17 +4077,17 @@
         return self
 
 
 class DescribeCdnDomainConfigsRequest(TeaModel):
     def __init__(self, config_id=None, domain_name=None, function_names=None, owner_id=None, security_token=None):
         # The ID of the configuration. For more information about ConfigId, see [Usage notes on ConfigId](~~388994~~).
         self.config_id = config_id  # type: str
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name  # type: str
-        # The names of the features. Separate multiple feature names with commas (,). For more information, see [BatchSetCdnDomainConfig](~~388460~~).
+        # The names of the features. Separate multiple feature names with commas (,). For more information, see [Parameters for configuring features for domain names](~~388460~~).
         self.function_names = function_names  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
@@ -4258,15 +4191,17 @@
     def __init__(self, config_id=None, function_args=None, function_name=None, parent_id=None, status=None):
         # The ID of the configuration.
         self.config_id = config_id  # type: str
         # The configuration of each feature.
         self.function_args = function_args  # type: DescribeCdnDomainConfigsResponseBodyDomainConfigsDomainConfigFunctionArgs
         # The name of the feature.
         self.function_name = function_name  # type: str
-        # The ID of the rule condition. This parameter is optional. To create a rule condition, you can configure the **condition** feature that is described in the [BatchSetCdnDomainConfig and SetCdnDomainStagingConfig](~~388460~~) topic. A rule condition can identify parameters that are included in requests and filter requests based on the identified parameters. Each rule condition has a [ConfigId](~~388994~~). You can use ConfigId as ParentId that is referenced by other features. This way, you can combine rule conditions and features for flexible configurations.
+        # The ID of the rule condition. This parameter is optional.
+        # 
+        # To create a rule condition, you can configure the **condition** feature that is described in the [Parameters for configuring features for domain names](~~388460~~) topic. A rule condition can identify parameters that are included in requests and filter requests based on the identified parameters. Each rule condition has a [ConfigId](~~388994~~). You can use ConfigId as ParentId that is referenced by other features. This way, you can combine rule conditions and features for flexible configurations.
         # 
         # For more information, see [BatchSetCdnDomainConfig](~~90915~~) or ParentId configuration example in this topic.
         self.parent_id = parent_id  # type: str
         # The status of the configuration. Valid values:
         # 
         # *   **success**\
         # *   **testing**\
@@ -4459,17 +4394,17 @@
         self.enabled = enabled  # type: str
         # The port over which requests are redirected to the origin server. Ports 443 and 80 are supported.
         self.port = port  # type: int
         # The priority.
         self.priority = priority  # type: str
         # The type of the origin server. Valid values:
         # 
-        # *   **ipaddr:** an IP address.
-        # *   **domain:** a domain name
-        # *   **oss:** the OSS domain of an Object Storage Service (OSS) bucket
+        # *   **ipaddr**: an origin IP address
+        # *   **domain**: an origin domain name
+        # *   **oss**: the domain name of an Object Storage Service (OSS) bucket
         # *   **fc_domain:** a Function Compute domain name
         self.type = type  # type: str
         # The weight of the origin server if multiple origin servers have been specified.
         self.weight = weight  # type: str
 
     def validate(self):
         pass
@@ -4551,38 +4486,40 @@
         # 
         # *   **web**: images and small files
         # *   **download**: large files
         # *   **video**: on-demand video and audio streaming
         self.cdn_type = cdn_type  # type: str
         # The CNAME that is assigned to the accelerated domain name. You must add the CNAME record in the system of your DNS service provider to map the accelerated domain name to the CNAME.
         self.cname = cname  # type: str
-        # The description of the request.
+        # The description of the domain name.
         self.description = description  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
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
         self.domain_status = domain_status  # type: str
-        # The time when the audio or video file was created.
+        # The time when the domain name was created.
         self.gmt_created = gmt_created  # type: str
         # The time when the domain name was last modified.
         self.gmt_modified = gmt_modified  # type: str
         # The CNAME for which HTTPS is enabled.
         self.https_cname = https_cname  # type: str
         # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
         # The acceleration region.
         self.scope = scope  # type: str
-        # Indicates whether the Security Socket Layer (SSL) certificate is enabled. Valid values:
+        # Indicates whether the SSL certificate is enabled. Valid values:
         # 
         # *   **on**\
         # *   **off**\
         self.server_certificate_status = server_certificate_status  # type: str
         # The information about the origin server.
         self.source_models = source_models  # type: DescribeCdnDomainDetailResponseBodyGetDomainDetailModelSourceModels
 
@@ -5047,15 +4984,15 @@
             temp_model = DescribeCdnDomainLogsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCdnDomainStagingConfigRequest(TeaModel):
     def __init__(self, domain_name=None, function_names=None):
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name  # type: str
         # The list of feature names. Separate multiple values with commas (,). For more information, see [A list of features](~~388460~~).
         self.function_names = function_names  # type: str
 
     def validate(self):
         pass
 
@@ -5078,17 +5015,17 @@
         if m.get('FunctionNames') is not None:
             self.function_names = m.get('FunctionNames')
         return self
 
 
 class DescribeCdnDomainStagingConfigResponseBodyDomainConfigsFunctionArgs(TeaModel):
     def __init__(self, arg_name=None, arg_value=None):
-        # The name of the configuration.
+        # The configuration name.
         self.arg_name = arg_name  # type: str
-        # The value of the configuration.
+        # The configuration value.
         self.arg_value = arg_value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnDomainStagingConfigResponseBodyDomainConfigsFunctionArgs, self).to_map()
@@ -5109,30 +5046,28 @@
         if m.get('ArgValue') is not None:
             self.arg_value = m.get('ArgValue')
         return self
 
 
 class DescribeCdnDomainStagingConfigResponseBodyDomainConfigs(TeaModel):
     def __init__(self, config_id=None, function_args=None, function_name=None, parent_id=None, status=None):
-        # The ID of the configuration.
+        # The configuration ID.
         self.config_id = config_id  # type: str
         # The description of each feature.
         self.function_args = function_args  # type: list[DescribeCdnDomainStagingConfigResponseBodyDomainConfigsFunctionArgs]
-        # The name of the feature.
+        # The feature name.
         self.function_name = function_name  # type: str
-        # The ID of the rule condition. This parameter is optional. To create a rule condition, you can configure the **condition** feature that is described in the [BatchSetCdnDomainConfig and SetCdnDomainStagingConfig](~~388460~~) topic. A rule condition can identify parameters that are included in requests and filter requests based on the identified parameters. Each rule condition has a [ConfigId](~~388994~~). You can use ConfigId as ParentId that is referenced by other features. This way, you can combine rule conditions and features for flexible configurations.
-        # 
-        # For more information, see [BatchSetCdnDomainConfig](~~90915~~) or ParentId configuration example in this topic.
+        # The rule condition ID. This parameter is optional. To create a rule condition, you can configure the **condition** feature that is described in the [Parameters for configuring features for domain names](~~388460~~) topic. A rule condition can identify parameters that are included in requests and filter requests based on the identified parameters. Each rule condition has a [ConfigId](~~388994~~). You can reference ConfigId instead of ParentId in other features. This way, you can combine rule conditions and features for flexible configurations. For more information, see [BatchSetCdnDomainConfig](~~90915~~) or ParentId configuration example in this topic.
         self.parent_id = parent_id  # type: str
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
         self.status = status  # type: str
 
     def validate(self):
         if self.function_args:
             for k in self.function_args:
                 if k:
                     k.validate()
@@ -5173,19 +5108,19 @@
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
 class DescribeCdnDomainStagingConfigResponseBody(TeaModel):
     def __init__(self, domain_configs=None, domain_name=None, request_id=None):
-        # The configurations of the domain name.
+        # The domain name configurations.
         self.domain_configs = domain_configs  # type: list[DescribeCdnDomainStagingConfigResponseBodyDomainConfigs]
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.domain_configs:
             for k in self.domain_configs:
                 if k:
                     k.validate()
@@ -5615,15 +5550,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeCdnRegionAndIspResponseBodyIspsIsp(TeaModel):
     def __init__(self, name_en=None, name_zh=None):
-        # The English name of the region.
+        # The English name of the ISP.
         self.name_en = name_en  # type: str
         # The Chinese name of the ISP.
         self.name_zh = name_zh  # type: str
 
     def validate(self):
         pass
 
@@ -5741,17 +5676,17 @@
                 temp_model = DescribeCdnRegionAndIspResponseBodyRegionsRegion()
                 self.region.append(temp_model.from_map(k))
         return self
 
 
 class DescribeCdnRegionAndIspResponseBody(TeaModel):
     def __init__(self, isps=None, regions=None, request_id=None):
-        # A list of ISPs.
+        # The list of ISPs.
         self.isps = isps  # type: DescribeCdnRegionAndIspResponseBodyIsps
-        # A list of regions.
+        # The list of regions.
         self.regions = regions  # type: DescribeCdnRegionAndIspResponseBodyRegions
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.isps:
             self.isps.validate()
@@ -5823,40 +5758,40 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCdnReportRequest(TeaModel):
     def __init__(self, area=None, domain_name=None, end_time=None, http_code=None, is_overseas=None, report_id=None,
                  start_time=None):
-        # The region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
+        # The region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         # 
-        # *   If you do not specify a region, all regions are queried.
-        # *   If you specify a region, data in the specified region is returned. You can specify one or more regions. Separate regions with commas (,).
+        # *   If you do not specify a region, data in all regions is queried.
+        # *   If you specify a region, data in the specified region is queried. You can specify one or more regions. If you specify multiple regions, separate the regions with commas (,).
         self.area = area  # type: str
-        # The domain names that you want to query. Separate domain names with commas (,).
+        # The domain name that you want to query. Separate domain names with commas (,).
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time  # type: str
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
         self.http_code = http_code  # type: str
-        # Specify whether the region is outside the Chinese mainland. Valid values:
+        # Specifies whether the region is outside the Chinese mainland. Valid values:
         # 
         # *   **1**: outside the Chinese mainland
         # *   **0**: inside the Chinese mainland
         self.is_overseas = is_overseas  # type: str
-        # The ID of the operations report that you want to query. You can enter only one ID in each call. You can call the [DescribeCdnSubList](~~271655~~) operation to query the report ID.
+        # The ID of the operations report that you want to query. You can specify only one ID in each request. You can call the [DescribeCdnSubList](~~271655~~) operation to query report IDs.
         self.report_id = report_id  # type: long
-        # The beginning of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnReportRequest, self).to_map()
@@ -5992,15 +5927,15 @@
         if m.get('ReportId') is not None:
             self.report_id = m.get('ReportId')
         return self
 
 
 class DescribeCdnReportListResponseBody(TeaModel):
     def __init__(self, content=None, request_id=None):
-        # The information about the operations report.
+        # The information about the report that is queried.
         self.content = content  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
@@ -6098,27 +6033,27 @@
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeCdnSMCertificateDetailResponseBody(TeaModel):
     def __init__(self, cert_expire_time=None, cert_identifier=None, cert_name=None, cert_org=None, common_name=None,
                  encrypt_certificate=None, request_id=None, sans=None, sign_certificate=None):
-        # The time when the certificate expires. The time is displayed in UTC.
+        # The name of the certificate.
         self.cert_expire_time = cert_expire_time  # type: str
         # The ID of the certificate.
         self.cert_identifier = cert_identifier  # type: str
-        # The name of the certificate.
+        # The time when the certificate expires. The time is displayed in UTC.
         self.cert_name = cert_name  # type: str
         # The certificate authority (CA) that issued the certificate.
         self.cert_org = cert_org  # type: str
         # The top-level domain name.
         self.common_name = common_name  # type: str
-        # The content of the encryption certificate.
-        self.encrypt_certificate = encrypt_certificate  # type: str
         # The ID of the request.
+        self.encrypt_certificate = encrypt_certificate  # type: str
+        # The content of the encryption certificate.
         self.request_id = request_id  # type: str
         # The subdomain name.
         self.sans = sans  # type: str
         # The content of the signature certificate.
         self.sign_certificate = sign_certificate  # type: str
 
     def validate(self):
@@ -6320,15 +6255,15 @@
                 temp_model = DescribeCdnSMCertificateListResponseBodyCertificateListModelCertListCert()
                 self.cert.append(temp_model.from_map(k))
         return self
 
 
 class DescribeCdnSMCertificateListResponseBodyCertificateListModel(TeaModel):
     def __init__(self, cert_list=None, count=None):
-        # A list of certificates.
+        # The list of certificates.
         self.cert_list = cert_list  # type: DescribeCdnSMCertificateListResponseBodyCertificateListModelCertList
         # The number of certificates that are returned.
         self.count = count  # type: int
 
     def validate(self):
         if self.cert_list:
             self.cert_list.validate()
@@ -6454,15 +6389,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeCdnServiceResponseBodyOperationLocksLockReason(TeaModel):
     def __init__(self, lock_reason=None):
-        # The reason why Alibaba Cloud CDN is locked. A value of financial indicates that the service is locked due to overdue payments.
+        # The reason why the service is locked. A value of financial indicates that the service is locked due to overdue payments.
         self.lock_reason = lock_reason  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnServiceResponseBodyOperationLocksLockReason, self).to_map()
@@ -6512,31 +6447,31 @@
                 self.lock_reason.append(temp_model.from_map(k))
         return self
 
 
 class DescribeCdnServiceResponseBody(TeaModel):
     def __init__(self, changing_affect_time=None, changing_charge_type=None, instance_id=None,
                  internet_charge_type=None, opening_time=None, operation_locks=None, request_id=None):
-        # The time when the next billing method takes effect. The time is displayed in GMT.
+        # The time when the metering method for the next cycle takes effect. The time is displayed in GMT.
         self.changing_affect_time = changing_affect_time  # type: str
-        # The next billing method that Alibaba Cloud CDN will use. Valid values:
+        # The metering method for the next cycle. Valid values:
         # 
-        # *   **PayByTraffic**: pay-by-data-transfer.
-        # *   **PayByBandwidth**: pay-by-bandwidth.
+        # *   **PayByTraffic**: pay-by-data-transfer
+        # *   **PayByBandwidth**: pay-by-bandwidth
         self.changing_charge_type = changing_charge_type  # type: str
         # The ID of the instance.
         self.instance_id = instance_id  # type: str
-        # The current billing method of Alibaba Cloud CDN.
+        # The current metering method. Valid values:
         # 
-        # *   **PayByTraffic**: pay-by-data-transfer.
-        # *   **PayByBandwidth**: pay-by-bandwidth.
+        # *   **PayByTraffic**: pay-by-data-transfer
+        # *   **PayByBandwidth**: pay-by-bandwidth
         self.internet_charge_type = internet_charge_type  # type: str
-        # The time when Alibaba Cloud CDN was activated. The time follows the ISO 8601 standard in the yyyy-MM-ddThh:mmZ format.
+        # The time when the service was activated. The time follows the ISO 8601 standard.
         self.opening_time = opening_time  # type: str
-        # The lock status of Alibaba Cloud CDN.
+        # The lock status.
         self.operation_locks = operation_locks  # type: DescribeCdnServiceResponseBodyOperationLocks
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.operation_locks:
             self.operation_locks.validate()
@@ -6620,17 +6555,15 @@
             temp_model = DescribeCdnServiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCdnSubListResponseBody(TeaModel):
     def __init__(self, content=None, request_id=None):
-        # The information about the custom report.
         self.content = content  # type: str
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnSubListResponseBody, self).to_map()
@@ -6971,35 +6904,35 @@
         return self
 
 
 class DescribeCdnUserBillPredictionRequest(TeaModel):
     def __init__(self, area=None, dimension=None, end_time=None, start_time=None):
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
         self.area = area  # type: str
-        # The billable item. A value of flow indicates bandwidth.
+        # The billable item. A value of flow specifies bandwidth.
         self.dimension = dimension  # type: str
-        # The default value is the current time. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end time of the estimation. The default value is the current time. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The default value is 00:00 on the first day of the current month. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The start time of the estimation. The default value is 00:00 on the first day of the current month. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnUserBillPredictionRequest, self).to_map()
@@ -7030,15 +6963,15 @@
         return self
 
 
 class DescribeCdnUserBillPredictionResponseBodyBillPredictionDataBillPredictionDataItem(TeaModel):
     def __init__(self, area=None, time_stp=None, value=None):
         # The billable region.
         self.area = area  # type: str
-        # The time when the value used as the estimated value is generated. This field is returned only if the metering method is pay by 95th percentile, pay by 95th percentile bandwidth with 50% off from 00:00 to 08:00, or pay by 4th peak bandwidth per month.
+        # The time when the value used as the estimated value is generated. This parameter is returned only if the metering method is pay by 95th percentile, pay by 95th percentile bandwidth with 50% off from 00:00 to 08:00, or pay by 4th peak bandwidth per month.
         self.time_stp = time_stp  # type: str
         # The estimated value.
         self.value = value  # type: float
 
     def validate(self):
         pass
 
@@ -7097,31 +7030,31 @@
                 temp_model = DescribeCdnUserBillPredictionResponseBodyBillPredictionDataBillPredictionDataItem()
                 self.bill_prediction_data_item.append(temp_model.from_map(k))
         return self
 
 
 class DescribeCdnUserBillPredictionResponseBody(TeaModel):
     def __init__(self, bill_prediction_data=None, bill_type=None, end_time=None, request_id=None, start_time=None):
-        # The list of bill prediction data.
+        # The estimated bill data.
         self.bill_prediction_data = bill_prediction_data  # type: DescribeCdnUserBillPredictionResponseBodyBillPredictionData
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
         self.bill_type = bill_type  # type: str
         # The end time of the estimation.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
         # The start time of the estimation.
         self.start_time = start_time  # type: str
@@ -7420,18 +7353,17 @@
             temp_model = DescribeCdnUserBillTypeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCdnUserConfigsRequest(TeaModel):
     def __init__(self, function_name=None):
-        # The configuration item that you want to query. Valid values:
+        # The name of the parameter.
         # 
-        # *   **domain\_business\_control**: Alibaba Cloud CDN configurations
-        # *   **waf**: Web Application Firewall (WAF) configurations
+        # The configurations set by enterprise or government users.
         self.function_name = function_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnUserConfigsRequest, self).to_map()
@@ -7448,29 +7380,30 @@
         if m.get('FunctionName') is not None:
             self.function_name = m.get('FunctionName')
         return self
 
 
 class DescribeCdnUserConfigsResponseBodyConfigs(TeaModel):
     def __init__(self, arg_name=None, arg_value=None, function_name=None):
-        # The name of the parameter.
-        # 
-        # The configurations set by enterprise or government users.
+        # The name of the feature.
         self.arg_name = arg_name  # type: str
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
         self.arg_value = arg_value  # type: str
-        # The name of the feature.
+        # The configuration item that you want to query. Valid values:
+        # 
+        # *   **domain_business_control**: Alibaba Cloud CDN configurations
+        # *   **waf**: Web Application Firewall (WAF) configurations
         self.function_name = function_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnUserConfigsResponseBodyConfigs, self).to_map()
@@ -7495,17 +7428,17 @@
         if m.get('FunctionName') is not None:
             self.function_name = m.get('FunctionName')
         return self
 
 
 class DescribeCdnUserConfigsResponseBody(TeaModel):
     def __init__(self, configs=None, request_id=None):
-        # The configurations of Alibaba Cloud CDN.
+        # >  The maximum number of times that each user can call this operation per second is 30.
         self.configs = configs  # type: list[DescribeCdnUserConfigsResponseBodyConfigs]
-        # The ID of the request.
+        # The name of the feature.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.configs:
             for k in self.configs:
                 if k:
                     k.validate()
@@ -7573,25 +7506,17 @@
             temp_model = DescribeCdnUserConfigsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCdnUserDomainsByFuncRequest(TeaModel):
     def __init__(self, func_id=None, page_number=None, page_size=None, resource_group_id=None):
-        # The ID of the feature. For more information about how to query feature IDs, see [Feature settings for a domain name](~~388460~~). For example, the ID of the origin host feature (set_req_host_header) is 18.
         self.func_id = func_id  # type: int
-        # The number of the page to return. Default value: **1**.
-        # 
-        # Valid values: **1** to **100000**.
         self.page_number = page_number  # type: int
-        # The number of entries to return on each page. Default value: **20**.
-        # 
-        # Valid values: **1** to **50**.
         self.page_size = page_size  # type: int
-        # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnUserDomainsByFuncRequest, self).to_map()
@@ -7620,28 +7545,18 @@
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         return self
 
 
 class DescribeCdnUserDomainsByFuncResponseBodyDomainsPageDataSourcesSource(TeaModel):
     def __init__(self, content=None, port=None, priority=None, type=None, weight=None):
-        # The address of the origin server.
         self.content = content  # type: str
-        # The port of the origin server.
         self.port = port  # type: int
-        # The priority.
         self.priority = priority  # type: str
-        # The type of the origin server. Valid values:
-        # 
-        # *   **ipaddr**: an origin IP address
-        # *   **domain:** a domain name
-        # *   **oss:** the OSS domain of an Object Storage Service (OSS) bucket
-        # *   **fc_domain:** a Function Compute domain name
         self.type = type  # type: str
-        # The weight of the origin server if multiple origin servers have been specified.
         self.weight = weight  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnUserDomainsByFuncResponseBodyDomainsPageDataSourcesSource, self).to_map()
@@ -7707,50 +7622,23 @@
                 self.source.append(temp_model.from_map(k))
         return self
 
 
 class DescribeCdnUserDomainsByFuncResponseBodyDomainsPageData(TeaModel):
     def __init__(self, cdn_type=None, cname=None, description=None, domain_name=None, domain_status=None,
                  gmt_created=None, gmt_modified=None, resource_group_id=None, sources=None, ssl_protocol=None):
-        # The type of the workload accelerated by Alibaba Cloud CDN. Valid values:
-        # 
-        # *   **web**: image and small file distribution
-        # *   **download**: large file distribution
-        # *   **video**: on-demand video and audio streaming
-        # *   **liveStream**: live streaming
         self.cdn_type = cdn_type  # type: str
-        # The CNAME assigned to the accelerated domain name.
         self.cname = cname  # type: str
-        # The description of the accelerated domain name.
         self.description = description  # type: str
-        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
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
         self.domain_status = domain_status  # type: str
-        # The time when the accelerated domain name was added.
         self.gmt_created = gmt_created  # type: str
-        # The time when the accelerated domain name was modified.
         self.gmt_modified = gmt_modified  # type: str
-        # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
-        # The information about the origin server.
         self.sources = sources  # type: DescribeCdnUserDomainsByFuncResponseBodyDomainsPageDataSources
-        # Indicates whether HTTPS is enabled. Valid values:
-        # 
-        # *   **on**\
-        # *   **off**\
         self.ssl_protocol = ssl_protocol  # type: str
 
     def validate(self):
         if self.sources:
             self.sources.validate()
 
     def to_map(self):
@@ -7837,23 +7725,18 @@
                 temp_model = DescribeCdnUserDomainsByFuncResponseBodyDomainsPageData()
                 self.page_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeCdnUserDomainsByFuncResponseBody(TeaModel):
     def __init__(self, domains=None, page_number=None, page_size=None, request_id=None, total_count=None):
-        # The configurations of the accelerated domain name.
         self.domains = domains  # type: DescribeCdnUserDomainsByFuncResponseBodyDomains
-        # The page number of the returned page.
         self.page_number = page_number  # type: long
-        # The number of entries returned per page.
         self.page_size = page_size  # type: long
-        # The ID of the request.
         self.request_id = request_id  # type: str
-        # The total number of domain names returned.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.domains:
             self.domains.validate()
 
     def to_map(self):
@@ -7962,15 +7845,15 @@
     def __init__(self, block_quota=None, block_remain=None, domain_quota=None, ignore_params_quota=None,
                  ignore_params_remain=None, preload_quota=None, preload_remain=None, refresh_dir_quota=None, refresh_dir_remain=None,
                  refresh_url_quota=None, refresh_url_remain=None, request_id=None):
         # The maximum number of URLs and directories that can be blocked.
         self.block_quota = block_quota  # type: int
         # The remaining number of URLs and directories that can be blocked.
         self.block_remain = block_remain  # type: int
-        # The maximum number of accelerated domain names that can be added to Alibaba Cloud CDN.
+        # The maximum number of accelerated domain names.
         self.domain_quota = domain_quota  # type: int
         self.ignore_params_quota = ignore_params_quota  # type: int
         self.ignore_params_remain = ignore_params_remain  # type: int
         # The maximum number of URLs that can be prefetched.
         self.preload_quota = preload_quota  # type: int
         # The remaining number of URLs that can be prefetched.
         self.preload_remain = preload_remain  # type: int
@@ -8088,18 +7971,18 @@
         return self
 
 
 class DescribeCdnUserResourcePackageRequest(TeaModel):
     def __init__(self, owner_id=None, security_token=None, status=None):
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
-        # Resource plan status:
+        # The remaining quota of the resource plan.
         # 
-        # *   **valid**: valid
-        # *   **closed**: invalid
+        # *   The total amount of data transfer provided by the resource plan. Unit: bytes.
+        # *   The remaining number of requests provided by the resource plan.
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnUserResourcePackageRequest, self).to_map()
@@ -8125,40 +8008,37 @@
             self.status = m.get('Status')
         return self
 
 
 class DescribeCdnUserResourcePackageResponseBodyResourcePackageInfosResourcePackageInfo(TeaModel):
     def __init__(self, commodity_code=None, curr_capacity=None, display_name=None, end_time=None,
                  init_capacity=None, instance_id=None, start_time=None, status=None, template_name=None):
-        # The ID of the resource plan.
-        self.commodity_code = commodity_code  # type: str
-        # The remaining quota of the resource plan.
+        # The total quota of the resource plan.
         # 
         # *   The total amount of data transfer provided by the resource plan. Unit: bytes.
-        # *   The remaining number of requests provided by the resource plan.
+        # *   The total number of requests provided by the resource plan.
+        self.commodity_code = commodity_code  # type: str
+        # The ID of the instance.
         self.curr_capacity = curr_capacity  # type: str
-        # The name of the resource plan.
+        # The time when the resource plan took effect.
         self.display_name = display_name  # type: str
-        # The time when the resource plan expires.
+        # The operation that you want to perform. Set the value to **DescribeCdnUserResourcePackage**.
         self.end_time = end_time  # type: str
-        # The total quota of the resource plan.
-        # 
-        # *   The total amount of data transfer provided by the resource plan. Unit: bytes.
-        # *   The total number of requests provided by the resource plan.
+        # The ID of the resource plan.
         self.init_capacity = init_capacity  # type: str
-        # The ID of the instance.
+        # The ID of the request.
         self.instance_id = instance_id  # type: str
-        # The time when the resource plan took effect.
+        # The name of the template.
         self.start_time = start_time  # type: str
         # The status of the data transfer plan. Valid values:
         # 
         # *   **valid**: valid
         # *   **closed**: invalid
         self.status = status  # type: str
-        # The name of the template.
+        # The details about each resource plan. The details are organized in an array. The array consists of the subparameter values of the ResourcePackageInfo parameter.
         self.template_name = template_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnUserResourcePackageResponseBodyResourcePackageInfosResourcePackageInfo, self).to_map()
@@ -8239,17 +8119,17 @@
                 temp_model = DescribeCdnUserResourcePackageResponseBodyResourcePackageInfosResourcePackageInfo()
                 self.resource_package_info.append(temp_model.from_map(k))
         return self
 
 
 class DescribeCdnUserResourcePackageResponseBody(TeaModel):
     def __init__(self, request_id=None, resource_package_infos=None):
-        # The ID of the request.
+        # The name of the resource plan.
         self.request_id = request_id  # type: str
-        # The details about each resource plan. The details are organized in an array. The array consists of the subparameter values of the ResourcePackageInfo parameter.
+        # The time when the resource plan expires.
         self.resource_package_infos = resource_package_infos  # type: DescribeCdnUserResourcePackageResponseBodyResourcePackageInfos
 
     def validate(self):
         if self.resource_package_infos:
             self.resource_package_infos.validate()
 
     def to_map(self):
@@ -8311,17 +8191,28 @@
             temp_model = DescribeCdnUserResourcePackageResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCdnWafDomainRequest(TeaModel):
     def __init__(self, domain_name=None, region_id=None, resource_group_id=None):
-        # The accelerated domain name.
+        # The domain name that you want to query.
+        # 
+        # You can specify only one domain name in each request. You have three options to configure this parameter:
+        # 
+        # *   Specify an exact domain name. For example, if you set this parameter to example.com, configuration information of example.com is queried.
+        # *   Specify a keyword. For example, if you set this parameter to example, configuration information about all domain names that contain example is queried.
+        # *   Leave this parameter empty. If this parameter is left empty, all accelerated domain names for which WAF is configured are queried.
         self.domain_name = domain_name  # type: str
-        # The ID of the region.
+        # The region where WAF is enabled. Valid values:
+        # 
+        # *   **cn-hangzhou**: inside the Chinese mainland
+        # *   **ap-southeast-1**: outside the Chinese mainland
+        # 
+        # > ap-southeast-1 includes Hong Kong (China), Macao (China), Taiwan (China), and other countries and regions.
         self.region_id = region_id  # type: str
         # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
 
     def validate(self):
         pass
 
@@ -8348,19 +8239,36 @@
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         return self
 
 
 class DescribeCdnWafDomainResponseBodyOutPutDomains(TeaModel):
     def __init__(self, acl_status=None, cc_status=None, domain=None, status=None, waf_status=None):
+        # The status of the access control list (ACL) feature. Valid values:
+        # 
+        # *   **0**: disabled
+        # *   **1**: enabled
         self.acl_status = acl_status  # type: str
+        # The status of protection against HTTP flood attacks. Valid values:
+        # 
+        # *   **0**: disabled
+        # *   **1**: enabled
         self.cc_status = cc_status  # type: str
-        # The domain name.
+        # The accelerated domain name.
         self.domain = domain  # type: str
+        # The WAF status of the domain name. Valid values:
+        # 
+        # *   **1**: The domain name is added to WAF or valid.
+        # *   **10**: The domain name is being added to WAF.
+        # *   **11**: The domain name failed to be added to WAF.
         self.status = status  # type: str
+        # The status of WAF. Valid values:
+        # 
+        # *   **0**: disabled
+        # *   **1**: enabled
         self.waf_status = waf_status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnWafDomainResponseBodyOutPutDomains, self).to_map()
@@ -8393,18 +8301,19 @@
         if m.get('WafStatus') is not None:
             self.waf_status = m.get('WafStatus')
         return self
 
 
 class DescribeCdnWafDomainResponseBody(TeaModel):
     def __init__(self, out_put_domains=None, request_id=None, total_count=None):
+        # The information about the accelerated domain name.
         self.out_put_domains = out_put_domains  # type: list[DescribeCdnWafDomainResponseBodyOutPutDomains]
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The total number of entries returned.
+        # The number of accelerated domain names.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.out_put_domains:
             for k in self.out_put_domains:
                 if k:
                     k.validate()
@@ -8696,21 +8605,21 @@
         if m.get('ConfigId') is not None:
             self.config_id = m.get('ConfigId')
         return self
 
 
 class DescribeCustomLogConfigResponseBody(TeaModel):
     def __init__(self, remark=None, request_id=None, sample=None, tag=None):
-        # The format of the log configuration.
+        # The operation that you want to perform. Set the value to **DescribeCustomLogConfig**.
         self.remark = remark  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
         # A sample log configuration.
         self.sample = sample  # type: str
-        # The tag information about the log configuration.
+        # The format of the log configuration.
         self.tag = tag  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCustomLogConfigResponseBody, self).to_map()
@@ -8779,37 +8688,35 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainAverageResponseTimeRequest(TeaModel):
     def __init__(self, domain_name=None, domain_type=None, end_time=None, interval=None, isp_name_en=None,
                  location_name_en=None, start_time=None, time_merge=None):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
-        # 
-        # By default, this operation queries the bandwidth values during back-to-origin routing for all accelerated domain names that belong to your Alibaba Cloud account.
+        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you do not set this parameter, all ISPs are queried.
         self.domain_name = domain_name  # type: str
-        # The type of the query condition. Valid values: When you set the value to dynamic, this operation queries the average response time of dynamic resources and static resources. If you do not set this parameter, this operation queries the average response time of only static resources. By default, this parameter is not set.
-        self.domain_type = domain_type  # type: str
-        # The end of the time range queried. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # The end time must be later than the start time.
-        self.end_time = end_time  # type: str
         # The time interval between the data entries. Unit: seconds. The value varies based on the values of the **StartTime** and **EndTime** parameters. Valid values:
         # 
         # *   If the time span between StartTime and EndTime is less than 3 days (3 days excluded), valid values are **300**, **3600**, and **86400**. Default value: **300**.
         # *   If the time span between StartTime and EndTime is from 3 to 31 days (31 days excluded), valid values are **3600** and **86400**. Default value: **3600**.
         # *   If the time range between StartTime and EndTime is 31 days or longer, the valid value is **86400**. Default value: **86400**.
+        self.domain_type = domain_type  # type: str
+        # The end of the time range during which data was queried.
+        self.end_time = end_time  # type: str
+        # The beginning of the time range during which data was queried.
         self.interval = interval  # type: str
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you do not set this parameter, all ISPs are queried.
+        # The ID of the request.
         self.isp_name_en = isp_name_en  # type: str
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
+        # The accelerated domain name.
         self.location_name_en = location_name_en  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
         self.start_time = start_time  # type: str
-        # Specifies whether to automatically set the interval. If you set the value to 1, the value of the Interval parameter is automatically assigned based on the StartTime and EndTime parameters. You can set this parameter or the Interval parameter.
+        # The end of the time range queried. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # The end time must be later than the start time.
         self.time_merge = time_merge  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainAverageResponseTimeRequest, self).to_map()
@@ -8854,17 +8761,17 @@
         if m.get('TimeMerge') is not None:
             self.time_merge = m.get('TimeMerge')
         return self
 
 
 class DescribeDomainAverageResponseTimeResponseBodyAvgRTPerIntervalDataModule(TeaModel):
     def __init__(self, time_stamp=None, value=None):
-        # The timestamp of the returned data.
+        # The accelerated domain name.
         self.time_stamp = time_stamp  # type: str
-        # The average response time.
+        # The type of the query condition. Valid values: When you set the value to dynamic, this operation queries the average response time of dynamic resources and static resources. If you do not set this parameter, this operation queries the average response time of only static resources. By default, this parameter is not set.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainAverageResponseTimeResponseBodyAvgRTPerIntervalDataModule, self).to_map()
@@ -8918,25 +8825,29 @@
                 self.data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainAverageResponseTimeResponseBody(TeaModel):
     def __init__(self, avg_rtper_interval=None, data_interval=None, domain_name=None, end_time=None,
                  request_id=None, start_time=None):
-        # The average response time collected at each time interval.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
         self.avg_rtper_interval = avg_rtper_interval  # type: DescribeDomainAverageResponseTimeResponseBodyAvgRTPerInterval
-        # The time interval between the data entries returned.
+        # The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.  
+        # 
+        # > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        # - You can call this operation up to 100 times per second per account.
+        # - You can specify multiple domain names and separate them with commas (,). You can specify at most 50 domain names in each call.
         self.data_interval = data_interval  # type: str
-        # The accelerated domain name.
+        # The timestamp of the returned data.
         self.domain_name = domain_name  # type: str
-        # The end of the time range during which data was queried.
+        # The time interval between the data entries returned.
         self.end_time = end_time  # type: str
-        # The ID of the request.
+        # The average response time.
         self.request_id = request_id  # type: str
-        # The beginning of the time range during which data was queried.
+        # The average response time collected at each time interval.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.avg_rtper_interval:
             self.avg_rtper_interval.validate()
 
     def to_map(self):
@@ -9015,35 +8926,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainBpsDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, isp_name_en=None, location_name_en=None,
                  start_time=None):
-        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
-        # 
-        # By default, this operation queries bandwidth data for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time granularity of the data entries. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
-        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
-        # 
-        # If you do not set this parameter, data of all ISPs is queried.
         self.isp_name_en = isp_name_en  # type: str
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
-        # 
-        # If you do not specify a region, data in all regions is queried.
         self.location_name_en = location_name_en  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainBpsDataRequest, self).to_map()
@@ -9081,27 +8976,20 @@
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainBpsDataResponseBodyBpsDataPerIntervalDataModule(TeaModel):
     def __init__(self, domestic_value=None, https_domestic_value=None, https_overseas_value=None, https_value=None,
                  overseas_value=None, time_stamp=None, value=None):
-        # The bandwidth value in the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.domestic_value = domestic_value  # type: str
-        # The bandwidth data for HTTPS requests in the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.https_domestic_value = https_domestic_value  # type: str
-        # The bandwidth data for HTTPS requests in regions outside the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.https_overseas_value = https_overseas_value  # type: str
-        # The bandwidth value for HTTPS requests. Unit: bit/s.
         self.https_value = https_value  # type: str
-        # The bandwidth data in regions outside the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.overseas_value = overseas_value  # type: str
-        # The timestamp of the data returned.
         self.time_stamp = time_stamp  # type: str
-        # The bandwidth. Unit: bit/s.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainBpsDataResponseBodyBpsDataPerIntervalDataModule, self).to_map()
@@ -9175,29 +9063,21 @@
                 self.data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainBpsDataResponseBody(TeaModel):
     def __init__(self, bps_data_per_interval=None, data_interval=None, domain_name=None, end_time=None,
                  isp_name_en=None, location_name_en=None, request_id=None, start_time=None):
-        # The list of bandwidth data entries returned at each interval.
         self.bps_data_per_interval = bps_data_per_interval  # type: DescribeDomainBpsDataResponseBodyBpsDataPerInterval
-        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
-        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The name of the ISP.
         self.isp_name_en = isp_name_en  # type: str
-        # The name of the region.
         self.location_name_en = location_name_en  # type: str
-        # The ID of the request.
         self.request_id = request_id  # type: str
-        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.bps_data_per_interval:
             self.bps_data_per_interval.validate()
 
     def to_map(self):
@@ -9719,44 +9599,44 @@
 
 
 class DescribeDomainCcActivityLogRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, page_number=None, page_size=None, rule_name=None,
                  start_time=None, trigger_object=None, value=None):
         # The accelerated domain name. You can specify multiple domain names and separate them with commas (,).
         # 
-        # If you do not specify a domain name, data of all domain names is queried.
+        # If you do not specify this parameter, data of all accelerated domain names under your account is queried.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The number of the page to return. Default value: **1**.
+        # The page number of the page to return. Default value: **1**.
         self.page_number = page_number  # type: long
         # The number of entries to return on each page. Default value: **30**.
         self.page_size = page_size  # type: long
         # A custom rule name. Valid values:
         # 
-        # *   Default mode: default_normal.
-        # *   Emergency mode: default_attack.
+        # *   default_normal: rule for the normal mode
+        # *   default_attack: rule for the emergency mode
         # 
-        # If you do not set this parameter, all events that triggered rate limiting are queried.
+        # If you leave this parameter empty, events that triggered rate limiting based on all rules are queried.
         self.rule_name = rule_name  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # Data is collected every 5 minutes.
+        # The minimum time granularity of data collection is 5 minutes.
         # 
-        # If you do not set this parameter, data within the last 24 hours is queried.
+        # If you leave this parameter empty, the data collected over the last 24 hours is queried.
         self.start_time = start_time  # type: str
-        # The object that triggered rate limiting.
+        # The trigger of rate limiting by which you want to query data.
         # 
-        # If you do not set this parameter, all events that triggered rate limiting are queried.
+        # If you leave this parameter empty, all events that triggered rate limiting are queried.
         self.trigger_object = trigger_object  # type: str
-        # The value of the object that triggered rate limiting.
+        # The value of the trigger.
         # 
-        # If you do not set this parameter, the values of all events that triggered rate limiting are queried.
+        # If you leave this parameter empty, all events recorded for the trigger are queried.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainCcActivityLogRequest, self).to_map()
@@ -9806,23 +9686,23 @@
 class DescribeDomainCcActivityLogResponseBodyActivityLog(TeaModel):
     def __init__(self, action=None, domain_name=None, rule_name=None, time_stamp=None, trigger_object=None, ttl=None,
                  value=None):
         # The action that was triggered.
         self.action = action  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The name of the rule that was triggered
+        # The name of the rule based on which rate limiting was triggered.
         self.rule_name = rule_name  # type: str
-        # The timestamp of the data.
+        # The timestamp of the data returned.
         self.time_stamp = time_stamp  # type: str
-        # The object that triggered rate limiting.
+        # The trigger of rate limiting.
         self.trigger_object = trigger_object  # type: str
-        # The period of time that rate limiting remains effective.
+        # The period of time during which rate limiting remains effective.
         self.ttl = ttl  # type: long
-        # The value of the object that triggered rate limiting.
+        # The value of the trigger for rate limiting.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainCcActivityLogResponseBodyActivityLog, self).to_map()
@@ -9863,15 +9743,15 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class DescribeDomainCcActivityLogResponseBody(TeaModel):
     def __init__(self, activity_log=None, page_index=None, page_size=None, request_id=None, total=None):
-        # The log entry of the event that triggered rate limiting.
+        # The list of rate limiting logs.
         self.activity_log = activity_log  # type: list[DescribeDomainCcActivityLogResponseBodyActivityLog]
         # The page number of the returned page.
         self.page_index = page_index  # type: long
         # The number of entries returned per page.
         self.page_size = page_size  # type: long
         # The ID of the request.
         self.request_id = request_id  # type: str
@@ -9959,15 +9839,15 @@
             temp_model = DescribeDomainCcActivityLogResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainCertificateInfoRequest(TeaModel):
     def __init__(self, domain_name=None):
-        # The accelerated domain name. You can specify only one domain name in each query.
+        # The information about the SSL certificate.
         self.domain_name = domain_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainCertificateInfoRequest, self).to_map()
@@ -9986,68 +9866,70 @@
         return self
 
 
 class DescribeDomainCertificateInfoResponseBodyCertInfosCertInfo(TeaModel):
     def __init__(self, cert_domain_name=None, cert_expire_time=None, cert_id=None, cert_life=None, cert_name=None,
                  cert_org=None, cert_region=None, cert_start_time=None, cert_type=None, cert_update_time=None,
                  domain_cname_status=None, domain_name=None, server_certificate=None, server_certificate_status=None, status=None):
-        # The domain name that matches the SSL certificate.
+        # The name of the certificate authority (CA) that issued the SSL certificate.
         self.cert_domain_name = cert_domain_name  # type: str
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
         self.cert_expire_time = cert_expire_time  # type: str
+        # The domain name that matches the SSL certificate.
         self.cert_id = cert_id  # type: str
-        # The unit of the validity period of the SSL certificate.
-        # 
-        # *   **months**: The validity period is measured in months.
-        # *   **years**: The validity period is measured in years.
+        # The time when the certificate was renewed.
         self.cert_life = cert_life  # type: str
-        # The name of the SSL certificate.
+        # The public key of the SSL certificate.
         self.cert_name = cert_name  # type: str
-        # The name of the certificate authority (CA) that issued the SSL certificate.
+        # The time when the SSL certificate became effective.
         self.cert_org = cert_org  # type: str
+        # The status of HTTPS.
+        # 
+        # *   **on**: enabled.
+        # *   **off**: disabled.
         self.cert_region = cert_region  # type: str
-        # The time when the SSL certificate became effective.
+        # The name of the SSL certificate.
         self.cert_start_time = cert_start_time  # type: str
-        # The type of the SSL certificate. Valid values:
-        # 
-        # *   **free**: a free SSL certificate.
-        # *   **cas**: an SSL certificate purchased from Alibaba Cloud SSL Certificates Service.
-        # *   **upload**: a user-uploaded SSL certificate.
-        self.cert_type = cert_type  # type: str
-        # The time when the certificate was renewed.
-        self.cert_update_time = cert_update_time  # type: str
         # The status of the CNAME of the domain name.
         # 
         # *   **ok**: The domain name points to the CNAME assigned from Alibaba Cloud Content Delivery Network (CDN).
         # *   **cname_error**: An error occurred and the domain name cannot point to the CNAME.
         # *   **top_domain_cname_error**: An error occurred to the CNAME of the top-level domain name. The domain name cannot point to the CNAME.
         # *   **unsupport_wildcard**: Wildcard domain names are not supported.
-        self.domain_cname_status = domain_cname_status  # type: str
-        # The accelerated domain name.
-        self.domain_name = domain_name  # type: str
-        # The public key of the SSL certificate.
-        self.server_certificate = server_certificate  # type: str
+        self.cert_type = cert_type  # type: str
         # The status of HTTPS.
         # 
         # *   **on**: enabled.
         # *   **off**: disabled.
-        self.server_certificate_status = server_certificate_status  # type: str
-        # The status of the SSL certificate.
+        self.cert_update_time = cert_update_time  # type: str
+        # >  The maximum number of times that each user can call this operation per second is 100.
+        self.domain_cname_status = domain_cname_status  # type: str
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
+        self.domain_name = domain_name  # type: str
+        # The public key of the SSL certificate.
+        self.server_certificate = server_certificate  # type: str
+        # The accelerated domain name.
+        self.server_certificate_status = server_certificate_status  # type: str
+        # The domain name that matches the SSL certificate.
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainCertificateInfoResponseBodyCertInfosCertInfo, self).to_map()
@@ -10152,17 +10034,20 @@
                 temp_model = DescribeDomainCertificateInfoResponseBodyCertInfosCertInfo()
                 self.cert_info.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainCertificateInfoResponseBody(TeaModel):
     def __init__(self, cert_infos=None, request_id=None):
-        # The information about the SSL certificate.
+        # The unit of the validity period of the SSL certificate.
+        # 
+        # *   **months**: The validity period is measured in months.
+        # *   **years**: The validity period is measured in years.
         self.cert_infos = cert_infos  # type: DescribeDomainCertificateInfoResponseBodyCertInfos
-        # The ID of the request.
+        # The time when the SSL certificate expires.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.cert_infos:
             self.cert_infos.validate()
 
     def to_map(self):
@@ -10418,23 +10303,23 @@
         if m.get('DomainName') is not None:
             self.domain_name = m.get('DomainName')
         return self
 
 
 class DescribeDomainCustomLogConfigResponseBody(TeaModel):
     def __init__(self, config_id=None, remark=None, request_id=None, sample=None, tag=None):
-        # The ID of the log configuration.
+        # The sample log configuration.
         self.config_id = config_id  # type: str
-        # The format of the log configuration.
-        self.remark = remark  # type: str
         # The ID of the request.
+        self.remark = remark  # type: str
+        # The format of the log configuration.
         self.request_id = request_id  # type: str
-        # The sample log configuration.
+        # The operation that you want to perform. Set the value to **DescribeDomainCustomLogConfig**.
         self.sample = sample  # type: str
-        # The tag information about the log configuration.
+        # The ID of the log configuration.
         self.tag = tag  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainCustomLogConfigResponseBody, self).to_map()
@@ -10507,35 +10392,35 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainDetailDataByLayerRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, field=None, isp_name_en=None, layer=None,
                  location_name_en=None, start_time=None):
-        # The domain name that you want to query. You can specify multiple domain names and separate them with commas (,). You can specify at most 30 domain names in each call.
-        self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # >  The end time must be later than the start time.
-        self.end_time = end_time  # type: str
-        # The metric that you want to query. You can specify one or more metrics and separate them with commas (,). Valid values: **bps**, **qps**, **traf**, **acc**, **ipv6\_traf**, **ipv6\_bps**, **ipv6\_acc**, **ipv6\_qps**, and **http_code**.
-        self.field = field  # type: str
         # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
         # 
         # If you do not specify an ISP, data of all ISPs is queried.
-        self.isp_name_en = isp_name_en  # type: str
+        self.domain_name = domain_name  # type: str
         # The protocol by which you want to query data. Valid values: **http**, **https**, **quic**, and **all**.
         # 
         # The default value is **all**.
+        self.end_time = end_time  # type: str
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # >  The end time must be later than the start time.
+        self.field = field  # type: str
+        # The ID of the request.
+        self.isp_name_en = isp_name_en  # type: str
+        # The amount of network traffic. Unit: bytes.
         self.layer = layer  # type: str
+        # The detailed data of the accelerated domain names.
+        self.location_name_en = location_name_en  # type: str
         # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         # 
         # If you do not specify a region, data in all regions is queried.
-        self.location_name_en = location_name_en  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainDetailDataByLayerRequest, self).to_map()
@@ -10577,35 +10462,46 @@
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainDetailDataByLayerResponseBodyDataDataModule(TeaModel):
     def __init__(self, acc=None, bps=None, domain_name=None, http_code=None, ipv_6acc=None, ipv_6bps=None,
                  ipv_6qps=None, ipv_6traf=None, qps=None, time_stamp=None, traf=None):
-        # The number of requests.
+        # The timestamp of the data returned.
         self.acc = acc  # type: long
-        # The bandwidth. Unit: bit/s.
+        # The bandwidth of IPv6 requests. Unit: bit/s.
         self.bps = bps  # type: float
-        # The domain name.
+        # The number of requests.
         self.domain_name = domain_name  # type: str
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
         self.http_code = http_code  # type: str
-        # The number of IPv6 requests.
+        # The bandwidth. Unit: bit/s.
         self.ipv_6acc = ipv_6acc  # type: long
-        # The bandwidth of IPv6 requests. Unit: bit/s.
+        # The number of IPv6 requests.
         self.ipv_6bps = ipv_6bps  # type: float
-        # The number of IPv6 requests per second.
-        self.ipv_6qps = ipv_6qps  # type: float
         # The amount of network traffic generated by IPv6 requests. Unit: bytes.
+        self.ipv_6qps = ipv_6qps  # type: float
+        # The proportions of HTTP status codes.
         self.ipv_6traf = ipv_6traf  # type: long
-        # The number of queries per second.
+        # The number of requests.
         self.qps = qps  # type: float
-        # The timestamp of the data returned.
+        # The domain name.
         self.time_stamp = time_stamp  # type: str
-        # The amount of network traffic. Unit: bytes.
+        # The bandwidth of IPv6 requests. Unit: bit/s.
         self.traf = traf  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainDetailDataByLayerResponseBodyDataDataModule, self).to_map()
@@ -10694,17 +10590,17 @@
                 temp_model = DescribeDomainDetailDataByLayerResponseBodyDataDataModule()
                 self.data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainDetailDataByLayerResponseBody(TeaModel):
     def __init__(self, data=None, request_id=None):
-        # The detailed data of the accelerated domain names.
+        # The number of IPv6 requests per second.
         self.data = data  # type: DescribeDomainDetailDataByLayerResponseBodyData
-        # The ID of the request.
+        # The number of queries per second.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -10766,31 +10662,17 @@
             temp_model = DescribeDomainDetailDataByLayerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainHitRateDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, start_time=None):
-        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
-        # 
-        # By default, this operation queries the byte hit ratios for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time granularity of the data entries. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
-        # The beginning of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainHitRateDataRequest, self).to_map()
@@ -10819,19 +10701,16 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainHitRateDataResponseBodyHitRateIntervalDataModule(TeaModel):
     def __init__(self, https_value=None, time_stamp=None, value=None):
-        # The byte hit ratio of HTTPS requests.
         self.https_value = https_value  # type: str
-        # The timestamp of the data returned.
         self.time_stamp = time_stamp  # type: str
-        # The byte hit ratio.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainHitRateDataResponseBodyHitRateIntervalDataModule, self).to_map()
@@ -10889,25 +10768,19 @@
                 self.data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainHitRateDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, hit_rate_interval=None, request_id=None,
                  start_time=None):
-        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
-        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The byte hit ratio at each time interval. The byte hit ratio is measured in percentage.
         self.hit_rate_interval = hit_rate_interval  # type: DescribeDomainHitRateDataResponseBodyHitRateInterval
-        # The ID of the request.
         self.request_id = request_id  # type: str
-        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.hit_rate_interval:
             self.hit_rate_interval.validate()
 
     def to_map(self):
@@ -10986,33 +10859,31 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainHttpCodeDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, isp_name_en=None, location_name_en=None,
                  start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the total number and proportions of HTTP status codes returned from all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries the number and proportions of HTTP status codes for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
+        # The name of the region. You can call the DescribeCdnRegionAndIsp operation to query regions. If you do not specify this parameter, data in all regions is queried.
         self.isp_name_en = isp_name_en  # type: str
+        # The name of the Internet service provider (ISP). You can call the DescribeCdnRegionAndIsp operation to query ISPs. If you do not specify this parameter, data of all ISPs is queried.
         self.location_name_en = location_name_en  # type: str
-        # The start of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainHttpCodeDataRequest, self).to_map()
@@ -11049,17 +10920,17 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainHttpCodeDataResponseBodyHttpCodeDataUsageDataValueCodeProportionData(TeaModel):
     def __init__(self, code=None, count=None, proportion=None):
-        # The HTTP status code.
+        # The HTTP status code returned.
         self.code = code  # type: str
-        # The total number of HTTP status code returned.
+        # The count of each HTTP status code.
         self.count = count  # type: str
         # The proportion of the HTTP status code.
         self.proportion = proportion  # type: str
 
     def validate(self):
         pass
 
@@ -11118,17 +10989,17 @@
                 temp_model = DescribeDomainHttpCodeDataResponseBodyHttpCodeDataUsageDataValueCodeProportionData()
                 self.code_proportion_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainHttpCodeDataResponseBodyHttpCodeDataUsageData(TeaModel):
     def __init__(self, time_stamp=None, value=None):
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
-        # The proportions of HTTP status codes.
+        # The information about the HTTP status codes.
         self.value = value  # type: DescribeDomainHttpCodeDataResponseBodyHttpCodeDataUsageDataValue
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -11184,25 +11055,25 @@
                 self.usage_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainHttpCodeDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, http_code_data=None, request_id=None,
                  start_time=None):
-        # The interval at which the monitoring data is queried.
+        # The time interval.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The proportions of HTTP status codes at each time interval.
         self.http_code_data = http_code_data  # type: DescribeDomainHttpCodeDataResponseBodyHttpCodeData
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The beginning of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.http_code_data:
             self.http_code_data.validate()
 
     def to_map(self):
@@ -11501,23 +11372,19 @@
             temp_model = DescribeDomainHttpCodeDataByLayerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainISPDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
-        # The accelerated domain name. You can specify only one domain name in each call.
-        # 
-        # By default, this operation queries the proportions of data usage for all accelerated domain names.
+        # The beginning of the time range that was queried.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # The end time must be later than the start time.
+        # The accelerated domain name.
         self.end_time = end_time  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The ID of the request.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainISPDataRequest, self).to_map()
@@ -11544,37 +11411,41 @@
         return self
 
 
 class DescribeDomainISPDataResponseBodyValueISPProportionData(TeaModel):
     def __init__(self, avg_object_size=None, avg_response_rate=None, avg_response_time=None, bps=None,
                  bytes_proportion=None, isp=None, isp_ename=None, proportion=None, qps=None, req_err_rate=None, total_bytes=None,
                  total_query=None):
-        # The average response size. Unit: bytes.
+        # The name of the ISP.
         self.avg_object_size = avg_object_size  # type: str
-        # The average response speed. Unit: byte/ms.
+        # The bandwidth value.
         self.avg_response_rate = avg_response_rate  # type: str
-        # The average response time. Unit: milliseconds.
+        # The number of queries per second.
         self.avg_response_time = avg_response_time  # type: str
-        # The bandwidth value.
+        # The information about the ISP.
         self.bps = bps  # type: str
-        # The proportion of network traffic.
+        # The total amount of network traffic.
         self.bytes_proportion = bytes_proportion  # type: str
-        # The information about the ISP.
-        self.isp = isp  # type: str
         # The name of the ISP.
+        self.isp = isp  # type: str
+        # The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.  
+        # 
+        # > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        # - This operation queries proportions of data usage of different ISPs only for a specific accelerated domain name, or for all accelerated domain names that belong your Alibaba Cloud account.
+        # - You can call this operation up to 100 times per second per account.
         self.isp_ename = isp_ename  # type: str
-        # The proportion of the HTTP status code.
+        # The proportion of network traffic.
         self.proportion = proportion  # type: str
-        # The number of queries per second.
+        # chinanet
         self.qps = qps  # type: str
-        # The request error rate.
+        # The proportion of the HTTP status code.
         self.req_err_rate = req_err_rate  # type: str
-        # The total amount of network traffic.
+        # The average response size. Unit: bytes.
         self.total_bytes = total_bytes  # type: str
-        # The total number of requests.
+        # The request error rate.
         self.total_query = total_query  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainISPDataResponseBodyValueISPProportionData, self).to_map()
@@ -11668,25 +11539,25 @@
                 self.ispproportion_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainISPDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, request_id=None, start_time=None,
                  value=None):
-        # The time interval between the data entries. Unit: seconds.
+        # The average response speed. Unit: byte/ms.
         self.data_interval = data_interval  # type: str
-        # The accelerated domain name.
+        # The total amount of network traffic.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The time interval between the data entries. Unit: seconds.
         self.end_time = end_time  # type: str
-        # The ID of the request.
+        # The total number of requests.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
-        self.start_time = start_time  # type: str
         # The access statistics by ISP.
+        self.start_time = start_time  # type: str
+        # The average response time. Unit: milliseconds.
         self.value = value  # type: DescribeDomainISPDataResponseBodyValue
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -12005,24 +11876,19 @@
             temp_model = DescribeDomainMax95BpsDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainMultiUsageDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
-        # The accelerated domain names. You can specify multiple accelerated domain names and separate domain names with commas (,).
-        # 
-        # > *   You can specify at most 30 accelerated domain names.
-        # *   If you do not set this parameter, the data of all accelerated domain names that belong to your Alibaba Cloud account is queried.
+        # The beginning of the time range that was queried.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # >  The end time must be later than the start time.
+        # The information about requests collected every 5 minutes.
         self.end_time = end_time  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The ID of the request.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainMultiUsageDataRequest, self).to_map()
@@ -12047,23 +11913,27 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainMultiUsageDataResponseBodyRequestPerIntervalRequestDataModule(TeaModel):
     def __init__(self, domain=None, request=None, time_stamp=None, type=None):
-        # The information about the accelerated domain name.
+        # The accelerated domain name.
         self.domain = domain  # type: str
-        # The number of requests.
-        self.request = request  # type: long
         # The timestamp of the data returned.
-        self.time_stamp = time_stamp  # type: str
-        # The type of data returned.
+        self.request = request  # type: long
+        # The type of data returned. Valid values:
         # 
-        # >  For Alibaba Cloud CDN, the valid value is Simple.
+        # - **StaticHttps**: the number of HTTPS requests for static content.
+        # - **DynamicHttps**: the number of HTTPS requests for dynamic content.
+        # - **DynamicHttp**: the number of HTTP requests for dynamic content.
+        # - **StaticQuic**: the number of QUIC requests for static content.
+        # - **DynamicQuic**: the number of QUIC requests for dynamic content.
+        self.time_stamp = time_stamp  # type: str
+        # The statistics about data transfer collected every 5 minutes.
         self.type = type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainMultiUsageDataResponseBodyRequestPerIntervalRequestDataModule, self).to_map()
@@ -12124,29 +11994,29 @@
                 temp_model = DescribeDomainMultiUsageDataResponseBodyRequestPerIntervalRequestDataModule()
                 self.request_data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainMultiUsageDataResponseBodyTrafficPerIntervalTrafficDataModule(TeaModel):
     def __init__(self, area=None, bps=None, domain=None, time_stamp=None, type=None):
-        # The name of the district.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # >  The end time must be later than the start time.
         self.area = area  # type: str
-        # The bandwidth. Unit: bit/s.
+        # The timestamp of the data returned.
         self.bps = bps  # type: float
-        # The accelerated domain name.
+        # > *   If you do not set StartTime or EndTime, data collected within the last 10 minutes is queried.
+        # *   The maximum time range between StartTime and EndTime can be 1 hour.
+        # *   You can query data within the last 90 days.
+        # *   You can query the amount of data transfer and the number of requests for accelerated domain names that have been already removed from Alibaba Cloud CDN.
+        # *   The maximum number of times that each user can call this operation per second is 50.
         self.domain = domain  # type: str
-        # The timestamp of the data returned.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.time_stamp = time_stamp  # type: str
-        # The type of data returned. Valid values:
-        # 
-        # - **StaticHttps**: the number of HTTPS requests for static content.
-        # - **DynamicHttps**: the number of HTTPS requests for dynamic content.
-        # - **DynamicHttp**: the number of HTTP requests for dynamic content.
-        # - **StaticQuic**: the number of QUIC requests for static content.
-        # - **DynamicQuic**: the number of QUIC requests for dynamic content.
+        # The bandwidth. Unit: bit/s.
         self.type = type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainMultiUsageDataResponseBodyTrafficPerIntervalTrafficDataModule, self).to_map()
@@ -12212,23 +12082,25 @@
                 self.traffic_data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainMultiUsageDataResponseBody(TeaModel):
     def __init__(self, end_time=None, request_id=None, request_per_interval=None, start_time=None,
                  traffic_per_interval=None):
-        # The end of the time range that was queried.
+        # The type of data returned.
+        # 
+        # >  For Alibaba Cloud CDN, the valid value is Simple.
         self.end_time = end_time  # type: str
-        # The ID of the request.
+        # The information about the accelerated domain name.
         self.request_id = request_id  # type: str
-        # The information about requests collected every 5 minutes.
+        # The number of requests.
         self.request_per_interval = request_per_interval  # type: DescribeDomainMultiUsageDataResponseBodyRequestPerInterval
-        # The beginning of the time range that was queried.
+        # The timestamp of the data returned.
         self.start_time = start_time  # type: str
-        # The statistics about data transfer collected every 5 minutes.
+        # The name of the district.
         self.traffic_per_interval = traffic_per_interval  # type: DescribeDomainMultiUsageDataResponseBodyTrafficPerInterval
 
     def validate(self):
         if self.request_per_interval:
             self.request_per_interval.validate()
         if self.traffic_per_interval:
             self.traffic_per_interval.validate()
@@ -12548,21 +12420,19 @@
             temp_model = DescribeDomainPathDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainPvDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
-        # The accelerated domain name. You can specify only one domain name.
+        # The beginning of the time range during which data was queried.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # The end time must be later than the start time.
+        # The accelerated domain name.
         self.end_time = end_time  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The ID of the request.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainPvDataRequest, self).to_map()
@@ -12587,15 +12457,15 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainPvDataResponseBodyPvDataIntervalUsageData(TeaModel):
     def __init__(self, time_stamp=None, value=None):
-        # The timestamp of the returned data.
+        # The accelerated domain name. You can specify only one domain name.
         self.time_stamp = time_stamp  # type: str
         # The number of PVs.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
@@ -12651,25 +12521,28 @@
                 self.usage_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainPvDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, pv_data_interval=None, request_id=None,
                  start_time=None):
-        # The time interval between the data entries. Unit: seconds.
+        # The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.  
+        # 
+        # > - If you do not set StartTime or EndTime, monitoring data within the last 24 hours is queried. If you set both StartTime and EndTime, monitoring data within the specified time range is queried.
+        # - You can call this operation up to 50 times per second per account.
         self.data_interval = data_interval  # type: str
-        # The accelerated domain name.
+        # The timestamp of the returned data.
         self.domain_name = domain_name  # type: str
-        # The end of the time range during which data was queried.
+        # The time interval between the data entries. Unit: seconds.
         self.end_time = end_time  # type: str
-        # The number of PVs at each interval.
+        # The end of the time range during which data was queried.
         self.pv_data_interval = pv_data_interval  # type: DescribeDomainPvDataResponseBodyPvDataInterval
-        # The ID of the request.
+        # The number of PVs.
         self.request_id = request_id  # type: str
-        # The beginning of the time range during which data was queried.
+        # The number of PVs at each interval.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.pv_data_interval:
             self.pv_data_interval.validate()
 
     def to_map(self):
@@ -13681,49 +13554,44 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRealTimeDetailDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, field=None, isp_name_en=None, location_name_en=None,
                  merge=None, merge_loc_isp=None, start_time=None):
-        # The accelerated domain name for which you want to query data. You can specify multiple accelerated domain names and separate them with commas (,).
-        self.domain_name = domain_name  # type: str
-        # The end of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. Example: 2019-11-30T05:40:00Z.
-        # 
-        # >  The end time must be later than the start time. The time range between the end time and the start time cannot exceed 10 minutes.
-        self.end_time = end_time  # type: str
         # The metrics that you want to query. You can specify multiple metrics and separate them with commas (,). Valid values:
         # 
         # *   **qps**: the number of queries per second
         # *   **bps**: bandwidth values
         # *   **http_code**: HTTP status codes
-        self.field = field  # type: str
+        self.domain_name = domain_name  # type: str
         # The name of the Internet service provider. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs.
-        self.isp_name_en = isp_name_en  # type: str
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
-        self.location_name_en = location_name_en  # type: str
+        self.end_time = end_time  # type: str
         # Specifies whether to merge the results. Valid values:
         # 
         # *   **true**: merges the results.
         # *   **false**: does not merge the results. This is the default value.
         # 
         # Default value: **false**.
-        self.merge = merge  # type: str
+        self.field = field  # type: str
+        # The data usage of each ISP and the number of visits in each region.
+        self.isp_name_en = isp_name_en  # type: str
         # Specifies whether to merge the results. Valid values:
         # 
         # *   **true**: groups the results by domain name and merges the results by region and ISP.
         # *   **false**: groups the results by domain name.
         # 
         # Default value: **false**.
+        self.location_name_en = location_name_en  # type: str
+        # The ID of the request.
+        self.merge = merge  # type: str
+        # - You can query data within the last seven days. Data is collected every minute.
+        # - The maximum number of times that each user can call this operation per second is 10.
         self.merge_loc_isp = merge_loc_isp  # type: str
-        # The beginning of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. Example: 2019-11-30T05:33:00Z.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeDetailDataRequest, self).to_map()
@@ -13768,17 +13636,17 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainRealTimeDetailDataResponseBody(TeaModel):
     def __init__(self, data=None, request_id=None):
-        # The data usage of each ISP and the number of visits in each region.
+        # The name of the Internet service provider. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs.
         self.data = data  # type: str
-        # The ID of the request.
+        # The accelerated domain name for which you want to query data. You can specify multiple accelerated domain names and separate them with commas (,).
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeDetailDataResponseBody, self).to_map()
@@ -13838,31 +13706,18 @@
             temp_model = DescribeDomainRealTimeDetailDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRealTimeHttpCodeDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, isp_name_en=None, location_name_en=None, start_time=None):
-        # The accelerated domain name. You can specify multiple accelerated domain names and separate them with commas (,).
-        # 
-        # > You can specify up to 100 accelerated domain names in each request.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
         self.isp_name_en = isp_name_en  # type: str
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions. If you do not specify a region, all regions are queried.
         self.location_name_en = location_name_en  # type: str
-        # The beginning of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeHttpCodeDataRequest, self).to_map()
@@ -13895,19 +13750,16 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainRealTimeHttpCodeDataResponseBodyRealTimeHttpCodeDataUsageDataValueRealTimeCodeProportionData(TeaModel):
     def __init__(self, code=None, count=None, proportion=None):
-        # The HTTP status code returned.
         self.code = code  # type: str
-        # The total number of entries.
         self.count = count  # type: str
-        # The proportion of the HTTP status code.
         self.proportion = proportion  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeHttpCodeDataResponseBodyRealTimeHttpCodeDataUsageDataValueRealTimeCodeProportionData, self).to_map()
@@ -13964,17 +13816,15 @@
                 temp_model = DescribeDomainRealTimeHttpCodeDataResponseBodyRealTimeHttpCodeDataUsageDataValueRealTimeCodeProportionData()
                 self.real_time_code_proportion_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainRealTimeHttpCodeDataResponseBodyRealTimeHttpCodeDataUsageData(TeaModel):
     def __init__(self, time_stamp=None, value=None):
-        # The timestamp of the data returned.
         self.time_stamp = time_stamp  # type: str
-        # The proportions of the HTTP status codes.
         self.value = value  # type: DescribeDomainRealTimeHttpCodeDataResponseBodyRealTimeHttpCodeDataUsageDataValue
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -14030,27 +13880,19 @@
                 self.usage_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainRealTimeHttpCodeDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, real_time_http_code_data=None,
                  request_id=None, start_time=None):
-        # The time interval between the data entries returned. Unit: seconds.
-        # 
-        # Depending on the maximum time range per query, the value is 60 (1 minute), 300 (5 minutes), or 3600 (1 hour). For more information, see the "Time granularity" section in Usage notes.
         self.data_interval = data_interval  # type: str
-        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The proportions of HTTP status codes at each time interval.
         self.real_time_http_code_data = real_time_http_code_data  # type: DescribeDomainRealTimeHttpCodeDataResponseBodyRealTimeHttpCodeData
-        # The ID of the request.
         self.request_id = request_id  # type: str
-        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.real_time_http_code_data:
             self.real_time_http_code_data.validate()
 
     def to_map(self):
@@ -14324,21 +14166,19 @@
             temp_model = DescribeDomainRealTimeQpsDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRealTimeReqHitRateDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 100 domain names in each call.
+        # The response parameters.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # >  The end time must be later than the start time.
+        # The timestamp. The time follows the ISO 8601 standard. The time is displayed in UTC.
         self.end_time = end_time  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The request hit ratio.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeReqHitRateDataRequest, self).to_map()
@@ -14363,17 +14203,17 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainRealTimeReqHitRateDataResponseBodyDataReqHitRateDataModel(TeaModel):
     def __init__(self, req_hit_rate=None, time_stamp=None):
-        # The request hit ratio.
+        # You can specify multiple domain names and separate them with commas (,). You can specify at most 100 domain names in each call.
         self.req_hit_rate = req_hit_rate  # type: float
-        # The timestamp. The time follows the ISO 8601 standard. The time is displayed in UTC.
+        # The request hit ratio.
         self.time_stamp = time_stamp  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeReqHitRateDataResponseBodyDataReqHitRateDataModel, self).to_map()
@@ -14426,17 +14266,30 @@
                 temp_model = DescribeDomainRealTimeReqHitRateDataResponseBodyDataReqHitRateDataModel()
                 self.req_hit_rate_data_model.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainRealTimeReqHitRateDataResponseBody(TeaModel):
     def __init__(self, data=None, request_id=None):
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
         self.data = data  # type: DescribeDomainRealTimeReqHitRateDataResponseBodyData
-        # The ID of the request.
+        # 624461
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -14498,23 +14351,16 @@
             temp_model = DescribeDomainRealTimeReqHitRateDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRealTimeSrcBpsDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
-        # The accelerated domain name. You can specify up to 100 domain names in each request. Separate multiple domain names with commas (,).
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The beginning of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeSrcBpsDataRequest, self).to_map()
@@ -14539,17 +14385,15 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainRealTimeSrcBpsDataResponseBodyRealTimeSrcBpsDataPerIntervalDataModule(TeaModel):
     def __init__(self, time_stamp=None, value=None):
-        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
-        # The bandwidth during back-to-origin routing. Unit: bit/s.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeSrcBpsDataResponseBodyRealTimeSrcBpsDataPerIntervalDataModule, self).to_map()
@@ -14603,27 +14447,19 @@
                 self.data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainRealTimeSrcBpsDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None,
                  real_time_src_bps_data_per_interval=None, request_id=None, start_time=None):
-        # The time interval between the data entries returned. Unit: seconds.
-        # 
-        # The time granularity varies with the maximum time range per query. Valid values: 60 (1 minute), 300 (5 minutes), and 3600(1 hour). For more information, see **Usage notes**.
         self.data_interval = data_interval  # type: str
-        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The origin bandwidth data at each interval.
         self.real_time_src_bps_data_per_interval = real_time_src_bps_data_per_interval  # type: DescribeDomainRealTimeSrcBpsDataResponseBodyRealTimeSrcBpsDataPerInterval
-        # The ID of the request.
         self.request_id = request_id  # type: str
-        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.real_time_src_bps_data_per_interval:
             self.real_time_src_bps_data_per_interval.validate()
 
     def to_map(self):
@@ -14701,25 +14537,18 @@
             temp_model = DescribeDomainRealTimeSrcBpsDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRealTimeSrcHttpCodeDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, isp_name_en=None, location_name_en=None, start_time=None):
-        # The accelerated domain name. You can specify up to 100 domain names in each call. Separate multiple domain names with commas (,).
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you leave this parameter empty, all ISPs are queried.
         self.isp_name_en = isp_name_en  # type: str
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions. If you leave this parameter empty, all regions are queried.
         self.location_name_en = location_name_en  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeSrcHttpCodeDataRequest, self).to_map()
@@ -14752,19 +14581,16 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeDataUsageDataValueRealTimeSrcCodeProportionData(TeaModel):
     def __init__(self, code=None, count=None, proportion=None):
-        # The HTTP status code returned.
         self.code = code  # type: str
-        # The count of each HTTP status code.
         self.count = count  # type: str
-        # The proportion of the HTTP status code.
         self.proportion = proportion  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeDataUsageDataValueRealTimeSrcCodeProportionData, self).to_map()
@@ -14821,17 +14647,15 @@
                 temp_model = DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeDataUsageDataValueRealTimeSrcCodeProportionData()
                 self.real_time_src_code_proportion_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeDataUsageData(TeaModel):
     def __init__(self, time_stamp=None, value=None):
-        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
-        # The proportions of the HTTP status codes.
         self.value = value  # type: DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeDataUsageDataValue
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -14887,25 +14711,19 @@
                 self.usage_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainRealTimeSrcHttpCodeDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, real_time_src_http_code_data=None,
                  request_id=None, start_time=None):
-        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
-        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The proportions of HTTP status codes at each time interval.
         self.real_time_src_http_code_data = real_time_src_http_code_data  # type: DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeData
-        # The ID of the request.
         self.request_id = request_id  # type: str
-        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.real_time_src_http_code_data:
             self.real_time_src_http_code_data.validate()
 
     def to_map(self):
@@ -15409,15 +15227,15 @@
             temp_model = DescribeDomainRealTimeTrafficDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRealtimeLogDeliveryRequest(TeaModel):
     def __init__(self, domain=None):
-        # The accelerated domain name for which real-time log delivery is enabled. You can specify only one domain name.
+        # The ID of the request.
         self.domain = domain  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealtimeLogDeliveryRequest, self).to_map()
@@ -15434,26 +15252,19 @@
         if m.get('Domain') is not None:
             self.domain = m.get('Domain')
         return self
 
 
 class DescribeDomainRealtimeLogDeliveryResponseBody(TeaModel):
     def __init__(self, logstore=None, project=None, region=None, request_id=None, status=None):
-        # The name of the Logstore where log entries are stored.
         self.logstore = logstore  # type: str
-        # The name of the Log Service project that is used for real-time log delivery.
         self.project = project  # type: str
-        # The ID of the region where the Log Service project is deployed.
         self.region = region  # type: str
-        # The ID of the request.
         self.request_id = request_id  # type: str
-        # The status of real-time log delivery. Valid values:
-        # 
-        # *   **online**\
-        # *   **offline**\
+        # The ID of the region where the Log Service project is deployed.
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealtimeLogDeliveryResponseBody, self).to_map()
@@ -15525,23 +15336,19 @@
             temp_model = DescribeDomainRealtimeLogDeliveryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRegionDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).  
-        # 
-        # By default, this operation queries the geographic distribution of users for all accelerated domain names.
+        # The ID of the request.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.  
-        # 
-        # The end time must be later than the start time.
+        # The time interval between the data entries returned. Unit: seconds.
         self.end_time = end_time  # type: str
-        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The accelerated domain name.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRegionDataRequest, self).to_map()
@@ -15568,37 +15375,41 @@
         return self
 
 
 class DescribeDomainRegionDataResponseBodyValueRegionProportionData(TeaModel):
     def __init__(self, avg_object_size=None, avg_response_rate=None, avg_response_time=None, bps=None,
                  bytes_proportion=None, proportion=None, qps=None, region=None, region_ename=None, req_err_rate=None,
                  total_bytes=None, total_query=None):
-        # The average response size. Unit: bytes.
+        # cn-shenzhen
         self.avg_object_size = avg_object_size  # type: str
-        # The average response speed. Unit: bit/s.
+        # The number of queries per second.
         self.avg_response_rate = avg_response_rate  # type: str
-        # The average response time. Unit: milliseconds.
+        # The name of the region.
         self.avg_response_time = avg_response_time  # type: str
-        # The bandwidth.
+        # The proportion of visits from each region. For example, a value of 90 indicates that 90% of the visits are from the specified area.
         self.bps = bps  # type: str
-        # The proportion of bytes transferred from each region. For example, a value of 90 indicates that 90% of the bytes are transferred from the specified area.
+        # The accelerated domain name.
         self.bytes_proportion = bytes_proportion  # type: str
-        # The proportion of visits from each region. For example, a value of 90 indicates that 90% of the visits are from the specified area.
+        # The request error rate. A value of 90 indicates that 90% of the requests encountered errors.
         self.proportion = proportion  # type: str
-        # The number of queries per second.
+        # The proportion of bytes transferred from each region. For example, a value of 90 indicates that 90% of the bytes are transferred from the specified area.
         self.qps = qps  # type: str
-        # The information of the regions.
+        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.region = region  # type: str
-        # The name of the region.
+        # The statistical analytics feature of Alibaba Cloud CDN is discontinued. The API operations related to the statistical analytics feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.  
+        # 
+        # > - If you do not set **StartTime** or **EndTime**, data collected within the last **24** hours is queried. If you set both **StartTime** and **EndTime**, data collected within the specified time range is queried.
+        # - You may fail to query the latest data. If you need to query data collected within the last day, we recommend that you query the data on the next day.
+        # - You can call this operation up to 100 times per second per account.
         self.region_ename = region_ename  # type: str
-        # The request error rate. A value of 90 indicates that 90% of the requests encountered errors.
+        # The information of the regions.
         self.req_err_rate = req_err_rate  # type: str
-        # The total traffic. Unit: bytes.
+        # The bandwidth.
         self.total_bytes = total_bytes  # type: str
-        # The total number of requests.
+        # The average response size. Unit: bytes.
         self.total_query = total_query  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRegionDataResponseBodyValueRegionProportionData, self).to_map()
@@ -15692,25 +15503,25 @@
                 self.region_proportion_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainRegionDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, request_id=None, start_time=None,
                  value=None):
-        # The time interval between the data entries returned. Unit: seconds.
+        # The average response time. Unit: milliseconds.
         self.data_interval = data_interval  # type: str
-        # The accelerated domain name.
+        # The average response speed. Unit: bit/s.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The proportions of requests initiated from each area.
         self.end_time = end_time  # type: str
-        # The ID of the request.
+        # The total traffic. Unit: bytes.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The total number of requests.
         self.start_time = start_time  # type: str
-        # The proportions of requests initiated from each area.
+        # The request error rate. A value of 90 indicates that 90% of the requests encountered errors.
         self.value = value  # type: DescribeDomainRegionDataResponseBodyValue
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -16715,28 +16526,21 @@
             temp_model = DescribeDomainSrcQpsDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainSrcTopUrlVisitRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, sort_by=None, start_time=None):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
+        # The number of visits to the URL.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # >  The end time must be later than the start time. The difference between the end time and the start time cannot exceed seven days.
+        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
         self.end_time = end_time  # type: str
-        # The method that is used to sort the returned URLs.**** Valid values:
-        # 
-        # *   **traf**: by network traffic.
-        # *   **pv**: by the number of page views. This is the default value.
+        # A list of frequently requested URLs.
         self.sort_by = sort_by  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # >  If you do not set the StartTime parameter, the data within the previous day is queried.
+        # The operation that you want to perform. Set the value to **DescribeDomainSrcTopUrlVisit**.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainSrcTopUrlVisitRequest, self).to_map()
@@ -16765,23 +16569,26 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainSrcTopUrlVisitResponseBodyAllUrlListUrlList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, url_detail=None, visit_data=None, visit_proportion=None):
-        # The amount of network traffic. Unit: bytes.
-        self.flow = flow  # type: str
         # The proportion of network traffic consumed to access the URL.
-        self.flow_proportion = flow_proportion  # type: float
+        self.flow = flow  # type: str
         # The complete URL.
+        self.flow_proportion = flow_proportion  # type: float
+        # The amount of network traffic. Unit: bytes.
         self.url_detail = url_detail  # type: str
-        # The number of visits to the URL.
+        # The beginning of the time range that was queried.
         self.visit_data = visit_data  # type: str
-        # The proportion of visits to the URL.
+        # The method that is used to sort the returned URLs.**** Valid values:
+        # 
+        # *   **traf**: by network traffic.
+        # *   **pv**: by the number of page views. This is the default value.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainSrcTopUrlVisitResponseBodyAllUrlListUrlList, self).to_map()
@@ -16846,23 +16653,19 @@
                 temp_model = DescribeDomainSrcTopUrlVisitResponseBodyAllUrlListUrlList()
                 self.url_list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainSrcTopUrlVisitResponseBodyUrl200ListUrlList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, url_detail=None, visit_data=None, visit_proportion=None):
-        # The amount of network traffic. Unit: bytes.
+        # Queries frequently requested back-to-origin URLs of one or more accelerated domain names.
         self.flow = flow  # type: str
-        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion  # type: float
-        # The complete URL.
         self.url_detail = url_detail  # type: str
-        # The number of visits to the URL.
         self.visit_data = visit_data  # type: str
-        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainSrcTopUrlVisitResponseBodyUrl200ListUrlList, self).to_map()
@@ -16927,23 +16730,18 @@
                 temp_model = DescribeDomainSrcTopUrlVisitResponseBodyUrl200ListUrlList()
                 self.url_list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainSrcTopUrlVisitResponseBodyUrl300ListUrlList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, url_detail=None, visit_data=None, visit_proportion=None):
-        # The amount of network traffic. Unit: bytes.
         self.flow = flow  # type: str
-        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion  # type: float
-        # The complete URL.
         self.url_detail = url_detail  # type: str
-        # The number of visits to the URL.
         self.visit_data = visit_data  # type: str
-        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainSrcTopUrlVisitResponseBodyUrl300ListUrlList, self).to_map()
@@ -17008,23 +16806,18 @@
                 temp_model = DescribeDomainSrcTopUrlVisitResponseBodyUrl300ListUrlList()
                 self.url_list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainSrcTopUrlVisitResponseBodyUrl400ListUrlList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, url_detail=None, visit_data=None, visit_proportion=None):
-        # The amount of network traffic. Unit: bytes.
         self.flow = flow  # type: str
-        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion  # type: float
-        # The complete URL.
         self.url_detail = url_detail  # type: str
-        # The number of visits to the URL.
         self.visit_data = visit_data  # type: str
-        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainSrcTopUrlVisitResponseBodyUrl400ListUrlList, self).to_map()
@@ -17089,23 +16882,18 @@
                 temp_model = DescribeDomainSrcTopUrlVisitResponseBodyUrl400ListUrlList()
                 self.url_list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainSrcTopUrlVisitResponseBodyUrl500ListUrlList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, url_detail=None, visit_data=None, visit_proportion=None):
-        # The network traffic consumed to visit the URL, in bytes.
         self.flow = flow  # type: str
-        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion  # type: float
-        # The complete URL.
         self.url_detail = url_detail  # type: str
-        # The number of visits to the URL.
         self.visit_data = visit_data  # type: str
-        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainSrcTopUrlVisitResponseBodyUrl500ListUrlList, self).to_map()
@@ -17171,29 +16959,30 @@
                 self.url_list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainSrcTopUrlVisitResponseBody(TeaModel):
     def __init__(self, all_url_list=None, domain_name=None, request_id=None, start_time=None, url_200list=None,
                  url_300list=None, url_400list=None, url_500list=None):
-        # A list of frequently requested URLs.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # >  The end time must be later than the start time. The difference between the end time and the start time cannot exceed seven days.
         self.all_url_list = all_url_list  # type: DescribeDomainSrcTopUrlVisitResponseBodyAllUrlList
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The ID of the request.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # >  If you do not set the StartTime parameter, the data within the previous day is queried.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The proportion of visits to the URL.
         self.start_time = start_time  # type: str
-        # A list of URLs for which 2xx status codes were returned.
+        # The ID of the request.
         self.url_200list = url_200list  # type: DescribeDomainSrcTopUrlVisitResponseBodyUrl200List
-        # A list of URLs for which 3xx status codes were returned.
         self.url_300list = url_300list  # type: DescribeDomainSrcTopUrlVisitResponseBodyUrl300List
-        # A list of URLs for which 4xx status codes were returned.
         self.url_400list = url_400list  # type: DescribeDomainSrcTopUrlVisitResponseBodyUrl400List
-        # A list of URLs for which 5xx status codes were returned.
         self.url_500list = url_500list  # type: DescribeDomainSrcTopUrlVisitResponseBodyUrl500List
 
     def validate(self):
         if self.all_url_list:
             self.all_url_list.validate()
         if self.url_200list:
             self.url_200list.validate()
@@ -17511,36 +17300,32 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainTopClientIpVisitRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, limit=None, location_name_en=None, sort_by=None,
                  start_time=None):
-        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
-        # 
-        # By default, this operation queries client IP addresses for all accelerated domain names.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # The end time must be later than the start time.
-        self.end_time = end_time  # type: str
         # The maximum number of entries to return. Maximum value: 100.
         # 
         # Default value: 20. The default value 20 specifies that the top 20 data entries are returned.
+        self.end_time = end_time  # type: str
+        # A list of client IP addresses.
         self.limit = limit  # type: str
-        # The name of the region. Separate multiple region names with commas (,).
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
+        # The end time must be later than the start time.
         self.location_name_en = location_name_en  # type: str
+        # The ID of the request.
+        self.sort_by = sort_by  # type: str
         # The method that is used to sort the client IP addresses. Valid values:
         # 
         # *   **traf**: by network traffic. This is the default value.
         # *   **acc**: by the number of requests.
-        self.sort_by = sort_by  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainTopClientIpVisitRequest, self).to_map()
@@ -17577,21 +17362,25 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainTopClientIpVisitResponseBodyClientIpList(TeaModel):
     def __init__(self, acc=None, client_ip=None, rank=None, traffic=None):
-        # The total number of requests.
+        # The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.  
+        # 
+        # > - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        # - Data is collected every hour.
+        # - You can call this operation up to 10 times per second per account.
         self.acc = acc  # type: long
-        # The client IP address returned. Only IPv4 addressed are supported.
+        # The total amount of network traffic consumed. Unit: bytes.
         self.client_ip = client_ip  # type: str
-        # The ranking of the client IP address returned.
+        # The total number of requests.
         self.rank = rank  # type: int
-        # The total amount of network traffic consumed. Unit: bytes.
+        # The total number of requests.
         self.traffic = traffic  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainTopClientIpVisitResponseBodyClientIpList, self).to_map()
@@ -17620,17 +17409,17 @@
         if m.get('Traffic') is not None:
             self.traffic = m.get('Traffic')
         return self
 
 
 class DescribeDomainTopClientIpVisitResponseBody(TeaModel):
     def __init__(self, client_ip_list=None, request_id=None):
-        # A list of client IP addresses.
+        # The client IP address returned. Only IPv4 addressed are supported.
         self.client_ip_list = client_ip_list  # type: list[DescribeDomainTopClientIpVisitResponseBodyClientIpList]
-        # The ID of the request.
+        # The ranking of the client IP address returned.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.client_ip_list:
             for k in self.client_ip_list:
                 if k:
                     k.validate()
@@ -17698,26 +17487,21 @@
             temp_model = DescribeDomainTopClientIpVisitResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainTopReferVisitRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, sort_by=None, start_time=None):
-        # The accelerated domain names. Separate multiple accelerated domain names with commas (,).
+        # The beginning of the time range that was queried.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # The end time must be later than the start time.
+        # The accelerated domain name.
         self.end_time = end_time  # type: str
-        # The sorting method. Valid values:
-        # 
-        # *   **traf**: by network traffic.
-        # *   **pv**: by the number of page views. This is the default value.
+        # The most frequently requested web pages.
         self.sort_by = sort_by  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The ID of the request.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainTopReferVisitRequest, self).to_map()
@@ -17746,23 +17530,29 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainTopReferVisitResponseBodyTopReferListReferList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, refer_detail=None, visit_data=None, visit_proportion=None):
-        # The amount of network traffic. Unit: bytes.
+        # The proportion of visits to the web page.
         self.flow = flow  # type: str
-        # The proportion of the amount of network traffic consumed for visiting the web page.
+        # The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to analyze data.  
+        # 
+        # > - If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
+        # - Data is collected at an interval of five minutes.
+        # - You can call this operation up to 10 times per second per account.
         self.flow_proportion = flow_proportion  # type: float
-        # The URLs to the most frequently requested web pages.
+        # The accelerated domain name.
         self.refer_detail = refer_detail  # type: str
-        # The number of visits to the web page.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.visit_data = visit_data  # type: str
-        # The proportion of visits to the web page.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # The end time must be later than the start time.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainTopReferVisitResponseBodyTopReferListReferList, self).to_map()
@@ -17827,21 +17617,21 @@
                 temp_model = DescribeDomainTopReferVisitResponseBodyTopReferListReferList()
                 self.refer_list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainTopReferVisitResponseBody(TeaModel):
     def __init__(self, domain_name=None, request_id=None, start_time=None, top_refer_list=None):
-        # The accelerated domain name.
+        # The number of visits to the web page.
         self.domain_name = domain_name  # type: str
-        # The ID of the request.
+        # The proportion of the amount of network traffic consumed for visiting the web page.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The amount of network traffic. Unit: bytes.
         self.start_time = start_time  # type: str
-        # The most frequently requested web pages.
+        # The URLs to the most frequently requested web pages.
         self.top_refer_list = top_refer_list  # type: DescribeDomainTopReferVisitResponseBodyTopReferList
 
     def validate(self):
         if self.top_refer_list:
             self.top_refer_list.validate()
 
     def to_map(self):
@@ -18749,69 +18539,69 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainUsageDataRequest(TeaModel):
     def __init__(self, area=None, data_protocol=None, domain_name=None, end_time=None, field=None, interval=None,
                  start_time=None, type=None):
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
         self.area = area  # type: str
-        # The protocol of the data that you want to query. Default value: all. Valid values:
+        # The protocol of the data that you want to query. Valid values:
         # 
         # *   **http**: HTTP
         # *   **https**: HTTPS
         # *   **quic**: QUIC
-        # *   **all**: HTTP, HTTPS, and QUIC
+        # *   **all** (default): HTTP, HTTPS, and QUIC
         self.data_protocol = data_protocol  # type: str
         # The accelerated domain name. You can specify up to 100 domain names in each request. Separate multiple domain names with commas (,).
         # 
         # > If you leave this parameter empty, the usage data of all accelerated domain names in your Alibaba Cloud account is returned.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # > The end time must be later than the start time. The maximum time range that can be specified is 31 days.
         self.end_time = end_time  # type: str
-        # The type of data that you want to query. Valid values:
+        # The type of the data that you want to query. Valid values:
         # 
         # *   **bps**: bandwidth
         # *   **traf**: traffic
         # *   **acc**: requests
         # 
         # > If you set this parameter to **acc**, the **Area** parameter is not supported.
         self.field = field  # type: str
-        # The time interval between the data entries to return. Unit: seconds. Valid values: **300** (5 minutes), **3600** (1 hour), and **86400** (1 day).
+        # The time granularity of the data entries. Unit: seconds. Valid values: **300** (5 minutes), **3600** (1 hour), and **86400** (1 day).
         # 
-        # *   If **Interval** is set to **300**, you can query usage data in the last six months. The maximum time range per query that can be specified is three days.
+        # *   If **Interval** is set to **300**, you can query usage data in the last 6 months. The maximum time range per query that can be specified is 3 days.
         # *   If **Interval** is set to **3600** or **86400**, you can query usage data of the previous year.
-        # *   If you do not set the **Interval** parameter, the maximum time range that you can query is one month. If you specify a time range of 1 to 3 days, the time interval between the entries that are returned is 1 hour. If you specify a time range of at least 4 days, the time interval between the entries that are returned is 1 day.
+        # *   If you leave the **Interval** parameter empty, the maximum time range that you can query is 1 month. If you specify a time range of 1 to 3 days, the time interval between the entries that are returned is 1 hour. If you specify a time range of at least 4 days, the time interval between the entries that are returned is 1 day.
         self.interval = interval  # type: str
         # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # > Data is collected every 5 minutes.
         self.start_time = start_time  # type: str
-        # The type of content that you want to query. Default value: all. Valid values:
+        # The type of content that you want to query. Valid values:
         # 
         # *   **static**: static content
         # *   **dynamic**: dynamic content
-        # *   **all**: both static and dynamic content
+        # *   **all** (default): both static and dynamic content
         self.type = type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainUsageDataRequest, self).to_map()
@@ -18858,21 +18648,21 @@
         return self
 
 
 class DescribeDomainUsageDataResponseBodyUsageDataPerIntervalDataModule(TeaModel):
     def __init__(self, peak_time=None, special_value=None, time_stamp=None, value=None):
         # The time of the peak bandwidth value if the **Field** parameter in the request is set to **bps**. Otherwise, this parameter returns the same value as the **TimeStamp** parameter.
         self.peak_time = peak_time  # type: str
-        # The data usage in a specific scenario.
+        # The resource usage in a specific scenario.
         # 
         # > SpecialValue indicates the data usage in a specific scenario. If no special billable item is specified, ignore this parameter.
         self.special_value = special_value  # type: str
         # The timestamp of the data returned.
         # 
-        # > **TimeStamp** indicates the timestamp of the returned data at each interval.
+        # > **TimeStamp** indicates the timestamp of the data returned at each interval.
         self.time_stamp = time_stamp  # type: str
         # The amount of resource usage.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
@@ -18936,25 +18726,25 @@
                 self.data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainUsageDataResponseBody(TeaModel):
     def __init__(self, area=None, data_interval=None, domain_name=None, end_time=None, request_id=None,
                  start_time=None, type=None, usage_data_per_interval=None):
-        # The billable region where the data was collected.
+        # The ID of the billable region where the data was collected.
         self.area = area  # type: str
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
         # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The start of the time range during which data was queried.
+        # The beginning of the time range during which data was queried.
         self.start_time = start_time  # type: str
         # The type of content.
         self.type = type  # type: str
         # The resource usage that was collected at each interval.
         self.usage_data_per_interval = usage_data_per_interval  # type: DescribeDomainUsageDataResponseBodyUsageDataPerInterval
 
     def validate(self):
@@ -19245,15 +19035,15 @@
         return self
 
 
 class DescribeDomainsBySourceRequest(TeaModel):
     def __init__(self, owner_id=None, security_token=None, sources=None):
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
-        # The origin servers. Separate origin servers with commas (,). Fuzzy match is not supported.
+        # The origin servers. Separate multiple origin servers with commas (,). Fuzzy match is not supported.
         self.sources = sources  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainsBySourceRequest, self).to_map()
@@ -19281,35 +19071,34 @@
 
 
 class DescribeDomainsBySourceResponseBodyDomainsListDomainsDataDomainInfosDomainInfo(TeaModel):
     def __init__(self, cdn_type=None, create_time=None, domain_cname=None, domain_name=None, status=None,
                  update_time=None):
         # The workload type of the accelerated domain name. Valid values:
         # 
-        # *   **web**: images and small files.
-        # *   **download**: large files.
-        # *   **video**: on-demand video and audio streaming.
+        # *   **web**: images and small files
+        # *   **download**: large files
+        # *   **video**: on-demand video and audio streaming
         self.cdn_type = cdn_type  # type: str
-        # The time when the domain name was added to Alibaba Cloud CDN.
+        # The creation time.
         self.create_time = create_time  # type: str
-        # The CNAME assigned to the domain name.
+        # The CNAME record assigned to the domain name.
         self.domain_cname = domain_cname  # type: str
         # The domain name.
         self.domain_name = domain_name  # type: str
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
         self.status = status  # type: str
-        # The time when the configuration was updated.
+        # The update time.
         self.update_time = update_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainsBySourceResponseBodyDomainsListDomainsDataDomainInfosDomainInfo, self).to_map()
@@ -19402,19 +19191,19 @@
         if m.get('domainNames') is not None:
             self.domain_names = m.get('domainNames')
         return self
 
 
 class DescribeDomainsBySourceResponseBodyDomainsListDomainsData(TeaModel):
     def __init__(self, domain_infos=None, domains=None, source=None):
-        # The detailed information about the domain name. The data is indicated by the domainInfo parameter. Data type: array.
+        # Information about the domain name.
         self.domain_infos = domain_infos  # type: DescribeDomainsBySourceResponseBodyDomainsListDomainsDataDomainInfos
-        # The domain names that correspond to each origin server. The domain name is indicated by the domainNames parameter.
+        # The domain names that correspond to each origin server.
         self.domains = domains  # type: DescribeDomainsBySourceResponseBodyDomainsListDomainsDataDomains
-        # An origin server.
+        # The origin server.
         self.source = source  # type: str
 
     def validate(self):
         if self.domain_infos:
             self.domain_infos.validate()
         if self.domains:
             self.domains.validate()
@@ -19476,15 +19265,15 @@
                 temp_model = DescribeDomainsBySourceResponseBodyDomainsListDomainsData()
                 self.domains_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainsBySourceResponseBody(TeaModel):
     def __init__(self, domains_list=None, request_id=None, sources=None):
-        # The domain names corresponding to each origin server. The data is indicated by the DomainsData parameter. Data type: array.
+        # The domain names corresponding to each origin server.
         self.domains_list = domains_list  # type: DescribeDomainsBySourceResponseBodyDomainsList
         # The ID of the request.
         self.request_id = request_id  # type: str
         # The origin servers.
         self.sources = sources  # type: str
 
     def validate(self):
@@ -19885,21 +19674,25 @@
             temp_model = DescribeDomainsUsageByDayResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeEsExceptionDataRequest(TeaModel):
     def __init__(self, end_time=None, rule_id=None, start_time=None):
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end of the time range to query.
         # 
-        # >  The end time must be later than the start time.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The ID of the script that you want to query. You can call the [DescribeCdnDomainConfigs](~~90924~~) operation to query script IDs.
+        # The script ID. You can call the [DescribeCdnDomainConfigs](~~90924~~) operation to query script IDs.
         self.rule_id = rule_id  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The beginning of the time range to query.
+        # 
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeEsExceptionDataRequest, self).to_map()
@@ -19924,14 +19717,15 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeEsExceptionDataResponseBodyContentsPoints(TeaModel):
     def __init__(self, points=None):
+        # The data points.
         self.points = points  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeEsExceptionDataResponseBodyContentsPoints, self).to_map()
@@ -19948,19 +19742,19 @@
         if m.get('Points') is not None:
             self.points = m.get('Points')
         return self
 
 
 class DescribeEsExceptionDataResponseBodyContents(TeaModel):
     def __init__(self, columns=None, name=None, points=None):
-        # The column names of the chart that shows the errors of the script and the time of each data entry.
+        # Information about the time column and the error column name.
         self.columns = columns  # type: list[str]
-        # The name of the chart that shows the errors of the script.
+        # The name of the table that shows the errors of the script.
         self.name = name  # type: str
-        # The value of each time and the column of each data entry.
+        # The time columns and error column names.
         self.points = points  # type: list[DescribeEsExceptionDataResponseBodyContentsPoints]
 
     def validate(self):
         if self.points:
             for k in self.points:
                 if k:
                     k.validate()
@@ -19993,15 +19787,15 @@
                 temp_model = DescribeEsExceptionDataResponseBodyContentsPoints()
                 self.points.append(temp_model.from_map(k))
         return self
 
 
 class DescribeEsExceptionDataResponseBody(TeaModel):
     def __init__(self, contents=None, request_id=None):
-        # The content of the script.
+        # The content of the script for which an error was reported.
         self.contents = contents  # type: list[DescribeEsExceptionDataResponseBodyContents]
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.contents:
             for k in self.contents:
@@ -20071,21 +19865,21 @@
             temp_model = DescribeEsExceptionDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeEsExecuteDataRequest(TeaModel):
     def __init__(self, end_time=None, rule_id=None, start_time=None):
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The ID of the script that you want to query. You can call the [DescribeCdnDomainConfigs](~~90924~~) operation to query script IDs.
+        # The ID of the rule. You can call the [DescribeCdnDomainConfigs](~~90924~~) operation to query script IDs.
         self.rule_id = rule_id  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeEsExecuteDataRequest, self).to_map()
@@ -20110,19 +19904,19 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeEsExecuteDataResponseBodyContents(TeaModel):
     def __init__(self, columns=None, name=None, points=None):
-        # The column names of the chart that shows the status of the script and the time of each data entry.
+        # The time and column names in the table that shows the status of the script.
         self.columns = columns  # type: list[str]
-        # The name of the chart that shows the status of the script.
+        # The name of the table that shows the status of the script.
         self.name = name  # type: str
-        # The value of each time and the column of each data entry.
+        # The list of timestamps and values in the corresponding columns of the table that shows the status of the script.
         self.points = points  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeEsExecuteDataResponseBodyContents, self).to_map()
@@ -20255,15 +20049,15 @@
 class DescribeFCTriggerResponseBodyFCTrigger(TeaModel):
     def __init__(self, event_meta_name=None, event_meta_version=None, notes=None, role_arn=None, source_arn=None,
                  trigger_arn=None):
         # The name of the event.
         self.event_meta_name = event_meta_name  # type: str
         # The version of the event.
         self.event_meta_version = event_meta_version  # type: str
-        # The remarks.
+        # The remarks of the Function Compute trigger.
         self.notes = notes  # type: str
         # The assigned Resource Access Management (RAM) role.
         self.role_arn = role_arn  # type: str
         # The resources and filters for event listening.
         self.source_arn = source_arn  # type: str
         # The trigger that corresponds to the Function Compute service.
         self.trigger_arn = trigger_arn  # type: str
@@ -20405,17 +20199,17 @@
         return self
 
 
 class DescribeIllegalUrlExportTaskResponseBody(TeaModel):
     def __init__(self, download_url=None, request_id=None, status=None):
         # The URL where you can download the file that contains invalid URLs. This parameter is valid only if the export task is successful.
         self.download_url = download_url  # type: str
-        # The ID of the request.
+        # The operation that you want to perform. Set the value to **DescribeIllegalUrlExportTask**.
         self.request_id = request_id  # type: str
-        # The status of the export task. A value of **complete** indicates that the task is successful.
+        # The ID of the request.
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeIllegalUrlExportTaskResponseBody, self).to_map()
@@ -20504,22 +20298,22 @@
         if m.get('IP') is not None:
             self.ip = m.get('IP')
         return self
 
 
 class DescribeIpInfoResponseBody(TeaModel):
     def __init__(self, cdn_ip=None, isp=None, isp_ename=None, region=None, region_ename=None, request_id=None):
-        # Indicates whether the specified IP address is assigned to an Alibaba Cloud CDN node.
+        # Indicates whether the IP address belongs to an Alibaba Cloud CDN POP.
         # 
-        # *   **True**: Yes
-        # *   **False**: No
+        # *   **True**\
+        # *   **False**\
         self.cdn_ip = cdn_ip  # type: str
-        # The Chinese name of the Internet service provider (ISP).
+        # The Chinese name of the ISP.
         self.isp = isp  # type: str
-        # The English name of the ISP.
+        # The English name of the Internet service provider (ISP).
         self.isp_ename = isp_ename  # type: str
         # The Chinese name of the region.
         self.region = region  # type: str
         # The English name of the region.
         self.region_ename = region_ename  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
@@ -20626,21 +20420,21 @@
         if m.get('Ips') is not None:
             self.ips = m.get('Ips')
         return self
 
 
 class DescribeIpStatusResponseBodyIpStatus(TeaModel):
     def __init__(self, ip=None, status=None):
-        # The IP address of the node.
+        # The IP address of the POP.
         self.ip = ip  # type: str
-        # The status. Valid values:
+        # The status.
         # 
-        # *   **nonali**: The node is not an Alibaba Cloud CDN edge node.
-        # *   **normal**: The node is an available Alibaba Cloud CDN edge node.
-        # *   **abnormal**: The node is an unavailable Alibaba Cloud CDN edge node.
+        # *   **nonali**: not an Alibaba Cloud CDN POP
+        # *   **normal**: an available Alibaba Cloud CDN POP
+        # *   **abnormal**: an unavailable Alibaba Cloud CDN POP
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeIpStatusResponseBodyIpStatus, self).to_map()
@@ -20661,15 +20455,15 @@
         if m.get('status') is not None:
             self.status = m.get('status')
         return self
 
 
 class DescribeIpStatusResponseBody(TeaModel):
     def __init__(self, ip_status=None, request_id=None):
-        # The status of the node IP addresses.
+        # The status of the IP addresses of the POPs.
         self.ip_status = ip_status  # type: list[DescribeIpStatusResponseBodyIpStatus]
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.ip_status:
             for k in self.ip_status:
@@ -21212,29 +21006,29 @@
             temp_model = DescribeRangeDataByLocateAndIspServiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRealtimeDeliveryAccRequest(TeaModel):
     def __init__(self, end_time=None, interval=None, log_store=None, project=None, start_time=None):
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # The end of the time range to query. The end time must be later than the start time.
+        # The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time interval between the data entries. Unit: seconds. The value varies based on the values of the **StartTime** and **EndTime** parameters. Valid values:
+        # The time granularity of the data entries. Unit: seconds. The value varies based on the values of the **StartTime** and **EndTime** parameters. Valid values:
         # 
         # *   If the time span between StartTime and EndTime is less than 3 days, valid values are **300**, **3600**, and **86400**. Default value: **300**.
-        # *   If the time span between StartTime and EndTime is from 3 to 31 days (31 days excluded), valid values are **3600** and **86400**. Default value: **3600**.
+        # *   If the time span between StartTime and EndTime is greater than or equal to 3 days and less than 31 days, valid values are **3600** and **86400**. Default value: **3600**.
         # *   If the time span between StartTime and EndTime is 31 days or longer, the valid value is **86400**. Default value: **86400**.
         self.interval = interval  # type: str
-        # The name of the Logstore that collects log data from Alibaba Cloud Content Delivery Network (CDN) in real time. By default, all Logstores are queried.
+        # The name of the Logstore that stores log data. If you do leave this parameter empty, real-time log deliveries of all Logstores are queried.
         self.log_store = log_store  # type: str
-        # The name of the Log Service project that is used for real-time log delivery. By default, all projects are queried.
+        # The name of the Log Service project that is used for real-time log delivery. If you do leave this parameter empty, real-time log deliveries of all projects are queried.
         self.project = project  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRealtimeDeliveryAccRequest, self).to_map()
@@ -21271,15 +21065,15 @@
 
 class DescribeRealtimeDeliveryAccResponseBodyReatTimeDeliveryAccDataAccData(TeaModel):
     def __init__(self, failed_num=None, success_num=None, time_stamp=None):
         # The number of failed attempts to deliver log data to Log Service.
         self.failed_num = failed_num  # type: int
         # The number of successful deliveries of log data to Log Service.
         self.success_num = success_num  # type: int
-        # The timestamp of the data.
+        # The timestamp of the data returned.
         self.time_stamp = time_stamp  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRealtimeDeliveryAccResponseBodyReatTimeDeliveryAccDataAccData, self).to_map()
@@ -21336,15 +21130,15 @@
                 temp_model = DescribeRealtimeDeliveryAccResponseBodyReatTimeDeliveryAccDataAccData()
                 self.acc_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeRealtimeDeliveryAccResponseBody(TeaModel):
     def __init__(self, reat_time_delivery_acc_data=None, request_id=None):
-        # The information about real-time log delivery.
+        # The statistics about real-time log deliveries.
         self.reat_time_delivery_acc_data = reat_time_delivery_acc_data  # type: DescribeRealtimeDeliveryAccResponseBodyReatTimeDeliveryAccData
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.reat_time_delivery_acc_data:
             self.reat_time_delivery_acc_data.validate()
@@ -21442,35 +21236,35 @@
 class DescribeRefreshQuotaResponseBody(TeaModel):
     def __init__(self, block_quota=None, block_remain=None, dir_quota=None, dir_remain=None,
                  ignore_params_quota=None, ignore_params_remain=None, preload_edge_quota=None, preload_edge_remain=None,
                  preload_quota=None, preload_remain=None, regex_quota=None, regex_remain=None, request_id=None, url_quota=None,
                  url_remain=None):
         # The maximum number of URLs and directories that can be blocked on the current day.
         self.block_quota = block_quota  # type: str
-        # The remaining number of URLs and directories that can be blocked on the current day.
+        # The remaining number of URLs that can be blocked on the current day.
         self.block_remain = block_remain  # type: str
         # The maximum number of directories that can be refreshed on the current day.
         self.dir_quota = dir_quota  # type: str
         # The remaining number of directories that can be refreshed on the current day.
         self.dir_remain = dir_remain  # type: str
         self.ignore_params_quota = ignore_params_quota  # type: str
         self.ignore_params_remain = ignore_params_remain  # type: str
-        # The maximum number of times that you can prefetch content to L1 nodes on the current day.
+        # The maximum number of times that you can prefetch content to L1 POPs on the current day.
         self.preload_edge_quota = preload_edge_quota  # type: str
-        # The remaining number of times that you can prefetch content to L1 nodes on the current day.
+        # The remaining number of times that you can prefetch content to L1 POPs on the current day.
         self.preload_edge_remain = preload_edge_remain  # type: str
-        # The maximum number of times that you can prefetch content to L2 nodes on the current day.
+        # The maximum number of times that you can prefetch content to L2 POPs on the current day.
         self.preload_quota = preload_quota  # type: str
-        # The remaining number of times that you can prefetch content to L2 nodes on the current day.
+        # The remaining number of times that you can prefetch content to L2 points of presence (POPs) on the current day.
         self.preload_remain = preload_remain  # type: str
-        # The maximum number of times that you can use regular expressions to refresh directories or URLs on the current day.
+        # The maximum number of URLs or directories that can be refreshed by using regular expressions on the current day.
         self.regex_quota = regex_quota  # type: str
-        # The remaining number of times that you can use regular expressions to refresh directories or URLs on the current day.
+        # The remaining number of URLs or directories that can be refreshed by using regular expressions on the current day.
         self.regex_remain = regex_remain  # type: str
-        # The ID of the request
+        # The ID of the request.
         self.request_id = request_id  # type: str
         # The maximum number of URLs that can be refreshed on the current day.
         self.url_quota = url_quota  # type: str
         # The remaining number of URLs that can be refreshed on the current day.
         self.url_remain = url_remain  # type: str
 
     def validate(self):
@@ -21586,19 +21380,20 @@
             temp_model = DescribeRefreshQuotaResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRefreshTaskByIdRequest(TeaModel):
     def __init__(self, task_id=None):
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
         self.task_id = task_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRefreshTaskByIdRequest, self).to_map()
@@ -21616,41 +21411,42 @@
             self.task_id = m.get('TaskId')
         return self
 
 
 class DescribeRefreshTaskByIdResponseBodyTasks(TeaModel):
     def __init__(self, creation_time=None, description=None, object_path=None, object_type=None, process=None,
                  status=None, task_id=None):
-        # The time when the task was created. The time is displayed in UTC.
+        # The path of the object refreshed by the refresh task.
         self.creation_time = creation_time  # type: str
-        # The error returned when the refresh or prefetch task failed. Valid values:
-        # 
-        # *   **Internal Error**: An internal error occurred.
-        # *   **Origin Timeout**: The response from the origin server timed out.
-        # *   **Origin Return StatusCode 5XX**: The origin server returned a 5XX error.
+        # The tasks.
         self.description = description  # type: str
-        # The path of the object refreshed by the refresh task.
-        self.object_path = object_path  # type: str
         # The type of the task. Valid values:
         # 
         # *   **file**: refreshes an individual file.
         # *   **directory**: refreshes files under the specified directory.
         # *   **preload**: prefetches an individual file.
         # *   **regex**: refreshes content based on a regular expression.
+        self.object_path = object_path  # type: str
+        # The ID of the task.
         self.object_type = object_type  # type: str
-        # The progress of the task, in percentage.
+        # > - You can query data within the last three days.
+        # - You can call this operation up to 30 times per second per account.
         self.process = process  # type: str
+        # The error returned when the refresh or prefetch task failed. Valid values:
+        # 
+        # *   **Internal Error**: An internal error occurred.
+        # *   **Origin Timeout**: The response from the origin server timed out.
+        # *   **Origin Return StatusCode 5XX**: The origin server returned a 5XX error.
+        self.status = status  # type: str
         # The status of the task. Valid values:
         # 
         # *   **Complete**: The task is complete.
         # *   **Pending**: The task is pending.
         # *   **Refreshing**: The task is running.
         # *   **Failed**: The task failed.
-        self.status = status  # type: str
-        # The ID of the task.
         self.task_id = task_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRefreshTaskByIdResponseBodyTasks, self).to_map()
@@ -21691,19 +21487,24 @@
         if m.get('TaskId') is not None:
             self.task_id = m.get('TaskId')
         return self
 
 
 class DescribeRefreshTaskByIdResponseBody(TeaModel):
     def __init__(self, request_id=None, tasks=None, total_count=None):
-        # The ID of the request.
+        # The type of the task. Valid values:
+        # 
+        # *   **file**: refreshes an individual file.
+        # *   **directory**: refreshes files under the specified directory.
+        # *   **preload**: prefetches an individual file.
+        # *   **regex**: refreshes content based on a regular expression.
         self.request_id = request_id  # type: str
-        # The tasks.
+        # The progress of the task, in percentage.
         self.tasks = tasks  # type: list[DescribeRefreshTaskByIdResponseBodyTasks]
-        # The total number of tasks.
+        # The time when the task was created. The time is displayed in UTC.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.tasks:
             for k in self.tasks:
                 if k:
                     k.validate()
@@ -21777,48 +21578,25 @@
         return self
 
 
 class DescribeRefreshTasksRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, object_path=None, object_type=None, owner_id=None,
                  page_number=None, page_size=None, resource_group_id=None, security_token=None, start_time=None, status=None,
                  task_id=None):
-        # The accelerated domain name. You can specify only one accelerated domain name in each call. By default, this operation queries the status of tasks for all accelerated domain names.
         self.domain_name = domain_name  # type: str
-        # The end time. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The path of the object. The path is used as a condition for exact matching.
         self.object_path = object_path  # type: str
-        # The type of the task. Valid values:
-        # 
-        # *   **file**: refreshes one or more files.
-        # *   **directory**: refreshes files in the specified directories.
-        # *   **regex**: refreshes content based on a regular expression.
-        # *   **preload**: prefetches one or more files.
-        # 
-        # > If you set the **DomainName** or **Status** parameter, you must also set the **ObjectType** parameter.
         self.object_type = object_type  # type: str
         self.owner_id = owner_id  # type: long
-        # The number of the page to return. Valid values: **1** to **100000**.
         self.page_number = page_number  # type: int
-        # The number of entries to return on each page. Default value: **20**. Maximum value: **100**. Valid values: **1** to **100**.
         self.page_size = page_size  # type: int
-        # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
         self.security_token = security_token  # type: str
-        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
-        # The status of the task. Valid values:
-        # 
-        # *   **Complete**: The task has completed.
-        # *   **Refreshing**: The task is in progress.
-        # *   **Failed**: The task failed.
         self.status = status  # type: str
-        # The ID of the task that you want to query.
         self.task_id = task_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRefreshTasksRequest, self).to_map()
@@ -21880,40 +21658,20 @@
             self.task_id = m.get('TaskId')
         return self
 
 
 class DescribeRefreshTasksResponseBodyTasksCDNTask(TeaModel):
     def __init__(self, creation_time=None, description=None, object_path=None, object_type=None, process=None,
                  status=None, task_id=None):
-        # The time when the task was created. The time is displayed in UTC.
         self.creation_time = creation_time  # type: str
-        # The type of the error returned when the refresh or prefetch task failed. Valid values:
-        # 
-        # *   **InternalError**: An internal error occurred.
-        # *   **OriginTimeout**: The response from the origin server timed out.
-        # *   **OriginReturnStatusCode 5XX**: The origin server returned a 5XX error.
         self.description = description  # type: str
-        # The URL of the object refreshed.
         self.object_path = object_path  # type: str
-        # The type of the task.
-        # 
-        # *   **file**: refreshes one or more files.
-        # *   **directory**: refreshes files in the specified directories.
-        # *   **regex**: refreshes content based on a regular expression.
-        # *   **preload**: prefetches one or more files.
         self.object_type = object_type  # type: str
-        # The progress of the task, in percentage.
         self.process = process  # type: str
-        # The status of the task. Valid values:
-        # 
-        # *   **Complete**: The task has completed.
-        # *   **Refreshing**: The task is in progress.
-        # *   **Failed**: The task failed.
         self.status = status  # type: str
-        # The ID of the task.
         self.task_id = task_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRefreshTasksResponseBodyTasksCDNTask, self).to_map()
@@ -21986,23 +21744,18 @@
                 temp_model = DescribeRefreshTasksResponseBodyTasksCDNTask()
                 self.cdntask.append(temp_model.from_map(k))
         return self
 
 
 class DescribeRefreshTasksResponseBody(TeaModel):
     def __init__(self, page_number=None, page_size=None, request_id=None, tasks=None, total_count=None):
-        # The page number of the returned page.
         self.page_number = page_number  # type: long
-        # The number of entries returned per page.
         self.page_size = page_size  # type: long
-        # The ID of the request.
         self.request_id = request_id  # type: str
-        # Details about tasks.
         self.tasks = tasks  # type: DescribeRefreshTasksResponseBodyTasks
-        # The total number of entries returned.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.tasks:
             self.tasks.validate()
 
     def to_map(self):
@@ -22100,17 +21853,17 @@
         if m.get('IPV4') is not None:
             self.ipv4 = m.get('IPV4')
         return self
 
 
 class DescribeStagingIpResponseBody(TeaModel):
     def __init__(self, ipv4s=None, request_id=None):
-        # The IPv4 addresses of the nodes.
-        self.ipv4s = ipv4s  # type: DescribeStagingIpResponseBodyIPV4s
         # The ID of the request.
+        self.ipv4s = ipv4s  # type: DescribeStagingIpResponseBodyIPV4s
+        # The IPv4 addresses of the nodes.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.ipv4s:
             self.ipv4s.validate()
 
     def to_map(self):
@@ -22172,17 +21925,15 @@
             temp_model = DescribeStagingIpResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeTagResourcesRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
-        # The key of the tag.
         self.key = key  # type: str
-        # The value of the tag.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTagResourcesRequestTag, self).to_map()
@@ -22203,19 +21954,16 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class DescribeTagResourcesRequest(TeaModel):
     def __init__(self, resource_id=None, resource_type=None, tag=None):
-        # The IDs of the resources. You can specify up to 50 IDs in each request.
         self.resource_id = resource_id  # type: list[str]
-        # The type of the resource. Set this value to **DOMAIN**.
         self.resource_type = resource_type  # type: str
-        # The tags. You can specify up to 20 tags in each request.
         self.tag = tag  # type: list[DescribeTagResourcesRequestTag]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -22248,17 +21996,15 @@
                 temp_model = DescribeTagResourcesRequestTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
 
 class DescribeTagResourcesResponseBodyTagResourcesTag(TeaModel):
     def __init__(self, key=None, value=None):
-        # The key of the tag.
         self.key = key  # type: str
-        # The value of the tag.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTagResourcesResponseBodyTagResourcesTag, self).to_map()
@@ -22279,17 +22025,15 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class DescribeTagResourcesResponseBodyTagResources(TeaModel):
     def __init__(self, resource_id=None, tag=None):
-        # The ID of the resource.
         self.resource_id = resource_id  # type: str
-        # The tags.
         self.tag = tag  # type: list[DescribeTagResourcesResponseBodyTagResourcesTag]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -22318,17 +22062,15 @@
                 temp_model = DescribeTagResourcesResponseBodyTagResourcesTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
 
 class DescribeTagResourcesResponseBody(TeaModel):
     def __init__(self, request_id=None, tag_resources=None):
-        # The ID of the request.
         self.request_id = request_id  # type: str
-        # Details about the tag.
         self.tag_resources = tag_resources  # type: list[DescribeTagResourcesResponseBodyTagResources]
 
     def validate(self):
         if self.tag_resources:
             for k in self.tag_resources:
                 if k:
                     k.validate()
@@ -22398,21 +22140,21 @@
         return self
 
 
 class DescribeTopDomainsByFlowRequest(TeaModel):
     def __init__(self, end_time=None, limit=None, start_time=None):
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
         # The maximum number of domain names to query. Valid values: **1** to **100**. Default value: **20**.
         self.limit = limit  # type: long
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  Set StartTime to UTC time in the yyyy-MM-ddTHH:mm:ssZ format. For example, if the local time is 00:00, June 1, 2021, set StartTime to 2021-05-31T16:00:00Z.
+        # > The value of StartTime must be in UTC. For example, if the local time is 00:00 on June 1, 2021, set StartTime to 2021-05-31T16:00:00Z.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTopDomainsByFlowRequest, self).to_map()
@@ -22446,19 +22188,19 @@
         self.domain_name = domain_name  # type: str
         # The peak bandwidth value.
         self.max_bps = max_bps  # type: float
         # The time when the bandwidth reached the peak value.
         self.max_bps_time = max_bps_time  # type: str
         # The ranking of the accelerated domain name.
         self.rank = rank  # type: long
-        # The number of visits to the accelerated domain name.
+        # The number of visits to the domain name.
         self.total_access = total_access  # type: long
-        # The total amount of network traffic.
+        # The total volume of traffic.
         self.total_traffic = total_traffic  # type: str
-        # The proportion of the amount of network traffic consumed for visiting the web page.
+        # The proportion of network traffic consumed to access the domain name.
         self.traffic_percent = traffic_percent  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTopDomainsByFlowResponseBodyTopDomainsTopDomain, self).to_map()
@@ -22540,15 +22282,15 @@
         self.domain_count = domain_count  # type: long
         # The total number of accelerated domain names that are in the **Enabled** state within the current Alibaba Cloud account.
         self.domain_online_count = domain_online_count  # type: long
         # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range during which data was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
         # The top N domain names ranked by network traffic.
         self.top_domains = top_domains  # type: DescribeTopDomainsByFlowResponseBodyTopDomains
 
     def validate(self):
         if self.top_domains:
             self.top_domains.validate()
@@ -22628,19 +22370,18 @@
             temp_model = DescribeTopDomainsByFlowResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeUserCertificateExpireCountResponseBody(TeaModel):
     def __init__(self, expire_within_30days_count=None, expired_count=None, request_id=None):
-        # The number of domain names whose SSL certificates are about to expire within 30 days.
+        # The ID of the request.
         self.expire_within_30days_count = expire_within_30days_count  # type: int
-        # The number of domain names whose SSL certificates have already expired.
         self.expired_count = expired_count  # type: int
-        # The ID of the request.
+        # The number of domain names whose SSL certificates have already expired.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeUserCertificateExpireCountResponseBody, self).to_map()
@@ -22704,14 +22445,15 @@
             temp_model = DescribeUserCertificateExpireCountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeUserConfigsRequest(TeaModel):
     def __init__(self, config=None, owner_id=None, security_token=None):
+        # The feature whose configurations you want to query. You can specify only one feature in each request. Valid values: oss, green_manager, waf, cc_rule, ddos_dispatch, edge_safe, blocked_regions, http_acl_policy, bot_manager, and ip_reputation.
         self.config = config  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
@@ -22738,16 +22480,19 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeUserConfigsResponseBodyConfigsOssLogConfig(TeaModel):
     def __init__(self, bucket=None, enable=None, prefix=None):
+        # The name of the bucket.
         self.bucket = bucket  # type: str
+        # Indicates whether the OSS bucket is enabled.
         self.enable = enable  # type: str
+        # The prefix.
         self.prefix = prefix  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeUserConfigsResponseBodyConfigsOssLogConfig, self).to_map()
@@ -22772,14 +22517,15 @@
         if m.get('Prefix') is not None:
             self.prefix = m.get('Prefix')
         return self
 
 
 class DescribeUserConfigsResponseBodyConfigsWafConfig(TeaModel):
     def __init__(self, enable=None):
+        # Indicates whether WAF is enabled.
         self.enable = enable  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeUserConfigsResponseBodyConfigsWafConfig, self).to_map()
@@ -22796,15 +22542,17 @@
         if m.get('Enable') is not None:
             self.enable = m.get('Enable')
         return self
 
 
 class DescribeUserConfigsResponseBodyConfigs(TeaModel):
     def __init__(self, oss_log_config=None, waf_config=None):
+        # The configurations of Object Storage Service (OSS).
         self.oss_log_config = oss_log_config  # type: DescribeUserConfigsResponseBodyConfigsOssLogConfig
+        # The configurations of Web Application Firewall (WAF).
         self.waf_config = waf_config  # type: DescribeUserConfigsResponseBodyConfigsWafConfig
 
     def validate(self):
         if self.oss_log_config:
             self.oss_log_config.validate()
         if self.waf_config:
             self.waf_config.validate()
@@ -22830,14 +22578,15 @@
             temp_model = DescribeUserConfigsResponseBodyConfigsWafConfig()
             self.waf_config = temp_model.from_map(m['WafConfig'])
         return self
 
 
 class DescribeUserConfigsResponseBody(TeaModel):
     def __init__(self, configs=None, request_id=None):
+        # The configurations of the specified feature.
         self.configs = configs  # type: DescribeUserConfigsResponseBodyConfigs
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.configs:
             self.configs.validate()
@@ -22901,19 +22650,19 @@
             temp_model = DescribeUserConfigsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeUserDomainsRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
-        # The key of the tag. Valid values of N: **1** to **20**.
+        # The key of a tag.
         # 
         # By default, all tag keys are queried.
         self.key = key  # type: str
-        # The value of the tag. Valid values of N: **1** to **20**.
+        # The value of the tag.
         # 
         # By default, all tag values are queried.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
@@ -22948,64 +22697,64 @@
         # *   **download**: large files
         # *   **video**: on-demand video and audio streaming
         # 
         # If you do not set this parameter, all service types are queried.
         self.cdn_type = cdn_type  # type: str
         # The end of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.change_end_time = change_end_time  # type: str
         # The beginning of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.change_start_time = change_start_time  # type: str
         # Specifies whether to display domain names that are under review, failed the review, or failed to be configured. Valid values:
         # 
-        # *   **true**: yes
-        # *   **false**: no
+        # *   **true**\
+        # *   **false**\
         self.check_domain_show = check_domain_show  # type: bool
-        # The accelerated region. By default, all accelerated regions are queried. Valid values:
+        # The acceleration region. By default, all acceleration regions are queried. Valid values:
         # 
         # *   **domestic**: Chinese mainland
-        # *   **global**\
-        # *   **overseas**: global (excluding the Chinese mainland)
+        # *   **global**: global
+        # *   **overseas**: outside the Chinese mainland
         self.coverage = coverage  # type: str
-        # The accelerated domain names. If you do not set this parameter, configurations of all domain names that match the conditions are returned.
+        # The accelerated domain. If you do not set this parameter, all domain names that match the conditions are returned.
         self.domain_name = domain_name  # type: str
         # The search mode. Valid values:
         # 
         # *   **fuzzy_match**: fuzzy match
         # *   **pre_match**: prefix match
         # *   **suf_match**: suffix match
         # *   **full_match** (default): exact match
         # 
-        # >  If you specify the domain names to query but do not set the DomainSearchType parameter, the exact match mode is used.
+        # > If you specify the domain names to query but do not set the DomainSearchType parameter, the exact match mode is used.
         self.domain_search_type = domain_search_type  # type: str
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
         self.domain_status = domain_status  # type: str
         self.owner_id = owner_id  # type: long
         # The number of the page to return. Valid values: **1** to **100000**.
         self.page_number = page_number  # type: int
         # The number of entries to return on each page. Valid values: **1 to 50**. Default value: **20**. Maximum value: **50**.
         self.page_size = page_size  # type: int
         # The ID of the resource group. By default, all IDs are queried.
         self.resource_group_id = resource_group_id  # type: str
         self.security_token = security_token  # type: str
         # The information about the origin server.
         self.source = source  # type: str
-        # The tags.
+        # The list of tags. Maximum number of elements in the list: 20
         self.tag = tag  # type: list[DescribeUserDomainsRequestTag]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -23090,19 +22839,19 @@
 
 class DescribeUserDomainsResponseBodyDomainsPageDataSourcesSource(TeaModel):
     def __init__(self, content=None, port=None, priority=None, type=None, weight=None):
         # The address of the origin server.
         self.content = content  # type: str
         # The port of the origin server.
         self.port = port  # type: int
-        # The priority of the origin server.
+        # The priority.
         self.priority = priority  # type: str
         # The type of the origin server.
         self.type = type  # type: str
-        # The weight of the origin server if multiple origin servers are specified.
+        # The weight of the origin server if multiple origin servers have been specified.
         self.weight = weight  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeUserDomainsResponseBodyDomainsPageDataSourcesSource, self).to_map()
@@ -23169,59 +22918,59 @@
         return self
 
 
 class DescribeUserDomainsResponseBodyDomainsPageData(TeaModel):
     def __init__(self, cdn_type=None, cname=None, coverage=None, description=None, domain_id=None, domain_name=None,
                  domain_status=None, gmt_created=None, gmt_modified=None, resource_group_id=None, sandbox=None, sources=None,
                  ssl_protocol=None):
-        # The type of workload accelerated by Alibaba Cloud CDN. Valid values:
+        # The type of the workload accelerated by Alibaba Cloud CDN. Valid values:
         # 
         # *   **web**: images and small files
         # *   **download**: large files
         # *   **video**: on-demand video and audio streaming
         self.cdn_type = cdn_type  # type: str
         # The CNAME assigned to the accelerated domain name.
         self.cname = cname  # type: str
         # The acceleration region. Valid values:
         # 
         # *   **domestic**: Chinese mainland
-        # *   **global**\
-        # *   **overseas**: global (excluding the Chinese mainland)
+        # *   **global**: global
+        # *   **overseas**: outside the Chinese mainland
         self.coverage = coverage  # type: str
-        # The information about the Internet Content Provider (ICP) number.
+        # The information about Internet Content Provider (ICP) filing.
         self.description = description  # type: str
         # The ID of the accelerated domain name.
         self.domain_id = domain_id  # type: long
-        # The accelerated domain names.
+        # The accelerated domain.
         self.domain_name = domain_name  # type: str
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
         self.domain_status = domain_status  # type: str
-        # The time when the accelerated domain name was added to Alibaba Cloud CDN.
+        # The time when the accelerated domain name was added.
         self.gmt_created = gmt_created  # type: str
-        # The time when the accelerated domain name was last modified.
+        # The time when the accelerated domain name was modified.
         self.gmt_modified = gmt_modified  # type: str
         # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
         # Indicates whether the accelerated domain name is in a sandbox.
         self.sandbox = sandbox  # type: str
         # The information about the origin server.
         self.sources = sources  # type: DescribeUserDomainsResponseBodyDomainsPageDataSources
         # Indicates whether HTTPS is enabled. Valid values:
         # 
-        # *   **on**: enabled
-        # *   **off**: disabled
+        # *   **on**\
+        # *   **off**\
         self.ssl_protocol = ssl_protocol  # type: str
 
     def validate(self):
         if self.sources:
             self.sources.validate()
 
     def to_map(self):
@@ -23320,23 +23069,23 @@
                 temp_model = DescribeUserDomainsResponseBodyDomainsPageData()
                 self.page_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeUserDomainsResponseBody(TeaModel):
     def __init__(self, domains=None, page_number=None, page_size=None, request_id=None, total_count=None):
-        # The information about the accelerated domain name.
+        # The list of the accelerated domain names returned.
         self.domains = domains  # type: DescribeUserDomainsResponseBodyDomains
         # The page number of the returned page.
         self.page_number = page_number  # type: long
         # The number of entries returned per page.
         self.page_size = page_size  # type: long
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # Indicates the total number of entries returned.
+        # The total number of entries returned.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.domains:
             self.domains.validate()
 
     def to_map(self):
@@ -23410,17 +23159,17 @@
             temp_model = DescribeUserDomainsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeUserTagsResponseBodyTags(TeaModel):
     def __init__(self, key=None, value=None):
-        # The key of the tag.
+        # The value of the tag.
         self.key = key  # type: str
-        # The list of tag value.
+        # The ID of the request.
         self.value = value  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeUserTagsResponseBodyTags, self).to_map()
@@ -23441,17 +23190,17 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class DescribeUserTagsResponseBody(TeaModel):
     def __init__(self, request_id=None, tags=None):
-        # The ID of the request.
-        self.request_id = request_id  # type: str
         # The list of tags returned.
+        self.request_id = request_id  # type: str
+        # The key of the tag.
         self.tags = tags  # type: list[DescribeUserTagsResponseBodyTags]
 
     def validate(self):
         if self.tags:
             for k in self.tags:
                 if k:
                     k.validate()
@@ -23519,19 +23268,17 @@
             temp_model = DescribeUserTagsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeUserUsageDataExportTaskRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None):
-        # The number of the page to return. Valid values: **1** to **100000**.
+        # The name of the task.
         self.page_number = page_number  # type: str
-        # The number of entries to return on each page. Default value: **20**. Maximum value: **50**.
-        # 
-        # Valid values: **1** to **50**.
+        # The usage details returned per page.
         self.page_size = page_size  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeUserUsageDataExportTaskRequest, self).to_map()
@@ -23552,17 +23299,17 @@
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         return self
 
 
 class DescribeUserUsageDataExportTaskResponseBodyUsageDataPerPageDataDataItemTaskConfig(TeaModel):
     def __init__(self, end_time=None, start_time=None):
-        # The end of the time range that was queried.
+        # The ID of the request.
         self.end_time = end_time  # type: str
-        # The start of the time range that was queried.
+        # The last time when the task was modified.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeUserUsageDataExportTaskResponseBodyUsageDataPerPageDataDataItemTaskConfig, self).to_map()
@@ -23584,31 +23331,29 @@
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeUserUsageDataExportTaskResponseBodyUsageDataPerPageDataDataItem(TeaModel):
     def __init__(self, create_time=None, download_url=None, status=None, task_config=None, task_id=None,
                  task_name=None, update_time=None):
-        # The time when the task was created.
-        self.create_time = create_time  # type: str
         # The download URL.
+        self.create_time = create_time  # type: str
+        # The configurations of the task.
         self.download_url = download_url  # type: str
-        # The status of the task.
-        # 
-        # *   created: The task is being created.
-        # *   success: The task has been created.
-        # *   failed: The creation of the task failed.
+        # The time when the task was created.
         self.status = status  # type: str
-        # The configurations of the task.
+        # The total number of entries returned.
         self.task_config = task_config  # type: DescribeUserUsageDataExportTaskResponseBodyUsageDataPerPageDataDataItemTaskConfig
-        # The ID of the task.
+        # The number of the current page.
         self.task_id = task_id  # type: str
-        # The name of the task.
+        # The number of entries to return on each page. Default value: **20**. Maximum value: **50**.
+        # 
+        # Valid values: **1** to **50**.
         self.task_name = task_name  # type: str
-        # The last time when the task was modified.
+        # The operation that you want to perform. Set the value to **DescribeUserUsageDataExportTask**.
         self.update_time = update_time  # type: str
 
     def validate(self):
         if self.task_config:
             self.task_config.validate()
 
     def to_map(self):
@@ -23683,21 +23428,25 @@
                 temp_model = DescribeUserUsageDataExportTaskResponseBodyUsageDataPerPageDataDataItem()
                 self.data_item.append(temp_model.from_map(k))
         return self
 
 
 class DescribeUserUsageDataExportTaskResponseBodyUsageDataPerPage(TeaModel):
     def __init__(self, data=None, page_number=None, page_size=None, total_count=None):
-        # The description of the task.
+        # The status of the task.
+        # 
+        # *   created: The task is being created.
+        # *   success: The task has been created.
+        # *   failed: The creation of the task failed.
         self.data = data  # type: DescribeUserUsageDataExportTaskResponseBodyUsageDataPerPageData
-        # The number of the current page.
+        # The number of the page to return. Valid values: **1** to **100000**.
         self.page_number = page_number  # type: int
-        # The number of entries returned per page.
+        # The description of the task.
         self.page_size = page_size  # type: int
-        # The total number of entries returned.
+        # The start of the time range that was queried.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -23728,17 +23477,17 @@
         if m.get('TotalCount') is not None:
             self.total_count = m.get('TotalCount')
         return self
 
 
 class DescribeUserUsageDataExportTaskResponseBody(TeaModel):
     def __init__(self, request_id=None, usage_data_per_page=None):
-        # The ID of the request.
+        # The ID of the task.
         self.request_id = request_id  # type: str
-        # The usage details returned per page.
+        # The end of the time range that was queried.
         self.usage_data_per_page = usage_data_per_page  # type: DescribeUserUsageDataExportTaskResponseBodyUsageDataPerPage
 
     def validate(self):
         if self.usage_data_per_page:
             self.usage_data_per_page.validate()
 
     def to_map(self):
@@ -23800,19 +23549,17 @@
             temp_model = DescribeUserUsageDataExportTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeUserUsageDetailDataExportTaskRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None):
-        # The number of the page to return. Valid values: **1** to **100000**.
+        # The name of the task.
         self.page_number = page_number  # type: str
-        # The number of entries to return on each page. Default value: **20**. Maximum value: **50**.
-        # 
-        # Valid values: **1** to **50**.
+        # The usage details returned per page.
         self.page_size = page_size  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeUserUsageDetailDataExportTaskRequest, self).to_map()
@@ -23833,17 +23580,17 @@
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         return self
 
 
 class DescribeUserUsageDetailDataExportTaskResponseBodyUsageDataPerPageDataDataItemTaskConfig(TeaModel):
     def __init__(self, end_time=None, start_time=None):
-        # The end of the time range that was queried.
+        # refresh
         self.end_time = end_time  # type: str
-        # The start of the time range that was queried.
+        # The ID of the request.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeUserUsageDetailDataExportTaskResponseBodyUsageDataPerPageDataDataItemTaskConfig, self).to_map()
@@ -23865,27 +23612,29 @@
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeUserUsageDetailDataExportTaskResponseBodyUsageDataPerPageDataDataItem(TeaModel):
     def __init__(self, create_time=None, download_url=None, status=None, task_config=None, task_id=None,
                  task_name=None, update_time=None):
-        # The time when the task was created.
-        self.create_time = create_time  # type: str
         # The download URL.
+        self.create_time = create_time  # type: str
+        # The configurations of the task.
         self.download_url = download_url  # type: str
-        # The status of the task.
+        # The time when the task was created.
         self.status = status  # type: str
-        # The configurations of the task.
+        # The total number of entries returned.
         self.task_config = task_config  # type: DescribeUserUsageDetailDataExportTaskResponseBodyUsageDataPerPageDataDataItemTaskConfig
-        # The ID of the task.
+        # The number of the page returned.
         self.task_id = task_id  # type: str
-        # The name of the task.
+        # The number of entries to return on each page. Default value: **20**. Maximum value: **50**.
+        # 
+        # Valid values: **1** to **50**.
         self.task_name = task_name  # type: str
-        # The last time when the task was modified.
+        # The operation that you want to perform. Set the value to **DescribeUserUsageDetailDataExportTask**.
         self.update_time = update_time  # type: str
 
     def validate(self):
         if self.task_config:
             self.task_config.validate()
 
     def to_map(self):
@@ -23960,21 +23709,21 @@
                 temp_model = DescribeUserUsageDetailDataExportTaskResponseBodyUsageDataPerPageDataDataItem()
                 self.data_item.append(temp_model.from_map(k))
         return self
 
 
 class DescribeUserUsageDetailDataExportTaskResponseBodyUsageDataPerPage(TeaModel):
     def __init__(self, data=None, page_number=None, page_size=None, total_count=None):
-        # The description of the task.
+        # The status of the task.
         self.data = data  # type: DescribeUserUsageDetailDataExportTaskResponseBodyUsageDataPerPageData
-        # The number of the page returned.
+        # The number of the page to return. Valid values: **1** to **100000**.
         self.page_number = page_number  # type: int
-        # The number of the entries returned per page.
+        # The description of the task.
         self.page_size = page_size  # type: int
-        # The total number of entries returned.
+        # The start of the time range that was queried.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -24005,17 +23754,17 @@
         if m.get('TotalCount') is not None:
             self.total_count = m.get('TotalCount')
         return self
 
 
 class DescribeUserUsageDetailDataExportTaskResponseBody(TeaModel):
     def __init__(self, request_id=None, usage_data_per_page=None):
-        # The ID of the request.
+        # The ID of the task.
         self.request_id = request_id  # type: str
-        # The usage details returned per page.
+        # The end of the time range that was queried.
         self.usage_data_per_page = usage_data_per_page  # type: DescribeUserUsageDetailDataExportTaskResponseBodyUsageDataPerPage
 
     def validate(self):
         if self.usage_data_per_page:
             self.usage_data_per_page.validate()
 
     def to_map(self):
@@ -24077,20 +23826,17 @@
             temp_model = DescribeUserUsageDetailDataExportTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeUserVipsByDomainRequest(TeaModel):
     def __init__(self, available=None, domain_name=None):
-        # Specifies whether to query the virtual IP addresses of only healthy CDN edge nodes. Valid values: Valid values:
-        # 
-        # *   **on**: healthy CDN edge nodes
-        # *   **off**: all CDN edge nodes
+        # The virtual IP address.
         self.available = available  # type: str
-        # The accelerated domain name. You can specify only one domain name.
+        # A list of virtual IP addresses.
         self.domain_name = domain_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeUserVipsByDomainRequest, self).to_map()
@@ -24135,19 +23881,19 @@
         if m.get('Vip') is not None:
             self.vip = m.get('Vip')
         return self
 
 
 class DescribeUserVipsByDomainResponseBody(TeaModel):
     def __init__(self, domain_name=None, request_id=None, vips=None):
-        # The domain name.
+        # >  The maximum number of times that each user can call this operation per second is 30.
         self.domain_name = domain_name  # type: str
-        # The ID of the request.
-        self.request_id = request_id  # type: str
         # A list of virtual IP addresses.
+        self.request_id = request_id  # type: str
+        # The accelerated domain name. You can specify only one domain name.
         self.vips = vips  # type: DescribeUserVipsByDomainResponseBodyVips
 
     def validate(self):
         if self.vips:
             self.vips.validate()
 
     def to_map(self):
@@ -24213,15 +23959,14 @@
             temp_model = DescribeUserVipsByDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeVerifyContentRequest(TeaModel):
     def __init__(self, domain_name=None):
-        # The domain name of which you want to verify the ownership. You can specify only one domain name.
         self.domain_name = domain_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeVerifyContentRequest, self).to_map()
@@ -24238,17 +23983,15 @@
         if m.get('DomainName') is not None:
             self.domain_name = m.get('DomainName')
         return self
 
 
 class DescribeVerifyContentResponseBody(TeaModel):
     def __init__(self, content=None, request_id=None):
-        # The verification result.
         self.content = content  # type: str
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeVerifyContentResponseBody, self).to_map()
@@ -24535,15 +24278,15 @@
         if m.get('Domain') is not None:
             self.domain = m.get('Domain')
         return self
 
 
 class ListDomainsByLogConfigIdResponseBody(TeaModel):
     def __init__(self, domains=None, request_id=None):
-        # The list of domain names.
+        # The domain names.
         self.domains = domains  # type: ListDomainsByLogConfigIdResponseBodyDomains
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.domains:
             self.domains.validate()
@@ -24607,15 +24350,15 @@
             temp_model = ListDomainsByLogConfigIdResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListFCTriggerRequest(TeaModel):
     def __init__(self, event_meta_name=None, event_meta_version=None):
-        # The name of the event for which the Function Compute trigger is set. You can specify only one name.
+        # The name of the event. You can specify only one name.
         self.event_meta_name = event_meta_name  # type: str
         # The version number of the event. You can specify only one version number.
         self.event_meta_version = event_meta_version  # type: str
 
     def validate(self):
         pass
 
@@ -24639,25 +24382,25 @@
             self.event_meta_version = m.get('EventMetaVersion')
         return self
 
 
 class ListFCTriggerResponseBodyFCTriggers(TeaModel):
     def __init__(self, event_meta_name=None, event_meta_version=None, notes=None, role_arn=None, source_arn=None,
                  trigger_arn=None):
-        # The name of the event for which the Function Compute trigger is set.
+        # The name of the event.
         self.event_meta_name = event_meta_name  # type: str
-        # The version of the event for which the Function Compute trigger is set.
+        # The version of the event.
         self.event_meta_version = event_meta_version  # type: str
-        # The remarks for the event.
+        # The remarks.
         self.notes = notes  # type: str
         # The Resource Access Management (RAM) role.
         self.role_arn = role_arn  # type: str
         # The resources and filters for event listening.
         self.source_arn = source_arn  # type: str
-        # The trigger corresponding to the Function Compute service.
+        # The trigger that corresponds to the Function Compute service.
         self.trigger_arn = trigger_arn  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListFCTriggerResponseBodyFCTriggers, self).to_map()
@@ -24694,15 +24437,15 @@
         if m.get('TriggerARN') is not None:
             self.trigger_arn = m.get('TriggerARN')
         return self
 
 
 class ListFCTriggerResponseBody(TeaModel):
     def __init__(self, fctriggers=None, request_id=None):
-        # The information about the Function Compute trigger returned.
+        # The Function Compute triggers that are set for Alibaba Cloud CDN events.
         self.fctriggers = fctriggers  # type: list[ListFCTriggerResponseBodyFCTriggers]
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.fctriggers:
             for k in self.fctriggers:
@@ -24772,15 +24515,15 @@
             temp_model = ListFCTriggerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListRealtimeLogDeliveryDomainsRequest(TeaModel):
     def __init__(self, logstore=None, project=None, region=None):
-        # The name of the Logstore that collects log data from Alibaba Cloud Content Delivery Network (CDN) in real time. You can specify multiple Logstore names and separate them with commas (,).
+        # The name of the Logstore that collects log data from Alibaba Cloud CDN in real time. You can specify multiple Logstore names and separate them with commas (,).
         self.logstore = logstore  # type: str
         # The name of the Log Service project that is used for real-time log delivery. You can specify multiple project names and separate them with commas (,).
         self.project = project  # type: str
         # The ID of the region where the Log Service project is deployed. You can specify multiple region IDs and separate them with commas (,).
         # 
         # For more information about regions, see [Regions that support real-time log delivery](~~144883~~).
         self.region = region  # type: str
@@ -24811,20 +24554,20 @@
         if m.get('Region') is not None:
             self.region = m.get('Region')
         return self
 
 
 class ListRealtimeLogDeliveryDomainsResponseBodyContentDomains(TeaModel):
     def __init__(self, domain_name=None, status=None):
-        # The accelerated domain name.
+        # The domain name.
         self.domain_name = domain_name  # type: str
-        # The status of the real-time log delivery feature. Valid values:
+        # The status. Valid values:
         # 
-        # *   **online**: The feature is enabled.
-        # *   **offline**: The feature is disabled.
+        # *   **online**: enabled
+        # *   **offline**: disabled
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListRealtimeLogDeliveryDomainsResponseBodyContentDomains, self).to_map()
@@ -24949,15 +24692,15 @@
             temp_model = ListRealtimeLogDeliveryDomainsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListRealtimeLogDeliveryInfosResponseBodyContentRealtimeLogDeliveryInfos(TeaModel):
     def __init__(self, logstore=None, project=None, region=None):
-        # The name of the Logstore that collects log data from Alibaba Cloud Content Delivery Network (CDN) in real time.
+        # The name of the Logstore that collects log data from Alibaba Cloud CDN in real time.
         self.logstore = logstore  # type: str
         # The name of the Log Service project that is used for real-time log delivery.
         self.project = project  # type: str
         # The ID of the region where the Log Service project is deployed. For more information, see [Regions that support real-time log delivery](~~144883~~).
         self.region = region  # type: str
 
     def validate(self):
@@ -25018,15 +24761,15 @@
                 temp_model = ListRealtimeLogDeliveryInfosResponseBodyContentRealtimeLogDeliveryInfos()
                 self.realtime_log_delivery_infos.append(temp_model.from_map(k))
         return self
 
 
 class ListRealtimeLogDeliveryInfosResponseBody(TeaModel):
     def __init__(self, content=None, request_id=None):
-        # The content of the log entry.
+        # The information about real-time log delivery.
         self.content = content  # type: ListRealtimeLogDeliveryInfosResponseBodyContent
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.content:
             self.content.validate()
@@ -25114,17 +24857,17 @@
         if m.get('ConfigId') is not None:
             self.config_id = m.get('ConfigId')
         return self
 
 
 class ListUserCustomLogConfigResponseBody(TeaModel):
     def __init__(self, config_ids=None, request_id=None):
-        # The list of configuration ID.
-        self.config_ids = config_ids  # type: ListUserCustomLogConfigResponseBodyConfigIds
         # The ID of the request.
+        self.config_ids = config_ids  # type: ListUserCustomLogConfigResponseBodyConfigIds
+        # The ID of the log configuration.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.config_ids:
             self.config_ids.validate()
 
     def to_map(self):
@@ -25187,27 +24930,27 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyCdnDomainRequest(TeaModel):
     def __init__(self, domain_name=None, owner_id=None, resource_group_id=None, security_token=None, sources=None,
                  top_level_domain=None):
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name  # type: str
         self.owner_id = owner_id  # type: long
         # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
         self.security_token = security_token  # type: str
-        # The list of origin URLs.
+        # The information about the addresses of origin servers.
         # 
-        # >  You cannot set both the **Sources** and **TopLevelDomain** parameters in the same request. Otherwise, ********the **TopLevelDomain** parameter cannot take effect.
+        # > Do not set **Sources** and **TopLevelDomain** at the same time. If you set **Sources** and **TopLevelDomain** at the same time, **TopLevelDomain** does not take effect.
         self.sources = sources  # type: str
-        # The top-level domain name. To add a top-level domain name, set the parameter CDN_TOP_LEVEL_DOMAIN_GREY_USER_LIST. This feature is available to only selected users.
+        # The root domain. To add a root domain name, you must be added to the whitelist specified by the CDN_TOP_LEVEL_DOMAIN_GREY_USER_LIST parameter.
         # 
-        # >  You cannot set both the **Sources** and **TopLevelDomain** parameters in the same request. Otherwise, ****the **TopLevelDomain** parameter cannot take effect.
+        # > Do not set **Sources** and **TopLevelDomain** at the same time. If you set **Sources** and **TopLevelDomain** at the same time, **TopLevelDomain** does not take effect.
         self.top_level_domain = top_level_domain  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyCdnDomainRequest, self).to_map()
@@ -25308,15 +25051,15 @@
             temp_model = ModifyCdnDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyCdnDomainSchdmByPropertyRequest(TeaModel):
     def __init__(self, domain_name=None, property=None):
-        # The accelerated domain name for which you want to change the accelerated region. You can specify only one domain name.
+        # The operation that you want to perform. Set the value to **ModifyCdnDomainSchdmByProperty**.
         self.domain_name = domain_name  # type: str
         # The accelerated region. Valid values for coverage:
         # 
         # *   **domestic**: Chinese mainland
         # *   **overseas**: global (excluding the Chinese mainland)
         # *   **global**: global
         self.property = property  # type: str
@@ -25343,15 +25086,14 @@
         if m.get('Property') is not None:
             self.property = m.get('Property')
         return self
 
 
 class ModifyCdnDomainSchdmByPropertyResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyCdnDomainSchdmByPropertyResponseBody, self).to_map()
@@ -25407,21 +25149,21 @@
             temp_model = ModifyCdnDomainSchdmByPropertyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyRealtimeLogDeliveryRequest(TeaModel):
     def __init__(self, domain=None, logstore=None, project=None, region=None):
-        # The accelerated domain name for which you want to modify the configurations of real-time log delivery. Only one domain name is supported.
+        # The ID of the request.
         self.domain = domain  # type: str
-        # The name of the Logstore.
+        # The accelerated domain name for which you want to modify the configurations of real-time log delivery. Only one domain name is supported.
         self.logstore = logstore  # type: str
-        # The name of the Log Service project that is used for real-time log delivery.
-        self.project = project  # type: str
         # The ID of the region where the Log Service project is deployed. For more information, see [Regions that support real-time log delivery](~~144883~~).
+        self.project = project  # type: str
+        # The name of the Log Service project that is used for real-time log delivery.
         self.region = region  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyRealtimeLogDeliveryRequest, self).to_map()
@@ -25450,15 +25192,15 @@
         if m.get('Region') is not None:
             self.region = m.get('Region')
         return self
 
 
 class ModifyRealtimeLogDeliveryResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
+        # The operation that you want to perform. Set the value to **ModifyRealtimeLogDelivery**.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyRealtimeLogDeliveryResponseBody, self).to_map()
@@ -25844,23 +25586,24 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RefreshObjectCachesRequest(TeaModel):
     def __init__(self, object_path=None, object_type=None, owner_id=None, security_token=None):
         self.object_path = object_path  # type: str
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
         self.object_type = object_type  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
@@ -25891,20 +25634,20 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class RefreshObjectCachesResponseBody(TeaModel):
     def __init__(self, refresh_task_id=None, request_id=None):
-        # The ID of the refresh task. If multiple tasks are returned, the IDs are separated by commas (,). The task IDs are merged based on the following rules:
+        # The refresh task ID. If multiple tasks are returned, the IDs are separated by commas (,). The task IDs are merged based on the following rules:
         # 
         # *   If the tasks are specified for the same accelerated domain name, submitted within the same second, and run to refresh content based on URLs instead of directories, the task IDs are merged into one task ID.
         # *   If the number of tasks that are specified for the same accelerated domain name, submitted within the same second, and run to refresh content based on URLs instead of directories exceeds 2,000, every 2,000 task IDs are merged into one task ID.
         self.refresh_task_id = refresh_task_id  # type: str
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RefreshObjectCachesResponseBody, self).to_map()
@@ -25964,15 +25707,15 @@
             temp_model = RefreshObjectCachesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RollbackStagingConfigRequest(TeaModel):
     def __init__(self, domain_name=None):
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RollbackStagingConfigRequest, self).to_map()
@@ -26053,15 +25796,15 @@
             temp_model = RollbackStagingConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SetCdnDomainCSRCertificateRequest(TeaModel):
     def __init__(self, domain_name=None, server_certificate=None):
-        # The accelerated domain name for which you want to configure an SSL certificate. The domain name must have HTTPS secure acceleration enabled.
+        # The ID of the request.
         self.domain_name = domain_name  # type: str
         # The content of the certificate. The certificate must match the certificate signing request (CSR) created by calling the [CreateCdnCertificateSigningRequest](~~144478~~) operation. Make sure that the certificate is in the PEM format, and the content of the certificate is encoded in Base64 and then encoded by encodeURIComponent.
         self.server_certificate = server_certificate  # type: str
 
     def validate(self):
         pass
 
@@ -26084,15 +25827,15 @@
         if m.get('ServerCertificate') is not None:
             self.server_certificate = m.get('ServerCertificate')
         return self
 
 
 class SetCdnDomainCSRCertificateResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
+        # The operation that you want to perform. Set the value to **SetCdnDomainCSRCertificate**.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetCdnDomainCSRCertificateResponseBody, self).to_map()
@@ -26148,25 +25891,25 @@
             temp_model = SetCdnDomainCSRCertificateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SetCdnDomainSMCertificateRequest(TeaModel):
     def __init__(self, cert_identifier=None, domain_name=None, owner_id=None, sslprotocol=None, security_token=None):
-        # The ID of the SM certificate that you want to configure.
+        # The ID of the SM certificate that you want to configure. The identifier of the certificate. The value is Certificate ID-cn-hangzhou. For example, if the certificate ID is 123, set the value of this parameter to 123-cn-hangzhou.
         self.cert_identifier = cert_identifier  # type: str
         # The accelerated domain name for which you want to configure the SM certificate.
         # 
-        # >  The domain name uses HTTPS secure acceleration.
+        # > The domain name must use HTTPS acceleration.
         self.domain_name = domain_name  # type: str
         self.owner_id = owner_id  # type: long
         # Specifies whether to enable the SSL certificate. Valid values:
         # 
-        # *   **on**: enables the SSL certificate.
-        # *   **off**: disables the SSL certificate.
+        # *   **on**\
+        # *   **off**\
         self.sslprotocol = sslprotocol  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -26262,41 +26005,150 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SetCdnDomainSMCertificateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SetCdnDomainSSLCertificateRequest(TeaModel):
+    def __init__(self, cert_id=None, cert_name=None, cert_region=None, cert_type=None, domain_name=None,
+                 owner_id=None, sslpri=None, sslprotocol=None, sslpub=None, security_token=None):
+        self.cert_id = cert_id  # type: long
+        self.cert_name = cert_name  # type: str
+        self.cert_region = cert_region  # type: str
+        self.cert_type = cert_type  # type: str
+        self.domain_name = domain_name  # type: str
+        self.owner_id = owner_id  # type: long
+        self.sslpri = sslpri  # type: str
+        self.sslprotocol = sslprotocol  # type: str
+        self.sslpub = sslpub  # type: str
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetCdnDomainSSLCertificateRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetCdnDomainSSLCertificateResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetCdnDomainSSLCertificateResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: SetCdnDomainSSLCertificateResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(SetCdnDomainSSLCertificateResponse, self).to_map()
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
+            temp_model = SetCdnDomainSSLCertificateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SetCdnDomainStagingConfigRequest(TeaModel):
     def __init__(self, domain_name=None, functions=None):
-        # The accelerated domain name. You can specify only one domain name.
         self.domain_name = domain_name  # type: str
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
         self.functions = functions  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetCdnDomainStagingConfigRequest, self).to_map()
@@ -26317,19 +26169,16 @@
         if m.get('Functions') is not None:
             self.functions = m.get('Functions')
         return self
 
 
 class SetCdnDomainStagingConfigResponseBodyDomainConfigList(TeaModel):
     def __init__(self, config_id=None, domain_name=None, function_name=None):
-        # The ID of the configuration.
         self.config_id = config_id  # type: long
-        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The function name.
         self.function_name = function_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetCdnDomainStagingConfigResponseBodyDomainConfigList, self).to_map()
@@ -26354,17 +26203,15 @@
         if m.get('FunctionName') is not None:
             self.function_name = m.get('FunctionName')
         return self
 
 
 class SetCdnDomainStagingConfigResponseBody(TeaModel):
     def __init__(self, domain_config_list=None, request_id=None):
-        # The list of the domain configuration.
         self.domain_config_list = domain_config_list  # type: list[SetCdnDomainStagingConfigResponseBodyDomainConfigList]
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.domain_config_list:
             for k in self.domain_config_list:
                 if k:
                     k.validate()
@@ -26433,40 +26280,38 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SetDomainServerCertificateRequest(TeaModel):
     def __init__(self, cert_name=None, cert_type=None, domain_name=None, force_set=None, owner_id=None,
                  private_key=None, security_token=None, server_certificate=None, server_certificate_status=None):
-        # The name of the SSL certificate. You can specify only one name.
+        # Specifies whether to check the certificate name for duplicates. If you set the value to 1, the system does not perform the check and overwrites the information of the existing certificate that uses the same name.
         self.cert_name = cert_name  # type: str
+        # The ID of the request.
+        self.cert_type = cert_type  # type: str
+        # The private key. Specify the private key only if you want to enable the SSL certificate.
+        self.domain_name = domain_name  # type: str
+        # Specifies whether to enable the SSL certificate. Valid values:
+        # 
+        # *   **on**: enables the SSL certificate.
+        # *   **off**: disables the SSL certificate. This is the default value.
+        self.force_set = force_set  # type: str
+        self.owner_id = owner_id  # type: long
+        # Specifies whether to check the certificate name for duplicates. If you set the value to 1, the system does not perform the check and overwrites the information of the existing certificate that uses the same name.
+        self.private_key = private_key  # type: str
+        self.security_token = security_token  # type: str
         # The type of the SSL certificate. Valid values:
         # 
         # *   **upload**: a user-uploaded SSL certificate.
         # *   **cas**: an SSL certificate that is issued by Alibaba Cloud SSL Certificates Service.
         # *   **free**: a free SSL certificate.
         # 
         # >  If this parameter is set to **cas**, the **PrivateKey** parameter is optional.
-        self.cert_type = cert_type  # type: str
-        # The accelerated domain name for which you want to configure the SSL certificate. The type of request supported by the domain name must be HTTPS.
-        # 
-        # You can specify one domain name in each call.
-        self.domain_name = domain_name  # type: str
-        # Specifies whether to check the certificate name for duplicates. If you set the value to 1, the system does not perform the check and overwrites the information of the existing certificate that uses the same name.
-        self.force_set = force_set  # type: str
-        self.owner_id = owner_id  # type: long
-        # The private key. Specify the private key only if you want to enable the SSL certificate.
-        self.private_key = private_key  # type: str
-        self.security_token = security_token  # type: str
-        # The content of the SSL certificate. Specify the content of the SSL certificate only if you want to enable the SSL certificate.
         self.server_certificate = server_certificate  # type: str
-        # Specifies whether to enable the SSL certificate. Valid values:
-        # 
-        # *   **on**: enables the SSL certificate.
-        # *   **off**: disables the SSL certificate. This is the default value.
+        # The name of the SSL certificate. You can specify only one name.
         self.server_certificate_status = server_certificate_status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetDomainServerCertificateRequest, self).to_map()
@@ -26581,21 +26426,21 @@
         return self
 
 
 class SetReqHeaderConfigRequest(TeaModel):
     def __init__(self, config_id=None, domain_name=None, key=None, owner_id=None, security_token=None, value=None):
         # The ID of the configuration.
         self.config_id = config_id  # type: long
-        # The accelerated domain names. You can specify one or more domain names and separate them with commas (,).
+        # The accelerated domain name. Separate multiple domain names with commas (,).
         self.domain_name = domain_name  # type: str
-        # The parameter of the custom header.
+        # The name of the custom header.
         self.key = key  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
-        # The value of the custom parameter.
+        # The value of the custom header.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetReqHeaderConfigRequest, self).to_map()
@@ -26701,17 +26546,17 @@
 class SetWaitingRoomConfigRequest(TeaModel):
     def __init__(self, allow_pct=None, domain_name=None, gap_time=None, max_time_wait=None, wait_uri=None,
                  wait_url=None):
         # The percentage of requests that are allowed to be redirected to the origin server. Valid values: **0** to **100**.
         self.allow_pct = allow_pct  # type: int
         # The accelerated domain name. You can specify only one domain name.
         self.domain_name = domain_name  # type: str
-        # The length of waiting time to skip after users exit the queue. Unit: seconds.
+        # The length of waiting time to skip after an exit from the queue. Unit: seconds.
         self.gap_time = gap_time  # type: int
-        # The maximum length of time that users need to wait in the queue. Unit: seconds.
+        # The maximum length of waiting time in the queue. Unit: seconds.
         self.max_time_wait = max_time_wait  # type: int
         # The regular expression that is used to match URI strings for which the virtual waiting room feature is enabled.
         self.wait_uri = wait_uri  # type: str
         # The URL of the waiting page.
         self.wait_url = wait_url  # type: str
 
     def validate(self):
@@ -26816,15 +26661,15 @@
             temp_model = SetWaitingRoomConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class StartCdnDomainRequest(TeaModel):
     def __init__(self, domain_name=None, owner_id=None, security_token=None):
-        # The domain name that you want to enable. You can specify only one domain name.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
@@ -26915,15 +26760,15 @@
             temp_model = StartCdnDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class StopCdnDomainRequest(TeaModel):
     def __init__(self, domain_name=None, owner_id=None, security_token=None):
-        # The accelerated domain name that you want to disable. You can specify only one domain name.
+        # The accelerated domain name that you want to disable. You can specify only one domain name in each request.
         self.domain_name = domain_name  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
@@ -27014,17 +26859,17 @@
             temp_model = StopCdnDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class TagResourcesRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
-        # The key of the tag. Valid values of N: **1** to **20**.
+        # The ID of the request.
         self.key = key  # type: str
-        # The value of the tag. Valid values of N: **1** to **20**.
+        # The operation that you want to perform. Set the value to **TagResources**.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(TagResourcesRequestTag, self).to_map()
@@ -27045,19 +26890,19 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class TagResourcesRequest(TeaModel):
     def __init__(self, resource_id=None, resource_type=None, tag=None):
-        # The list of resource ID.
+        # The ID of the resource. Valid values of N: **1** to **50**.
         self.resource_id = resource_id  # type: list[str]
-        # The type of resource. The resource type. Set the value to **DOMAIN**.
+        # >  The maximum number of times that each user can call this operation per second is 100.
         self.resource_type = resource_type  # type: str
-        # The tags.
+        # The type of resource. The resource type. Set the value to **DOMAIN**.
         self.tag = tag  # type: list[TagResourcesRequestTag]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -27090,15 +26935,15 @@
                 temp_model = TagResourcesRequestTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
 
 class TagResourcesResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
+        # Adds tags to a resource.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(TagResourcesResponseBody, self).to_map()
@@ -27154,26 +26999,26 @@
             temp_model = TagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UntagResourcesRequest(TeaModel):
     def __init__(self, all=None, resource_id=None, resource_type=None, tag_key=None):
-        # Specifies whether to delete all tags. Valid values:
+        # Specifies whether to remove all tags. Valid values:
         # 
         # *   **true**: yes.
         # *   **false**: no.
         # 
         # Default value: **false**.
         self.all = all  # type: bool
-        # The list of resource ID. The max items count is up to 20.
+        # The list of resource IDs. You can specify up to 50 resource IDs in the list.
         self.resource_id = resource_id  # type: list[str]
-        # The type of resource. The resource type. Set the value to **DOMAIN**.
+        # The type of the resources from which you want to remove tags. Set this parameter to **DOMAIN**.
         self.resource_type = resource_type  # type: str
-        # The list of tag key.
+        # The list of tag keys. You can specify up to 20 tag keys in the list.
         self.tag_key = tag_key  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UntagResourcesRequest, self).to_map()
@@ -27270,17 +27115,15 @@
 
 class UpdateCdnDeliverTaskRequest(TeaModel):
     def __init__(self, deliver=None, deliver_id=None, domain_name=None, name=None, reports=None, schedule=None):
         # The method that is used to send operations reports. Operations reports are sent to you only by email. The settings must be escaped in JSON.
         self.deliver = deliver  # type: str
         # The ID of the tracking task that you want to update.
         self.deliver_id = deliver_id  # type: long
-        # The domain name that you want to track. You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
-        # 
-        # If you do not specify a domain name, the task collects data from all domain names that belong to your Alibaba Cloud account.
+        # The domain name that you want to track. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,). If you do not specify a domain name, the task collects data from all domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
         # The name of the tracking task.
         self.name = name  # type: str
         # The operations reports that are tracked by the task. The data must be escaped in JSON.
         self.reports = reports  # type: str
         # The parameters that specify the time interval at which the tracking task sends operations reports. The settings must be escaped in JSON.
         self.schedule = schedule  # type: str
@@ -27387,23 +27230,21 @@
             temp_model = UpdateCdnDeliverTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateCdnSubTaskRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, report_ids=None, start_time=None):
-        # The domain names that you want to track. You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
-        # 
-        # If you do not specify a domain name, the task collects data from all domain names that belong to your Alibaba Cloud account.
+        # The domain name that you want to track. You can specify up to 500 domain names in each request. If you specify multiple domain names, separate them with commas (,). If you do not specify a domain name, operations reports are updated for all domain names in your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
-        # The end time of the operations report. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end time of the operations report. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time  # type: str
         # The IDs of operations reports that you want to update. Separate IDs with commas (,).
         self.report_ids = report_ids  # type: str
-        # The start time of the operations report. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The start time of the operations report. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateCdnSubTaskRequest, self).to_map()
@@ -27500,15 +27341,15 @@
 
 class UpdateFCTriggerRequest(TeaModel):
     def __init__(self, function_arn=None, notes=None, role_arn=None, source_arn=None, trigger_arn=None):
         # The feature trigger.
         self.function_arn = function_arn  # type: str
         # The remarks.
         self.notes = notes  # type: str
-        # The assigned Resource Access Management (RAM) role.
+        # The assigned RAM role.
         self.role_arn = role_arn  # type: str
         # The resources and filters for event listening.
         self.source_arn = source_arn  # type: str
         # The trigger that corresponds to the Function Compute service.
         self.trigger_arn = trigger_arn  # type: str
 
     def validate(self):
@@ -27647,15 +27488,15 @@
 
 class VerifyDomainOwnerResponseBody(TeaModel):
     def __init__(self, content=None, request_id=None):
         # The verification result.
         # 
         # > This parameter is returned only if the operation fails.
         self.content = content  # type: str
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(VerifyDomainOwnerResponseBody, self).to_map()
```

### Comparing `alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510_py2.egg-info/PKG-INFO` & `alibabacloud_cdn20180510_py2-1.2.8/alibabacloud_cdn20180510_py2.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cdn20180510-py2
-Version: 1.2.7
+Version: 1.2.8
 Summary: Alibaba Cloud Alibaba Cloud CDN (20180510) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cdn20180510_py2-1.2.7/setup.py` & `alibabacloud_cdn20180510_py2-1.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cdn20180510_py2.
 
-Created on 25/04/2023
+Created on 04/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cdn20180510"
 NAME = "alibabacloud_cdn20180510_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Alibaba Cloud CDN (20180510) SDK Library for Python2"
```

