# Comparing `tmp/vgs-cli-1.9.4.tar.gz` & `tmp/vgs-cli-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vgs-cli-1.9.4.tar", last modified: Mon Dec 13 10:51:12 2021, max compression
+gzip compressed data, was "vgs-cli-1.9.5.tar", last modified: Fri Dec 17 12:46:08 2021, max compression
```

## Comparing `vgs-cli-1.9.4.tar` & `vgs-cli-1.9.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-13 10:51:12.445244 vgs-cli-1.9.4/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1082 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3777 2021-12-13 10:51:12.445244 vgs-cli-1.9.4/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3213 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      407 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      116 2021-12-13 10:51:12.445244 vgs-cli-1.9.4/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1512 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      110 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/test-requirements.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-13 10:51:12.441244 vgs-cli-1.9.4/vgs_cli.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3777 2021-12-13 10:51:12.000000 vgs-cli-1.9.4/vgs_cli.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1335 2021-12-13 10:51:12.000000 vgs-cli-1.9.4/vgs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-12-13 10:51:12.000000 vgs-cli-1.9.4/vgs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       58 2021-12-13 10:51:12.000000 vgs-cli-1.9.4/vgs_cli.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-12-13 10:51:11.000000 vgs-cli-1.9.4/vgs_cli.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      527 2021-12-13 10:51:12.000000 vgs-cli-1.9.4/vgs_cli.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2021-12-13 10:51:12.000000 vgs-cli-1.9.4/vgs_cli.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-13 10:51:12.445244 vgs-cli-1.9.4/vgscli/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      786 2021-12-13 10:50:33.000000 vgs-cli-1.9.4/vgscli/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1837 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/access_logs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2281 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/accounts_api.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-13 10:51:12.445244 vgs-cli-1.9.4/vgscli/api/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/api/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1659 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/api/account_mgmt.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1437 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/api/vault_mgmt.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3194 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/audits_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1815 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/auth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2116 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/auth_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3743 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/auth_server.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      602 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/auth_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1056 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/callback_server.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-13 10:51:12.445244 vgs-cli-1.9.4/vgscli/cli/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/cli/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-13 10:51:12.445244 vgs-cli-1.9.4/vgscli/cli/commands/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/cli/commands/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4546 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/cli/commands/apply.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      606 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/cli/commands/generate.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-13 10:51:12.445244 vgs-cli-1.9.4/vgscli/cli/types/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      107 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/cli/types/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1171 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/cli/types/resource_id.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      413 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/cli/types/variable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3115 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/click_extensions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1513 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/config_file.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6101 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      689 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/file_token_util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1538 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/id_generator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3598 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/keyring_token_util.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-13 10:51:12.445244 vgs-cli-1.9.4/vgscli/resource-templates/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-13 10:51:12.445244 vgs-cli-1.9.4/vgscli/resource-templates/service-account/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/resource-templates/service-account/calm.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      156 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/resource-templates/service-account/vgs-cli.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      383 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/resource-templates/vault-template.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1447 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/routes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2459 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/serializers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1222 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/testing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      172 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/text.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      184 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/token_handler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3393 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-13 10:51:12.445244 vgs-cli-1.9.4/vgscli/validation-schemas/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      617 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/validation-schemas/service-account-schema.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      622 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/validation-schemas/vault-schema.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/vaults_api.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     9255 2021-12-13 10:50:30.000000 vgs-cli-1.9.4/vgscli/vgs.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-17 12:46:08.603143 vgs-cli-1.9.5/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1082 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3777 2021-12-17 12:46:08.603143 vgs-cli-1.9.5/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3213 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      407 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      116 2021-12-17 12:46:08.603143 vgs-cli-1.9.5/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1512 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      110 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/test-requirements.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-17 12:46:08.599143 vgs-cli-1.9.5/vgs_cli.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3777 2021-12-17 12:46:08.000000 vgs-cli-1.9.5/vgs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1335 2021-12-17 12:46:08.000000 vgs-cli-1.9.5/vgs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-12-17 12:46:08.000000 vgs-cli-1.9.5/vgs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       58 2021-12-17 12:46:08.000000 vgs-cli-1.9.5/vgs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-12-17 12:46:07.000000 vgs-cli-1.9.5/vgs_cli.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      527 2021-12-17 12:46:08.000000 vgs-cli-1.9.5/vgs_cli.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2021-12-17 12:46:08.000000 vgs-cli-1.9.5/vgs_cli.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-17 12:46:08.603143 vgs-cli-1.9.5/vgscli/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      786 2021-12-17 12:45:27.000000 vgs-cli-1.9.5/vgscli/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1837 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/access_logs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2281 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/accounts_api.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-17 12:46:08.603143 vgs-cli-1.9.5/vgscli/api/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/api/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1659 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/api/account_mgmt.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1437 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/api/vault_mgmt.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3194 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/audits_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1815 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/auth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2116 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/auth_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3743 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/auth_server.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      602 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/auth_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1056 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/callback_server.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-17 12:46:08.603143 vgs-cli-1.9.5/vgscli/cli/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/cli/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-17 12:46:08.603143 vgs-cli-1.9.5/vgscli/cli/commands/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/cli/commands/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4546 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/cli/commands/apply.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      606 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/cli/commands/generate.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-17 12:46:08.603143 vgs-cli-1.9.5/vgscli/cli/types/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      107 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/cli/types/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1171 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/cli/types/resource_id.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      413 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/cli/types/variable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3115 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/click_extensions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1513 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/config_file.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6101 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      689 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/file_token_util.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1538 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/id_generator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3598 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/keyring_token_util.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-17 12:46:08.603143 vgs-cli-1.9.5/vgscli/resource-templates/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-17 12:46:08.603143 vgs-cli-1.9.5/vgscli/resource-templates/service-account/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/resource-templates/service-account/calm.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      156 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/resource-templates/service-account/vgs-cli.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      383 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/resource-templates/vault-template.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1447 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/routes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2459 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/serializers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1222 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/testing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      172 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/text.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      184 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/token_handler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3393 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-12-17 12:46:08.603143 vgs-cli-1.9.5/vgscli/validation-schemas/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      617 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/validation-schemas/service-account-schema.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      622 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/validation-schemas/vault-schema.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/vaults_api.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     9410 2021-12-17 12:45:24.000000 vgs-cli-1.9.5/vgscli/vgs.py
```

### Comparing `vgs-cli-1.9.4/LICENSE` & `vgs-cli-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/PKG-INFO` & `vgs-cli-1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgs-cli
-Version: 1.9.4
+Version: 1.9.5
 Summary: VGS Client
 Home-page: https://github.com/verygoodsecurity/vgs-cli
 Author: Very Good Security
 Author-email: dev@verygoodsecurity.com
 License: BSD
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `vgs-cli-1.9.4/README.md` & `vgs-cli-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/setup.py` & `vgs-cli-1.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgs_cli.egg-info/PKG-INFO` & `vgs-cli-1.9.5/vgs_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgs-cli
-Version: 1.9.4
+Version: 1.9.5
 Summary: VGS Client
 Home-page: https://github.com/verygoodsecurity/vgs-cli
 Author: Very Good Security
 Author-email: dev@verygoodsecurity.com
 License: BSD
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `vgs-cli-1.9.4/vgs_cli.egg-info/SOURCES.txt` & `vgs-cli-1.9.5/vgs_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgs_cli.egg-info/requires.txt` & `vgs-cli-1.9.5/vgs_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/_version.py` & `vgs-cli-1.9.5/vgscli/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import click
 import requests
 from semver import VersionInfo
 
 from vgscli.text import bold, green
 
-__version__ = '1.9.4'
+__version__ = '1.9.5'
 
 
 # noinspection PyBroadException
 def get_latest_version(**kwargs) -> Optional[VersionInfo]:
     try:
         response_json = requests.get('https://pypi.org/pypi/vgs-cli/json', **kwargs).json()
         return VersionInfo.parse(response_json['info']['version'])
```

### Comparing `vgs-cli-1.9.4/vgscli/access_logs.py` & `vgs-cli-1.9.5/vgscli/access_logs.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/accounts_api.py` & `vgs-cli-1.9.5/vgscli/accounts_api.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/api/__init__.py` & `vgs-cli-1.9.5/vgscli/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/api/account_mgmt.py` & `vgs-cli-1.9.5/vgscli/api/account_mgmt.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/api/vault_mgmt.py` & `vgs-cli-1.9.5/vgscli/api/vault_mgmt.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/audits_api.py` & `vgs-cli-1.9.5/vgscli/audits_api.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/auth.py` & `vgs-cli-1.9.5/vgscli/auth.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/auth_api.py` & `vgs-cli-1.9.5/vgscli/auth_api.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/auth_server.py` & `vgs-cli-1.9.5/vgscli/auth_server.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/auth_utils.py` & `vgs-cli-1.9.5/vgscli/auth_utils.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/callback_server.py` & `vgs-cli-1.9.5/vgscli/callback_server.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/cli/commands/apply.py` & `vgs-cli-1.9.5/vgscli/cli/commands/apply.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/cli/commands/generate.py` & `vgs-cli-1.9.5/vgscli/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/cli/types/resource_id.py` & `vgs-cli-1.9.5/vgscli/cli/types/resource_id.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/click_extensions.py` & `vgs-cli-1.9.5/vgscli/click_extensions.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/config_file.py` & `vgs-cli-1.9.5/vgscli/config_file.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/errors.py` & `vgs-cli-1.9.5/vgscli/errors.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/file_token_util.py` & `vgs-cli-1.9.5/vgscli/file_token_util.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/id_generator.py` & `vgs-cli-1.9.5/vgscli/id_generator.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/keyring_token_util.py` & `vgs-cli-1.9.5/vgscli/keyring_token_util.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/routes.py` & `vgs-cli-1.9.5/vgscli/routes.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/serializers.py` & `vgs-cli-1.9.5/vgscli/serializers.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/testing.py` & `vgs-cli-1.9.5/vgscli/testing.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/utils.py` & `vgs-cli-1.9.5/vgscli/utils.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/validation-schemas/service-account-schema.yaml` & `vgs-cli-1.9.5/vgscli/validation-schemas/service-account-schema.yaml`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/validation-schemas/vault-schema.yaml` & `vgs-cli-1.9.5/vgscli/validation-schemas/vault-schema.yaml`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/vaults_api.py` & `vgs-cli-1.9.5/vgscli/vaults_api.py`

 * *Files identical despite different names*

### Comparing `vgs-cli-1.9.4/vgscli/vgs.py` & `vgs-cli-1.9.5/vgscli/vgs.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,17 @@
               type=DateTimeDuration(formats=["%Y-%m-%dT%H:%M:%S"]))
 @click.option('--tail', help='Number of log records to show. Defaults to all logs if unspecified.', default=-1,
               callback=validate_tail)
 @click.option('--until',
               help='Only show logs older than a relative duration like 30s, 5m, or 3h or before a specific RFC 3339 date.',
               type=DateTimeDuration(formats=["%Y-%m-%dT%H:%M:%S"]))
 @click.option('--vault', '-V', help="Vault ID", required=True)
+@click.option('--proxy', '-P', help="Show access logs for a specific proxy", type=click.Choice(['http', 'sftp', 'tcp']))
 @click.pass_context
-def access(ctx, vault, **kwargs):
+def access(ctx, vault, proxy, **kwargs):
     """
     Get access logs
 
     \b\bExamples:
 
     # Show access logs available for a vault\t\t\t\t\t\t
     vgs logs access -V <VAULT_ID>
@@ -129,14 +130,15 @@
     """
     handshake(ctx, ctx.obj.env)
 
     audits_api = create_audits_api(ctx, vault, ctx.obj.env, token_util.get_access_token())
 
     filters = prepare_filter({
         'tenant_id': vault,
+        'protocol': proxy,
         'from': kwargs.get('since'),
         'to': kwargs.get('until'),
     })
 
     for res in fetch_logs(audits_api, filters, kwargs.get('tail')):
         click.echo(format_logs(wrap_records(res), kwargs.get('output')))
```

