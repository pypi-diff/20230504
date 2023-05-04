# Comparing `tmp/landingzone_organization-0.2.2.tar.gz` & `tmp/landingzone_organization-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingzone_organization-0.2.2.tar", max compression
+gzip compressed data, was "landingzone_organization-0.3.0.tar", max compression
```

## Comparing `landingzone_organization-0.2.2.tar` & `landingzone_organization-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0      980 2023-05-03 12:25:03.774561 landingzone_organization-0.2.2/README.md
--rw-r--r--   0        0        0      390 2023-05-03 12:25:04.598577 landingzone_organization-0.2.2/landingzone_organization/__init__.py
--rw-r--r--   0        0        0      395 2023-05-03 12:25:03.774561 landingzone_organization-0.2.2/landingzone_organization/account.py
--rw-r--r--   0        0        0       75 2023-05-03 12:25:03.774561 landingzone_organization-0.2.2/landingzone_organization/adapters/__init__.py
--rw-r--r--   0        0        0     3248 2023-05-03 12:25:03.778561 landingzone_organization-0.2.2/landingzone_organization/adapters/aws_organization.py
--rw-r--r--   0        0        0      509 2023-05-03 12:25:03.778561 landingzone_organization-0.2.2/landingzone_organization/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 12:25:03.778561 landingzone_organization-0.2.2/landingzone_organization/cli/commands/__init__.py
--rw-r--r--   0        0        0      598 2023-05-03 12:25:03.778561 landingzone_organization-0.2.2/landingzone_organization/cli/commands/account.py
--rw-r--r--   0        0        0      558 2023-05-03 12:25:03.778561 landingzone_organization-0.2.2/landingzone_organization/cli/commands/organization.py
--rw-r--r--   0        0        0      707 2023-05-03 12:25:03.778561 landingzone_organization-0.2.2/landingzone_organization/cli/commands/workload.py
--rw-r--r--   0        0        0     1517 2023-05-03 12:25:03.778561 landingzone_organization-0.2.2/landingzone_organization/cli/context.py
--rw-r--r--   0        0        0      744 2023-05-03 12:25:03.778561 landingzone_organization-0.2.2/landingzone_organization/cli/handler.py
--rw-r--r--   0        0        0      666 2023-05-03 12:25:03.778561 landingzone_organization-0.2.2/landingzone_organization/filtering.py
--rw-r--r--   0        0        0     1035 2023-05-03 12:25:03.778561 landingzone_organization-0.2.2/landingzone_organization/group.py
--rw-r--r--   0        0        0      929 2023-05-03 12:25:03.778561 landingzone_organization-0.2.2/landingzone_organization/groups.py
--rw-r--r--   0        0        0     2537 2023-05-03 12:25:03.778561 landingzone_organization-0.2.2/landingzone_organization/organization.py
--rw-r--r--   0        0        0      938 2023-05-03 12:25:03.778561 landingzone_organization-0.2.2/landingzone_organization/organization_unit.py
--rw-r--r--   0        0        0      887 2023-05-03 12:25:03.778561 landingzone_organization-0.2.2/landingzone_organization/workload.py
--rw-r--r--   0        0        0     1559 2023-05-03 12:25:03.778561 landingzone_organization-0.2.2/landingzone_organization/workloads.py
--rw-r--r--   0        0        0     1387 2023-05-03 12:25:04.598577 landingzone_organization-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 landingzone_organization-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      981 2023-05-04 10:23:39.767821 landingzone_organization-0.3.0/README.md
+-rw-r--r--   0        0        0      443 2023-05-04 10:23:40.455830 landingzone_organization-0.3.0/landingzone_organization/__init__.py
+-rw-r--r--   0        0        0      395 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/account.py
+-rw-r--r--   0        0        0       75 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/adapters/__init__.py
+-rw-r--r--   0        0        0     3248 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/adapters/aws_organization.py
+-rw-r--r--   0        0        0      509 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/cli/commands/__init__.py
+-rw-r--r--   0        0        0      598 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/cli/commands/account.py
+-rw-r--r--   0        0        0      558 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/cli/commands/organization.py
+-rw-r--r--   0        0        0     2096 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/cli/commands/profiles.py
+-rw-r--r--   0        0        0      707 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/cli/commands/workload.py
+-rw-r--r--   0        0        0     1517 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/cli/context.py
+-rw-r--r--   0        0        0      744 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/cli/handler.py
+-rw-r--r--   0        0        0      666 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/filtering.py
+-rw-r--r--   0        0        0     1035 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/group.py
+-rw-r--r--   0        0        0      929 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/groups.py
+-rw-r--r--   0        0        0     3220 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/organization.py
+-rw-r--r--   0        0        0      938 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/organization_unit.py
+-rw-r--r--   0        0        0      917 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/profile.py
+-rw-r--r--   0        0        0      887 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/workload.py
+-rw-r--r--   0        0        0     1559 2023-05-04 10:23:39.771821 landingzone_organization-0.3.0/landingzone_organization/workloads.py
+-rw-r--r--   0        0        0     1387 2023-05-04 10:23:40.455830 landingzone_organization-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 landingzone_organization-0.3.0/PKG-INFO
```

### Comparing `landingzone_organization-0.2.2/README.md` & `landingzone_organization-0.3.0/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 [![Continuous Integration](https://github.com/binxio/landingzone-organization/actions/workflows/ci.yml/badge.svg)](https://github.com/binxio/landingzone-organization/actions/workflows/ci.yml)
 
 This module allows you to query your landingzone organization. For example, if you want to know the names of all workloads that run in your AWS Cloud? You can use this module to fetch this information directly from the APIs from AWS.
 
 **Useful links:**
 - [Documentation](https://binxio.github.io/landingzone-organization/)
 - [Bug Tracker](https://github.com/binxio/landingzone-organization/issues)
-- [PyPi](https://pypi.org/project/landingzone-organization/)
+- [PyPi](https://pypi.org/project/landingzone-organization/)
```

### Comparing `landingzone_organization-0.2.2/landingzone_organization/adapters/aws_organization.py` & `landingzone_organization-0.3.0/landingzone_organization/adapters/aws_organization.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.2/landingzone_organization/cli/commands/account.py` & `landingzone_organization-0.3.0/landingzone_organization/cli/commands/account.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.2/landingzone_organization/cli/commands/organization.py` & `landingzone_organization-0.3.0/landingzone_organization/cli/commands/organization.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.2/landingzone_organization/cli/commands/workload.py` & `landingzone_organization-0.3.0/landingzone_organization/cli/commands/workload.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.2/landingzone_organization/cli/context.py` & `landingzone_organization-0.3.0/landingzone_organization/cli/context.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.2/landingzone_organization/cli/handler.py` & `landingzone_organization-0.3.0/landingzone_organization/cli/handler.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.2/landingzone_organization/filtering.py` & `landingzone_organization-0.3.0/landingzone_organization/filtering.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.2/landingzone_organization/group.py` & `landingzone_organization-0.3.0/landingzone_organization/group.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.2/landingzone_organization/groups.py` & `landingzone_organization-0.3.0/landingzone_organization/groups.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.2/landingzone_organization/organization.py` & `landingzone_organization-0.3.0/landingzone_organization/organization.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,35 +2,36 @@
 from typing import List, Optional
 import jsonpickle
 from dataclasses import dataclass
 
 from landingzone_organization.filtering import match_workload_pattern
 from landingzone_organization.account import Account
 from landingzone_organization.organization_unit import OrganizationUnit
+from landingzone_organization.profile import Profile
 from landingzone_organization.workloads import Workloads
 
 
 @dataclass
 class Organization:
     """
     Understands the organization structure
     """
 
     id: str
     unit: OrganizationUnit
 
     @property
-    def all_accounts(self) -> List[Account]:
+    def accounts_recursive(self) -> List[Account]:
         return self.unit.accounts_recursive
 
     def by_name(self, name: str) -> OrganizationUnit:
         return self.unit.by_name(name)
 
     def by_account_id(self, account_id: str) -> Optional[Account]:
-        return next(filter(lambda account: account.account_id == account_id, self.all_accounts), None)  # type: ignore
+        return next(filter(lambda account: account.account_id == account_id, self.accounts_recursive), None)  # type: ignore
 
     def __resolve_organization_unit(
         self, ou_names: List[str]
     ) -> Optional[OrganizationUnit]:
         unit = self.unit
 
         for ou_name in ou_names:
@@ -65,15 +66,34 @@
         workload_account_ids = list(
             map(lambda account: account.account_id, workload_accounts)
         )
 
         def not_a_workload_account(account: Account):
             return account.account_id not in workload_account_ids
 
-        return list(filter(not_a_workload_account, self.all_accounts))
+        return list(filter(not_a_workload_account, self.accounts_recursive))
+
+    def sso_profiles(
+        self,
+        sso_start_url: str,
+        sso_region: str,
+        sso_role_name: str,
+        role_session_name: str,
+    ) -> List[Profile]:
+        def create_profile(account: Account) -> Profile:
+            return Profile(
+                sso_start_url=sso_start_url,
+                sso_region=sso_region,
+                sso_role_name=sso_role_name,
+                role_session_name=role_session_name,
+                account_id=account.account_id,
+                account_name=account.name,
+            )
+
+        return list(map(create_profile, self.accounts_recursive))
 
     def dump(self) -> str:
         return jsonpickle.encode(self)
 
     @staticmethod
     def load(data: str) -> Organization:
         obj = jsonpickle.decode(data)
```

### Comparing `landingzone_organization-0.2.2/landingzone_organization/organization_unit.py` & `landingzone_organization-0.3.0/landingzone_organization/organization_unit.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.2/landingzone_organization/workload.py` & `landingzone_organization-0.3.0/landingzone_organization/workload.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.2/landingzone_organization/workloads.py` & `landingzone_organization-0.3.0/landingzone_organization/workloads.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.2/pyproject.toml` & `landingzone_organization-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "landingzone-organization"
-version = "0.2.2"
+version = "0.3.0"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 readme = "README.md"
 homepage = "https://binxio.github.io/landingzone-organization/"
 documentation = "https://binxio.github.io/landingzone-organization/3-user-documentation/"
 repository = "https://github.com/binxio/landingzone-organization"
 packages = [{include = "landingzone_organization"}]
```

### Comparing `landingzone_organization-0.2.2/PKG-INFO` & `landingzone_organization-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landingzone-organization
-Version: 0.2.2
+Version: 0.3.0
 Summary: 
 Home-page: https://binxio.github.io/landingzone-organization/
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -25,7 +25,8 @@
 
 This module allows you to query your landingzone organization. For example, if you want to know the names of all workloads that run in your AWS Cloud? You can use this module to fetch this information directly from the APIs from AWS.
 
 **Useful links:**
 - [Documentation](https://binxio.github.io/landingzone-organization/)
 - [Bug Tracker](https://github.com/binxio/landingzone-organization/issues)
 - [PyPi](https://pypi.org/project/landingzone-organization/)
+
```

