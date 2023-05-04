# Comparing `tmp/ape-etherscan-0.6.3.tar.gz` & `tmp/ape-etherscan-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-etherscan-0.6.3.tar", last modified: Fri Mar 31 19:01:13 2023, max compression
+gzip compressed data, was "ape-etherscan-0.6.4.tar", last modified: Thu May  4 20:15:14 2023, max compression
```

## Comparing `ape-etherscan-0.6.3.tar` & `ape-etherscan-0.6.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:01:13.414370 ape-etherscan-0.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:01:13.406370 ape-etherscan-0.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:01:13.410370 ape-etherscan-0.6.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:01:13.410370 ape-etherscan-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-03-31 19:01:13.414370 ape-etherscan-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:01:13.410370 ape-etherscan-0.6.3/ape_etherscan/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/ape_etherscan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/ape_etherscan/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/ape_etherscan/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/ape_etherscan/explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/ape_etherscan/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/ape_etherscan/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/ape_etherscan/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/ape_etherscan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/ape_etherscan/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-31 19:01:13.000000 ape-etherscan-0.6.3/ape_etherscan/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:01:13.410370 ape-etherscan-0.6.3/ape_etherscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-03-31 19:01:13.000000 ape-etherscan-0.6.3/ape_etherscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-31 19:01:13.000000 ape-etherscan-0.6.3/ape_etherscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 19:01:13.000000 ape-etherscan-0.6.3/ape_etherscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 19:01:13.000000 ape-etherscan-0.6.3/ape_etherscan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-31 19:01:13.000000 ape-etherscan-0.6.3/ape_etherscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-31 19:01:13.000000 ape-etherscan-0.6.3/ape_etherscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-31 19:01:13.414370 ape-etherscan-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:01:13.410370 ape-etherscan-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:01:13.414370 ape-etherscan-0.6.3/tests/mock_responses/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/tests/mock_responses/get_account_transactions.json
--rw-r--r--   0 runner    (1001) docker     (123)    85181 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/tests/mock_responses/get_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    93453 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/tests/mock_responses/get_proxy_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    93483 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/tests/mock_responses/get_vyper_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-03-31 18:59:44.000000 ape-etherscan-0.6.3/tests/test_etherscan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.030023 ape-etherscan-0.6.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.026023 ape-etherscan-0.6.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.026023 ape-etherscan-0.6.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.026023 ape-etherscan-0.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-04 20:15:14.030023 ape-etherscan-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.030023 ape-etherscan-0.6.4/ape_etherscan/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/ape_etherscan/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 20:15:13.000000 ape-etherscan-0.6.4/ape_etherscan/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.030023 ape-etherscan-0.6.4/ape_etherscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-04 20:15:13.000000 ape-etherscan-0.6.4/ape_etherscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-04 20:15:13.000000 ape-etherscan-0.6.4/ape_etherscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:15:13.000000 ape-etherscan-0.6.4/ape_etherscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:15:13.000000 ape-etherscan-0.6.4/ape_etherscan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-04 20:15:13.000000 ape-etherscan-0.6.4/ape_etherscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 20:15:13.000000 ape-etherscan-0.6.4/ape_etherscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-04 20:15:14.030023 ape-etherscan-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.030023 ape-etherscan-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:15:14.030023 ape-etherscan-0.6.4/tests/mock_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/tests/mock_responses/get_account_transactions.json
+-rw-r--r--   0 runner    (1001) docker     (123)    85181 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/tests/mock_responses/get_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    93453 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/tests/mock_responses/get_proxy_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    93483 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/tests/mock_responses/get_vyper_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-05-04 20:14:16.000000 ape-etherscan-0.6.4/tests/test_etherscan.py
```

### Comparing `ape-etherscan-0.6.3/.github/ISSUE_TEMPLATE/bug.md` & `ape-etherscan-0.6.4/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/.github/ISSUE_TEMPLATE/feature.md` & `ape-etherscan-0.6.4/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/.github/ISSUE_TEMPLATE/work-item.md` & `ape-etherscan-0.6.4/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/.github/release-drafter.yml` & `ape-etherscan-0.6.4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/.github/workflows/codeql.yml` & `ape-etherscan-0.6.4/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/.github/workflows/commit.yaml` & `ape-etherscan-0.6.4/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/.github/workflows/prtitle.yaml` & `ape-etherscan-0.6.4/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/.github/workflows/publish.yaml` & `ape-etherscan-0.6.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/.github/workflows/stale-prs.yml` & `ape-etherscan-0.6.4/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/.github/workflows/test.yaml` & `ape-etherscan-0.6.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/.gitignore` & `ape-etherscan-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/.pre-commit-config.yaml` & `ape-etherscan-0.6.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/CONTRIBUTING.md` & `ape-etherscan-0.6.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/LICENSE` & `ape-etherscan-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/PKG-INFO` & `ape-etherscan-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.6.3
+Version: 0.6.4
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-etherscan-0.6.3/README.md` & `ape-etherscan-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/ape_etherscan/client.py` & `ape-etherscan-0.6.4/ape_etherscan/client.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/ape_etherscan/exceptions.py` & `ape-etherscan-0.6.4/ape_etherscan/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/ape_etherscan/explorer.py` & `ape-etherscan-0.6.4/ape_etherscan/explorer.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/ape_etherscan/query.py` & `ape-etherscan-0.6.4/ape_etherscan/query.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from ape.api import QueryAPI, QueryType, ReceiptAPI
 from ape.api.query import AccountTransactionQuery
 from ape.exceptions import QueryEngineError
 from ape.utils import singledispatchmethod
 
 from ape_etherscan.client import ClientFactory
+from ape_etherscan.utils import NETWORKS
 
 
 class EtherscanQueryEngine(QueryAPI):
     @property
     def _client_factory(self) -> ClientFactory:
         return ClientFactory(
             self.provider.network.ecosystem.name,
@@ -17,15 +18,22 @@
         )
 
     @singledispatchmethod
     def estimate_query(self, query: QueryType) -> Optional[int]:  # type: ignore[override]
         return None
 
     @estimate_query.register
-    def estimate_account_transaction_query(self, query: AccountTransactionQuery) -> int:
+    def estimate_account_transaction_query(self, query: AccountTransactionQuery) -> Optional[int]:
+        if self.network_manager.active_provider:
+            # Ignore unsupported networks.
+            ecosystem = self.network_manager.provider.network.ecosystem.name
+            network = self.network_manager.provider.network.name
+            if network not in NETWORKS.get(ecosystem, {}):
+                return None
+
         # About 15 ms per page of 100 transactions
         return 1500 * (1 + query.stop_nonce - query.start_nonce) // 100
 
     @singledispatchmethod
     def perform_query(self, query: QueryType) -> Iterator:  # type: ignore[override]
         raise QueryEngineError(
             f"{self.__class__.__name__} cannot handle {query.__class__.__name__} queries."
```

### Comparing `ape-etherscan-0.6.3/ape_etherscan/types.py` & `ape-etherscan-0.6.4/ape_etherscan/types.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/ape_etherscan/verify.py` & `ape-etherscan-0.6.4/ape_etherscan/verify.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/ape_etherscan.egg-info/PKG-INFO` & `ape-etherscan-0.6.4/ape_etherscan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.6.3
+Version: 0.6.4
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-etherscan-0.6.3/ape_etherscan.egg-info/SOURCES.txt` & `ape-etherscan-0.6.4/ape_etherscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/ape_etherscan.egg-info/requires.txt` & `ape-etherscan-0.6.4/ape_etherscan.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/pyproject.toml` & `ape-etherscan-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/setup.py` & `ape-etherscan-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/tests/conftest.py` & `ape-etherscan-0.6.4/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,14 +219,15 @@
         com_url = get_url_f(tld="com")
         com_testnet_url = get_url_f(testnet=True, tld="com")
 
         return {
             "ethereum": {
                 "mainnet": url("etherscan"),
                 "goerli": testnet_url("goerli", "etherscan"),
+                "sepolia": testnet_url("sepolia", "etherscan"),
             },
             "arbitrum": {
                 "mainnet": url("arbiscan"),
                 "goerli": testnet_url("goerli", "arbiscan"),
             },
             "fantom": {
                 "opera": com_url("ftmscan"),
```

### Comparing `ape-etherscan-0.6.3/tests/mock_responses/get_account_transactions.json` & `ape-etherscan-0.6.4/tests/mock_responses/get_account_transactions.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/tests/mock_responses/get_contract_response.json` & `ape-etherscan-0.6.4/tests/mock_responses/get_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/tests/mock_responses/get_proxy_contract_response.json` & `ape-etherscan-0.6.4/tests/mock_responses/get_proxy_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/tests/mock_responses/get_vyper_contract_response.json` & `ape-etherscan-0.6.4/tests/mock_responses/get_vyper_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.3/tests/test_etherscan.py` & `ape-etherscan-0.6.4/tests/test_etherscan.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 base_url_test = pytest.mark.parametrize(
     "ecosystem,network,url",
     [
         ("ethereum", "mainnet", "etherscan.io"),
         ("ethereum", "mainnet-fork", "etherscan.io"),
         ("ethereum", "goerli", "goerli.etherscan.io"),
         ("ethereum", "goerli-fork", "goerli.etherscan.io"),
+        ("ethereum", "sepolia", "sepolia.etherscan.io"),
         ("fantom", "opera", "ftmscan.com"),
         ("fantom", "opera-fork", "ftmscan.com"),
         ("fantom", "testnet", "testnet.ftmscan.com"),
         ("fantom", "testnet-fork", "testnet.ftmscan.com"),
         ("arbitrum", "mainnet", "arbiscan.io"),
         ("arbitrum", "mainnet-fork", "arbiscan.io"),
         ("arbitrum", "goerli", "goerli.arbiscan.io"),
```

