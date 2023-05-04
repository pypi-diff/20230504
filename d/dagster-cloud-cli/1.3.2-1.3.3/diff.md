# Comparing `tmp/dagster_cloud_cli-1.3.2.tar.gz` & `tmp/dagster_cloud_cli-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud_cli-1.3.2.tar", last modified: Thu Apr 27 19:42:16 2023, max compression
+gzip compressed data, was "dagster_cloud_cli-1.3.3.tar", last modified: Thu May  4 17:55:45 2023, max compression
```

## Comparing `dagster_cloud_cli-1.3.2.tar` & `dagster_cloud_cli-1.3.3.tar`

### file list

```diff
@@ -1,81 +1,87 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:16.069875 dagster_cloud_cli-1.3.2/
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-27 19:42:16.065875 dagster_cloud_cli-1.3.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:14.873871 dagster_cloud_cli-1.3.2/dagster_cloud_cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:14.881871 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:14.881871 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/branch_deployment/
--rw-r--r--   0 root         (0) root         (0)     4612 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/branch_deployment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7791 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/ci.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:14.889871 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/deployment/
--rw-r--r--   0 root         (0) root         (0)     1508 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:14.945871 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/deployment/alert_policies/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
--rw-r--r--   0 root         (0) root         (0)     5883 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:14.953871 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/job/
--rw-r--r--   0 root         (0) root         (0)     1926 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3454 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:14.957871 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/organization/
--rw-r--r--   0 root         (0) root         (0)     2129 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:14.957871 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/organization/saml/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/organization/saml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2707 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/organization/saml/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:14.961871 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/run/
--rw-r--r--   0 root         (0) root         (0)      669 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/run/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:14.973872 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/serverless/
--rw-r--r--   0 root         (0) root         (0)     1499 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/serverless/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      628 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
--rw-r--r--   0 root         (0) root         (0)    19784 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/serverless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:14.981871 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/workspace/
--rw-r--r--   0 root         (0) root         (0)    11997 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17972 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/config_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:15.037872 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      424 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/_utils.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/docker_runner.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/errors.py
--rw-r--r--   0 root         (0) root         (0)     9228 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:15.041872 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/headers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/headers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/headers/auth.py
--rw-r--r--   0 root         (0) root         (0)      958 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/headers/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:15.041872 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/headers/versioning/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/headers/versioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/headers/versioning/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:15.513873 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/code_location.py
--rw-r--r--   0 root         (0) root         (0)     9467 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/deploy.py
--rw-r--r--   0 root         (0) root         (0)    13847 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/deps.py
--rw-r--r--   0 root         (0) root         (0)     5976 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/github_context.py
--rw-r--r--   0 root         (0) root         (0)     1232 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/parse_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4655 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/pex_registry.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/selftest.py
--rw-r--r--   0 root         (0) root         (0)     4496 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/source.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/util.py
--rw-r--r--   0 root         (0) root         (0)     1920 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pydantic_yaml.py
--rw-r--r--   0 root         (0) root         (0)     5384 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/workspace.py
--rw-r--r--   0 root         (0) root         (0)     6700 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    18577 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/gql.py
--rw-r--r--   0 root         (0) root         (0)     5859 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/pex_utils.py
--rw-r--r--   0 root         (0) root         (0)     1378 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/types.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/ui.py
--rw-r--r--   0 root         (0) root         (0)     3434 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:14.873871 dagster_cloud_cli-1.3.2/dagster_cloud_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-27 19:42:14.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2566 2023-04-27 19:42:14.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:42:14.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-27 19:42:14.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2023-04-27 19:42:14.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-27 19:42:14.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:42:15.837874 dagster_cloud_cli-1.3.2/dagster_cloud_cli_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2738 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli_tests/test_check.py
--rw-r--r--   0 root         (0) root         (0)      659 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli_tests/test_gql.py
--rw-r--r--   0 root         (0) root         (0)     8588 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/dagster_cloud_cli_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 19:42:16.069875 dagster_cloud_cli-1.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1101 2023-04-27 18:31:35.000000 dagster_cloud_cli-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.817916 dagster_cloud_cli-1.3.3/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-04 17:55:45.817916 dagster_cloud_cli-1.3.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.793916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.793916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.793916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/branch_deployment/
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/branch_deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.797916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/ci/
+-rw-r--r--   0 root         (0) root         (0)    17040 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/ci/checks.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/ci/state.py
+-rw-r--r--   0 root         (0) root         (0)      529 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/ci/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.797916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.797916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/alert_policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
+-rw-r--r--   0 root         (0) root         (0)     5883 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.797916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/job/
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.801916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/organization/
+-rw-r--r--   0 root         (0) root         (0)     2129 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.801916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/organization/saml/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/organization/saml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/organization/saml/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.801916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/run/
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/run/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.801916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/serverless/
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/serverless/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      628 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/serverless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.805916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/workspace/
+-rw-r--r--   0 root         (0) root         (0)    11997 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17972 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/config_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.809916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      424 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/docker_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     9228 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.809916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/auth.py
+-rw-r--r--   0 root         (0) root         (0)      958 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.809916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/versioning/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/versioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/versioning/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.817916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     9467 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/deploy.py
+-rw-r--r--   0 root         (0) root         (0)    13847 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/deps.py
+-rw-r--r--   0 root         (0) root         (0)     5976 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/github_context.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/parse_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/pex_registry.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/selftest.py
+-rw-r--r--   0 root         (0) root         (0)     4496 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/source.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/util.py
+-rw-r--r--   0 root         (0) root         (0)     1920 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pydantic_yaml.py
+-rw-r--r--   0 root         (0) root         (0)     5384 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/workspace.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6700 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    18577 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/gql.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/pex_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/types.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/ui.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.793916 dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-04 17:55:45.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2765 2023-05-04 17:55:45.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:55:45.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-04 17:55:45.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2023-05-04 17:55:45.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-04 17:55:45.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.817916 dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2738 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/test_check.py
+-rw-r--r--   0 root         (0) root         (0)      659 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/test_gql.py
+-rw-r--r--   0 root         (0) root         (0)     8588 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     9821 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/test_state.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 17:55:45.817916 dagster_cloud_cli-1.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/setup.py
```

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/branch_deployment/__init__.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/branch_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/config.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/deployment/__init__.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/deployment/alert_policies/commands.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/alert_policies/commands.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/job/__init__.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/job/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/metrics.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/organization/__init__.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/organization/saml/commands.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/organization/saml/commands.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/run/__init__.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/run/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/serverless/Dockerfile` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/serverless/Dockerfile`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/serverless/__init__.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/serverless/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import base64
 import json
 import os
 import subprocess
-import sys
-import uuid
-from contextlib import contextmanager
 from pathlib import Path
 from typing import List
 
-import pkg_resources
 from typer import Argument, Option, Typer
 
-from dagster_cloud_cli import gql, pex_utils, ui
+from dagster_cloud_cli import docker_utils, gql, pex_utils, ui
 from dagster_cloud_cli.commands import metrics
 from dagster_cloud_cli.commands.workspace import wait_for_load
 from dagster_cloud_cli.config_utils import (
     DEPLOYMENT_CLI_OPTIONS,
     dagster_cloud_options,
     get_location_document,
 )
@@ -74,47 +70,14 @@
             exists=False,
             help="Environment variable to be defined in image, in the form of `MY_ENV_VAR=hello`",
         ),
     ),
 }
 
 
-@contextmanager
-def _template_dockerfile(env_vars, custom_base_image=None):
-    DOCKERFILE_TEMPLATE = pkg_resources.resource_filename(
-        "dagster_cloud_cli", "commands/serverless/Dockerfile"
-    )
-    base_image_command = (
-        f"FROM {custom_base_image}" if custom_base_image else "FROM python:3.8-slim"
-    )
-    with open(DOCKERFILE_TEMPLATE, "r", encoding="utf-8") as template:
-        dockerfile_content = "\n".join(
-            [base_image_command, template.read(), *[f"ENV {env_var}" for env_var in env_vars]]
-        )
-
-        yield bytes(dockerfile_content, "utf-8")
-
-
-def _build_image(source_directory, image, registry_info, env_vars, base_image):
-    registry = registry_info["registry_url"]
-    with _template_dockerfile(env_vars, base_image) as dockerfile_content:
-        cmd = [
-            "docker",
-            "build",
-            source_directory,
-            "-t",
-            f"{registry}:{image}",
-            "-f",
-            "-",
-            "--platform",
-            "linux/amd64",
-        ]
-        return subprocess.run(cmd, input=dockerfile_content, check=True).returncode
-
-
 @app.command(name="build", short_help="Build image for Dagster Cloud code location.", hidden=True)
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 @add_options(_BUILD_OPTIONS)
 @metrics.instrument(CliEventType.BUILD, tags=[CliEventTags.server_strategy.docker])
 def build_command(
     api_token: str,
     url: str,
@@ -123,51 +86,29 @@
     image: str = Argument(None, help="Image name."),
     **kwargs,
 ):
     """Add or update the image for a code location in the workspace."""
     source_directory = str(kwargs.get("source_directory"))
     base_image = kwargs.get("base_image")
     env_vars = kwargs.get("env", [])
-    _verify_docker()
+    docker_utils.verify_docker()
 
     with gql.graphql_client_from_url(url, api_token) as client:
         ecr_info = gql.get_ecr_info(client)
         registry = ecr_info["registry_url"]
 
         if base_image and not ecr_info.get("allow_custom_base"):
             ui.warn("Custom base images are not enabled for this organization.")
             base_image = None
 
-        retval = _build_image(source_directory, image, ecr_info, env_vars, base_image)
+        retval = docker_utils.build_image(source_directory, image, ecr_info, env_vars, base_image)
         if retval == 0:
             ui.print(f"Built image {registry}:{image}")
 
 
-def _upload_image(image, registry_info):
-    registry = registry_info["registry_url"]
-    aws_token = registry_info["aws_auth_token"]
-    if not registry or not aws_token:
-        raise ui.error(
-            "No registry found. You may need to wait for your Dagster serverless deployment to"
-            " activate."
-        )
-
-    username, password = base64.b64decode(aws_token).decode("utf-8").split(":")
-    subprocess.check_output(
-        (
-            f"echo {str(password)} | docker login --username {str(username)} --password-stdin"
-            f" {registry}"
-        ),
-        shell=True,
-    )
-    return subprocess.call(
-        ["docker", "push", f"{registry}:{image}"], stderr=sys.stderr, stdout=sys.stdout
-    )
-
-
 @app.command(
     name="upload",
     short_help="Upload the built code location image to Dagster Cloud's image repository.",
     hidden=True,
 )
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 @metrics.instrument(CliEventType.UPLOAD, tags=[CliEventTags.server_strategy.docker])
@@ -176,20 +117,20 @@
     url: str,
     location_load_timeout: int,
     agent_heartbeat_timeout: int,
     image: str = Argument(None, help="Image name."),
     **kwargs,
 ):
     """Add or update the image for a code location in the workspace."""
-    _verify_docker()
+    docker_utils.verify_docker()
 
     with gql.graphql_client_from_url(url, api_token) as client:
         ecr_info = gql.get_ecr_info(client)
         registry = ecr_info["registry_url"]
-        retval = _upload_image(image, ecr_info)
+        retval = docker_utils.upload_image(image, ecr_info)
         if retval == 0:
             ui.print(f"Pushed image {image} to {registry}")
 
 
 @app.command(
     name="registry-info",
     short_help="Get registry information and temporary creds for an image repository",
@@ -257,32 +198,35 @@
             "No location name provided. You must specify the location name as an argument."
         )
 
     if not source_directory:
         raise ui.error("No source directory provided.")
 
     _check_source_directory(source_directory)
-    _verify_docker()
+    docker_utils.verify_docker()
 
     env_vars = kwargs.get("env", [])
     base_image = kwargs.get("base_image")
 
     with gql.graphql_client_from_url(url, api_token) as client:
         ecr_info = gql.get_ecr_info(client)
         registry = ecr_info["registry_url"]
 
-        commit_hash = kwargs.get("commit_hash") or str(uuid.uuid4().hex)
-        default_image_tag = f"{deployment}-{location_name}-{commit_hash}"
-        image_tag = kwargs.get("image") or default_image_tag
+        image_tag = kwargs.get(
+            "image",
+            docker_utils.default_image_tag(deployment, location_name, kwargs.get("commit_hash")),
+        )
 
-        retval = _build_image(source_directory, image_tag, ecr_info, env_vars, base_image)
+        retval = docker_utils.build_image(
+            source_directory, image_tag, ecr_info, env_vars, base_image
+        )
         if retval != 0:
             return
 
-        retval = _upload_image(image_tag, ecr_info)
+        retval = docker_utils.upload_image(image_tag, ecr_info)
         if retval != 0:
             return
 
         location_args = {**kwargs, "image": f"{registry}:{image_tag}"}
         location_document = get_location_document(location_name, location_args)
         gql.add_or_update_code_location(client, location_document)
 
@@ -341,15 +285,15 @@
             subprocess.run(cmd, check=True, capture_output=True)
         except subprocess.CalledProcessError as err:
             raise ui.error(
                 f"Error tagging local image {local_image}: " + err.stderr.decode("utf-8")
             )
 
         # upload tagged image
-        retval = _upload_image(image=published_tag, registry_info=ecr_info)
+        retval = docker_utils.upload_image(image=published_tag, registry_info=ecr_info)
         if retval == 0:
             ui.print(f"Pushed image {published_tag} to {registry}.")
             ui.print(
                 "To use the uploaded image run: "
                 f"dagster-cloud deploy-python-executable --base-image-tag={published_tag} [ARGS]"
             )
 
@@ -553,19 +497,14 @@
         workspace_url = f"{url}/locations"
         ui.print(
             f"Added or updated locations: {', '.join([location.name for location in locations])}. "
             f"View the status of your workspace at {workspace_url}."
         )
 
 
-def _verify_docker():
-    if subprocess.call("docker -v", shell=True) != 0:
-        raise ui.error("Docker must be installed locally to deploy to Dagster Cloud Serverless")
-
-
 SOURCE_INSTRUCTIONS = (
     "You can specify the directory you want to deploy by using the `--source-directory` argument "
     "(defaults to current directory)."
 )
 
 
 def _check_source_directory(source_directory):
```

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/commands/workspace/__init__.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/config_utils.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/docker_runner.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/docker_runner.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/errors.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/graphql_client.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/graphql_client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/headers/impl.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/impl.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/code_location.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/deploy.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/deploy.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/deps.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/deps.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/github_context.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/github_context.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/parse_workspace.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/parse_workspace.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/pex_registry.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/pex_registry.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/selftest.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/selftest.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/source.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/source.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pex_builder/util.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/util.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/pydantic_yaml.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pydantic_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/core/workspace.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/entrypoint.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/gql.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/gql.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/pex_utils.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/pex_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/types.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/types.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/ui.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/ui.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli/utils.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,17 @@
             },
         )
 
         @functools.wraps(to_wrap)
         def wrap_function(*args, **kwargs):
             modified_kwargs = kwargs
             if not has_kwargs and not hasattr(to_wrap, "modified_options"):
-                modified_kwargs = {k: v for k, v in kwargs.items() if k in to_wrap_sig.parameters}
+                modified_kwargs: dict[Any, Any] = {
+                    k: v for k, v in kwargs.items() if k in to_wrap_sig.parameters
+                }
             return to_wrap(*args, **modified_kwargs)
 
         wrap_function.__signature__ = sig
         wrap_function.modified_options = True
         return wrap_function
 
     return decorator
```

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli.egg-info/SOURCES.txt` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 MANIFEST.in
 setup.py
 dagster_cloud_cli/__init__.py
 dagster_cloud_cli/config_utils.py
+dagster_cloud_cli/docker_utils.py
 dagster_cloud_cli/entrypoint.py
 dagster_cloud_cli/gql.py
 dagster_cloud_cli/pex_utils.py
 dagster_cloud_cli/types.py
 dagster_cloud_cli/ui.py
 dagster_cloud_cli/utils.py
 dagster_cloud_cli/version.py
 dagster_cloud_cli.egg-info/PKG-INFO
 dagster_cloud_cli.egg-info/SOURCES.txt
 dagster_cloud_cli.egg-info/dependency_links.txt
 dagster_cloud_cli.egg-info/entry_points.txt
 dagster_cloud_cli.egg-info/requires.txt
 dagster_cloud_cli.egg-info/top_level.txt
 dagster_cloud_cli/commands/__init__.py
-dagster_cloud_cli/commands/ci.py
 dagster_cloud_cli/commands/config.py
 dagster_cloud_cli/commands/metrics.py
 dagster_cloud_cli/commands/branch_deployment/__init__.py
+dagster_cloud_cli/commands/ci/__init__.py
+dagster_cloud_cli/commands/ci/checks.py
+dagster_cloud_cli/commands/ci/state.py
+dagster_cloud_cli/commands/ci/utils.py
 dagster_cloud_cli/commands/deployment/__init__.py
 dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
 dagster_cloud_cli/commands/deployment/alert_policies/commands.py
 dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
 dagster_cloud_cli/commands/job/__init__.py
 dagster_cloud_cli/commands/organization/__init__.py
 dagster_cloud_cli/commands/organization/saml/__init__.py
@@ -54,8 +58,9 @@
 dagster_cloud_cli/core/pex_builder/pex_registry.py
 dagster_cloud_cli/core/pex_builder/selftest.py
 dagster_cloud_cli/core/pex_builder/source.py
 dagster_cloud_cli/core/pex_builder/util.py
 dagster_cloud_cli_tests/__init__.py
 dagster_cloud_cli_tests/test_check.py
 dagster_cloud_cli_tests/test_gql.py
-dagster_cloud_cli_tests/test_metrics.py
+dagster_cloud_cli_tests/test_metrics.py
+dagster_cloud_cli_tests/test_state.py
```

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli_tests/test_check.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/test_check.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli_tests/test_gql.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/test_gql.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/dagster_cloud_cli_tests/test_metrics.py` & `dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.2/setup.py` & `dagster_cloud_cli-1.3.3/setup.py`

 * *Files identical despite different names*

