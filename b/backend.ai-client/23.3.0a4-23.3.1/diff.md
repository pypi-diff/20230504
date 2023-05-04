# Comparing `tmp/backend.ai-client-23.3.0a4.tar.gz` & `tmp/backend.ai-client-23.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-client-23.3.0a4.tar", last modified: Thu Mar 16 02:53:02 2023, max compression
+gzip compressed data, was "backend.ai-client-23.3.1.tar", last modified: Thu May  4 05:10:16 2023, max compression
```

## Comparing `backend.ai-client-23.3.0a4.tar` & `backend.ai-client-23.3.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:02.968271 backend.ai-client-23.3.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-03-16 02:53:02.964271 backend.ai-client-23.3.0a4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:02.948270 backend.ai-client-23.3.0a4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:02.948270 backend.ai-client-23.3.0a4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:02.952270 backend.ai-client-23.3.0a4/ai/backend/client/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:02.956270 backend.ai-client-23.3.0a4/ai/backend/client/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:02.960271 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/license.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9526 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/pretty.py
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    31706 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/server_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    47595 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26776 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/cli/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:02.964271 backend.ai-client-23.3.0a4/ai/backend/client/func/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/bgtask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/keypair_resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/server_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    49910 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21853 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/func/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/load_balancing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:02.964271 backend.ai-client-23.3.0a4/ai/backend/client/output/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/output/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/output/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/output/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/output/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/output/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30106 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    16829 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/ai/backend/client/versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:02.964271 backend.ai-client-23.3.0a4/backend.ai_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/backend.ai_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/backend.ai_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/backend.ai_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/backend.ai_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/backend.ai_client.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/backend.ai_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/backend.ai_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/backend.ai_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 02:53:02.968271 backend.ai-client-23.3.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-03-16 02:53:02.000000 backend.ai-client-23.3.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.510685 backend.ai-client-23.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-05-04 05:10:16.510685 backend.ai-client-23.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.498685 backend.ai-client-23.3.1/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.498685 backend.ai-client-23.3.1/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.502685 backend.ai-client-23.3.1/ai/backend/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.502685 backend.ai-client-23.3.1/ai/backend/client/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.506685 backend.ai-client-23.3.1/ai/backend/client/cli/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/admin/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31836 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/server_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48183 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/cli/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.506685 backend.ai-client-23.3.1/ai/backend/client/func/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/bgtask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/keypair_resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/server_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49999 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22380 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/func/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/load_balancing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.510685 backend.ai-client-23.3.1/ai/backend/client/output/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/output/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/output/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/output/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/output/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/output/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    30097 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16938 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/ai/backend/client/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.510685 backend.ai-client-23.3.1/backend.ai_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-05-04 05:10:16.000000 backend.ai-client-23.3.1/backend.ai_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-04 05:10:16.000000 backend.ai-client-23.3.1/backend.ai_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:16.000000 backend.ai-client-23.3.1/backend.ai_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 05:10:16.000000 backend.ai-client-23.3.1/backend.ai_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:16.000000 backend.ai-client-23.3.1/backend.ai_client.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:16.000000 backend.ai-client-23.3.1/backend.ai_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-04 05:10:16.000000 backend.ai-client-23.3.1/backend.ai_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 05:10:16.000000 backend.ai-client-23.3.1/backend.ai_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:16.510685 backend.ai-client-23.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-05-04 05:10:15.000000 backend.ai-client-23.3.1/setup.py
```

### Comparing `backend.ai-client-23.3.0a4/PKG-INFO` & `backend.ai-client-23.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-client
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Client SDK
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/x-rst
 
 Backend.AI Client
 =================
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/auth.py` & `backend.ai-client-23.3.1/ai/backend/client/auth.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/__init__.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/acl.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/agent.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/domain.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,18 @@
 @click.option("-d", "--description", type=str, default="", help="Description of new domain")
 @click.option("-i", "--inactive", is_flag=True, help="New domain will be inactive.")
 @click.option("--total-resource-slots", type=str, default="{}", help="Set total resource slots.")
 @click.option(
     "--allowed-vfolder-hosts",
     type=str,
     default="{}",
-    help="Allowed virtual folder hosts. "
-    'It must be JSON string (e.g: --allowed-vfolder-hosts=\'{"HOST_NAME": ["create-vfolder", "modify-vfolder"]}\')',
+    help=(
+        "Allowed virtual folder hosts. It must be JSON string (e.g:"
+        ' --allowed-vfolder-hosts=\'{"HOST_NAME": ["create-vfolder", "modify-vfolder"]}\')'
+    ),
 )
 @click.option(
     "--allowed-docker-registries", type=str, multiple=True, help="Allowed docker registries."
 )
 def add(
     ctx: CLIContext,
     name,
@@ -121,16 +123,18 @@
 @click.option("--new-name", type=str, help="New name of the domain")
 @click.option("--description", type=str, help="Description of the domain")
 @click.option("--is-active", type=bool, help="Set domain inactive.")
 @click.option("--total-resource-slots", type=str, help="Update total resource slots.")
 @click.option(
     "--allowed-vfolder-hosts",
     type=str,
-    help="Allowed virtual folder hosts. "
-    'It must be JSON string (e.g: --allowed-vfolder-hosts=\'{"HOST_NAME": ["create-vfolder", "modify-vfolder"]}\')',
+    help=(
+        "Allowed virtual folder hosts. It must be JSON string (e.g:"
+        ' --allowed-vfolder-hosts=\'{"HOST_NAME": ["create-vfolder", "modify-vfolder"]}\')'
+    ),
 )
 @click.option(
     "--allowed-docker-registries", type=str, multiple=True, help="Allowed docker registries."
 )
 def update(
     ctx: CLIContext,
     name,
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/etcd.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/group.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,18 @@
 @click.option("-d", "--description", type=str, default="", help="Description of new group.")
 @click.option("-i", "--inactive", is_flag=True, help="New group will be inactive.")
 @click.option("--total-resource-slots", type=str, default="{}", help="Set total resource slots.")
 @click.option(
     "--allowed-vfolder-hosts",
     type=str,
     default="{}",
-    help="Allowed virtual folder hosts. "
-    'It must be JSON string (e.g: --allowed-vfolder-hosts=\'{"HOST_NAME": ["create-vfolder", "modify-vfolder"]}\')',
+    help=(
+        "Allowed virtual folder hosts. It must be JSON string (e.g:"
+        ' --allowed-vfolder-hosts=\'{"HOST_NAME": ["create-vfolder", "modify-vfolder"]}\')'
+    ),
 )
 def add(
     ctx: CLIContext,
     domain_name,
     name,
     description,
     inactive,
@@ -147,16 +149,18 @@
 @click.option("-n", "--name", type=str, help="New name of the group")
 @click.option("-d", "--description", type=str, help="Description of the group")
 @click.option("--is-active", type=bool, help="Set group inactive.")
 @click.option("--total-resource-slots", type=str, help="Update total resource slots.")
 @click.option(
     "--allowed-vfolder-hosts",
     type=str,
-    help="Allowed virtual folder hosts. "
-    'It must be JSON string (e.g: --allowed-vfolder-hosts=\'{"HOST_NAME": ["create-vfolder", "modify-vfolder"]}\')',
+    help=(
+        "Allowed virtual folder hosts. It must be JSON string (e.g:"
+        ' --allowed-vfolder-hosts=\'{"HOST_NAME": ["create-vfolder", "modify-vfolder"]}\')'
+    ),
 )
 def update(
     ctx: CLIContext, gid, name, description, is_active, total_resource_slots, allowed_vfolder_hosts
 ):
     """
     Update an existing group. Domain name is not necessary since group ID is unique.
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/image.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 @image.command()
 @click.option(
     "-r",
     "--registry",
     type=str,
     default=None,
-    help='The name (usually hostname or "lablup") ' "of the Docker registry configured.",
+    help='The name (usually hostname or "lablup") of the Docker registry configured.',
 )
 def rescan(registry: str) -> None:
     """
     Update the kernel image metadata from all configured docker registries.
     """
 
     async def rescan_images_impl(registry: str) -> None:
@@ -82,15 +82,15 @@
                                 pbar.write(data["message"])
                                 pbar.update(data["current_progress"] - pbar.n)
                         elif ev.event == "bgtask_failed":
                             error_msg = data["message"]
                             completion_msg_func = lambda: print_fail(f"Error occurred: {error_msg}")
                         elif ev.event == "bgtask_cancelled":
                             completion_msg_func = lambda: print_warn(
-                                "Registry scanning has been " "cancelled in the middle."
+                                "Registry scanning has been cancelled in the middle."
                             )
             finally:
                 completion_msg_func()
 
     asyncio_run(rescan_images_impl(registry))
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/keypair.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/license.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/license.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/manager.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,26 +37,26 @@
         sys.exit(ExitCode.FAILURE)
 
 
 @manager.command()
 @click.option(
     "--wait",
     is_flag=True,
-    help="Hold up freezing the manager until " "there are no running sessions in the manager.",
+    help="Hold up freezing the manager until there are no running sessions in the manager.",
 )
 @click.option(
     "--force-kill",
     is_flag=True,
     help="Kill all running sessions immediately and freeze the manager.",
 )
 def freeze(wait, force_kill):
     """Freeze manager."""
     if wait and force_kill:
         print(
-            "You cannot use both --wait and --force-kill options " "at the same time.",
+            "You cannot use both --wait and --force-kill options at the same time.",
             file=sys.stderr,
         )
         return
     try:
         with Session() as session:
             if wait:
                 while True:
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/resource.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/resource_policy.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/resource_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 @keypair_resource_policy.command()
 @pass_ctx_obj
 @click.argument("name", type=str, default=None, metavar="NAME")
 @click.option(
     "--default-for-unspecified",
     type=str,
     default="UNLIMITED",
-    help="Default behavior for unspecified resources: " "LIMITED, UNLIMITED",
+    help="Default behavior for unspecified resources: LIMITED, UNLIMITED",
 )
 @click.option("--total-resource-slots", type=str, default="{}", help="Set total resource slots.")
 @click.option(
     "--max-session-lifetime", type=int, default=0, help="Maximum lifetime to keep session alive."
 )
 @click.option(
     "--max-concurrent-sessions", type=int, default=30, help="Number of maximum concurrent sessions."
@@ -89,26 +89,28 @@
 @click.option(
     "--max-vfolder-size", type=int, default=0, help="Maximum virtual folder size (future plan)."
 )
 @click.option(
     "--idle-timeout",
     type=int,
     default=1800,
-    help="The maximum period of time allowed for kernels to wait " "further requests.",
+    help="The maximum period of time allowed for kernels to wait further requests.",
 )
 @click.option(
     "--allowed-vfolder-hosts",
     type=str,
     default=json.dumps(
         {
             "local:volume1": [perm.value for perm in VFolderHostPermission],
         }
     ),
-    help="Allowed virtual folder hosts. "
-    'It must be JSON string (e.g: --allowed-vfolder-hosts=\'{"HOST_NAME": ["create-vfolder", "modify-vfolder"]}\')',
+    help=(
+        "Allowed virtual folder hosts. It must be JSON string (e.g:"
+        ' --allowed-vfolder-hosts=\'{"HOST_NAME": ["create-vfolder", "modify-vfolder"]}\')'
+    ),
 )
 def add(
     ctx: CLIContext,
     name,
     default_for_unspecified,
     total_resource_slots,
     max_session_lifetime,
@@ -160,36 +162,38 @@
 
 @keypair_resource_policy.command()
 @pass_ctx_obj
 @click.argument("name", type=str, default=None, metavar="NAME")
 @click.option(
     "--default-for-unspecified",
     type=str,
-    help="Default behavior for unspecified resources: " "LIMITED, UNLIMITED",
+    help="Default behavior for unspecified resources: LIMITED, UNLIMITED",
 )
 @click.option("--total-resource-slots", type=str, help="Set total resource slots.")
 @click.option(
     "--max-session-lifetime", type=int, default=0, help="Maximum lifetime to keep session alive."
 )
 @click.option("--max-concurrent-sessions", type=int, help="Number of maximum concurrent sessions.")
 @click.option(
     "--max-containers-per-session", type=int, help="Number of maximum containers per session."
 )
 @click.option("--max-vfolder-count", type=int, help="Number of maximum virtual folders allowed.")
 @click.option("--max-vfolder-size", type=int, help="Maximum virtual folder size (future plan).")
 @click.option(
     "--idle-timeout",
     type=int,
-    help="The maximum period of time allowed for kernels to wait " "further requests.",
+    help="The maximum period of time allowed for kernels to wait further requests.",
 )
 @click.option(
     "--allowed-vfolder-hosts",
     type=str,
-    help="Allowed virtual folder hosts. "
-    'It must be JSON string (e.g: --allowed-vfolder-hosts=\'{"HOST_NAME": ["create-vfolder", "modify-vfolder"]}\')',
+    help=(
+        "Allowed virtual folder hosts. It must be JSON string (e.g:"
+        ' --allowed-vfolder-hosts=\'{"HOST_NAME": ["create-vfolder", "modify-vfolder"]}\')'
+    ),
 )
 def update(
     ctx: CLIContext,
     name,
     default_for_unspecified,
     total_resource_slots,
     max_session_lifetime,
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/scaling_group.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/scaling_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,14 +67,23 @@
 
 
 @scaling_group.command()
 @pass_ctx_obj
 @click.argument("name", type=str, metavar="NAME")
 @click.option("-d", "--description", type=str, default="", help="Description of new scaling group")
 @click.option("-i", "--inactive", is_flag=True, help="New scaling group will be inactive.")
+@click.option(
+    "-p",
+    "--private",
+    is_flag=True,
+    help=(
+        "New scaling group will be private. "
+        "Private scaling groups cannot be used when users create new sessions."
+    ),
+)
 @click.option("--driver", type=str, default="static", help="Set driver.")
 @click.option(
     "--driver-opts", type=JSONParamType(), default="{}", help="Set driver options as a JSON string."
 )
 @click.option("--scheduler", type=str, default="fifo", help="Set scheduler.")
 @click.option(
     "--scheduler-opts",
@@ -86,14 +95,15 @@
     "--use-host-network", is_flag=True, help="If true, run containers on host networking mode."
 )
 def add(
     ctx: CLIContext,
     name,
     description,
     inactive,
+    private,
     driver,
     driver_opts,
     scheduler,
     scheduler_opts,
     use_host_network,
 ):
     """
@@ -103,14 +113,15 @@
     """
     with Session() as session:
         try:
             data = session.ScalingGroup.create(
                 name,
                 description=description,
                 is_active=not inactive,
+                is_public=not private,
                 driver=driver,
                 driver_opts=driver_opts,
                 scheduler=scheduler,
                 scheduler_opts=scheduler_opts,
                 use_host_network=use_host_network,
             )
         except Exception as e:
@@ -134,14 +145,23 @@
 
 
 @scaling_group.command()
 @pass_ctx_obj
 @click.argument("name", type=str, metavar="NAME")
 @click.option("-d", "--description", type=str, default="", help="Description of new scaling group")
 @click.option("-i", "--inactive", is_flag=True, help="New scaling group will be inactive.")
+@click.option(
+    "-p",
+    "--private",
+    is_flag=True,
+    help=(
+        "The scaling group will be private. "
+        "Private scaling groups cannot be used when users create new sessions."
+    ),
+)
 @click.option("--driver", type=str, default="static", help="Set driver.")
 @click.option(
     "--driver-opts", type=JSONParamType(), default=None, help="Set driver options as a JSON string."
 )
 @click.option("--scheduler", type=str, default="fifo", help="Set scheduler.")
 @click.option(
     "--scheduler-opts",
@@ -153,14 +173,15 @@
     "--use-host-network", is_flag=True, help="If true, run containers on host networking mode."
 )
 def update(
     ctx: CLIContext,
     name,
     description,
     inactive,
+    private,
     driver,
     driver_opts,
     scheduler,
     scheduler_opts,
     use_host_network,
 ):
     """
@@ -170,14 +191,15 @@
     """
     with Session() as session:
         try:
             data = session.ScalingGroup.update(
                 name,
                 description=description,
                 is_active=not inactive,
+                is_public=not private,
                 driver=driver,
                 driver_opts=driver_opts,
                 scheduler=scheduler,
                 scheduler_opts=scheduler_opts,
                 use_host_network=use_host_network,
             )
         except Exception as e:
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/session.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         ),
         help="Filter by the given status",
     )
     @click.option(
         "--access-key",
         type=str,
         default=None,
-        help="Get sessions for a specific access key " "(only works if you are a super-admin)",
+        help="Get sessions for a specific access key (only works if you are a super-admin)",
     )
     @click.option("--name-only", is_flag=True, help="Display session names only.")
     @click.option(
         "--dead", is_flag=True, help="Filter only dead sessions. Ignores --status option."
     )
     @click.option(
         "--running",
@@ -82,15 +82,18 @@
     )
     @click.option("--limit", default=None, type=int, help="The page size for pagination.")
     @click.option(
         "-a",
         "--all",
         is_flag=True,
         default=False,
-        help='Alias of "backend.ai ps --status=ALL" listing all sessions regardless of status. Ignores --status option.',
+        help=(
+            'Alias of "backend.ai ps --status=ALL" listing all sessions regardless of status.'
+            " Ignores --status option."
+        ),
     )
     def list(
         ctx: CLIContext,
         status: str | None,
         access_key: str | None,
         name_only: str | None,
         dead: bool,
@@ -251,22 +254,23 @@
                     session_fields["tag"],
                     session_fields["created_at"],
                     session_fields["terminated_at"],
                     session_fields["status"],
                     session_fields["status_info"],
                     session_fields["status_data"],
                     session_fields["occupying_slots"],
+                    session_fields["idle_checks"],
                 ]
             )
             if session_.api_version[0] >= 6:
                 fields.append(session_fields["containers"])
             else:
                 fields.append(session_fields_v5["containers"])
             fields.append(session_fields["dependencies"])
-            q = "query($id: UUID!) {" "  compute_session(id: $id) {" "    $fields" "  }" "}"
+            q = "query($id: UUID!) {  compute_session(id: $id) {    $fields  }}"
             try:
                 uuid.UUID(session_id)
             except ValueError:
                 print_fail("In API v5 or later, the session ID must be given in the UUID format.")
                 sys.exit(ExitCode.FAILURE)
             v = {"id": session_id}
             q = q.replace("$fields", " ".join(f.field_ref for f in fields))
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/storage.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/user.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,23 +188,27 @@
     type=str,
     default="active",
     help="Account status. One of (active, inactive, deleted, before-verification).",
 )
 @click.option(
     "--need-password-change",
     is_flag=True,
-    help="Flag indicate that user needs to change password. "
-    "Useful when admin manually create password.",
+    help=(
+        "Flag indicate that user needs to change password. "
+        "Useful when admin manually create password."
+    ),
 )
 @click.option(
     "--allowed-ip",
     type=list_expr,
     default=None,
-    help="Allowed client IP. IPv4 and IPv6 are allowed. CIDR type is recommended. "
-    '(e.g., --allowed-ip "127.0.0.1","127.0.0.2",...)',
+    help=(
+        "Allowed client IP. IPv4 and IPv6 are allowed. CIDR type is recommended. "
+        '(e.g., --allowed-ip "127.0.0.1","127.0.0.2",...)'
+    ),
 )
 @click.option("--description", type=str, default="", help="Description of the user.")
 def add(
     ctx: CLIContext,
     domain_name,
     email,
     password,
@@ -276,23 +280,27 @@
     "--status",
     type=str,
     help="Account status. One of (active, inactive, deleted, before-verification).",
 )
 @click.option(
     "--need-password-change",
     is_flag=True,
-    help="Flag indicate that user needs to change password. "
-    "Useful when admin manually create password.",
+    help=(
+        "Flag indicate that user needs to change password. "
+        "Useful when admin manually create password."
+    ),
 )
 @click.option(
     "--allowed-ip",
     type=list_expr,
     default=None,
-    help="Allowed client IP. IPv4 and IPv6 are allowed. CIDR type is recommended. "
-    '(e.g., --allowed-ip "127.0.0.1","127.0.0.2",...)',
+    help=(
+        "Allowed client IP. IPv4 and IPv6 are allowed. CIDR type is recommended. "
+        '(e.g., --allowed-ip "127.0.0.1","127.0.0.2",...)'
+    ),
 )
 @click.option("--description", type=str, default="", help="Description of the user.")
 def update(
     ctx: CLIContext,
     email,
     password,
     username,
@@ -384,17 +392,19 @@
 @user.command()
 @pass_ctx_obj
 @click.argument("email", type=str, metavar="EMAIL")
 @click.option(
     "--purge-shared-vfolders",
     is_flag=True,
     default=False,
-    help="Delete user's all virtual folders. "
-    "If False, shared folders will not be deleted "
-    "and migrated the ownership to the requested admin.",
+    help=(
+        "Delete user's all virtual folders. "
+        "If False, shared folders will not be deleted "
+        "and migrated the ownership to the requested admin."
+    ),
 )
 def purge(ctx: CLIContext, email, purge_shared_vfolders):
     """
     Delete an existing user. This action cannot be undone.
 
     \b
     NAME: Name of a domain to delete.
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/admin/vfolder.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/admin/vfolder.py`

 * *Files 6% similar despite different names*

```diff
@@ -373,7 +373,27 @@
         try:
             resp = session.VFolder.update_shared_vfolder(vfolder_id, user_id, None)
             print("Removed.")
         except Exception as e:
             print_error(e)
             sys.exit(ExitCode.FAILURE)
         print(resp)
+
+
+@vfolder.command()
+@click.argument("vfolder_id", type=str)
+@click.argument("user_email", type=str)
+def change_vfolder_ownership(vfolder_id, user_email):
+    """
+    Change the ownership of vfolder
+
+    \b
+    VFOLDER_ID: ID of a virtual folder.
+    USER_EMAIL:  user email to have the ownership of current vfolder
+    """
+    with Session() as session:
+        try:
+            session.VFolder.change_vfolder_ownership(vfolder_id, user_email)
+            print(f"Now ownership of VFolder:{vfolder_id} goes to User:{user_email}")
+        except Exception as e:
+            print_error(e)
+            sys.exit(ExitCode.FAILURE)
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/announcement.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/announcement.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/app.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/app.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/config.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/dotfile.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/dotfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,21 @@
 
 
 @dotfile.command()
 @click.argument("path", metavar="PATH")
 @click.option(
     "--perm",
     "permission",
-    help="Linux permission represented in octal number (e.g. 755) "
-    "Defaults to 755 if not specified",
+    help="Linux permission represented in octal number (e.g. 755) Defaults to 755 if not specified",
 )
 @click.option(
     "-f",
     "--file",
     "dotfile_path",
-    help="Path to dotfile to upload. "
-    "If not specified, client will try to read file from STDIN. ",
+    help="Path to dotfile to upload. If not specified, client will try to read file from STDIN. ",
 )
 @click.option(
     "-o",
     "--owner",
     "--owner-access-key",
     "owner_access_key",
     metavar="ACCESS_KEY",
@@ -41,16 +39,18 @@
 @click.option(
     "-d", "--domain", "domain", metavar="DOMAIN", help="Specify the domain name of domain dotfiles."
 )
 @click.option(
     "-g",
     "--group",
     metavar="GROUP",
-    help="Specify the group name or id of group dotfiles. "
-    "(If group name is provided, domain name must be specified with option -d)",
+    help=(
+        "Specify the group name or id of group dotfiles. "
+        "(If group name is provided, domain name must be specified with option -d)"
+    ),
 )
 def create(path, permission, dotfile_path, owner_access_key, domain, group):
     """
     Store dotfile to Backend.AI Manager.
     Dotfiles will be automatically loaded when creating kernels.
 
     PATH: Where dotfiles will be created when starting kernel
@@ -94,16 +94,18 @@
 @click.option(
     "-d", "--domain", "domain", metavar="DOMAIN", help="Specify the domain name of domain dotfiles."
 )
 @click.option(
     "-g",
     "--group",
     metavar="GROUP",
-    help="Specify the group name or id of group dotfiles. "
-    "(If group name is provided, domain name must be specified with option -d)",
+    help=(
+        "Specify the group name or id of group dotfiles. "
+        "(If group name is provided, domain name must be specified with option -d)"
+    ),
 )
 def get(path, owner_access_key, domain, group):
     """
     Print dotfile content.
     """
     with Session() as session:
         try:
@@ -129,16 +131,18 @@
 @click.option(
     "-d", "--domain", "domain", metavar="DOMAIN", help="Specify the domain name of domain dotfiles."
 )
 @click.option(
     "-g",
     "--group",
     metavar="GROUP",
-    help="Specify the group name or id of group dotfiles. "
-    "(If group name is provided, domain name must be specified with option -d)",
+    help=(
+        "Specify the group name or id of group dotfiles. "
+        "(If group name is provided, domain name must be specified with option -d)"
+    ),
 )
 def list(owner_access_key, domain, group):
     """
     List available user/domain/group dotfiles.
     """
     fields = [
         ("Path", "path", None),
@@ -168,23 +172,21 @@
 
 
 @dotfile.command()
 @click.argument("path", metavar="PATH")
 @click.option(
     "--perm",
     "permission",
-    help="Linux permission represented in octal number (e.g. 755) "
-    "Defaults to 755 if not specified",
+    help="Linux permission represented in octal number (e.g. 755) Defaults to 755 if not specified",
 )
 @click.option(
     "-f",
     "--file",
     "dotfile_path",
-    help="Path to dotfile to upload. "
-    "If not specified, client will try to read file from STDIN. ",
+    help="Path to dotfile to upload. If not specified, client will try to read file from STDIN. ",
 )
 @click.option(
     "-o",
     "--owner",
     "--owner-access-key",
     "owner_access_key",
     metavar="ACCESS_KEY",
@@ -193,16 +195,18 @@
 @click.option(
     "-d", "--domain", "domain", metavar="DOMAIN", help="Specify the domain name of domain dotfiles."
 )
 @click.option(
     "-g",
     "--group",
     metavar="GROUP",
-    help="Specify the group name or id of group dotfiles. "
-    "(If group name is provided, domain name must be specified with option -d)",
+    help=(
+        "Specify the group name or id of group dotfiles. "
+        "(If group name is provided, domain name must be specified with option -d)"
+    ),
 )
 def update(path, permission, dotfile_path, owner_access_key, domain, group):
     """
     Update dotfile stored in Backend.AI Manager.
     """
 
     if dotfile_path:
@@ -240,16 +244,18 @@
 @click.option(
     "-d", "--domain", "domain", metavar="DOMAIN", help="Specify the domain name of domain dotfiles."
 )
 @click.option(
     "-g",
     "--group",
     metavar="GROUP",
-    help="Specify the group name or id of group dotfiles. "
-    "(If group name is provided, domain name must be specified with option -d)",
+    help=(
+        "Specify the group name or id of group dotfiles. "
+        "(If group name is provided, domain name must be specified with option -d)"
+    ),
 )
 def delete(path, force, owner_access_key, domain, group):
     """
     Delete dotfile from Backend.AI Manager.
     """
     with Session() as session:
         dotfile_ = session.Dotfile(
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/extensions.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/extensions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/logs.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/main.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/main.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/model.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,36 +100,42 @@
     help="Group ID or NAME.",
 )
 @click.option(
     "--unmanaged",
     "host_path",
     type=bool,
     is_flag=True,
-    help="Treats HOST as a mount point of unmanaged model. "
-    "This option can only be used by Admin or Superadmin.",
+    help=(
+        "Treats HOST as a mount point of unmanaged model. "
+        "This option can only be used by Admin or Superadmin."
+    ),
 )
 @click.option(
     "-p",
     "--permission",
     metavar="PERMISSION",
     type=str,
     default="rw",
-    help="Folder's innate permission. "
-    'Group folders can be shared as read-only by setting this option to "ro". '
-    "Invited folders override this setting by its own invitation permission.",
+    help=(
+        "Folder's innate permission. "
+        'Group folders can be shared as read-only by setting this option to "ro". '
+        "Invited folders override this setting by its own invitation permission."
+    ),
 )
 @click.option(
     "-q",
     "--quota",
     metavar="QUOTA",
     type=ByteSizeParamCheckType(),
     default="0",
-    help="Quota of the virtual folder. "
-    "(Use 'm' for megabytes, 'g' for gigabytes, and etc.) "
-    "Default is maximum amount possible.",
+    help=(
+        "Quota of the virtual folder. "
+        "(Use 'm' for megabytes, 'g' for gigabytes, and etc.) "
+        "Default is maximum amount possible."
+    ),
 )
 @click.option(
     "--cloneable",
     "--allow-clone",
     type=bool,
     is_flag=True,
     help="Allows the virtual folder to be cloned by users.",
@@ -197,33 +203,39 @@
 @click.argument("filenames", type=Path, nargs=-1)
 @click.argument("model_version", metavar="MODEL_VER", type=str)
 @click.option(
     "-b",
     "--base-dir",
     type=Path,
     default=None,
-    help="The local parent directory which contains the file to be uploaded.  "
-    "[default: current working directry]",
+    help=(
+        "The local parent directory which contains the file to be uploaded.  "
+        "[default: current working directry]"
+    ),
 )
 @click.option(
     "--chunk-size",
     type=ByteSizeParamType(),
     default=humanize.naturalsize(DEFAULT_CHUNK_SIZE, binary=True, gnu=True),
-    help='Transfer the file with the given chunk size with binary suffixes (e.g., "16m"). '
-    "Set this between 8 to 64 megabytes for high-speed disks (e.g., SSD RAID) "
-    "and networks (e.g., 40 GbE) for the maximum throughput.",
+    help=(
+        'Transfer the file with the given chunk size with binary suffixes (e.g., "16m"). '
+        "Set this between 8 to 64 megabytes for high-speed disks (e.g., SSD RAID) "
+        "and networks (e.g., 40 GbE) for the maximum throughput."
+    ),
 )
 @click.option(
     "--override-storage-proxy",
     type=CommaSeparatedKVListParamType(),
     default=None,
-    help="Overrides storage proxy address. "
-    'The value must shape like "X1=Y1,X2=Y2...". '
-    "Each Yn address must at least include the IP address "
-    "or the hostname and may include the protocol part and the port number to replace.",
+    help=(
+        "Overrides storage proxy address. "
+        'The value must shape like "X1=Y1,X2=Y2...". '
+        "Each Yn address must at least include the IP address "
+        "or the hostname and may include the protocol part and the port number to replace."
+    ),
 )
 def upload(
     ctx: CLIContext,
     model_name,
     filenames,
     model_version,
     base_dir,
@@ -262,33 +274,39 @@
 @click.argument("filenames", type=Path, nargs=-1)
 @click.argument("model_version", metavar="MODEL_VER", type=str)
 @click.option(
     "-b",
     "--base-dir",
     type=Path,
     default=None,
-    help="The local parent directory which will contain the downloaded file.  "
-    "[default: current working directry]",
+    help=(
+        "The local parent directory which will contain the downloaded file.  "
+        "[default: current working directry]"
+    ),
 )
 @click.option(
     "--chunk-size",
     type=ByteSizeParamType(),
     default=humanize.naturalsize(DEFAULT_CHUNK_SIZE, binary=True, gnu=True),
-    help='Transfer the file with the given chunk size with binary suffixes (e.g., "16m"). '
-    "Set this between 8 to 64 megabytes for high-speed disks (e.g., SSD RAID) "
-    "and networks (e.g., 40 GbE) for the maximum throughput.",
+    help=(
+        'Transfer the file with the given chunk size with binary suffixes (e.g., "16m"). '
+        "Set this between 8 to 64 megabytes for high-speed disks (e.g., SSD RAID) "
+        "and networks (e.g., 40 GbE) for the maximum throughput."
+    ),
 )
 @click.option(
     "--override-storage-proxy",
     type=CommaSeparatedKVListParamType(),
     default=None,
-    help="Overrides storage proxy address. "
-    'The value must shape like "X1=Y1,X2=Y2...". '
-    "Each Yn address must at least include the IP address "
-    "or the hostname and may include the protocol part and the port number to replace.",
+    help=(
+        "Overrides storage proxy address. "
+        'The value must shape like "X1=Y1,X2=Y2...". '
+        "Each Yn address must at least include the IP address "
+        "or the hostname and may include the protocol part and the port number to replace."
+    ),
 )
 @click.option(
     "--max-retries",
     type=int,
     default=20,
     help="Maximum retry attempt when any failure occurs.",
 )
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/pagination.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/pagination.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/params.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/params.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/pretty.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/pretty.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     return "\x1b[3m" + text + "\x1b[23m"
 
 
 def format_pretty(msg, status=PrintStatus.NONE, colored=True):
     if status == PrintStatus.NONE:
         indicator = style("\u2219", fg="bright_cyan", reset=False)
     elif status == PrintStatus.WAITING:
-        indicator = style("\u22EF", fg="bright_yellow", reset=False)
+        indicator = style("\u22ef", fg="bright_yellow", reset=False)
     elif status == PrintStatus.DONE:
         indicator = style("\u2714", fg="bright_green", reset=False)
     elif status == PrintStatus.FAILED:
         indicator = style("\u2718", fg="bright_red", reset=False)
     elif status == PrintStatus.WARNING:
         indicator = style("\u2219", fg="yellow", reset=False)
     else:
@@ -76,15 +76,15 @@
 def print_pretty(msg, *, status=PrintStatus.NONE, file=None):
     if file is None:
         file = sys.stderr
     if status == PrintStatus.NONE:
         indicator = style("\u2219", fg="bright_cyan", reset=False)
     elif status == PrintStatus.WAITING:
         assert "\n" not in msg, "Waiting message must be a single line."
-        indicator = style("\u22EF", fg="bright_yellow", reset=False)
+        indicator = style("\u22ef", fg="bright_yellow", reset=False)
     elif status == PrintStatus.DONE:
         indicator = style("\u2713", fg="bright_green", reset=False)
     elif status == PrintStatus.FAILED:
         indicator = style("\u2717", fg="bright_red", reset=False)
     elif status == PrintStatus.WARNING:
         indicator = style("\u2219", fg="yellow", reset=False)
     else:
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/proxy.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
     "--bind", type=str, default="localhost", help="The IP/host address to bind this proxy."
 )
 @click.option(
     "-p",
     "--port",
     type=int,
     default=8084,
-    help="The TCP port to accept non-encrypted non-authorized " "API requests.",
+    help="The TCP port to accept non-encrypted non-authorized API requests.",
 )
 @click.pass_context
 def proxy(ctx, bind, port):
     """
     Run a non-encrypted non-authorized API proxy server.
     Use this only for development and testing!
     """
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/run.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,15 @@
 @click.argument("image", type=str)
 @click.argument("files", nargs=-1, type=click.Path())
 @click.option(
     "-t",
     "--name",
     "--client-token",
     metavar="NAME",
-    help="Specify a human-readable session name. " "If not set, a random hex string is used.",
+    help="Specify a human-readable session name. If not set, a random hex string is used.",
 )
 # job scheduling options
 @click.option(
     "--type",
     metavar="SESSTYPE",
     type=click.Choice(["batch", "interactive"]),
     default="interactive",
@@ -319,16 +319,18 @@
 @click.option("--build", metavar="CMD", help="Custom shell command for building the given files")
 @click.option("--exec", metavar="CMD", help="Custom shell command for executing the given files")
 @click.option(
     "--basedir",
     metavar="PATH",
     type=click.Path(),
     default=None,
-    help="Base directory path of uploaded files. "
-    "All uploaded files must reside inside this directory.",
+    help=(
+        "Base directory path of uploaded files. "
+        "All uploaded files must reside inside this directory."
+    ),
 )
 # execution environment
 @click.option(
     "-e",
     "--env",
     metavar="KEY=VAL",
     type=str,
@@ -342,21 +344,21 @@
     type=click.File("r"),
     default=None,
     help="A user-defined script to execute on startup.",
 )
 @click.option(
     "--rm",
     is_flag=True,
-    help="Terminate the session immediately after running " "the given code or files",
+    help="Terminate the session immediately after running the given code or files",
 )
 @click.option(
     "-s",
     "--stats",
     is_flag=True,
-    help="Show resource usage statistics after termination " '(only works if "--rm" is given)',
+    help='Show resource usage statistics after termination (only works if "--rm" is given)',
 )
 @click.option("--tag", type=str, default=None, help="User-defined tag string to annotate sessions.")
 @click.option(
     "-q",
     "--quiet",
     is_flag=True,
     help="Hide execution details but show only the compute_session outputs.",
@@ -396,37 +398,41 @@
     "--volume",
     "-m",
     "--mount",
     "mount",
     metavar="NAME[=PATH]",
     type=str,
     multiple=True,
-    help="User-owned virtual folder names to mount. "
-    "If path is not provided, virtual folder will be mounted under /home/work. "
-    "When the target path is relative, it is placed under /home/work "
-    "with auto-created parent directories if any. "
-    "Absolute paths are mounted as-is, but it is prohibited to "
-    "override the predefined Linux system directories.",
+    help=(
+        "User-owned virtual folder names to mount. "
+        "If path is not provided, virtual folder will be mounted under /home/work. "
+        "When the target path is relative, it is placed under /home/work "
+        "with auto-created parent directories if any. "
+        "Absolute paths are mounted as-is, but it is prohibited to "
+        "override the predefined Linux system directories."
+    ),
 )
 @click.option(
     "--scaling-group",
     "--sgroup",
     type=str,
     default=None,
-    help="The scaling group to execute session. If not specified, "
-    "all available scaling groups are included in the scheduling.",
+    help=(
+        "The scaling group to execute session. If not specified, "
+        "all available scaling groups are included in the scheduling."
+    ),
 )
 @click.option(
     "-r",
     "--resources",
     "--resource",
     metavar="KEY=VAL",
     type=str,
     multiple=True,
-    help="Set computation resources " "(e.g: -r cpu=2 -r mem=256 -r cuda.device=1)",
+    help="Set computation resources (e.g: -r cpu=2 -r mem=256 -r cuda.device=1)",
 )
 @click.option(
     "--cluster-size",
     metavar="NUMBER",
     type=int,
     default=1,
     help="The size of cluster in number of containers.",
@@ -439,15 +445,15 @@
     help="The mode of clustering.",
 )
 @click.option(
     "--resource-opts",
     metavar="KEY=VAL",
     type=str,
     multiple=True,
-    help="Resource options for creating compute session. " "(e.g: shmem=64m)",
+    help="Resource options for creating compute session. (e.g: shmem=64m)",
 )
 @click.option(
     "--arch",
     "--architecture",
     "architecture",
     metavar="ARCH_NAME",
     type=str,
@@ -456,33 +462,39 @@
 )
 # resource grouping
 @click.option(
     "-d",
     "--domain",
     metavar="DOMAIN_NAME",
     default=None,
-    help="Domain name where the session will be spawned. "
-    "If not specified, config's domain name will be used.",
+    help=(
+        "Domain name where the session will be spawned. "
+        "If not specified, config's domain name will be used."
+    ),
 )
 @click.option(
     "-g",
     "--group",
     metavar="GROUP_NAME",
     default=None,
-    help="Group name where the session is spawned. "
-    "User should be a member of the group to execute the code.",
+    help=(
+        "Group name where the session is spawned. "
+        "User should be a member of the group to execute the code."
+    ),
 )
 @click.option("--preopen", default=None, type=list_expr, help="Pre-open service ports")
 @click.option(
     "--assign-agent",
     default=None,
     type=list_expr,
-    help="Show mapping list of tuple which mapped containers with agent. "
-    "When user role is Super Admin. "
-    "(e.g., --assign-agent agent_id_1,agent_id_2,...)",
+    help=(
+        "Show mapping list of tuple which mapped containers with agent. "
+        "When user role is Super Admin. "
+        "(e.g., --assign-agent agent_id_1,agent_id_2,...)"
+    ),
 )
 def run(
     image,
     files,
     name,  # base args
     type,
     starts_at,
@@ -531,22 +543,22 @@
     if quiet:
         vprint_info = vprint_wait = vprint_done = _noop
     else:
         vprint_info = print_info
         vprint_wait = print_wait
         vprint_done = print_done
     if files and code:
-        print(
-            "You can run only either source files or command-line " "code snippet.", file=sys.stderr
-        )
+        print("You can run only either source files or command-line code snippet.", file=sys.stderr)
         sys.exit(ExitCode.INVALID_ARGUMENT)
     if not files and not code:
         print(
-            "You should provide the command-line code snippet using "
-            '"-c" option if run without files.',
+            (
+                "You should provide the command-line code snippet using "
+                '"-c" option if run without files.'
+            ),
             file=sys.stderr,
         )
         sys.exit(ExitCode.INVALID_ARGUMENT)
 
     envs = prepare_env_arg(env)
     resources = prepare_resource_arg(resources)
     resource_opts = prepare_resource_arg(resource_opts)
@@ -596,15 +608,15 @@
             interpolated_exec = "*"
         case_set[(interpolated_envs, interpolated_build, interpolated_exec)] = 1
 
     is_multi = len(case_set) > 1
     if is_multi:
         if max_parallel <= 0:
             print(
-                "The number maximum parallel sessions must be " "a positive integer.",
+                "The number maximum parallel sessions must be a positive integer.",
                 file=sys.stderr,
             )
             sys.exit(ExitCode.INVALID_ARGUMENT)
         if terminal:
             print("You cannot run multiple cases with terminal.", file=sys.stderr)
             sys.exit(ExitCode.INVALID_ARGUMENT)
         if not quiet:
@@ -689,15 +701,15 @@
                         "batch",
                         "",
                         opts=opts,
                         vprint_done=vprint_done,
                     )
             if terminal:
                 raise NotImplementedError(
-                    "Terminal access is not supported in " "the legacy synchronous mode."
+                    "Terminal access is not supported in the legacy synchronous mode."
                 )
             if code:
                 exec_loop_sync(
                     sys.stdout, sys.stderr, compute_session, "query", code, vprint_done=vprint_done
                 )
             vprint_done("[{0}] Execution finished.".format(idx))
         except Exception as e:
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/server_log.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/server_log.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/service.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/session.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 def _create_cmd(docs: str = None):
     @click.argument("image")
     @click.option(
         "-t",
         "--name",
         "--client-token",
         metavar="NAME",
-        help="Specify a human-readable session name. " "If not set, a random hex string is used.",
+        help="Specify a human-readable session name. If not set, a random hex string is used.",
     )
     @click.option(
         "-o",
         "--owner",
         "--owner-access-key",
         metavar="ACCESS_KEY",
         help="Set the owner of the target session explicitly.",
@@ -97,16 +97,18 @@
         "--no-reuse", is_flag=True, help="Do not reuse existing sessions but return an error."
     )
     @click.option(
         "--depends",
         metavar="SESSION_ID",
         type=str,
         multiple=True,
-        help="Set the list of session ID or names that the newly created session depends on. "
-        "The session will get scheduled after all of them successfully finish.",
+        help=(
+            "Set the list of session ID or names that the newly created session depends on. "
+            "The session will get scheduled after all of them successfully finish."
+        ),
     )
     @click.option(
         "--callback-url",
         metavar="CALLBACK_URL",
         type=str,
         default=None,
         help="Callback URL which will be called upon sesison lifecycle events.",
@@ -146,39 +148,45 @@
         "--volume",
         "-m",
         "--mount",
         "mount",
         metavar="NAME[=PATH]",
         type=str,
         multiple=True,
-        help="User-owned virtual folder names to mount. "
-        "If path is not provided, virtual folder will be mounted under /home/work. "
-        "When the target path is relative, it is placed under /home/work "
-        "with auto-created parent directories if any. "
-        "Absolute paths are mounted as-is, but it is prohibited to "
-        "override the predefined Linux system directories.",
+        help=(
+            "User-owned virtual folder names to mount. "
+            "If path is not provided, virtual folder will be mounted under /home/work. "
+            "When the target path is relative, it is placed under /home/work "
+            "with auto-created parent directories if any. "
+            "Absolute paths are mounted as-is, but it is prohibited to "
+            "override the predefined Linux system directories."
+        ),
     )
     @click.option(
         "--scaling-group",
         "--sgroup",
         type=str,
         default=None,
-        help="The scaling group to execute session. If not specified, "
-        "all available scaling groups are included in the scheduling.",
+        help=(
+            "The scaling group to execute session. If not specified, "
+            "all available scaling groups are included in the scheduling."
+        ),
     )
     @click.option(
         "-r",
         "--resources",
         metavar="KEY=VAL",
         type=str,
         multiple=True,
-        help="Set computation resources used by the session "
-        "(e.g: -r cpu=2 -r mem=256 -r gpu=1)."
-        "1 slot of cpu/gpu represents 1 core. "
-        "The unit of mem(ory) is MiB.",
+        help=(
+            "Set computation resources used by the session "
+            "(e.g: -r cpu=2 -r mem=256 -r gpu=1)."
+            "1 slot of cpu/gpu represents 1 core. "
+            "The unit of mem(ory) is MiB."
+        ),
     )
     @click.option(
         "--cluster-size",
         metavar="NUMBER",
         type=int,
         default=1,
         help="The size of cluster in number of containers.",
@@ -191,41 +199,47 @@
         help="The mode of clustering.",
     )
     @click.option(
         "--resource-opts",
         metavar="KEY=VAL",
         type=str,
         multiple=True,
-        help="Resource options for creating compute session " "(e.g: shmem=64m)",
+        help="Resource options for creating compute session (e.g: shmem=64m)",
     )
     @click.option("--preopen", default=None, type=list_expr, help="Pre-open service ports")
     # resource grouping
     @click.option(
         "-d",
         "--domain",
         metavar="DOMAIN_NAME",
         default=None,
-        help="Domain name where the session will be spawned. "
-        "If not specified, config's domain name will be used.",
+        help=(
+            "Domain name where the session will be spawned. "
+            "If not specified, config's domain name will be used."
+        ),
     )
     @click.option(
         "-g",
         "--group",
         metavar="GROUP_NAME",
         default=None,
-        help="Group name where the session is spawned. "
-        "User should be a member of the group to execute the code.",
+        help=(
+            "Group name where the session is spawned. "
+            "User should be a member of the group to execute the code."
+        ),
     )
     @click.option(
         "--assign-agent",
         default=None,
         type=list_expr,
-        help="Show mapping list of tuple which mapped containers with agent. "
-        "When user role is Super Admin. "
-        "(e.g., --assign-agent agent_id_1,agent_id_2,...)",
+        help=(
+            "Show mapping list of tuple which mapped containers with agent. "
+            "When user role is Super Admin. "
+            "(e.g., --assign-agent agent_id_1,agent_id_2,...)"
+        ),
     )
     def create(
         # base args
         image: str,
         name: str | None,
         owner: str | None,
         # job scheduling options
@@ -301,17 +315,17 @@
                     startup_command=startup_command,
                     resources=resources,
                     resource_opts=resource_opts,
                     owner_access_key=owner,
                     domain_name=domain,
                     group_name=group,
                     scaling_group=scaling_group,
-                    bootstrap_script=bootstrap_script.read()
-                    if bootstrap_script is not None
-                    else None,
+                    bootstrap_script=(
+                        bootstrap_script.read() if bootstrap_script is not None else None
+                    ),
                     tag=tag,
                     architecture=architecture,
                     preopen_ports=preopen_ports,
                     assign_agent=assigned_agent_list,
                 )
             except Exception as e:
                 print_error(e)
@@ -353,17 +367,16 @@
                     )
                 elif compute_session.status == "TIMEOUT":
                     print_info(
                         "Session ID {0} is still on the job queue.".format(compute_session.id)
                     )
                 elif compute_session.status in ("ERROR", "CANCELLED"):
                     print_fail(
-                        "Session ID {0} has an error during scheduling/startup or cancelled.".format(
-                            compute_session.id
-                        )
+                        "Session ID {0} has an error during scheduling/startup or cancelled."
+                        .format(compute_session.id)
                     )
 
     if docs is not None:
         create.__doc__ = docs
     return create
 
 
@@ -375,15 +388,15 @@
     @click.argument("template_id")
     @click.option(
         "-t",
         "--name",
         "--client-token",
         metavar="NAME",
         default=undefined,
-        help="Specify a human-readable session name. " "If not set, a random hex string is used.",
+        help="Specify a human-readable session name. If not set, a random hex string is used.",
     )
     @click.option(
         "-o",
         "--owner",
         "--owner-access-key",
         metavar="ACCESS_KEY",
         default=undefined,
@@ -429,16 +442,18 @@
         "--no-reuse", is_flag=True, help="Do not reuse existing sessions but return an error."
     )
     @click.option(
         "--depends",
         metavar="SESSION_ID",
         type=str,
         multiple=True,
-        help="Set the list of session ID or names that the newly created session depends on. "
-        "The session will get scheduled after all of them successfully finish.",
+        help=(
+            "Set the list of session ID or names that the newly created session depends on. "
+            "The session will get scheduled after all of them successfully finish."
+        ),
     )
     @click.option(
         "--callback-url",
         metavar="CALLBACK_URL",
         type=str,
         default=None,
         help="Callback URL which will be called upon session lifecycle events.",
@@ -459,88 +474,104 @@
     # resource spec
     @click.option(
         "-m",
         "--mount",
         metavar="NAME[=PATH]",
         type=str,
         multiple=True,
-        help="User-owned virtual folder names to mount. "
-        "When the target path is relative, it is placed under /home/work "
-        "with auto-created parent directories if any. "
-        "Absolute paths are mounted as-is, but it is prohibited to "
-        "override the predefined Linux system directories.",
+        help=(
+            "User-owned virtual folder names to mount. "
+            "When the target path is relative, it is placed under /home/work "
+            "with auto-created parent directories if any. "
+            "Absolute paths are mounted as-is, but it is prohibited to "
+            "override the predefined Linux system directories."
+        ),
     )
     @click.option(
         "--scaling-group",
         "--sgroup",
         type=str,
         default=undefined,
-        help="The scaling group to execute session. If not specified, "
-        "all available scaling groups are included in the scheduling.",
+        help=(
+            "The scaling group to execute session. If not specified, "
+            "all available scaling groups are included in the scheduling."
+        ),
     )
     @click.option(
         "-r",
         "--resources",
         metavar="KEY=VAL",
         type=str,
         multiple=True,
-        help="Set computation resources used by the session "
-        "(e.g: -r cpu=2 -r mem=256 -r gpu=1)."
-        "1 slot of cpu/gpu represents 1 core. "
-        "The unit of mem(ory) is MiB.",
+        help=(
+            "Set computation resources used by the session "
+            "(e.g: -r cpu=2 -r mem=256 -r gpu=1)."
+            "1 slot of cpu/gpu represents 1 core. "
+            "The unit of mem(ory) is MiB."
+        ),
     )
     @click.option(
         "--cluster-size",
         metavar="NUMBER",
         type=int,
         default=undefined,
         help="The size of cluster in number of containers.",
     )
     @click.option(
         "--resource-opts",
         metavar="KEY=VAL",
         type=str,
         multiple=True,
-        help="Resource options for creating compute session " "(e.g: shmem=64m)",
+        help="Resource options for creating compute session (e.g: shmem=64m)",
     )
     # resource grouping
     @click.option(
         "-d",
         "--domain",
         metavar="DOMAIN_NAME",
         default=None,
-        help="Domain name where the session will be spawned. "
-        "If not specified, config's domain name will be used.",
+        help=(
+            "Domain name where the session will be spawned. "
+            "If not specified, config's domain name will be used."
+        ),
     )
     @click.option(
         "-g",
         "--group",
         metavar="GROUP_NAME",
         default=None,
-        help="Group name where the session is spawned. "
-        "User should be a member of the group to execute the code.",
+        help=(
+            "Group name where the session is spawned. "
+            "User should be a member of the group to execute the code."
+        ),
     )
     # template overrides
     @click.option(
         "--no-mount",
         is_flag=True,
-        help="If specified, client.py will tell server not to mount "
-        "any vFolders specified at template,",
+        help=(
+            "If specified, client.py will tell server not to mount "
+            "any vFolders specified at template,"
+        ),
     )
     @click.option(
         "--no-env",
         is_flag=True,
-        help="If specified, client.py will tell server not to add "
-        "any environs specified at template,",
+        help=(
+            "If specified, client.py will tell server not to add "
+            "any environs specified at template,"
+        ),
     )
     @click.option(
         "--no-resource",
         is_flag=True,
-        help="If specified, client.py will tell server not to add "
-        "any resource specified at template,",
+        help=(
+            "If specified, client.py will tell server not to add "
+            "any resource specified at template,"
+        ),
     )
     def create_from_template(
         # base args
         template_id: str,
         name: str | Undefined,
         owner: str | Undefined,
         # job scheduling options
@@ -647,17 +678,16 @@
                         "Session ID {0} is already terminated.\n"
                         "This may be an error in the compute_session image.".format(name)
                     )
                 elif compute_session.status == "TIMEOUT":
                     print_info("Session ID {0} is still on the job queue.".format(name))
                 elif compute_session.status in ("ERROR", "CANCELLED"):
                     print_fail(
-                        "Session ID {0} has an error during scheduling/startup or cancelled.".format(
-                            name
-                        )
+                        "Session ID {0} has an error during scheduling/startup or cancelled."
+                        .format(name)
                     )
 
     if docs is not None:
         create_from_template.__doc__ = docs
     return create_from_template
 
 
@@ -681,30 +711,34 @@
         "--owner-access-key",
         metavar="ACCESS_KEY",
         help="Specify the owner of the target session explicitly.",
     )
     @click.option(
         "-s", "--stats", is_flag=True, help="Show resource usage statistics after termination"
     )
-    def destroy(session_names, forced, owner, stats):
+    @click.option(
+        "-r", "--recursive", is_flag=True, help="Cancel all the dependant sessions recursively"
+    )
+    def destroy(session_names, forced, owner, stats, recursive):
         """
         Terminate and destroy the given session.
 
         SESSID: session ID given/generated when creating the session.
         """
         if len(session_names) == 0:
             print_warn('Specify at least one session ID. Check usage with "-h" option.')
             sys.exit(ExitCode.INVALID_ARGUMENT)
         print_wait("Terminating the session(s)...")
         with Session() as session:
             has_failure = False
             for session_name in session_names:
                 try:
                     compute_session = session.ComputeSession(session_name, owner)
-                    ret = compute_session.destroy(forced=forced)
+                    ret = compute_session.destroy(forced=forced, recursive=recursive)
+
                 except BackendAPIError as e:
                     print_error(e)
                     if e.status == 404:
                         print_info(
                             'If you are an admin, use "-o" / "--owner" option '
                             "to terminate other user's session."
                         )
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/session_template.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/session_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,32 +16,37 @@
 
 
 @session_template.command()
 @click.option(
     "-f",
     "--file",
     "template_path",
-    help="Path to task template file. "
-    "If not specified, client will try to read config from STDIN. ",
+    help=(
+        "Path to task template file. If not specified, client will try to read config from STDIN. "
+    ),
 )
 @click.option(
     "-d",
     "--domain",
     metavar="DOMAIN_NAME",
     default=None,
-    help="Domain name where the session will be spawned. "
-    "If not specified, config's domain name will be used.",
+    help=(
+        "Domain name where the session will be spawned. "
+        "If not specified, config's domain name will be used."
+    ),
 )
 @click.option(
     "-g",
     "--group",
     metavar="GROUP_NAME",
     default=None,
-    help="Group name where the session is spawned. "
-    "User should be a member of the group to execute the code.",
+    help=(
+        "Group name where the session is spawned. "
+        "User should be a member of the group to execute the code."
+    ),
 )
 @click.option(
     "-o",
     "--owner",
     "--owner-access-key",
     "owner_access_key",
     metavar="ACCESS_KEY",
@@ -139,16 +144,17 @@
 
 @session_template.command()
 @click.argument("template_id", metavar="TEMPLATEID")
 @click.option(
     "-f",
     "--file",
     "template_path",
-    help="Path to task template file. "
-    "If not specified, client will try to read config from STDIN. ",
+    help=(
+        "Path to task template file. If not specified, client will try to read config from STDIN. "
+    ),
 )
 @click.option(
     "-o",
     "--owner",
     "--owner-access-key",
     "owner_access_key",
     metavar="ACCESS_KEY",
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/ssh.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/ssh.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     try:
         lines: List[bytes] = []
         while True:
             line = proxy_proc.stdout.readline(1024)
             if not line:
                 proxy_proc.wait()
                 print_fail(
-                    f"Unexpected early termination of the sshd app command "
+                    "Unexpected early termination of the sshd app command "
                     f"(exit: {proxy_proc.returncode}):"
                 )
                 print((b"\n".join(lines)).decode())
                 sys.exit(ExitCode.FAILURE)
             if f"127.0.0.1:{port}".encode() in line:
                 break
             lines.append(line)
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/cli/vfolder.py` & `backend.ai-client-23.3.1/ai/backend/client/cli/vfolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,46 +69,54 @@
     help="Group ID or NAME. Specify this option if you want to create a group folder.",
 )
 @click.option(
     "--unmanaged",
     "host_path",
     type=bool,
     is_flag=True,
-    help="Treats HOST as a mount point of unmanaged virtual folder. "
-    "This option can only be used by Admin or Superadmin.",
+    help=(
+        "Treats HOST as a mount point of unmanaged virtual folder. "
+        "This option can only be used by Admin or Superadmin."
+    ),
 )
 @click.option(
     "-m",
     "--usage-mode",
     metavar="USAGE_MODE",
     type=str,
     default="general",
-    help='Purpose of the folder. Normal folders are usually set to "general". '
-    'Available options: "general", "data" (provides data to users), '
-    'and "model" (provides pre-trained models).',
+    help=(
+        'Purpose of the folder. Normal folders are usually set to "general". '
+        'Available options: "general", "data" (provides data to users), '
+        'and "model" (provides pre-trained models).'
+    ),
 )
 @click.option(
     "-p",
     "--permission",
     metavar="PERMISSION",
     type=str,
     default="rw",
-    help="Folder's innate permission. "
-    'Group folders can be shared as read-only by setting this option to "ro". '
-    "Invited folders override this setting by its own invitation permission. ",
+    help=(
+        "Folder's innate permission. "
+        'Group folders can be shared as read-only by setting this option to "ro". '
+        "Invited folders override this setting by its own invitation permission. "
+    ),
 )
 @click.option(
     "-q",
     "--quota",
     metavar="QUOTA",
     type=ByteSizeParamCheckType(),
     default="0",
-    help="Quota of the virtual folder. "
-    "(Use 'm' for megabytes, 'g' for gigabytes, and etc.) "
-    "Default is maximum amount possible.",
+    help=(
+        "Quota of the virtual folder. "
+        "(Use 'm' for megabytes, 'g' for gigabytes, and etc.) "
+        "Default is maximum amount possible."
+    ),
 )
 @click.option(
     "--cloneable",
     "--allow-clone",
     type=bool,
     is_flag=True,
     help="Allows the virtual folder to be cloned by users.",
@@ -218,33 +226,39 @@
 @click.argument("name", type=str)
 @click.argument("filenames", type=Path, nargs=-1)
 @click.option(
     "-b",
     "--base-dir",
     type=Path,
     default=None,
-    help="The local parent directory which contains the file to be uploaded. "
-    "[default: current working directory]",
+    help=(
+        "The local parent directory which contains the file to be uploaded. "
+        "[default: current working directory]"
+    ),
 )
 @click.option(
     "--chunk-size",
     type=ByteSizeParamType(),
     default=humanize.naturalsize(DEFAULT_CHUNK_SIZE, binary=True, gnu=True),
-    help='Transfer the file with the given chunk size with binary suffixes (e.g., "16m"). '
-    "Set this between 8 to 64 megabytes for high-speed disks (e.g., SSD RAID) "
-    "and networks (e.g., 40 GbE) for the maximum throughput.",
+    help=(
+        'Transfer the file with the given chunk size with binary suffixes (e.g., "16m"). '
+        "Set this between 8 to 64 megabytes for high-speed disks (e.g., SSD RAID) "
+        "and networks (e.g., 40 GbE) for the maximum throughput."
+    ),
 )
 @click.option(
     "--override-storage-proxy",
     type=CommaSeparatedKVListParamType(),
     default=None,
-    help="Overrides storage proxy address. "
-    'The value must shape like "X1=Y1,X2=Y2...". '
-    "Each Yn address must at least include the IP address "
-    "or the hostname and may include the protocol part and the port number to replace.",
+    help=(
+        "Overrides storage proxy address. "
+        'The value must shape like "X1=Y1,X2=Y2...". '
+        "Each Yn address must at least include the IP address "
+        "or the hostname and may include the protocol part and the port number to replace."
+    ),
 )
 def upload(name, filenames, base_dir, chunk_size, override_storage_proxy):
     """
     TUS Upload a file to the virtual folder from the current working directory.
     The files with the same names will be overwritten.
 
     \b
@@ -271,33 +285,39 @@
 @click.argument("name", type=str)
 @click.argument("filenames", type=Path, nargs=-1)
 @click.option(
     "-b",
     "--base-dir",
     type=Path,
     default=None,
-    help="The local parent directory which will contain the downloaded file.  "
-    "[default: current working directory]",
+    help=(
+        "The local parent directory which will contain the downloaded file.  "
+        "[default: current working directory]"
+    ),
 )
 @click.option(
     "--chunk-size",
     type=ByteSizeParamType(),
     default=humanize.naturalsize(DEFAULT_CHUNK_SIZE, binary=True, gnu=True),
-    help='Transfer the file with the given chunk size with binary suffixes (e.g., "16m"). '
-    "Set this between 8 to 64 megabytes for high-speed disks (e.g., SSD RAID) "
-    "and networks (e.g., 40 GbE) for the maximum throughput.",
+    help=(
+        'Transfer the file with the given chunk size with binary suffixes (e.g., "16m"). '
+        "Set this between 8 to 64 megabytes for high-speed disks (e.g., SSD RAID) "
+        "and networks (e.g., 40 GbE) for the maximum throughput."
+    ),
 )
 @click.option(
     "--override-storage-proxy",
     type=CommaSeparatedKVListParamType(),
     default=None,
-    help="Overrides storage proxy address. "
-    'The value must shape like "X1=Y1,X2=Y2...". '
-    "Each Yn address must at least include the IP address "
-    "or the hostname and may include the protocol part and the port number to replace.",
+    help=(
+        "Overrides storage proxy address. "
+        'The value must shape like "X1=Y1,X2=Y2...". '
+        "Each Yn address must at least include the IP address "
+        "or the hostname and may include the protocol part and the port number to replace."
+    ),
 )
 @click.option(
     "--max-retries",
     type=int,
     default=20,
     help="Maximum retry attempt when any failure occurs.",
 )
@@ -681,23 +701,23 @@
 @click.argument("target_host", type=str)
 @click.option(
     "-m",
     "--usage-mode",
     metavar="USAGE_MODE",
     type=str,
     default="general",
-    help="Purpose of the cloned virtual folder. " "Default value is 'general'.",
+    help="Purpose of the cloned virtual folder. Default value is 'general'.",
 )
 @click.option(
     "-p",
     "--permission",
     metavar="PERMISSION",
     type=str,
     default="rw",
-    help="Cloned virtual folder's permission. " "Default value is 'rw'.",
+    help="Cloned virtual folder's permission. Default value is 'rw'.",
 )
 def clone(name, target_name, target_host, usage_mode, permission):
     """Clone a virtual folder.
 
     \b
     NAME: Name of the virtual folder to clone from.
     TARGET_NAME: Name of the virtual folder to clone to.
@@ -728,16 +748,18 @@
         async with AsyncSession() as session:
             try:
                 bgtask = session.BackgroundTask(bgtask_id)
                 completion_msg_func = lambda: print_done("Cloning the vfolder is complete.")
                 async with (
                     bgtask.listen_events() as response,
                     ProgressViewer(
-                        "Cloning the vfolder... "
-                        "(This may take a while depending on its size and number of files!)",
+                        (
+                            "Cloning the vfolder... "
+                            "(This may take a while depending on its size and number of files!)"
+                        ),
                     ) as viewer,
                 ):
                     async for ev in response:
                         data = json.loads(ev.data)
                         if ev.event == "bgtask_updated":
                             if viewer.tqdm is None:
                                 pbar = await viewer.to_tqdm()
@@ -748,16 +770,18 @@
                         elif ev.event == "bgtask_failed":
                             error_msg = data["message"]
                             completion_msg_func = lambda: print_fail(
                                 f"Error during the operation: {error_msg}",
                             )
                         elif ev.event == "bgtask_cancelled":
                             completion_msg_func = lambda: print_warn(
-                                "The operation has been cancelled in the middle. "
-                                "(This may be due to server shutdown.)",
+                                (
+                                    "The operation has been cancelled in the middle. "
+                                    "(This may be due to server shutdown.)"
+                                ),
                             )
             finally:
                 completion_msg_func()
 
     if bgtask_id is None:
         print_done("Cloning the vfolder is complete.")
     else:
@@ -769,16 +793,18 @@
 @click.option(
     "-p", "--permission", type=str, metavar="PERMISSION", help="Folder's innate permission."
 )
 @click.option(
     "--set-cloneable",
     type=bool,
     metavar="BOOLEXPR",
-    help="A boolean-interpretable string whether a virtual folder can be cloned. "
-    "If not set, the cloneable property is not changed.",
+    help=(
+        "A boolean-interpretable string whether a virtual folder can be cloned. "
+        "If not set, the cloneable property is not changed."
+    ),
 )
 def update_options(name, permission, set_cloneable):
     """Update an existing virtual folder.
 
     \b
     NAME: Name of the virtual folder to update.
     """
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/compat.py` & `backend.ai-client-23.3.1/ai/backend/client/compat.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/config.py` & `backend.ai-client-23.3.1/ai/backend/client/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/exceptions.py` & `backend.ai-client-23.3.1/ai/backend/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/acl.py` & `backend.ai-client-23.3.1/ai/backend/client/func/acl.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,15 @@
         fields: Sequence[FieldSpec] = _default_list_fields,
     ) -> Sequence[str]:
         """
         Fetches the list of atomic permissions.
 
         :param fields: Additional permission query fields to fetch.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             query {
                 vfolder_host_permissions {$fields}
             }
-        """
-        )
+        """)
         query = query.replace("$fields", " ".join(f.field_ref for f in fields))
         data = await api_session.get().Admin._query(query)
         return data["vfolder_host_permissions"]
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/admin.py` & `backend.ai-client-23.3.1/ai/backend/client/func/admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/agent.py` & `backend.ai-client-23.3.1/ai/backend/client/func/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,21 +84,19 @@
     @api_function
     @classmethod
     async def detail(
         cls,
         agent_id: str,
         fields: Sequence[FieldSpec] = _default_detail_fields,
     ) -> Sequence[dict]:
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             query($agent_id: String!) {
                 agent(agent_id: $agent_id) {$fields}
             }
-        """
-        )
+        """)
         query = query.replace("$fields", " ".join(f.field_ref for f in fields))
         variables = {"agent_id": agent_id}
         data = await api_session.get().Admin._query(query, variables)
         return data["agent"]
 
 
 class AgentWatcher(BaseFunction):
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/auth.py` & `backend.ai-client-23.3.1/ai/backend/client/func/auth.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/base.py` & `backend.ai-client-23.3.1/ai/backend/client/func/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         # We need to keep the original attributes so that they could be correctly
         # bound to the class/instance at runtime.
         func = getattr(cls, orig_name)
         coro = func(*args, **kwargs)
         _api_session = api_session.get()
         if _api_session is None:
             raise RuntimeError(
-                "API functions must be called " "inside the context of a valid API session",
+                "API functions must be called inside the context of a valid API session",
             )
         if isinstance(_api_session, AsyncSession):
             return coro
         else:
             if inspect.isasyncgen(coro):
                 return _api_session.worker_thread.execute_generator(coro)
             else:
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/bgtask.py` & `backend.ai-client-23.3.1/ai/backend/client/func/bgtask.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/domain.py` & `backend.ai-client-23.3.1/ai/backend/client/func/domain.py`

 * *Files 13% similar despite different names*

```diff
@@ -51,21 +51,19 @@
         fields: Sequence[FieldSpec] = _default_list_fields,
     ) -> Sequence[dict]:
         """
         Fetches the list of domains.
 
         :param fields: Additional per-domain query fields to fetch.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             query {
                 domains {$fields}
             }
-        """
-        )
+        """)
         query = query.replace("$fields", " ".join(f.field_ref for f in fields))
         data = await api_session.get().Admin._query(query)
         return data["domains"]
 
     @api_function
     @classmethod
     async def detail(
@@ -75,21 +73,19 @@
     ) -> dict:
         """
         Fetch information of a domain with name.
 
         :param name: Name of the domain to fetch.
         :param fields: Additional per-domain query fields to fetch.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             query($name: String) {
                 domain(name: $name) {$fields}
             }
-        """
-        )
+        """)
         query = query.replace("$fields", " ".join(f.field_ref for f in fields))
         variables = {"name": name}
         data = await api_session.get().Admin._query(query, variables)
         return data["domain"]
 
     @api_function
     @classmethod
@@ -104,23 +100,21 @@
         integration_id: str = None,
         fields: Iterable[FieldSpec | str] = None,
     ) -> dict:
         """
         Creates a new domain with the given options.
         You need an admin privilege for this operation.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($name: String!, $input: DomainInput!) {
                 create_domain(name: $name, props: $input) {
                     ok msg domain {$fields}
                 }
             }
-        """
-        )
+        """)
         resolved_fields = resolve_fields(fields, domain_fields, (domain_fields["name"],))
         query = query.replace("$fields", " ".join(resolved_fields))
         variables = {
             "name": name,
             "input": {
                 "description": description,
                 "is_active": is_active,
@@ -147,23 +141,21 @@
         integration_id: str = None,
         fields: Iterable[FieldSpec | str] = None,
     ) -> dict:
         """
         Update existing domain.
         You need an admin privilege for this operation.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($name: String!, $input: ModifyDomainInput!) {
                 modify_domain(name: $name, props: $input) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {
             "name": name,
             "input": {
                 "name": new_name,
                 "description": description,
                 "is_active": is_active,
                 "total_resource_slots": total_resource_slots,
@@ -177,38 +169,34 @@
 
     @api_function
     @classmethod
     async def delete(cls, name: str):
         """
         Inactivates an existing domain.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($name: String!) {
                 delete_domain(name: $name) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {"name": name}
         data = await api_session.get().Admin._query(query, variables)
         return data["delete_domain"]
 
     @api_function
     @classmethod
     async def purge(cls, name: str):
         """
         Deletes an existing domain.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($name: String!) {
                 purge_domain(name: $name) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {"name": name}
         data = await api_session.get().Admin._query(query, variables)
         return data["purge_domain"]
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/dotfile.py` & `backend.ai-client-23.3.1/ai/backend/client/func/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/etcd.py` & `backend.ai-client-23.3.1/ai/backend/client/func/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/group.py` & `backend.ai-client-23.3.1/ai/backend/client/func/group.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,21 +54,19 @@
         It may return multiple groups when there are groups with the same name
         in different domains and it is invoked with a super-admin account
         without setting the domain name.
 
         :param domain_name: Name of domain to get groups from.
         :param fields: Per-group query fields to fetch.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             query($name: String!, $domain_name: String) {
                 groups_by_name(name: $name, domain_name: $domain_name) {$fields}
             }
-        """
-        )
+        """)
         resolved_fields = resolve_fields(fields, group_fields, _default_detail_fields)
         query = query.replace("$fields", " ".join(resolved_fields))
         variables = {
             "name": name,
             "domain_name": domain_name,
         }
         data = await api_session.get().Admin._query(query, variables)
@@ -85,21 +83,19 @@
         Fetches the list of groups.
 
         :param domain_name: Name of domain to list groups.
         :param fields: Per-group query fields to fetch.
         """
         if fields is None:
             fields = _default_list_fields
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             query($domain_name: String) {
                 groups(domain_name: $domain_name) {$fields}
             }
-        """
-        )
+        """)
         query = query.replace("$fields", " ".join(f.field_ref for f in fields))
         variables = {"domain_name": domain_name}
         data = await api_session.get().Admin._query(query, variables)
         return data["groups"]
 
     @api_function
     @classmethod
@@ -112,21 +108,19 @@
         Fetch information of a group with group ID.
 
         :param gid: ID of the group to fetch.
         :param fields: Additional per-group query fields to fetch.
         """
         if fields is None:
             fields = _default_detail_fields
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             query($gid: UUID!) {
                 group(id: $gid) {$fields}
             }
-        """
-        )
+        """)
         query = query.replace("$fields", " ".join(f.field_ref for f in fields))
         variables = {"gid": gid}
         data = await api_session.get().Admin._query(query, variables)
         return data["group"]
 
     @api_function
     @classmethod
@@ -141,23 +135,21 @@
         integration_id: str = None,
         fields: Iterable[FieldSpec | str] = None,
     ) -> dict:
         """
         Creates a new group with the given options.
         You need an admin privilege for this operation.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($name: String!, $input: GroupInput!) {
                 create_group(name: $name, props: $input) {
                     ok msg group {$fields}
                 }
             }
-        """
-        )
+        """)
         resolved_fields = resolve_fields(
             fields,
             group_fields,
             (group_fields["id"], group_fields["domain_name"], group_fields["name"]),
         )
         query = query.replace("$fields", " ".join(resolved_fields))
         variables = {
@@ -187,23 +179,21 @@
         integration_id: str = None,
         fields: Iterable[FieldSpec | str] = None,
     ) -> dict:
         """
         Update existing group.
         You need an admin privilege for this operation.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($gid: UUID!, $input: ModifyGroupInput!) {
                 modify_group(gid: $gid, props: $input) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {
             "gid": gid,
             "input": {
                 "name": name,
                 "description": description,
                 "is_active": is_active,
                 "total_resource_slots": total_resource_slots,
@@ -216,64 +206,58 @@
 
     @api_function
     @classmethod
     async def delete(cls, gid: str):
         """
         Inactivates the existing group. Does not actually delete it for safety.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($gid: UUID!) {
                 delete_group(gid: $gid) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {"gid": gid}
         data = await api_session.get().Admin._query(query, variables)
         return data["delete_group"]
 
     @api_function
     @classmethod
     async def purge(cls, gid: str):
         """
         Delete the existing group. This action cannot be undone.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($gid: UUID!) {
                 purge_group(gid: $gid) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {"gid": gid}
         data = await api_session.get().Admin._query(query, variables)
         return data["purge_group"]
 
     @api_function
     @classmethod
     async def add_users(
         cls, gid: str, user_uuids: Iterable[str], fields: Iterable[FieldSpec | str] = None
     ) -> dict:
         """
         Add users to a group.
         You need an admin privilege for this operation.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($gid: UUID!, $input: ModifyGroupInput!) {
                 modify_group(gid: $gid, props: $input) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {
             "gid": gid,
             "input": {
                 "user_update_mode": "add",
                 "user_uuids": user_uuids,
             },
         }
@@ -285,23 +269,21 @@
     async def remove_users(
         cls, gid: str, user_uuids: Iterable[str], fields: Iterable[FieldSpec | str] = None
     ) -> dict:
         """
         Remove users from a group.
         You need an admin privilege for this operation.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($gid: UUID!, $input: ModifyGroupInput!) {
                 modify_group(gid: $gid, props: $input) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {
             "gid": gid,
             "input": {
                 "user_update_mode": "remove",
                 "user_uuids": user_uuids,
             },
         }
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/image.py` & `backend.ai-client-23.3.1/ai/backend/client/func/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,21 +33,15 @@
         cls,
         operation: bool = False,
         fields: Sequence[FieldSpec] = _default_list_fields_admin,
     ) -> Sequence[dict]:
         """
         Fetches the list of registered images in this cluster.
         """
-        q = (
-            "query($is_operation: Boolean) {"
-            "  images(is_operation: $is_operation) {"
-            "    $fields"
-            "  }"
-            "}"
-        )
+        q = "query($is_operation: Boolean) {  images(is_operation: $is_operation) {    $fields  }}"
         q = q.replace("$fields", " ".join(f.field_ref for f in fields))
         variables = {
             "is_operation": operation,
         }
         data = await api_session.get().Admin._query(q, variables)
         return data["images"]
 
@@ -90,15 +84,15 @@
             variables = {"architecture": arch, **variables}
         data = await api_session.get().Admin._query(q, variables)
         return data["alias_image"]
 
     @api_function
     @classmethod
     async def dealias_image(cls, alias: str) -> dict:
-        q = "mutation($alias: String!) {" "  dealias_image(alias: $alias) {" "   ok msg" "  }" "}"
+        q = "mutation($alias: String!) {  dealias_image(alias: $alias) {   ok msg  }}"
         variables = {
             "alias": alias,
         }
         data = await api_session.get().Admin._query(q, variables)
         return data["dealias_image"]
 
     @api_function
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/keypair.py` & `backend.ai-client-23.3.1/ai/backend/client/func/keypair.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,18 +88,15 @@
     ) -> dict:
         """
         Creates a new keypair with the given options.
         You need an admin privilege for this operation.
         """
         q = (
             "mutation($access_key: String!, $input: ModifyKeyPairInput!) {"
-            + "  modify_keypair(access_key: $access_key, props: $input) {"
-            "    ok msg"
-            "  }"
-            "}"
+            + "  modify_keypair(access_key: $access_key, props: $input) {    ok msg  }}"
         )
         variables = {
             "access_key": access_key,
             "input": {
                 "is_active": is_active,
                 "is_admin": is_admin,
                 "resource_policy": resource_policy,
@@ -137,29 +134,20 @@
         fields: Sequence[FieldSpec] = _default_list_fields,
     ) -> Sequence[dict]:
         """
         Lists the keypairs.
         You need an admin privilege for this operation.
         """
         if user_id is None:
-            q = (
-                "query($is_active: Boolean) {"
-                "  keypairs(is_active: $is_active) {"
-                "    $fields"
-                "  }"
-                "}"
-            )
+            q = "query($is_active: Boolean) {  keypairs(is_active: $is_active) {    $fields  }}"
         else:
             uid_type = "Int!" if isinstance(user_id, int) else "String!"
             q = (
                 "query($email: {0}, $is_active: Boolean) {{".format(uid_type)
-                + "  keypairs(email: $email, is_active: $is_active) {"
-                "    $fields"
-                "  }"
-                "}"
+                + "  keypairs(email: $email, is_active: $is_active) {    $fields  }}"
             )
         q = q.replace("$fields", " ".join(f.field_ref for f in fields))
         variables: Dict[str, Any] = {
             "is_active": is_active,
         }
         if user_id is not None:
             variables["email"] = user_id
@@ -205,32 +193,29 @@
         """
         Returns the keypair's information such as resource limits.
 
         :param fields: Additional per-agent query fields to fetch.
 
         .. versionadded:: 18.12
         """
-        q = "query {" "  keypair {" "    $fields" "  }" "}"
+        q = "query {  keypair {    $fields  }}"
         q = q.replace("$fields", " ".join(f.field_ref for f in fields))
         data = await api_session.get().Admin._query(q)
         return data["keypair"]
 
     @api_function
     @classmethod
     async def activate(cls, access_key: str) -> dict:
         """
         Activates this keypair.
         You need an admin privilege for this operation.
         """
         q = (
             "mutation($access_key: String!, $input: ModifyKeyPairInput!) {"
-            + "  modify_keypair(access_key: $access_key, props: $input) {"
-            "    ok msg"
-            "  }"
-            "}"
+            + "  modify_keypair(access_key: $access_key, props: $input) {    ok msg  }}"
         )
         variables = {
             "access_key": access_key,
             "input": {
                 "is_active": True,
                 "is_admin": None,
                 "resource_policy": None,
@@ -247,18 +232,15 @@
         Deactivates this keypair.
         Deactivated keypairs cannot make any API requests
         unless activated again by an administrator.
         You need an admin privilege for this operation.
         """
         q = (
             "mutation($access_key: String!, $input: ModifyKeyPairInput!) {"
-            + "  modify_keypair(access_key: $access_key, props: $input) {"
-            "    ok msg"
-            "  }"
-            "}"
+            + "  modify_keypair(access_key: $access_key, props: $input) {    ok msg  }}"
         )
         variables = {
             "access_key": access_key,
             "input": {
                 "is_active": False,
                 "is_admin": None,
                 "resource_policy": None,
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/keypair_resource_policy.py` & `backend.ai-client-23.3.1/ai/backend/client/func/keypair_resource_policy.py`

 * *Files 14% similar despite different names*

```diff
@@ -106,18 +106,15 @@
     ) -> dict:
         """
         Updates an existing keypair resource policy with the given options.
         You need an admin privilege for this operation.
         """
         q = (
             "mutation($name: String!, $input: ModifyKeyPairResourcePolicyInput!) {"
-            + "  modify_keypair_resource_policy(name: $name, props: $input) {"
-            "    ok msg"
-            "  }"
-            "}"
+            + "  modify_keypair_resource_policy(name: $name, props: $input) {    ok msg  }}"
         )
         variables = {
             "name": name,
             "input": {
                 "default_for_unspecified": default_for_unspecified,
                 "total_resource_slots": total_resource_slots,
                 "max_session_lifetime": max_session_lifetime,
@@ -136,18 +133,16 @@
     @classmethod
     async def delete(cls, name: str) -> dict:
         """
         Deletes an existing keypair resource policy with given name.
         You need an admin privilege for this operation.
         """
         q = (
-            "mutation($name: String!) {" + "  delete_keypair_resource_policy(name: $name) {"
-            "    ok msg"
-            "  }"
-            "}"
+            "mutation($name: String!) {"
+            + "  delete_keypair_resource_policy(name: $name) {    ok msg  }}"
         )
         variables = {
             "name": name,
         }
         data = await api_session.get().Admin._query(q, variables)
         return data["delete_keypair_resource_policy"]
 
@@ -157,15 +152,15 @@
         cls,
         fields: Sequence[FieldSpec] = _default_list_fields,
     ) -> Sequence[dict]:
         """
         Lists the keypair resource policies.
         You need an admin privilege for this operation.
         """
-        q = "query {" "  keypair_resource_policies {" "    $fields" "  }" "}"
+        q = "query {  keypair_resource_policies {    $fields  }}"
         q = q.replace("$fields", " ".join(f.field_ref for f in fields))
         data = await api_session.get().Admin._query(q)
         return data["keypair_resource_policies"]
 
     @api_function
     async def info(
         self,
@@ -175,20 +170,14 @@
         """
         Returns the resource policy's information.
 
         :param fields: Additional per-agent query fields to fetch.
 
         .. versionadded:: 19.03
         """
-        q = (
-            "query($name: String) {"
-            "  keypair_resource_policy(name: $name) {"
-            "    $fields"
-            "  }"
-            "}"
-        )
+        q = "query($name: String) {  keypair_resource_policy(name: $name) {    $fields  }}"
         q = q.replace("$fields", " ".join(f.field_ref for f in fields))
         variables = {
             "name": name,
         }
         data = await api_session.get().Admin._query(q, variables)
         return data["keypair_resource_policy"]
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/manager.py` & `backend.ai-client-23.3.1/ai/backend/client/func/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/model.py` & `backend.ai-client-23.3.1/ai/backend/client/func/model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/resource.py` & `backend.ai-client-23.3.1/ai/backend/client/func/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/scaling_group.py` & `backend.ai-client-23.3.1/ai/backend/client/func/scaling_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 
 __all__ = ("ScalingGroup",)
 
 _default_list_fields = (
     scaling_group_fields["name"],
     scaling_group_fields["description"],
     scaling_group_fields["is_active"],
+    scaling_group_fields["is_public"],
     scaling_group_fields["created_at"],
     scaling_group_fields["driver"],
     scaling_group_fields["scheduler"],
     scaling_group_fields["use_host_network"],
 )
 
 _default_detail_fields = (
     scaling_group_fields["name"],
     scaling_group_fields["description"],
     scaling_group_fields["is_active"],
+    scaling_group_fields["is_public"],
     scaling_group_fields["created_at"],
     scaling_group_fields["driver"],
     scaling_group_fields["driver_opts"],
     scaling_group_fields["scheduler"],
     scaling_group_fields["scheduler_opts"],
     scaling_group_fields["use_host_network"],
 )
@@ -69,23 +71,21 @@
         cls,
         fields: Sequence[FieldSpec] = _default_list_fields,
     ) -> Sequence[dict]:
         """
         List available scaling groups for the current user,
         considering the user, the user's domain, and the designated user group.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             query($is_active: Boolean) {
                 scaling_groups(is_active: $is_active) {
                     $fields
                 }
             }
-        """
-        )
+        """)
         query = query.replace("$fields", " ".join(f.field_ref for f in fields))
         variables = {"is_active": None}
         data = await api_session.get().Admin._query(query, variables)
         return data["scaling_groups"]
 
     @api_function
     @classmethod
@@ -96,61 +96,59 @@
     ) -> dict:
         """
         Fetch information of a scaling group by name.
 
         :param name: Name of the scaling group.
         :param fields: Additional per-scaling-group query fields.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             query($name: String) {
                 scaling_group(name: $name) {$fields}
             }
-        """
-        )
+        """)
         query = query.replace("$fields", " ".join(f.field_ref for f in fields))
         variables = {"name": name}
         data = await api_session.get().Admin._query(query, variables)
         return data["scaling_group"]
 
     @api_function
     @classmethod
     async def create(
         cls,
         name: str,
         description: str = "",
         is_active: bool = True,
+        is_public: bool = True,
         driver: str = None,
         driver_opts: Mapping[str, str] = None,
         scheduler: str = None,
         scheduler_opts: Mapping[str, str] = None,
         use_host_network: bool = False,
         fields: Iterable[FieldSpec | str] = None,
     ) -> dict:
         """
         Creates a new scaling group with the given options.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($name: String!, $input: CreateScalingGroupInput!) {
                 create_scaling_group(name: $name, props: $input) {
                     ok msg scaling_group {$fields}
                 }
             }
-        """
-        )
+        """)
         resolved_fields = resolve_fields(
             fields, scaling_group_fields, (scaling_group_fields["name"],)
         )
         query = query.replace("$fields", " ".join(resolved_fields))
         variables = {
             "name": name,
             "input": {
                 "description": description,
                 "is_active": is_active,
+                "is_public": is_public,
                 "driver": driver,
                 "driver_opts": json.dumps(driver_opts),
                 "scheduler": scheduler,
                 "scheduler_opts": json.dumps(scheduler_opts),
                 "use_host_network": use_host_network,
             },
         }
@@ -160,42 +158,42 @@
     @api_function
     @classmethod
     async def update(
         cls,
         name: str,
         description: str = "",
         is_active: bool = True,
+        is_public: bool = True,
         driver: str = None,
         driver_opts: Mapping[str, str] = None,
         scheduler: str = None,
         scheduler_opts: Mapping[str, str] = None,
         use_host_network: bool = False,
         fields: Iterable[FieldSpec | str] = None,
     ) -> dict:
         """
         Update existing scaling group.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($name: String!, $input: ModifyScalingGroupInput!) {
                 modify_scaling_group(name: $name, props: $input) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         resolved_fields = resolve_fields(
             fields, scaling_group_fields, (scaling_group_fields["name"],)
         )
         query = query.replace("$fields", " ".join(resolved_fields))
         variables = {
             "name": name,
             "input": {
                 "description": description,
                 "is_active": is_active,
+                "is_public": is_public,
                 "driver": driver,
                 "driver_opts": None if driver_opts is None else json.dumps(driver_opts),
                 "scheduler": scheduler,
                 "scheduler_opts": None if scheduler_opts is None else json.dumps(scheduler_opts),
                 "use_host_network": use_host_network,
             },
         }
@@ -204,153 +202,139 @@
 
     @api_function
     @classmethod
     async def delete(cls, name: str):
         """
         Deletes an existing scaling group.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($name: String!) {
                 delete_scaling_group(name: $name) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {"name": name}
         data = await api_session.get().Admin._query(query, variables)
         return data["delete_scaling_group"]
 
     @api_function
     @classmethod
     async def associate_domain(cls, scaling_group: str, domain: str):
         """
         Associate scaling_group with domain.
 
         :param scaling_group: The name of a scaling group.
         :param domain: The name of a domain.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($scaling_group: String!, $domain: String!) {
                 associate_scaling_group_with_domain(
                         scaling_group: $scaling_group, domain: $domain) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {"scaling_group": scaling_group, "domain": domain}
         data = await api_session.get().Admin._query(query, variables)
         return data["associate_scaling_group_with_domain"]
 
     @api_function
     @classmethod
     async def dissociate_domain(cls, scaling_group: str, domain: str):
         """
         Dissociate scaling_group from domain.
 
         :param scaling_group: The name of a scaling group.
         :param domain: The name of a domain.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($scaling_group: String!, $domain: String!) {
                 disassociate_scaling_group_with_domain(
                         scaling_group: $scaling_group, domain: $domain) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {"scaling_group": scaling_group, "domain": domain}
         data = await api_session.get().Admin._query(query, variables)
         return data["disassociate_scaling_group_with_domain"]
 
     @api_function
     @classmethod
     async def dissociate_all_domain(cls, domain: str):
         """
         Dissociate all scaling_groups from domain.
 
         :param domain: The name of a domain.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($domain: String!) {
                 disassociate_all_scaling_groups_with_domain(domain: $domain) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {"domain": domain}
         data = await api_session.get().Admin._query(query, variables)
         return data["disassociate_all_scaling_groups_with_domain"]
 
     @api_function
     @classmethod
     async def associate_group(cls, scaling_group: str, group_id: str):
         """
         Associate scaling_group with group.
 
         :param scaling_group: The name of a scaling group.
         :param group_id: The ID of a group.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($scaling_group: String!, $user_group: UUID!) {
                 associate_scaling_group_with_user_group(
                         scaling_group: $scaling_group, user_group: $user_group) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {"scaling_group": scaling_group, "user_group": group_id}
         data = await api_session.get().Admin._query(query, variables)
         return data["associate_scaling_group_with_user_group"]
 
     @api_function
     @classmethod
     async def dissociate_group(cls, scaling_group: str, group_id: str):
         """
         Dissociate scaling_group from group.
 
         :param scaling_group: The name of a scaling group.
         :param group_id: The ID of a group.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($scaling_group: String!, $user_group: String!) {
                 disassociate_scaling_group_with_user_group(
                         scaling_group: $scaling_group, user_group: $user_group) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {"scaling_group": scaling_group, "user_group": group_id}
         data = await api_session.get().Admin._query(query, variables)
         return data["disassociate_scaling_group_with_user_group"]
 
     @api_function
     @classmethod
     async def dissociate_all_group(cls, group_id: str):
         """
         Dissociate all scaling_groups from group.
 
         :param group_id: The ID of a group.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($group_id: UUID!) {
                 disassociate_all_scaling_groups_with_group(user_group: $group_id) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {"group_id": group_id}
         data = await api_session.get().Admin._query(query, variables)
         return data["disassociate_all_scaling_groups_with_group"]
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/server_log.py` & `backend.ai-client-23.3.1/ai/backend/client/func/server_log.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/service.py` & `backend.ai-client-23.3.1/ai/backend/client/func/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,21 +56,19 @@
     @api_function
     @classmethod
     async def detail(
         cls,
         service_id: str,
         fields: Sequence[FieldSpec] = _default_detail_fields,
     ) -> Sequence[dict]:
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             query($service_id: UUID!) {
                 service(service_id: $service_id) {$fields}
             }
-        """
-        )
+        """)
         query = query.replace("$fields", " ".join(f.field_ref for f in fields))
         variables = {"service_id": service_id}
         data = await api_session.get().Admin._query(query, variables)
         return data["agent"]
 
     @api_function
     @classmethod
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/session.py` & `backend.ai-client-23.3.1/ai/backend/client/func/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,26 +523,29 @@
                 "sessionName": self.name,
             }
             if self.owner_access_key:
                 identity_params["owner_access_key"] = self.owner_access_key
         return identity_params
 
     @api_function
-    async def destroy(self, *, forced: bool = False):
+    async def destroy(self, *, forced: bool = False, recursive: bool = False):
         """
         Destroys the compute session.
         Since the server literally kills the container(s), all ongoing executions are
         forcibly interrupted.
         """
         params = {}
         if self.owner_access_key is not None:
             params["owner_access_key"] = self.owner_access_key
         prefix = get_naming(api_session.get().api_version, "path")
         if forced:
             params["forced"] = "true"
+        if recursive:
+            params["recursive"] = "true"
+
         rqst = Request(
             "DELETE",
             f"/{prefix}/{self.name}",
             params=params,
         )
         async with rqst.fetch() as resp:
             if resp.status == 200:
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/session_template.py` & `backend.ai-client-23.3.1/ai/backend/client/func/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/storage.py` & `backend.ai-client-23.3.1/ai/backend/client/func/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,18 +68,16 @@
     @api_function
     @classmethod
     async def detail(
         cls,
         vfolder_host: str,
         fields: Sequence[FieldSpec] = _default_detail_fields,
     ) -> dict:
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             query($vfolder_host: String!) {
                 storage_volume(id: $vfolder_host) {$fields}
             }
-        """
-        )
+        """)
         query = query.replace("$fields", " ".join(f.field_ref for f in fields))
         variables = {"vfolder_host": vfolder_host}
         data = await api_session.get().Admin._query(query, variables)
         return data["storage_volume"]
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/system.py` & `backend.ai-client-23.3.1/ai/backend/client/func/system.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/user.py` & `backend.ai-client-23.3.1/ai/backend/client/func/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,21 +127,19 @@
         Fetches the list of users. Domain admins can only get domain users.
 
         :param status: Fetches users in a specific status
                        (active, inactive, deleted, before-verification).
         :param group: Fetch users in a specific group.
         :param fields: Additional per-user query fields to fetch.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             query($status: String, $group: UUID) {
                 users(status: $status, group_id: $group) {$fields}
             }
-        """
-        )
+        """)
         query = query.replace("$fields", " ".join(f.field_ref for f in fields))
         variables = {
             "status": status,
             "group": group,
         }
         data = await api_session.get().Admin._query(query, variables)
         return data["users"]
@@ -191,29 +189,25 @@
         Fetch information of a user. If email is not specified,
         requester's information will be returned.
 
         :param email: Email of the user to fetch.
         :param fields: Additional per-user query fields to fetch.
         """
         if email is None:
-            query = textwrap.dedent(
-                """\
+            query = textwrap.dedent("""\
                 query {
                     user {$fields}
                 }
-            """
-            )
+            """)
         else:
-            query = textwrap.dedent(
-                """\
+            query = textwrap.dedent("""\
                 query($email: String) {
                     user(email: $email) {$fields}
                 }
-            """
-            )
+            """)
         query = query.replace("$fields", " ".join(f.field_ref for f in fields))
         variables = {"email": email}
         data = await api_session.get().Admin._query(query, variables if email is not None else None)
         return data["user"]
 
     @api_function
     @classmethod
@@ -226,29 +220,25 @@
         Fetch information of a user by user's uuid. If user_uuid is not specified,
         requester's information will be returned.
 
         :param user_uuid: UUID of the user to fetch.
         :param fields: Additional per-user query fields to fetch.
         """
         if user_uuid is None:
-            query = textwrap.dedent(
-                """\
+            query = textwrap.dedent("""\
                 query {
                     user {$fields}
                 }
-            """
-            )
+            """)
         else:
-            query = textwrap.dedent(
-                """\
+            query = textwrap.dedent("""\
                 query($user_id: ID) {
                     user_from_uuid(user_id: $user_id) {$fields}
                 }
-            """
-            )
+            """)
         query = query.replace("$fields", " ".join(f.field_ref for f in fields))
         variables = {"user_id": str(user_uuid)}
         data = await api_session.get().Admin._query(
             query, variables if user_uuid is not None else None
         )
         return data["user_from_uuid"]
 
@@ -270,23 +260,21 @@
         group_ids: Iterable[str] = None,
         fields: Iterable[FieldSpec | str] = None,
     ) -> dict:
         """
         Creates a new user with the given options.
         You need an admin privilege for this operation.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($email: String!, $input: UserInput!) {
                 create_user(email: $email, props: $input) {
                     ok msg user {$fields}
                 }
             }
-        """
-        )
+        """)
         default_fields = (
             user_fields["domain_name"],
             user_fields["email"],
             user_fields["username"],
             user_fields["uuid"],
         )
         resolved_fields = resolve_fields(fields, user_fields, default_fields)
@@ -328,23 +316,21 @@
         group_ids: Iterable[str] = None,
         fields: Iterable[FieldSpec | str] = None,
     ) -> dict:
         """
         Update existing user.
         You need an admin privilege for this operation.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($email: String!, $input: ModifyUserInput!) {
                 modify_user(email: $email, props: $input) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {
             "email": email,
             "input": {
                 "password": password,
                 "username": username,
                 "full_name": full_name,
                 "domain_name": domain_name,
@@ -362,46 +348,42 @@
 
     @api_function
     @classmethod
     async def delete(cls, email: str):
         """
         Inactivates an existing user.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($email: String!) {
                 delete_user(email: $email) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {"email": email}
         data = await api_session.get().Admin._query(query, variables)
         return data["delete_user"]
 
     @api_function
     @classmethod
     async def purge(cls, email: str, purge_shared_vfolders=False):
         """
         Deletes an existing user.
 
         User's virtual folders are also deleted, except the ones shared with other users.
         Shared virtual folder's ownership will be transferred to the requested admin.
         To delete shared folders as well, set ``purge_shared_vfolders`` to ``True``.
         """
-        query = textwrap.dedent(
-            """\
+        query = textwrap.dedent("""\
             mutation($email: String!, $input: PurgeUserInput!) {
                 purge_user(email: $email, props: $input) {
                     ok msg
                 }
             }
-        """
-        )
+        """)
         variables = {
             "email": email,
             "input": {
                 "purge_shared_vfolders": purge_shared_vfolders,
             },
         }
         data = await api_session.get().Admin._query(query, variables)
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/func/vfolder.py` & `backend.ai-client-23.3.1/ai/backend/client/func/vfolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,16 +299,18 @@
                 download_info = await resp.json()
                 overriden_url = download_info["url"]
                 if address_map:
                     if download_info["url"] in address_map:
                         overriden_url = address_map[download_info["url"]]
                     else:
                         raise BackendClientError(
-                            "Overriding storage proxy addresses are given, "
-                            "but no url matches with any of them.\n",
+                            (
+                                "Overriding storage proxy addresses are given, "
+                                "but no url matches with any of them.\n"
+                            ),
                         )
 
                 params = {"token": download_info["token"]}
                 if dst_dir is not None:
                     params["dst_dir"] = dst_dir
                 download_url = URL(overriden_url).with_query(params)
             await self._download_file(
@@ -344,16 +346,18 @@
                 upload_info = await resp.json()
                 overriden_url = upload_info["url"]
                 if address_map:
                     if upload_info["url"] in address_map:
                         overriden_url = address_map[upload_info["url"]]
                     else:
                         raise BackendClientError(
-                            "Overriding storage proxy addresses are given, "
-                            "but no url matches with any of them.\n",
+                            (
+                                "Overriding storage proxy addresses are given, "
+                                "but no url matches with any of them.\n"
+                            ),
                         )
                 params = {"token": upload_info["token"]}
                 if dst_dir is not None:
                     params["dst_dir"] = dst_dir
                 upload_url = URL(overriden_url).with_query(params)
             tus_client = client.TusClient()
             if basedir:
@@ -617,7 +621,20 @@
                 "vfolder": vfolder,
                 "user": user,
                 "perm": perm,
             }
         )
         async with rqst.fetch() as resp:
             return await resp.json()
+
+    @api_function
+    @classmethod
+    async def change_vfolder_ownership(cls, vfolder: str, user_email: str):
+        rqst = Request("POST", "/folders/_/change-ownership")
+        rqst.set_json(
+            {
+                "vfolder": vfolder,
+                "user_email": user_email,
+            }
+        )
+        async with rqst.fetch() as resp:
+            return await resp.json()
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/load_balancing.py` & `backend.ai-client-23.3.1/ai/backend/client/load_balancing.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/output/__init__.py` & `backend.ai-client-23.3.1/ai/backend/client/output/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/output/console.py` & `backend.ai-client-23.3.1/ai/backend/client/output/console.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/output/fields.py` & `backend.ai-client-23.3.1/ai/backend/client/output/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,15 @@
 
 
 scaling_group_fields = FieldSet(
     [
         FieldSpec("name"),
         FieldSpec("description"),
         FieldSpec("is_active"),
+        FieldSpec("is_public"),
         FieldSpec("created_at"),
         FieldSpec("driver"),
         FieldSpec("driver_opts", formatter=nested_dict_formatter),
         FieldSpec("scheduler"),
         FieldSpec("scheduler_opts", formatter=nested_dict_formatter),
         FieldSpec("use_host_network"),
     ]
@@ -204,14 +205,15 @@
             formatter=ContainerListFormatter(),
         ),
         FieldSpec(
             "dependencies { name id }",
             formatter=DependencyListFormatter(),
         ),
         FieldSpec("abusing_reports"),
+        FieldSpec("idle_checks"),
     ]
 )
 
 session_fields_v5 = FieldSet(
     [
         FieldSpec(
             "containers",
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/output/formatters.py` & `backend.ai-client-23.3.1/ai/backend/client/output/formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,16 @@
             else:
                 if outer_value is None:
                     rows.append(f"- {outer_key}: (null)")
                 else:
                     # TODO: refactor as a formatter
                     if outer_key == "shmem":
                         rows.append(
-                            f"- {outer_key}: {humanize.naturalsize(str(outer_value), binary=True, gnu=True)}"
+                            f"- {outer_key}:"
+                            f" {humanize.naturalsize(str(outer_value), binary=True, gnu=True)}"
                         )
                     else:
                         rows.append(f"- {outer_key}: {outer_value}")
     return "\n".join(rows)
 
 
 def format_value(value: Any) -> str:
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/output/json.py` & `backend.ai-client-23.3.1/ai/backend/client/output/json.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,17 +31,17 @@
         print(
             json.dumps(
                 {
                     "count": 1,
                     "total_count": 1,
                     "items": [
                         {
-                            field_map[k]
-                            .alt_name: field_map[k]
-                            .formatter.format_json(v, field_map[k])
+                            field_map[k].alt_name: field_map[k].formatter.format_json(
+                                v, field_map[k]
+                            )
                             for k, v in item.items()
                             if k in field_map
                         },
                     ],
                 },
                 **_json_opts,
             )
@@ -56,17 +56,17 @@
         print(
             json.dumps(
                 {
                     "count": len(items),
                     "total_count": len(items),
                     "items": [
                         {
-                            field_map[k]
-                            .alt_name: field_map[k]
-                            .formatter.format_json(v, field_map[k])
+                            field_map[k].alt_name: field_map[k].formatter.format_json(
+                                v, field_map[k]
+                            )
                             for k, v in item.items()
                             if k in field_map
                         }
                         for item in items
                     ],
                 },
                 **_json_opts,
@@ -121,17 +121,17 @@
         print(
             json.dumps(
                 {
                     "count": len(result.items),
                     "total_count": result.total_count,
                     "items": [
                         {
-                            field_map[k]
-                            .alt_name: field_map[k]
-                            .formatter.format_json(v, field_map[k])
+                            field_map[k].alt_name: field_map[k].formatter.format_json(
+                                v, field_map[k]
+                            )
                             for k, v in item.items()
                             if k in field_map
                         }
                         for item in result.items
                     ],
                 },
                 **_json_opts,
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/output/types.py` & `backend.ai-client-23.3.1/ai/backend/client/output/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/pagination.py` & `backend.ai-client-23.3.1/ai/backend/client/pagination.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/request.py` & `backend.ai-client-23.3.1/ai/backend/client/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -592,15 +592,15 @@
                         "\u279c {!r}".format(e)
                     )
                     raise BackendClientError(msg) from e
                 else:
                     self.session.config.rotate_endpoints()
                     continue
             except aiohttp.ClientResponseError as e:
-                msg = "API endpoint response error.\n" "\u279c {!r}".format(e)
+                msg = "API endpoint response error.\n\u279c {!r}".format(e)
                 await raw_resp.__aexit__(*sys.exc_info())
                 raise BackendClientError(msg) from e
             finally:
                 self.session.config.load_balance_endpoints()
 
     async def __aexit__(self, *exc_info) -> Optional[bool]:
         assert self._rqst_ctx is not None
@@ -733,15 +733,15 @@
                         "Error detail: {!r}".format(e)
                     )
                     raise BackendClientError(msg) from e
                 else:
                     self.session.config.rotate_endpoints()
                     continue
             except aiohttp.ClientResponseError as e:
-                msg = "API endpoint response error.\n" "\u279c {!r}".format(e)
+                msg = "API endpoint response error.\n\u279c {!r}".format(e)
                 raise BackendClientError(msg) from e
             else:
                 break
             finally:
                 self.session.config.load_balance_endpoints()
 
         wrapped_ws = self.response_cls(self.session, cast(aiohttp.ClientResponse, raw_ws))
@@ -895,15 +895,15 @@
                         "\u279c {!r}".format(e)
                     )
                     raise BackendClientError(msg) from e
                 else:
                     self.session.config.rotate_endpoints()
                     continue
             except aiohttp.ClientResponseError as e:
-                msg = "API endpoint response error.\n" "\u279c {!r}".format(e)
+                msg = "API endpoint response error.\n\u279c {!r}".format(e)
                 raise BackendClientError(msg) from e
             finally:
                 self.session.config.load_balance_endpoints()
 
     async def __aexit__(self, *args) -> Optional[bool]:
         assert self._rqst_ctx is not None
         await self._rqst_ctx.__aexit__(*args)
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/session.py` & `backend.ai-client-23.3.1/ai/backend/client/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,24 +59,28 @@
         )
         async with http_session.get(probe_url, timeout=timeout_config, headers=headers) as resp:
             resp.raise_for_status()
             server_info = await resp.json()
             server_version = parse_api_version(server_info["version"])
             if server_version > client_version:
                 warnings.warn(
-                    "The server API version is higher than the client. "
-                    "Please upgrade the client package.",
+                    (
+                        "The server API version is higher than the client. "
+                        "Please upgrade the client package."
+                    ),
                     category=APIVersionWarning,
                 )
             if server_version < MIN_API_VERSION:
                 warnings.warn(
-                    f"The server is too old and does not meet the minimum API version requirement: "
-                    f"v{MIN_API_VERSION[0]}.{MIN_API_VERSION[1]}\n"
-                    f"Please upgrade the server or downgrade/reinstall the client SDK with "
-                    f"the same major.minor release of the server.",
+                    (
+                        "The server is too old and does not meet the minimum API version"
+                        f" requirement: v{MIN_API_VERSION[0]}.{MIN_API_VERSION[1]}\nPlease upgrade"
+                        " the server or downgrade/reinstall the client SDK with the same"
+                        " major.minor release of the server."
+                    ),
                     category=APIVersionWarning,
                 )
             return min(server_version, client_version)
     except (asyncio.TimeoutError, aiohttp.ClientError):
         # fallback to the configured API version
         return client_version
```

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/utils.py` & `backend.ai-client-23.3.1/ai/backend/client/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/ai/backend/client/versioning.py` & `backend.ai-client-23.3.1/ai/backend/client/versioning.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/backend.ai_client.egg-info/PKG-INFO` & `backend.ai-client-23.3.1/backend.ai_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-client
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Client SDK
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/x-rst
 
 Backend.AI Client
 =================
```

### Comparing `backend.ai-client-23.3.0a4/backend.ai_client.egg-info/SOURCES.txt` & `backend.ai-client-23.3.1/backend.ai_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/backend_shim.py` & `backend.ai-client-23.3.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.0a4/setup.py` & `backend.ai-client-23.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,34 +11,34 @@
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
     ],
     'description': 'Backend.AI Client SDK',
     'entry_points': {
         'backendai_cli_v10': [
             '_ = ai.backend.client.cli.main:main',
         ],
     },
     'install_requires': (
         'aiohttp~=3.8.1',
         'aiotusclient~=0.1.4',
         'appdirs~=1.4.4',
         'async_timeout~=4.0',
         'attrs>=20.3',
-        """backend.ai-cli==23.03.0a4
+        """backend.ai-cli==23.03.1
 """,
-        """backend.ai-common==23.03.0a4
+        """backend.ai-common==23.03.1
 """,
-        """backend.ai-plugin==23.03.0a4
+        """backend.ai-plugin==23.03.1
 """,
         'click>=7.1.2',
         'faker~=13.12.0',
         'humanize>=3.1.0',
         'inquirer~=2.9.2',
         'janus~=1.0.0',
         'multidict>=6.0',
@@ -278,11 +278,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.0a4
+    'version': """23.03.1
 """,
     'zip_safe': False,
 })
```

