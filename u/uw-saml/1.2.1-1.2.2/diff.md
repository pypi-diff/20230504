# Comparing `tmp/uw_saml-1.2.1.tar.gz` & `tmp/uw_saml-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uw_saml-1.2.1.tar", max compression
+gzip compressed data, was "uw_saml-1.2.2.tar", max compression
```

## Comparing `uw_saml-1.2.1.tar` & `uw_saml-1.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      564 2023-05-03 21:52:56.227831 uw_saml-1.2.1/LICENSE
--rw-r--r--   0        0        0      606 2023-05-03 21:52:56.227831 uw_saml-1.2.1/pyproject.toml
--rw-r--r--   0        0        0       53 2023-05-03 21:52:56.227831 uw_saml-1.2.1/uw_saml2/VERSION
--rw-r--r--   0        0        0       70 2023-05-03 21:52:56.227831 uw_saml-1.2.1/uw_saml2/__init__.py
--rw-r--r--   0        0        0     3221 2023-05-03 21:52:56.227831 uw_saml-1.2.1/uw_saml2/auth.py
--rw-r--r--   0        0        0      389 2023-05-03 21:52:56.227831 uw_saml-1.2.1/uw_saml2/idp/__init__.py
--rw-r--r--   0        0        0     1619 2023-05-03 21:52:56.227831 uw_saml-1.2.1/uw_saml2/idp/attribute.py
--rw-r--r--   0        0        0     9896 2023-05-03 21:52:56.227831 uw_saml-1.2.1/uw_saml2/idp/federated.py
--rw-r--r--   0        0        0     2589 2023-05-03 21:52:56.227831 uw_saml-1.2.1/uw_saml2/idp/uw.py
--rw-r--r--   0        0        0     1538 2023-05-03 21:52:56.231831 uw_saml-1.2.1/uw_saml2/mock.py
--rw-r--r--   0        0        0      279 2023-05-03 21:52:56.231831 uw_saml-1.2.1/uw_saml2/python3_saml.py
--rw-r--r--   0        0        0     2302 2023-05-03 21:52:56.231831 uw_saml-1.2.1/uw_saml2/sp.py
--rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 uw_saml-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      564 2023-05-03 22:16:45.560744 uw_saml-1.2.2/LICENSE
+-rw-r--r--   0        0        0      606 2023-05-03 22:16:45.564744 uw_saml-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/VERSION
+-rw-r--r--   0        0        0       70 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/__init__.py
+-rw-r--r--   0        0        0     3221 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/auth.py
+-rw-r--r--   0        0        0      389 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/idp/__init__.py
+-rw-r--r--   0        0        0     1619 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/idp/attribute.py
+-rw-r--r--   0        0        0     9878 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/idp/federated.py
+-rw-r--r--   0        0        0     2589 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/idp/uw.py
+-rw-r--r--   0        0        0     1538 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/mock.py
+-rw-r--r--   0        0        0      279 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/python3_saml.py
+-rw-r--r--   0        0        0     2302 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/sp.py
+-rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 uw_saml-1.2.2/PKG-INFO
```

### Comparing `uw_saml-1.2.1/LICENSE` & `uw_saml-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.1/pyproject.toml` & `uw_saml-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uw-saml"
-version = "1.2.1"
+version = "1.2.2"
 description = "A UW-specific adapter to the python3-saml package."
 authors = []
 license = "Apache 2.0"
 packages = [
     { include = 'uw_saml2' }
 ]
```

### Comparing `uw_saml-1.2.1/uw_saml2/auth.py` & `uw_saml-1.2.2/uw_saml2/auth.py`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.1/uw_saml2/idp/attribute.py` & `uw_saml-1.2.2/uw_saml2/idp/attribute.py`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.1/uw_saml2/idp/federated.py` & `uw_saml-1.2.2/uw_saml2/idp/federated.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,32 +9,30 @@
     #  _attribute_prefix, id_attribute from FredHutchAzureIdp(IdpConfig)
     #  x509_cert from
     #  CCFederationMetadata.xml IDPSSODescriptor/KeyDescriptor/signing
     entity_id = "http://sts.cascadia.edu/adfs/services/trust"
     sso_url = "https://sts.cascadia.edu/adfs/ls/"
     id_attribute = "employeeNumber"
     x509_cert = """
-        MIIC3DCCAcSgAwIBAgIQXrfPPZMKPYlC3T8Lh+ONhDANBgkqhkiG9w0B
-        AQsFADAqMSgwJgYDVQQDEx9BREZTIFNpZ25pbmcgLSBzdHMuY2FzY2Fk
-        aWEuZWR1MB4XDTIyMDUwNjA5MjkwMloXDTIzMDUwNjA5MjkwMlowKjEo
-        MCYGA1UEAxMfQURGUyBTaWduaW5nIC0gc3RzLmNhc2NhZGlhLmVkdTCC
-        ASIwDQYJKoZIhvcNAQEBBQADggEPADCCAQoCggEBALNtzF2VwFEaKpsp
-        H0AmNQHy3rx23wd3bj3NvwsfyHafydWxxivu9oOLne4MMzB1I20NvEN9
-        Jw5gB9n+gBPB4K8njsHtBESUoy6wFPj4V+kYDpHJmX9xuIP1rG0OZ/X8
-        8uYbImnN1//dDPR6WFg65VBs9TWF4pxFXMnPmAqV7kgVIJhZfbA3Dmfc
-        1SzIoA/YGQ2bOuXktN2ZOiRcYgtmR3W1yFepcGotL616gWANRa6qg85t
-        ReKde3286HE3MFBXa1lM2i2fDpYkwQuZVsXVKZiRyCYepTW6Y+zvZzDT
-        jqqOSU++wSJj32nz2XqYeKhk89FljDgNWNUEh3bE8NwuQIUCAwEAATAN
-        BgkqhkiG9w0BAQsFAAOCAQEAm3AYm9qdrh2EKK7+8JVXysx90OS+rz+o
-        MGtGKDwPK9SLCx56wcyMF+332hNrHgA3+RmZCndUjSaap2xdoA5Ubn1V
-        SNWAZR4ERcinhojIJntKEUtPkE3GoBdr2Ta7xC6kiI+bt3R5/yLQ/1AU
-        w8vQoMv6LEYGZ82zRihwVo5SfAc/TxvjNYAMrF5YPj1OHCEKXJITnf5v
-        ChARq3CysO6F1oY/yxBT9VeHvqWYQc9eWIeUwVflBsl6QWRi6kjv3ezQ
-        xPUjFRIVJr31JLd7h3eI4AGCDiuZP0Ro8xrxJOObcKMPdBE6PkT+q8JA
-        krm7bWjDEu8/wRKVz894pKIC/oiklg==
+        MIIC3DCCAcSgAwIBAgIQMIdwSJDYuLVNwseBCkxA4zANBgkqhkiG9w0BAQsFADAq
+        MSgwJgYDVQQDEx9BREZTIFNpZ25pbmcgLSBzdHMuY2FzY2FkaWEuZWR1MB4XDTIz
+        MDQxNjEwNDY1NFoXDTI0MDQxNTEwNDY1NFowKjEoMCYGA1UEAxMfQURGUyBTaWdu
+        aW5nIC0gc3RzLmNhc2NhZGlhLmVkdTCCASIwDQYJKoZIhvcNAQEBBQADggEPADCC
+        AQoCggEBAMe4H/m7hmZkSXYtYSRq9Uc23FwiXqPyeP/DwPR5+1lPVRrA5NskAtLI
+        5W4FLm7d+PAKBgCr9RvWzEkvG7YeQOXWInqF2/KObTa0LNogO3zI4Pr2yzIOsFkd
+        9X/xx0CSlpckMDJdoc15aXTpSC5PDn/yoKR0+Qk+tP3Pd8X1fg0ShbGhnhPl6tk5
+        nXwJSTqPwrKgPr36Sk8vf3uPDvoU6vXjW7Dk9Yoo4gu6RwO+riujjrELdR44aaJ2
+        8INho3yL6pLQ9UyT+J5agEIwsTEJeVabdhO8bAsRwXK3UOgbqrJbfcCGQJiQKQWv
+        6NL5eYDH8yyjyTwzl8aYWNqhmQVGIXkCAwEAATANBgkqhkiG9w0BAQsFAAOCAQEA
+        TZul0d3Ambn5rg75I2IsjqQJckDJfVB9fhSQ2fK9fK1yZ9lRQDox5Zidu8q95ugn
+        4cmtSqS/260TvsWvRcJK3KbiZ46DmrlANF9qiAjClKIrv3uYHZb0pJd2j+ZKdVOT
+        8EQ2uSOElcY7ZBx+55yAzCW8TSGA3TMLRcKXozfk++HFoLEXbZaTo447BUb9b82U
+        Mv42rFI66/59obGWdQ6UHyGCvyN4FBd4nYCcpM6pKxOfhMbAA7F6rcCRYisSjkZe
+        5FymL4FYVDuJ6WdSaWEIbpojD8+nnJpS8Yal/8qicwMWCT9VpUDHmsZC5WiKmTXm
+        RXE3esrKhhuPEkK1Qk0mLw==
     """
 
 
 class CollegenetIdp(IdpConfig):
     """
     One thing of note about collegenet is that it encrypts attributes and thus
     requires an SP cert and key.
```

### Comparing `uw_saml-1.2.1/uw_saml2/idp/uw.py` & `uw_saml-1.2.2/uw_saml2/idp/uw.py`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.1/uw_saml2/mock.py` & `uw_saml-1.2.2/uw_saml2/mock.py`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.1/uw_saml2/sp.py` & `uw_saml-1.2.2/uw_saml2/sp.py`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.1/PKG-INFO` & `uw_saml-1.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uw-saml
-Version: 1.2.1
+Version: 1.2.2
 Summary: A UW-specific adapter to the python3-saml package.
 License: Apache 2.0
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

