# Comparing `tmp/qiskit-ibm-provider-0.5.2.tar.gz` & `tmp/qiskit-ibm-provider-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qiskit-ibm-provider-0.5.2.tar", last modified: Mon Apr 10 21:25:21 2023, max compression
+gzip compressed data, was "qiskit-ibm-provider-0.5.3.tar", last modified: Thu May  4 20:55:26 2023, max compression
```

## Comparing `qiskit-ibm-provider-0.5.2.tar` & `qiskit-ibm-provider-0.5.3.tar`

### file list

```diff
@@ -1,197 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/client_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/runtime_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/program_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/utils/data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/apiconstants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/hub_group_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    37988 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    29558 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_backend_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_qubit_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    32324 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/ibm_circuit_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    48879 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/ibm_composite_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/ibm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/job_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/queueinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/sub_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/backend_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/config_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/backend_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/gates_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/jobs_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/qubits_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/proxies/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/proxies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/proxies/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38998 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/value.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/type_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/basis/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py
--rw-r--r--   0 runner    (1001) docker     (123)    23298 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/backend_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/backend_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/hgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/json_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/qobj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/device_layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/error_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/gate_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/contextmanagers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/e2e/test_real_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/e2e/test_tutorials.py
--rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/fake_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/ibm_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_basic_server_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    38625 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_composite_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_filter_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_ibm_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20848 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_ibm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_ibm_job_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_ibm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_ibm_qasm_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_websocket_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/jobtestcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/proxy_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/unit/mock/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/mock/fake_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/mock/fake_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    22540 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/test_ibm_job_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/test_ibm_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/test_websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/basis/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/control_flow_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    26825 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py
--rw-r--r--   0 runner    (1001) docker     (123)    58260 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/utils/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/ws_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.562969 qiskit-ibm-provider-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-04 20:55:26.562969 qiskit-ibm-provider-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.542968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.542968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/accounts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/accounts/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/accounts/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.542968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/client_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.546968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/runtime_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.546968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/program_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.546968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/utils/data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/apiconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/hub_group_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37528 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/ibm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29558 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/ibm_backend_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/ibm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/ibm_qubit_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.546968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31705 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/ibm_circuit_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48879 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/ibm_composite_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/ibm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/job_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/queueinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/sub_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.550968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/backend_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/config_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.550968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/backend_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/gates_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/jobs_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/qubits_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.550968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/proxies/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/proxies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/proxies/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.550968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.550968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/binary_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/binary_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40086 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/binary_io/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/binary_io/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12654 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/binary_io/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/type_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.550968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.550968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.550968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.554968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23298 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.554968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/backend_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/hgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14949 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/json_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/qobj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.554968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/device_layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.554968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/interactive/error_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/interactive/gate_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.542968 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-04 20:55:26.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-04 20:55:26.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:55:26.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-04 20:55:26.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:55:26.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-04 20:55:26.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 20:55:26.000000 qiskit-ibm-provider-0.5.3/qiskit_ibm_provider.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-04 20:55:26.562969 qiskit-ibm-provider-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.554968 qiskit-ibm-provider-0.5.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/contextmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.558968 qiskit-ibm-provider-0.5.3/test/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/e2e/test_real_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/e2e/test_tutorials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/fake_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/ibm_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.558968 qiskit-ibm-provider-0.5.3/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/integration/test_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/integration/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/integration/test_basic_server_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40183 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/integration/test_composite_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/integration/test_filter_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/integration/test_ibm_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20823 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/integration/test_ibm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/integration/test_ibm_job_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/integration/test_ibm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/integration/test_ibm_qasm_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/integration/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/integration/test_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/integration/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/integration/test_websocket_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/jobtestcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/proxy_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.558968 qiskit-ibm-provider-0.5.3/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.558968 qiskit-ibm-provider-0.5.3/test/unit/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/mock/fake_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/mock/fake_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22540 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/test_ibm_job_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/test_ibm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/test_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.558968 qiskit-ibm-provider-0.5.3/test/unit/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.558968 qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.562969 qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.562969 qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/scheduling/control_flow_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26825 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58260 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/scheduling/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/scheduling/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:55:26.562969 qiskit-ibm-provider-0.5.3/test/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/unit/utils/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-04 20:55:11.000000 qiskit-ibm-provider-0.5.3/test/ws_server.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qiskit-ibm-provider-0.5.2/LICENSE.txt` & `qiskit-ibm-provider-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/PKG-INFO` & `qiskit-ibm-provider-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-provider
-Version: 0.5.2
+Version: 0.5.3
 Summary: Qiskit IBM Quantum Provider for accessing the quantum devices and simulators at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-provider
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-provider/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
@@ -14,20 +14,19 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: visualization
 License-File: LICENSE.txt
 
 # Qiskit IBM Quantum Provider
 
 [![License](https://img.shields.io/github/license/Qiskit/qiskit-ibm-provider.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)
```

### Comparing `qiskit-ibm-provider-0.5.2/README.md` & `qiskit-ibm-provider-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/account.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/accounts/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/exceptions.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/accounts/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/management.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/accounts/management.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/storage.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/accounts/storage.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/auth.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/client_parameters.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/client_parameters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/account.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/auth.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/base.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/runtime.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/runtime.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/runtime_ws.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/runtime_ws.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/version.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/websocket.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/clients/websocket.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/exceptions.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/backend.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,16 +101,16 @@
             "backend_name": self.backend_name,
             "backend_version": response.get("backend_version", "0.0.0"),
             "status_msg": response.get("status", ""),
             "operational": bool(response.get("state", False)),
         }
 
         # 'pending_jobs' is required, and should be >= 0.
-        if "lengthQueue" in response:
-            ret["pending_jobs"] = max(response["lengthQueue"], 0)
+        if "length_queue" in response:
+            ret["pending_jobs"] = max(response["length_queue"], 0)
         else:
             ret["pending_jobs"] = 0
 
         return ret
 
     def configuration(self) -> Dict[str, Any]:
         """Return backend configuration.
```

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/base.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/job.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/program_job.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/program_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/root.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/root.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/runtime.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/runtime.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/utils/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/utils/data_mapper.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/rest/utils/data_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/session.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/api/session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/apiconstants.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/apiconstants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/exceptions.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/hub_group_project.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/hub_group_project.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_backend.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/ibm_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,19 +54,20 @@
 )
 from .job import IBMJob, IBMCircuitJob
 from .transpiler.passes.basis.convert_id_to_delay import (
     ConvertIdToDelay,
 )
 from .utils import validate_job_tags
 from .utils.options import QASM2Options, QASM3Options
-from .utils.backend_converter import (
-    convert_to_target,
-)
 from .utils.converters import local_to_utc
-from .utils.json_decoder import defaults_from_server_data, properties_from_server_data
+from .utils.json_decoder import (
+    defaults_from_server_data,
+    properties_from_server_data,
+    target_from_server_data,
+)
 from .api.exceptions import RequestsApiError
 
 
 logger = logging.getLogger(__name__)
 
 
 QOBJRUNNERPROGRAMID = "circuit-runner"
@@ -233,19 +234,14 @@
         # Prevent recursion since these properties are accessed within __getattr__
         if name in ["_properties", "_defaults", "_target"]:
             raise AttributeError(
                 "'{}' object has no attribute '{}'".format(
                     self.__class__.__name__, name
                 )
             )
-        # Lazy load properties and pulse defaults and construct the target object.
-        self._get_properties()
-        self._get_defaults()
-        self._convert_to_target()
-        # Check if the attribute now is available on IBMBackend class due to above steps
         try:
             return super().__getattribute__(name)
         except AttributeError:
             pass
         # If attribute is still not available on IBMBackend class,
         # fallback to check if the attribute is available in configuration
         try:
@@ -253,43 +249,40 @@
         except AttributeError:
             raise AttributeError(
                 "'{}' object has no attribute '{}'".format(
                     self.__class__.__name__, name
                 )
             )
 
-    def _get_properties(self, datetime: Optional[python_datetime] = None) -> None:
-        """Gets backend properties and decodes it"""
-        if not self._properties:
-            if datetime:
-                datetime = local_to_utc(datetime)
-            api_properties = self.provider._runtime_client.backend_properties(
-                self.name, datetime=datetime
-            )
-            if api_properties:
-                backend_properties = properties_from_server_data(api_properties)
-                self._properties = backend_properties
-
-    def _get_defaults(self) -> None:
-        """Gets defaults if pulse backend and decodes it"""
-        if not self._defaults:
-            api_defaults = self.provider._runtime_client.backend_pulse_defaults(
-                self.name
-            )
-            if api_defaults:
-                self._defaults = defaults_from_server_data(api_defaults)
+    def _get_target(
+        self,
+        *,
+        datetime: Optional[python_datetime] = None,
+        refresh: bool = False,
+    ) -> Target:
+        """Gets target from configuration, properties and pulse defaults."""
+        if datetime:
+            if not isinstance(datetime, python_datetime):
+                raise TypeError("'{}' is not of type 'datetime'.")
+            datetime = local_to_utc(datetime)
 
-    def _convert_to_target(self) -> None:
-        """Converts backend configuration, properties and defaults to Target object"""
-        if not self._target:
-            self._target = convert_to_target(
+        if datetime or refresh or self._target is None:
+            client = getattr(self.provider, "_runtime_client")
+            api_properties = client.backend_properties(self.name, datetime=datetime)
+            api_pulse_defaults = client.backend_pulse_defaults(self.name)
+            target = target_from_server_data(
                 configuration=self._configuration,
-                properties=self._properties,
-                defaults=self._defaults,
+                pulse_defaults=api_pulse_defaults,
+                properties=api_properties,
             )
+            if datetime:
+                # Don't cache result.
+                return target
+            self._target = target
+        return self._target
 
     @classmethod
     def _default_options(cls) -> Options:
         """Default runtime options."""
         return Options(**{**asdict(QASM3Options()), **asdict(QASM2Options())})
 
     @property
@@ -320,28 +313,22 @@
 
     @property
     def target(self) -> Target:
         """A :class:`qiskit.transpiler.Target` object for the backend.
         Returns:
             Target
         """
-        self._get_properties()
-        self._get_defaults()
-        self._convert_to_target()
-        return self._target
+        return self._get_target()
 
     def target_history(self, datetime: Optional[python_datetime] = None) -> Target:
         """A :class:`qiskit.transpiler.Target` object for the backend.
         Returns:
             Target with properties found on `datetime`
         """
-        self._get_properties(datetime=datetime)
-        self._get_defaults()
-        self._convert_to_target()
-        return self._target
+        return self._get_target(datetime=datetime)
 
     def run(
         self,
         circuits: Union[
             QuantumCircuit, Schedule, List[Union[QuantumCircuit, Schedule]]
         ],
         dynamic: bool = False,
@@ -436,14 +423,19 @@
                 - If an input parameter value is not valid.
                 - If ESP readout is used and the backend does not support this.
         """
         # pylint: disable=arguments-differ
 
         validate_job_tags(job_tags, IBMBackendValueError)
 
+        if dynamic and "qasm3" not in getattr(
+            self.configuration(), "supported_features", []
+        ):
+            warnings.warn(f"The backend {self.name} does not support dynamic circuits.")
+
         status = self.status()
         if status.operational is True and status.status_msg != "active":
             warnings.warn(f"The backend {self.name} is currently paused.")
 
         program_id = str(run_config.get("program_id", ""))
         if not program_id:
             if dynamic:
@@ -790,15 +782,15 @@
 
             self.id_warning_issued = True
 
         # Make sure we don't mutate user's input circuits
         circuits = copy.deepcopy(circuits)
         # Convert id gates to delays.
         pm = PassManager(  # pylint: disable=invalid-name
-            ConvertIdToDelay(self._target.durations())
+            ConvertIdToDelay(self.target.durations())
         )
         circuits = pm.run(circuits)
 
         return circuits
 
     def get_translation_stage_plugin(self) -> str:
         """Return the default translation stage plugin name for IBM backends."""
```

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_backend_service.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/ibm_backend_service.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_provider.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/ibm_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_qubit_properties.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/ibm_qubit_properties.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/constants.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/exceptions.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/ibm_circuit_job.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/ibm_circuit_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,14 @@
     instance as attributes. Given that Qiskit and the server can be updated
     independently, some of these attributes might be deprecated or experimental.
     Supported attributes can be retrieved via methods. For example, you
     can use :meth:`creation_date()` to retrieve the job creation date,
     which is a supported attribute.
     """
 
-    _data = {}  # type: Dict
-
     _executor = futures.ThreadPoolExecutor()
     """Threads used for asynchronous processing."""
 
     def __init__(
         self,
         backend: "ibm_backend.IBMBackend",
         api_client: AccountClient,
@@ -167,19 +165,14 @@
         self._params: Dict[str, Any] = None
         self._queue_info: QueueInfo = None
         if status is not None:
             self._status = api_status_to_job_status(status)
         self._client_version = self._extract_client_version(client_info)
         self._set_result(result)
 
-        self._data = {}
-        for key, value in kwargs.items():
-            # Append suffix to key to avoid conflicts.
-            self._data[key + "_"] = value
-
         # Properties used for caching.
         self._cancelled = False
         self._job_error_msg = None  # type: Optional[str]
         self._refreshed = False
 
         self._ws_client_future = None  # type: Optional[futures.Future]
         self._result_queue = queue.Queue()  # type: queue.Queue
@@ -356,18 +349,14 @@
         with api_to_job_error():
             api_response = self._runtime_client.job_get(self.job_id())["state"]
             # response state possibly has two values: status and reason
             # reason is not used in the current interface
             self._api_status = api_response["status"]
             self._status = api_status_to_job_status(self._api_status)
 
-        # Get all job attributes if the job is done.
-        if self._status in JOB_FINAL_STATES:
-            self.refresh()
-
         return self._status
 
     def error_message(self) -> Optional[str]:
         """Provide details about the reason of failure.
 
         Returns:
             An error report if the job failed or ``None`` otherwise.
@@ -553,17 +542,14 @@
             api_metadata.get("qiskit_version", None)
         )
         if self._status == JobStatus.DONE:
             api_result = self._download_external_result(
                 self._runtime_client.job_results(self.job_id())
             )
             self._set_result(api_result)
-
-        for key, value in api_response.items():
-            self._data[key + "_"] = value
         self._refreshed = True
 
     def backend_options(self) -> Dict:
         """Return the backend configuration options used for this job.
 
         Options that are not applicable to the job execution are not returned.
         Some but not all of the options with default values are returned.
@@ -833,13 +819,7 @@
         Raises:
             NotImplementedError: Upon invocation.
         """
         raise NotImplementedError(
             "job.submit() is not supported. Please use "
             "IBMBackend.run() to submit a job."
         )
-
-    def __getattr__(self, name: str) -> Any:
-        try:
-            return self._data[name]
-        except KeyError:
-            raise AttributeError("Attribute {} is not defined.".format(name)) from None
```

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/ibm_composite_job.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/ibm_composite_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/ibm_job.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/ibm_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/job_monitor.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/job_monitor.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/queueinfo.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/queueinfo.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/sub_job.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/sub_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/utils.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/job/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/backend_info.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/backend_info.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/config_widget.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/config_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/backend_update.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/backend_update.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/constants.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/dashboard.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/utils.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/gates_widget.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/gates_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/jobs_widget.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/jobs_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/qubits_widget.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/jupyter/qubits_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/proxies/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/proxies/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/proxies/configuration.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/proxies/configuration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/binary_io/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/circuits.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/binary_io/circuits.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,41 +121,57 @@
         if data.type.decode("utf8") == "q":
             registers["q"][name] = (data.standalone, bit_indices, True)
         else:
             registers["c"][name] = (data.standalone, bit_indices, True)
     return registers
 
 
-def _loads_instruction_parameter(type_key, data_bytes, version, vectors):  # type: ignore[no-untyped-def]
+def _loads_instruction_parameter(  # type: ignore[no-untyped-def]
+    type_key, data_bytes, version, vectors, registers, circuit
+):
     if type_key == type_keys.Program.CIRCUIT:
         param = common.data_from_binary(data_bytes, read_circuit, version=version)
     elif type_key == type_keys.Container.RANGE:
         data = formats.RANGE._make(struct.unpack(formats.RANGE_PACK, data_bytes))
         param = range(data.start, data.stop, data.step)
     elif type_key == type_keys.Container.TUPLE:
         param = tuple(
             common.sequence_from_binary(
                 data_bytes,
                 _loads_instruction_parameter,
                 version=version,
                 vectors=vectors,
+                registers=registers,
+                circuit=circuit,
             )
         )
     elif type_key == type_keys.Value.INTEGER:
         # TODO This uses little endian. Should be fixed in the next QPY version.
         param = struct.unpack("<q", data_bytes)[0]
     elif type_key == type_keys.Value.FLOAT:
         # TODO This uses little endian. Should be fixed in the next QPY version.
         param = struct.unpack("<d", data_bytes)[0]
+    elif type_key == type_keys.Value.REGISTER:
+        param = _loads_register_param(
+            data_bytes.decode(common.ENCODE), circuit, registers
+        )
     else:
         param = value.loads_value(type_key, data_bytes, version, vectors)
 
     return param
 
 
+def _loads_register_param(data_bytes, circuit, registers):  # type: ignore[no-untyped-def]
+    # If register name prefixed with null character it's a clbit index for single bit condition.
+    if data_bytes[0] == "\x00":
+        conditional_bit = int(data_bytes[1:])
+        return circuit.clbits[conditional_bit]
+    return registers["c"][data_bytes]
+
+
 def _read_instruction(  # type: ignore[no-untyped-def]
     file_obj, circuit, registers, custom_operations, version, vectors
 ):
     if version < 5:
         instruction = formats.CIRCUIT_INSTRUCTION._make(
             struct.unpack(
                 formats.CIRCUIT_INSTRUCTION_PACK,
@@ -176,25 +192,18 @@
     )
     qargs = []
     cargs = []
     params = []
     condition_tuple = None
     if instruction.has_condition:
         # If register name prefixed with null character it's a clbit index for single bit condition.
-        if condition_register[0] == "\x00":
-            conditional_bit = int(condition_register[1:])
-            condition_tuple = (
-                circuit.clbits[conditional_bit],
-                instruction.condition_value,
-            )
-        else:
-            condition_tuple = (
-                registers["c"][condition_register],
-                instruction.condition_value,
-            )
+        condition_tuple = (
+            _loads_register_param(condition_register, circuit, registers),
+            instruction.condition_value,
+        )
     if circuit is not None:
         qubit_indices = dict(enumerate(circuit.qubits))
         clbit_indices = dict(enumerate(circuit.clbits))
     else:
         qubit_indices = {}
         clbit_indices = {}
 
@@ -220,15 +229,17 @@
             if carg.type.decode(common.ENCODE) == "q":
                 raise TypeError("Invalid input qarg after all qargs")
             cargs.append(clbit_indices[carg.size])
 
     # Load Parameters
     for _param in range(instruction.num_parameters):
         type_key, data_bytes = common.read_generic_typed_data(file_obj)
-        param = _loads_instruction_parameter(type_key, data_bytes, version, vectors)
+        param = _loads_instruction_parameter(
+            type_key, data_bytes, version, vectors, registers, circuit
+        )
         params.append(param)
 
     # Load Gate object
     if gate_name in {"Gate", "Instruction", "ControlledGate"}:
         inst_obj = _parse_custom_operation(
             custom_operations, gate_name, params, version, vectors, registers
         )
@@ -277,15 +288,21 @@
             gate = gate_class(*params, instruction.num_ctrl_qubits)
         else:
             gate = gate_class(*params)
             gate.num_ctrl_qubits = instruction.num_ctrl_qubits
             gate.ctrl_state = instruction.ctrl_state
         gate.condition = condition_tuple
     else:
-        if gate_name in {"Initialize", "UCRXGate", "UCRYGate", "UCRZGate"}:
+        if gate_name in {
+            "Initialize",
+            "StatePreparation",
+            "UCRXGate",
+            "UCRYGate",
+            "UCRZGate",
+        }:
             gate = gate_class(params)
         else:
             if gate_name == "Barrier":
                 params = [len(qargs)]
             elif gate_name in {"BreakLoopOp", "ContinueLoopOp"}:
                 params = [len(qargs), len(cargs)]
             gate = gate_class(*params)
@@ -489,34 +506,46 @@
             calibrations[name] = {(qubits, params): schedule}
         else:
             calibrations[name][(qubits, params)] = schedule
 
     return calibrations
 
 
-def _dumps_instruction_parameter(param):  # type: ignore[no-untyped-def]
+def _dumps_register(register, index_map):  # type: ignore[no-untyped-def]
+    if isinstance(register, ClassicalRegister):
+        return register.name.encode(common.ENCODE)
+    # Clbit.
+    return b"\x00" + str(index_map["c"][register]).encode(common.ENCODE)
+
+
+def _dumps_instruction_parameter(param, index_map):  # type: ignore[no-untyped-def]
     if isinstance(param, QuantumCircuit):
         type_key = type_keys.Program.CIRCUIT
         data_bytes = common.data_to_binary(param, write_circuit)
     elif isinstance(param, range):
         type_key = type_keys.Container.RANGE
         data_bytes = struct.pack(
             formats.RANGE_PACK, param.start, param.stop, param.step
         )
     elif isinstance(param, tuple):
         type_key = type_keys.Container.TUPLE
-        data_bytes = common.sequence_to_binary(param, _dumps_instruction_parameter)
+        data_bytes = common.sequence_to_binary(
+            param, _dumps_instruction_parameter, index_map=index_map
+        )
     elif isinstance(param, int):
         # TODO This uses little endian. This should be fixed in next QPY version.
         type_key = type_keys.Value.INTEGER
         data_bytes = struct.pack("<q", param)
     elif isinstance(param, float):
         # TODO This uses little endian. This should be fixed in next QPY version.
         type_key = type_keys.Value.FLOAT
         data_bytes = struct.pack("<d", param)
+    elif isinstance(param, (Clbit, ClassicalRegister)):
+        type_key = type_keys.Value.REGISTER
+        data_bytes = _dumps_register(param, index_map)
     else:
         type_key, data_bytes = value.dumps_value(param)
 
     return type_key, data_bytes
 
 
 # pylint: disable=too-many-boolean-expressions
@@ -549,38 +578,43 @@
         custom_operations_list.append(gate_class_name)
 
     has_condition = False
     condition_register = b""
     condition_value = 0
     if getattr(instruction.operation, "condition", None):
         has_condition = True
-        if isinstance(instruction.operation.condition[0], Clbit):
-            bit_index = index_map["c"][instruction.operation.condition[0]]
-            condition_register = b"\x00" + str(bit_index).encode(common.ENCODE)
-            condition_value = int(instruction.operation.condition[1])
-        else:
-            condition_register = instruction.operation.condition[0].name.encode(
-                common.ENCODE
-            )
-            condition_value = instruction.operation.condition[1]
+        condition_register = _dumps_register(
+            instruction.operation.condition[0], index_map
+        )
+        condition_value = int(instruction.operation.condition[1])
 
     gate_class_name = gate_class_name.encode(common.ENCODE)
     label = getattr(instruction.operation, "label")
     if label:
         label_raw = label.encode(common.ENCODE)
     else:
         label_raw = b""
 
+    # The instruction params we store are about being able to reconstruct the objects; they don't
+    # necessarily need to match one-to-one to the `params` field.
+    if isinstance(instruction.operation, controlflow.SwitchCaseOp):
+        instruction_params = [
+            instruction.operation.target,
+            tuple(instruction.operation.cases_specifier()),
+        ]
+    else:
+        instruction_params = instruction.operation.params
+
     num_ctrl_qubits = getattr(instruction.operation, "num_ctrl_qubits", 0)
     ctrl_state = getattr(instruction.operation, "ctrl_state", 0)
     instruction_raw = struct.pack(
         formats.CIRCUIT_INSTRUCTION_V2_PACK,
         len(gate_class_name),
         len(label_raw),
-        len(instruction.operation.params),
+        len(instruction_params),
         instruction.operation.num_qubits,
         instruction.operation.num_clbits,
         has_condition,
         len(condition_register),
         condition_value,
         num_ctrl_qubits,
         ctrl_state,
@@ -597,16 +631,16 @@
         file_obj.write(instruction_arg_raw)
     for clbit in instruction.clbits:
         instruction_arg_raw = struct.pack(
             formats.CIRCUIT_INSTRUCTION_ARG_PACK, b"c", index_map["c"][clbit]
         )
         file_obj.write(instruction_arg_raw)
     # Encode instruction params
-    for param in instruction.operation.params:
-        type_key, data_bytes = _dumps_instruction_parameter(param)
+    for param in instruction_params:
+        type_key, data_bytes = _dumps_instruction_parameter(param, index_map)
         common.write_generic_typed_data(file_obj, type_key, data_bytes)
     return custom_operations_list
 
 
 def _write_pauli_evolution_gate(file_obj, evolution_gate):  # type: ignore[no-untyped-def]
     operator_list = evolution_gate.operator
     standalone = False
```

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/schedules.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/binary_io/schedules.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 import struct
 import zlib
 import warnings
 
 import numpy as np
 
 from qiskit.exceptions import QiskitError
-from qiskit.pulse import library, channels
+from qiskit.pulse import library, channels, instructions
 from qiskit.pulse.schedule import ScheduleBlock
 from qiskit.utils import optionals as _optional
 from .. import formats, common, type_keys
+from ..exceptions import QpyError
 from . import value
 
 
 if _optional.HAS_SYMENGINE:
     import symengine as sym
 else:
     import sympy as sym
@@ -245,14 +246,16 @@
             )
         else:
             return common.data_from_binary(
                 data_bytes, _read_symbolic_pulse_v6, version=version
             )
     if type_key == type_keys.ScheduleOperand.CHANNEL:
         return common.data_from_binary(data_bytes, _read_channel, version=version)
+    if type_key == type_keys.ScheduleOperand.OPERAND_STR:
+        return data_bytes.decode(common.ENCODE)
 
     return value.loads_value(type_key, data_bytes, version, {})
 
 
 def _read_element(file_obj, version, metadata_deserializer):  # type: ignore[no-untyped-def]
     type_key = common.read_type_key(file_obj)
 
@@ -268,14 +271,34 @@
     instance._operands = tuple(operands)
     instance._name = name
     instance._hash = None
 
     return instance
 
 
+def _loads_reference_item(  # type: ignore[no-untyped-def]
+    type_key, data_bytes, version, metadata_deserializer
+):
+    if type_key == type_keys.Value.NULL:
+        return None
+    if type_key == type_keys.Program.SCHEDULE_BLOCK:
+        return common.data_from_binary(
+            data_bytes,
+            deserializer=read_schedule_block,
+            version=version,
+            metadata_deserializer=metadata_deserializer,
+        )
+
+    raise QpyError(
+        f"Loaded schedule reference item is neither None nor ScheduleBlock. "
+        f"Type key {type_key} is not valid data type for a reference items. "
+        "This data cannot be loaded. Please check QPY version."
+    )
+
+
 def _write_channel(file_obj, data):  # type: ignore[no-untyped-def]
     type_key = type_keys.ScheduleChannel.assign(data)
     common.write_type_key(file_obj, type_key)
     value.write_value(file_obj, data.index)
 
 
 def _write_waveform(file_obj, data):  # type: ignore[no-untyped-def]
@@ -349,14 +372,17 @@
         data_bytes = common.data_to_binary(operand, _write_waveform)
     elif isinstance(operand, library.SymbolicPulse):
         type_key = type_keys.ScheduleOperand.SYMBOLIC_PULSE
         data_bytes = common.data_to_binary(operand, _write_symbolic_pulse)
     elif isinstance(operand, channels.Channel):
         type_key = type_keys.ScheduleOperand.CHANNEL
         data_bytes = common.data_to_binary(operand, _write_channel)
+    elif isinstance(operand, str):
+        type_key = type_keys.ScheduleOperand.OPERAND_STR
+        data_bytes = operand.encode(common.ENCODE)
     else:
         type_key, data_bytes = value.dumps_value(operand)
 
     return type_key, data_bytes
 
 
 def _write_element(file_obj, element, metadata_serializer):  # type: ignore[no-untyped-def]
@@ -370,14 +396,28 @@
             file_obj,
             sequence=element.operands,
             serializer=_dumps_operand,
         )
         value.write_value(file_obj, element.name)
 
 
+def _dumps_reference_item(schedule, metadata_serializer):  # type: ignore[no-untyped-def]
+    if schedule is None:
+        type_key = type_keys.Value.NULL
+        data_bytes = b""
+    else:
+        type_key = type_keys.Program.SCHEDULE_BLOCK
+        data_bytes = common.data_to_binary(
+            obj=schedule,
+            serializer=write_schedule_block,
+            metadata_serializer=metadata_serializer,
+        )
+    return type_key, data_bytes
+
+
 def read_schedule_block(file_obj, version, metadata_deserializer=None):  # type: ignore[no-untyped-def]
     """Read a single ScheduleBlock from the file like object.
 
     Args:
         file_obj (File): A file like object that contains the QPY binary data.
         version (int): QPY version.
         metadata_deserializer (JSONDecoder): An optional JSONDecoder class
@@ -415,14 +455,32 @@
         metadata=metadata,
         alignment_context=context,
     )
     for _ in range(data.num_elements):
         block_elm = _read_element(file_obj, version, metadata_deserializer)
         block.append(block_elm, inplace=True)
 
+    # Load references
+    if version >= 7:
+        flat_key_refdict = common.read_mapping(
+            file_obj=file_obj,
+            deserializer=_loads_reference_item,
+            version=version,
+            metadata_deserializer=metadata_deserializer,
+        )
+        ref_dict = {}
+        for key_str, schedule in flat_key_refdict.items():
+            if schedule is not None:
+                composite_key = tuple(
+                    key_str.split(instructions.Reference.key_delimiter)
+                )
+                ref_dict[composite_key] = schedule
+        if ref_dict:
+            block.assign_references(ref_dict, inplace=True)
+
     return block
 
 
 def write_schedule_block(file_obj, block, metadata_serializer=None):  # type: ignore[no-untyped-def]
     """Write a single ScheduleBlock object in the file like object.
 
     Args:
@@ -449,9 +507,22 @@
     )
     header = struct.pack(formats.SCHEDULE_BLOCK_HEADER_PACK, *header_raw)
     file_obj.write(header)
     file_obj.write(block_name)
     file_obj.write(metadata)
 
     _write_alignment_context(file_obj, block.alignment_context)
-    for block_elm in block.blocks:
+    for block_elm in block._blocks:
         _write_element(file_obj, block_elm, metadata_serializer)
+
+    # Write references
+    flat_key_refdict = {}
+    for ref_keys, schedule in block._reference_manager.items():
+        # Do not call block.reference. This returns the reference of most outer program by design.
+        key_str = instructions.Reference.key_delimiter.join(ref_keys)
+        flat_key_refdict[key_str] = schedule
+    common.write_mapping(
+        file_obj=file_obj,
+        mapping=flat_key_refdict,
+        serializer=_dumps_reference_item,
+        metadata_serializer=metadata_serializer,
+    )
```

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/value.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/binary_io/value.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import struct
 from typing import Any
 import uuid
 
 import numpy as np
 
+from qiskit.circuit import CASE_DEFAULT
 from qiskit.circuit.parameter import Parameter
 from qiskit.circuit.parameterexpression import ParameterExpression
 from qiskit.circuit.parametervector import ParameterVector, ParameterVectorElement
 from qiskit.utils import optionals as _optional
 
 from .. import common, formats, exceptions, type_keys
 
@@ -241,15 +242,15 @@
         binary_data = struct.pack("!d", obj)
     elif type_key == type_keys.Value.COMPLEX:
         binary_data = struct.pack(formats.COMPLEX_PACK, obj.real, obj.imag)
     elif type_key == type_keys.Value.NUMPY_OBJ:
         binary_data = common.data_to_binary(obj, np.save)
     elif type_key == type_keys.Value.STRING:
         binary_data = obj.encode(common.ENCODE)
-    elif type_key == type_keys.Value.NULL:
+    elif type_key in (type_keys.Value.NULL, type_keys.Value.CASE_DEFAULT):
         binary_data = b""
     elif type_key == type_keys.Value.PARAMETER_VECTOR:
         binary_data = common.data_to_binary(obj, _write_parameter_vec)
     elif type_key == type_keys.Value.PARAMETER:
         binary_data = common.data_to_binary(obj, _write_parameter)
     elif type_key == type_keys.Value.PARAMETER_EXPRESSION:
         binary_data = common.data_to_binary(
@@ -298,14 +299,16 @@
         return complex(*struct.unpack(formats.COMPLEX_PACK, binary_data))
     if type_key == type_keys.Value.NUMPY_OBJ:
         return common.data_from_binary(binary_data, np.load)
     if type_key == type_keys.Value.STRING:
         return binary_data.decode(common.ENCODE)
     if type_key == type_keys.Value.NULL:
         return None
+    if type_key == type_keys.Value.CASE_DEFAULT:
+        return CASE_DEFAULT
     if type_key == type_keys.Value.PARAMETER_VECTOR:
         return common.data_from_binary(
             binary_data, _read_parameter_vec, vectors=vectors
         )
     if type_key == type_keys.Value.PARAMETER:
         return common.data_from_binary(binary_data, _read_parameter)
     if type_key == type_keys.Value.PARAMETER_EXPRESSION:
```

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/common.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 
 import io
 import struct
 
 from . import formats
 
-QPY_VERSION = 6
+QPY_VERSION = 7
 ENCODE = "utf8"
 
 
 def read_generic_typed_data(file_obj):  # type: ignore[no-untyped-def]
     """Read a single data chunk from the file like object.
 
     Args:
```

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/exceptions.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/formats.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/formats.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/interface.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import warnings
 import re
 
 from qiskit.circuit import QuantumCircuit
 from qiskit.pulse import ScheduleBlock
 from qiskit.exceptions import QiskitError
 from qiskit.version import __version__
-from qiskit.utils.deprecation import deprecate_arguments
+from qiskit.utils.deprecation import deprecate_arg
 
 from . import formats, common, binary_io, type_keys
 from .exceptions import QpyError
 
 
 # pylint: disable=invalid-name
 QPY_SUPPORTED_TYPES = Union[QuantumCircuit, ScheduleBlock]
@@ -70,15 +70,15 @@
     (?:\+(?P<local>[a-z0-9]+(?:[-_\.][a-z0-9]+)*))?       # local version
 """
     + "$"
 )
 VERSION_PATTERN_REGEX = re.compile(VERSION_PATTERN, re.VERBOSE | re.IGNORECASE)
 
 
-@deprecate_arguments({"circuits": "programs"})
+@deprecate_arg("circuits", new_alias="programs", since="0.21.0")
 def dump(  # type: ignore[no-untyped-def]
     programs: Union[List[QPY_SUPPORTED_TYPES], QPY_SUPPORTED_TYPES],
     file_obj: BinaryIO,
     metadata_serializer: Optional[Type[JSONEncoder]] = None,
 ):
     """Write QPY binary data to a file
```

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/type_keys.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/qpy/type_keys.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,23 @@
 """
 
 from abc import abstractmethod
 from enum import Enum
 
 import numpy as np
 
-from qiskit.circuit import Gate, Instruction, QuantumCircuit, ControlledGate
+from qiskit.circuit import (
+    Gate,
+    Instruction,
+    QuantumCircuit,
+    ControlledGate,
+    CASE_DEFAULT,
+    Clbit,
+    ClassicalRegister,
+)
 from qiskit.circuit.library import PauliEvolutionGate
 from qiskit.circuit.parameter import Parameter
 from qiskit.circuit.parameterexpression import ParameterExpression
 from qiskit.circuit.parametervector import ParameterVectorElement
 from qiskit.pulse.channels import (
     Channel,
     DriveChannel,
@@ -41,14 +49,15 @@
     Delay,
     SetFrequency,
     ShiftFrequency,
     SetPhase,
     ShiftPhase,
     RelativeBarrier,
     TimeBlockade,
+    Reference,
 )
 from qiskit.pulse.library import Waveform, SymbolicPulse
 from qiskit.pulse.schedule import ScheduleBlock
 from qiskit.pulse.transforms.alignments import (
     AlignLeft,
     AlignRight,
     AlignSequential,
@@ -91,14 +100,16 @@
     COMPLEX = b"c"
     NUMPY_OBJ = b"n"
     PARAMETER = b"p"
     PARAMETER_VECTOR = b"v"
     PARAMETER_EXPRESSION = b"e"
     STRING = b"s"
     NULL = b"z"
+    CASE_DEFAULT = b"d"
+    REGISTER = b"R"
 
     @classmethod
     def assign(cls, obj):  # type: ignore[no-untyped-def]
         if isinstance(obj, int):
             return cls.INTEGER
         if isinstance(obj, float):
             return cls.FLOAT
@@ -110,16 +121,20 @@
             return cls.PARAMETER_VECTOR
         if isinstance(obj, Parameter):
             return cls.PARAMETER
         if isinstance(obj, ParameterExpression):
             return cls.PARAMETER_EXPRESSION
         if isinstance(obj, str):
             return cls.STRING
+        if isinstance(obj, (Clbit, ClassicalRegister)):
+            return cls.REGISTER
         if obj is None:
             return cls.NULL
+        if obj is CASE_DEFAULT:
+            return cls.CASE_DEFAULT
 
         raise exceptions.QpyError(
             f"Object type '{type(obj)}' is not supported in {cls.__name__} namespace."
         )
 
     @classmethod
     def retrieve(cls, type_key):  # type: ignore[no-untyped-def]
@@ -225,14 +240,15 @@
     DELAY = b"d"
     SET_FREQUENCY = b"f"
     SHIFT_FREQUENCY = b"g"
     SET_PHASE = b"q"
     SHIFT_PHASE = b"r"
     BARRIER = b"b"
     TIME_BLOCKADE = b"t"
+    REFERENCE = b"y"
 
     # 's' is reserved by ScheduleBlock, i.e. block can be nested as an element.
     # Call instructon is not supported by QPY.
     # This instruction has been excluded from ScheduleBlock instructions with
     # qiskit-terra/#8005 and new instruction Reference will be added instead.
     # Call is only applied to Schedule which is not supported by QPY.
     # Also snapshot is not suppored because of its limited usecase.
@@ -253,14 +269,16 @@
             return cls.SET_PHASE
         if isinstance(obj, ShiftPhase):
             return cls.SHIFT_PHASE
         if isinstance(obj, RelativeBarrier):
             return cls.BARRIER
         if isinstance(obj, TimeBlockade):
             return cls.TIME_BLOCKADE
+        if isinstance(obj, Reference):
+            return cls.REFERENCE
 
         raise exceptions.QpyError(
             f"Object type '{type(obj)}' is not supported in {cls.__name__} namespace."
         )
 
     @classmethod
     def retrieve(cls, type_key):  # type: ignore[no-untyped-def]
@@ -278,14 +296,16 @@
             return SetPhase
         if type_key == cls.SHIFT_PHASE:
             return ShiftPhase
         if type_key == cls.BARRIER:
             return RelativeBarrier
         if type_key == cls.TIME_BLOCKADE:
             return TimeBlockade
+        if type_key == cls.REFERENCE:
+            return Reference
 
         raise exceptions.QpyError(
             f"A class corresponding to type key '{type_key}' is not found in {cls.__name__} namespace."
         )
 
 
 class ScheduleOperand(TypeKeyBase):
@@ -295,14 +315,20 @@
     SYMBOLIC_PULSE = b"s"
     CHANNEL = b"c"
 
     # Discriminator and Acquire instance are not serialzied.
     # Data format of these object is somewhat opaque and not defiend well.
     # It's rarely used in the Qiskit experiements. Of course these can be added later.
 
+    # We need to have own string type definition for operands of schedule instruction.
+    # Note that string type is already defined in the Value namespace,
+    # but its key "s" conflicts with the SYMBOLIC_PULSE in the ScheduleOperand namespace.
+    # New in QPY version 7.
+    OPERAND_STR = b"o"
+
     @classmethod
     def assign(cls, obj):  # type: ignore[no-untyped-def]
         if isinstance(obj, Waveform):
             return cls.WAVEFORM
         if isinstance(obj, SymbolicPulse):
             return cls.SYMBOLIC_PULSE
         if isinstance(obj, Channel):
```

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/basis/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/basis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Utility functions for scheduling passes."""
 
+import warnings
 from typing import List, Generator, Optional, Tuple, Union
 
 from qiskit.circuit import ControlFlowOp, Measure, Reset, Parameter
 from qiskit.dagcircuit import DAGCircuit, DAGOpNode
 from qiskit.transpiler.instruction_durations import (
     InstructionDurations,
     InstructionDurationsType,
@@ -133,14 +134,15 @@
     required for the legacy Qobj-based path. For now we use this
     class to report updated InstructionDurations.
     TODO: This would be mitigated by a specialized Backend/Target for
     dynamic circuit backends.
     """
 
     MEASURE_PATCH_CYCLES = 160
+    MEASURE_PATCH_ODD_OFFSET = 64
 
     def __init__(
         self,
         instruction_durations: Optional[InstructionDurationsType] = None,
         dt: float = None,
         enable_patching: bool = True,
     ):
@@ -207,15 +209,18 @@
     def _patch_measurement(self, key: InstrKey) -> None:
         """Patch measurement duration by extending duration by 160dt as temporarily
         required by the dynamic circuit backend.
         """
         prev_duration, unit = self._get_duration_dt(key)
         if unit != "dt":
             raise TranspilerError('Can currently only patch durations of "dt".')
-        self._patch_key(key, prev_duration + self.MEASURE_PATCH_CYCLES, unit)
+        odd_cycle_correction = self._get_odd_cycle_correction()
+        self._patch_key(
+            key, prev_duration + self.MEASURE_PATCH_CYCLES + odd_cycle_correction, unit
+        )
         # Enforce patching of reset on measurement update
         self._patch_reset(("reset", key[1], key[2]))
 
     def _patch_reset(self, key: InstrKey) -> None:
         """Patch reset duration by extending duration by measurement patch as temporarily
         required by the dynamic circuit backend.
         """
@@ -227,15 +232,20 @@
             measure_duration, unit = self._get_duration_dt(measure_key)
             self._patch_key(key, measure_duration, unit)
         except KeyError:
             # Fall back to reset key if measure not available
             prev_duration, unit = self._get_duration_dt(key)
             if unit != "dt":
                 raise TranspilerError('Can currently only patch durations of "dt".')
-            self._patch_key(key, prev_duration + self.MEASURE_PATCH_CYCLES, unit)
+            odd_cycle_correction = self._get_odd_cycle_correction()
+            self._patch_key(
+                key,
+                prev_duration + self.MEASURE_PATCH_CYCLES + odd_cycle_correction,
+                unit,
+            )
 
     def _get_duration_dt(self, key: InstrKey) -> Tuple[int, str]:
         """Handling for the complicated structure of this class.
 
         TODO: This class implementation should be simplified in Qiskit. Too many edge cases.
         """
         if key[1] is None and key[2] is None:
@@ -252,7 +262,28 @@
         """
         if key[1] is None and key[2] is None:
             self.duration_by_name[key[0]] = (duration, unit)
         elif key[2] is None:
             self.duration_by_name_qubits[(key[0], key[1])] = (duration, unit)
 
         self.duration_by_name_qubits_params[key] = (duration, unit)
+
+    def _get_odd_cycle_correction(self) -> int:
+        """Determine the amount of the odd cycle correction to apply
+        For devices with short gates with odd lenghts we add an extra 16dt to the measurement
+
+        TODO: Eliminate the need for this correction
+        """
+        key_pulse = "sx"
+        key_qubit = 0
+        try:
+            key_duration = self.get(key_pulse, key_qubit, "dt")
+        except TranspilerError:
+            warnings.warn(
+                f"No {key_pulse} gate found for {key_qubit} for detection of "
+                "short odd gate lengths, default measurement timing will be used."
+            )
+            key_duration = 160  # keyPulse gate not found
+
+        if key_duration < 160 and key_duration % 32:
+            return self.MEASURE_PATCH_ODD_OFFSET
+        return 0
```

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/plugin.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/transpiler/plugin.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/backend_decoder.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/backend_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/converters.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/converters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/hgp.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/hgp.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/json.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/json.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/json_encoder.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/options.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/options.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/qobj_utils.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/qobj_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/utils.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/version.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/colormaps.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/colormaps.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/device_layouts.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/device_layouts.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/exceptions.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/__init__.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/error_map.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/interactive/error_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/gate_map.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/interactive/gate_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/PKG-INFO` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-provider
-Version: 0.5.2
+Version: 0.5.3
 Summary: Qiskit IBM Quantum Provider for accessing the quantum devices and simulators at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-provider
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-provider/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
@@ -14,20 +14,19 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: visualization
 License-File: LICENSE.txt
 
 # Qiskit IBM Quantum Provider
 
 [![License](https://img.shields.io/github/license/Qiskit/qiskit-ibm-provider.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)
```

### Comparing `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/SOURCES.txt` & `qiskit-ibm-provider-0.5.3/qiskit_ibm_provider.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py
 qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py
 qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py
 qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py
 qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py
 qiskit_ibm_provider/transpiler/passes/scheduling/utils.py
 qiskit_ibm_provider/utils/__init__.py
-qiskit_ibm_provider/utils/backend_converter.py
 qiskit_ibm_provider/utils/backend_decoder.py
 qiskit_ibm_provider/utils/converters.py
 qiskit_ibm_provider/utils/hgp.py
 qiskit_ibm_provider/utils/json.py
 qiskit_ibm_provider/utils/json_decoder.py
 qiskit_ibm_provider/utils/json_encoder.py
 qiskit_ibm_provider/utils/options.py
```

### Comparing `qiskit-ibm-provider-0.5.2/setup.cfg` & `qiskit-ibm-provider-0.5.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [coverage:run]
 source = qiskit_ibm_provider
 omit = qiskit_ibm_provider/jupyter/*,qiskit_ibm_provider/visualization/*
 
 [mypy]
 exclude = test/integration/test_jupyter.py
-python_version = 3.7
+python_version = 3.8
 namespace_packages = True
 ignore_missing_imports = True
 warn_redundant_casts = True
 warn_unreachable = True
 strict_equality = True
 disallow_untyped_calls = True
 disallow_untyped_defs = True
```

### Comparing `qiskit-ibm-provider-0.5.2/setup.py` & `qiskit-ibm-provider-0.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Setup qiskit_ibm_provider"""
 
 import os
 
 import setuptools
 
 REQUIREMENTS = [
-    "qiskit-terra>=0.23.1",
+    "qiskit-terra>=0.24.0",
     "requests>=2.19",
     "requests-ntlm>=1.1.0",
     "numpy>=1.13",
     "urllib3>=1.21.1",
     "python-dateutil>=2.8.0",
     "websocket-client>=1.5.1",
     "websockets>=10.0",
@@ -59,25 +59,24 @@
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering",
     ],
     keywords="qiskit sdk quantum api ibmq",
     packages=setuptools.find_packages(exclude=["test*"]),
     install_requires=REQUIREMENTS,
     include_package_data=True,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     zip_safe=False,
     extras_require={
         "visualization": [
             "matplotlib>=2.1",
             "ipywidgets<8.0.0",
             "seaborn>=0.9.0",
             "plotly>=4.4",
```

### Comparing `qiskit-ibm-provider-0.5.2/test/__init__.py` & `qiskit-ibm-provider-0.5.3/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/account.py` & `qiskit-ibm-provider-0.5.3/test/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/contextmanagers.py` & `qiskit-ibm-provider-0.5.3/test/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/decorators.py` & `qiskit-ibm-provider-0.5.3/test/decorators.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/e2e/test_real_devices.py` & `qiskit-ibm-provider-0.5.3/test/e2e/test_real_devices.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/e2e/test_tutorials.py` & `qiskit-ibm-provider-0.5.3/test/e2e/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/fake_account_client.py` & `qiskit-ibm-provider-0.5.3/test/fake_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/http_server.py` & `qiskit-ibm-provider-0.5.3/test/http_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/ibm_test_case.py` & `qiskit-ibm-provider-0.5.3/test/ibm_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/integration/test_account_client.py` & `qiskit-ibm-provider-0.5.3/test/integration/test_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/integration/test_backend.py` & `qiskit-ibm-provider-0.5.3/test/integration/test_backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,19 @@
     ) -> None:
         """Initial class level setup."""
         # pylint: disable=arguments-differ
         super().setUpClass()
         cls.backend = backend
         cls.dependencies = dependencies
 
+    def test_backend_pending_jobs(self):
+        """Test pending jobs are returned."""
+        backends = self.dependencies.provider.backends()
+        self.assertTrue(any(backend.status().pending_jobs > 0 for backend in backends))
+
     def test_backend_status(self):
         """Check the status of a backend."""
         self.dependencies.provider.backends()
         self.assertTrue(self.backend.status().operational)
 
     def test_backend_properties(self):
         """Check the properties of calibration of a real chip."""
@@ -73,14 +78,15 @@
         provider = self.backend.provider
         for backend in provider.backends():
             with self.subTest(backend_name=backend.name):
                 defaults = backend.defaults()
                 if backend.configuration().open_pulse:
                     self.assertIsNotNone(defaults)
 
+    @skip("See Terra issue #9488")
     def test_backend_options(self):
         """Test backend options."""
         provider: IBMProvider = self.backend.provider
         backends = provider.backends(
             open_pulse=True,
             operational=True,
             instance=self.dependencies.instance,
@@ -150,18 +156,18 @@
         )
 
         with patch.object(self.backend, "configuration", return_value=config):
             with self.assertWarnsRegex(DeprecationWarning, r"'id' instruction"):
                 mutated_circuit = self.backend._deprecate_id_instruction(
                     circuit_with_id
                 )
-
-            self.assertEqual(mutated_circuit[0].count_ops(), {"delay": 3})
+            self.assertEqual(mutated_circuit.count_ops(), {"delay": 3})
             self.assertEqual(circuit_with_id.count_ops(), {"id": 3})
 
+    @skip("This is a Terra issue and test. Not related to Provider.")
     def test_transpile_converts_id(self):
         """Test that when targeting an IBM backend id is translated to delay."""
         circ = QuantumCircuit(2)
         circ.id(0)
         circ.id(1)
         tqc = transpile(circ, self.backend)
         op_counts = tqc.count_ops()
```

### Comparing `qiskit-ibm-provider-0.5.2/test/integration/test_basic_server_paths.py` & `qiskit-ibm-provider-0.5.3/test/integration/test_basic_server_paths.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/integration/test_composite_job.py` & `qiskit-ibm-provider-0.5.3/test/integration/test_composite_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,33 +84,36 @@
         self.fake_backend._api_client.tear_down()
 
     def _set_fake_client(self, fake_client):
         self.fake_backend._api_client = fake_client
         self.fake_provider._api_client = fake_client
         self.fake_provider.backend._default_hgp._api_client = fake_client
 
+    @skip("Until CompositeJob is fixed")
     def test_split_circuits(self):
         """Test having circuits split into multiple jobs."""
         max_circs = self.fake_backend.configuration().max_experiments
 
         circs = []
         for _ in range(max_circs + 2):
             circs.append(self._qc)
         job_set = self.fake_backend.run(circs)
         result = job_set.result()
 
         self.assertEqual(len(job_set.sub_jobs()), 2)
         self.assertEqual(len(result.results), max_circs + 2)
         self.assertTrue(job_set.job_id().startswith(IBM_COMPOSITE_JOB_ID_PREFIX))
 
+    @skip("Until CompositeJob is fixed")
     def test_custom_split_circuits(self):
         """Test having circuits split with custom slices."""
         job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
         self.assertEqual(len(job_set.sub_jobs()), 2)
 
+    @skip("Until CompositeJob is fixed")
     def test_job_report(self):
         """Test job report."""
         job_classes = [
             BaseFakeJob,
             FailedFakeJob,
             CancelableFakeJob,
             CancelableFakeJob,
@@ -151,14 +154,15 @@
                         JobStatus.VALIDATING,
                     ]:
                         self.assertIn(f"Status: {stat}", report)
                 else:
                     for sub_job in job_set.sub_jobs():
                         self.assertNotIn(sub_job.job_id(), report)
 
+    @skip("Until CompositeJob is fixed")
     def test_job_pending_status(self):
         """Test pending and running status."""
         sub_tests = [
             (ApiJobStatus.VALIDATING, JobStatus.VALIDATING, "Pending"),
             (ApiJobStatus.RUNNING, JobStatus.RUNNING, "Running"),
             (ApiJobStatus.QUEUED, JobStatus.QUEUED, "Pending"),
         ]
@@ -185,103 +189,113 @@
                 self.assertIsNotNone(
                     re.search(
                         rf"Job ID: {stat_job.job_id()}\s*Status: {job_status}", report
                     ),
                     report,
                 )
 
+    @skip("Until CompositeJob is fixed")
     def test_status_done(self):
         """Test job status of completed."""
         job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
         job_set.wait_for_final_state()
         self.assertEqual(job_set.status(), JobStatus.DONE)
         for sub_job in job_set.sub_jobs():
             self.assertEqual(sub_job.status(), JobStatus.DONE)
         self.assertIn("Successful jobs: 2", job_set.report())
 
+    @skip("Until CompositeJob is fixed")
     def test_job_circuits(self):
         """Test job circuits."""
         circs = []
         for _ in range(3):
             circs.append(random_circuit(num_qubits=2, depth=3, measure=True))
         circs_copied = circs.copy()
         job_set = self.fake_backend.run(circs, max_circuits_per_job=1)
         job_circuits = job_set.circuits()
         self.assertEqual(job_circuits, circs_copied)
         for i, sub_job in enumerate(job_set.sub_jobs()):
             self.assertEqual(sub_job.circuits()[0], circs_copied[i])
 
+    @skip("Until CompositeJob is fixed")
     def test_job_backend_options(self):
         """Test getting backend options."""
         custom_options = {"shots": 100, "memory": True}
         job_set = self.fake_backend.run(
             [self._qc] * 2, max_circuits_per_job=1, **custom_options
         )
         self.assertLessEqual(custom_options.items(), job_set.backend_options().items())
         job_set.block_for_submit()
         rjob_set = self.fake_provider.backend.job(job_set.job_id())
         self.assertLessEqual(custom_options.items(), rjob_set.backend_options().items())
 
+    @skip("Until CompositeJob is fixed")
     def test_job_header(self):
         """Test getting job header."""
         custom_header = {"test": "test_job_header"}
         job_set = self.fake_backend.run(
             [self._qc] * 2, max_circuits_per_job=1, header=custom_header
         )
         self.assertLessEqual(custom_header.items(), job_set.header().items())
         job_set.block_for_submit()
         rjob_set = self.fake_provider.backend.job(job_set.job_id())
         self.assertLessEqual(custom_header.items(), rjob_set.header().items())
 
+    @skip("Until CompositeJob is fixed")
     def test_job_backend(self):
         """Test getting job backend."""
         job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
         self.assertEqual(job_set.backend().name, self.fake_backend.name)
         job_set.block_for_submit()
         rjob_set = self.fake_provider.backend.job(job_set.job_id())
         self.assertEqual(rjob_set.backend().name, self.fake_backend.name)
 
+    @skip("Until CompositeJob is fixed")
     def test_job_name(self):
         """Test job name."""
         custom_name = "batman"
         job_set = self.fake_backend.run(
             [self._qc] * 2, max_circuits_per_job=1, job_name=custom_name
         )
         self.assertEqual(job_set.name(), custom_name)
         job_set.block_for_submit()
         rjob_set = self.fake_provider.backend.job(job_set.job_id())
         self.assertEqual(rjob_set.name(), custom_name)
 
+    @skip("Until CompositeJob is fixed")
     def test_job_name_update(self):
         """Test changing the name associated with a job."""
         new_name = "robin"
         job_set = self.fake_backend.run(
             [self._qc] * 2, max_circuits_per_job=1, job_name="batman"
         )
         job_set.update_name(new_name)
         self.assertEqual(job_set.name(), new_name)
         job_set.block_for_submit()
         rjob_set = self.fake_provider.backend.job(job_set.job_id())
         self.assertEqual(rjob_set.name(), new_name)
 
+    @skip("Until CompositeJob is fixed")
     def test_job_properties(self):
         """Test job properties."""
         job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
         self.assertIsInstance(job_set.properties(), BackendProperties)
 
+    @skip("Until CompositeJob is fixed")
     def test_multiple_job_properties(self):
         """Test multiple job properties."""
         self._set_fake_client(BaseFakeAccountClient(props_count=2))
 
         job_set = self.fake_backend.run([self._qc] * 3, max_circuits_per_job=1)
         props = job_set.properties()
         self.assertIsInstance(props, list)
         self.assertEqual(len(props), 2)
         self.assertTrue(all(isinstance(prop, BackendProperties) for prop in props))
 
+    @skip("Until CompositeJob is fixed")
     def test_error_message_one(self):
         """Test error message when one job failed."""
         failure_types = ["validation", "partial", "result"]
         for fail_type in failure_types:
             with self.subTest(fail_type=fail_type):
                 self._set_fake_client(
                     BaseFakeAccountClient(
@@ -306,14 +320,15 @@
                     self.assertIn("Experiment 1:", error_msg)
                 else:
                     self.assertIsNotNone(
                         re.search(r"Error code: \d{4}", error_msg),
                         f"Error msg: {error_msg}",
                     )
 
+    @skip("Until CompositeJob is fixed")
     def test_error_message_all(self):
         """Test error message report when all jobs failed."""
         self._set_fake_client(BaseFakeAccountClient(job_class=FailedFakeJob))
 
         job_set = self.fake_backend.run([self._qc] * 4, max_circuits_per_job=2)
         error_msg = job_set.error_message()
         self.assertIsNotNone(error_msg)
@@ -323,14 +338,15 @@
                     f"Circuits {idx*2}-{idx*2+1}: Job {job.job_id()} failed: "
                     + r".+ Error code: \d{4}",
                     error_msg,
                 ),
                 f"Error msg: {error_msg}",
             )
 
+    @skip("Until CompositeJob is fixed")
     def test_async_submit_exception(self):
         """Test asynchronous job submit failed."""
         self.fake_backend._api_client = JobSubmitFailClient(failed_indexes=0)
 
         job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
         job_set.wait_for_final_state()
         self.assertEqual(job_set.status(), JobStatus.ERROR)
@@ -403,14 +419,15 @@
                 [self._qc] * (job_limit + 2), max_circuits_per_job=1
             )
             self.assertEqual(job_set.status(), JobStatus.INITIALIZING)
             job_set.wait_for_final_state(timeout=60)
         finally:
             job_set.cancel()
 
+    @skip("Until CompositeJob is fixed")
     def test_job_tags_replace(self):
         """Test updating job tags by replacing existing tags."""
         initial_job_tags = [uuid.uuid4().hex]
         job_set = self.fake_backend.run(
             [self._qc] * 2, max_circuits_per_job=1, job_tags=initial_job_tags
         )
         job_set.block_for_submit()
@@ -426,21 +443,23 @@
             }
             self.assertEqual(
                 set(job.tags()) - job_set_tags, set(replacement_tags), job.tags()
             )
             self.assertIn(job_set.job_id(), job_set_tags, job.tags())
             self.assertEqual(len(job_set_tags), 2, job.tags())
 
+    @skip("Until CompositeJob is fixed")
     def test_sub_job_tags_replace(self):
         """Test updating subjob tags."""
         job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
         job = job_set.sub_jobs()[0]
         job.update_tags(new_tags=[])
         self.assertIn(job_set.job_id(), job.tags())
 
+    @skip("Until CompositeJob is fixed")
     def test_skipped_result(self):
         """Test one of the jobs has no result."""
         sub_tests = [CancelableFakeJob, FailedFakeJob]
         for job_class in sub_tests:
             with self.subTest(job_class=job_class):
                 self.fake_backend._api_client = BaseFakeAccountClient(
                     job_class=[BaseFakeJob, job_class]
@@ -455,14 +474,15 @@
                 self.assertFalse(result.success)
                 self.assertTrue(result.results[0].success)
                 self.assertFalse(result.results[1].success)
                 self.assertTrue(result.get_counts(0))
                 with self.assertRaises(QiskitError):
                     result.get_counts(1)
 
+    @skip("Until CompositeJob is fixed")
     def test_partial_result(self):
         """Test one of the circuits has no result."""
         self.fake_backend._api_client = BaseFakeAccountClient(
             job_class=[BaseFakeJob, FailedFakeJob],
             job_kwargs={"failure_type": "partial"},
         )
         job_set = self.fake_backend.run([self._qc] * 4, max_circuits_per_job=2)
@@ -471,14 +491,15 @@
         self.assertEqual(len(result.results), 4)
         self.assertFalse(result.success)
         self.assertTrue(all(res.success for res in result.results[:3]))
         self.assertFalse(result.results[3].success)
         with self.assertRaises(QiskitError):
             result.get_counts(3)
 
+    @skip("Until CompositeJob is fixed")
     def test_job_result(self):
         """Test job result."""
         max_per_job = 3
         job_set = self.fake_backend.run(
             [self._qc] * max_per_job * 2, max_circuits_per_job=max_per_job
         )
         result = job_set.result()
@@ -488,50 +509,54 @@
                 result.get_counts(i),
                 job_set.sub_jobs()[int(i / max_per_job)]
                 .result()
                 .get_counts(i % max_per_job),
             )
             self.assertTrue(result.results[i].success)
 
+    @skip("Until CompositeJob is fixed")
     def test_cancel(self):
         """Test job cancellation."""
         self.fake_backend._api_client = BaseFakeAccountClient(
             job_class=[BaseFakeJob, CancelableFakeJob]
         )
 
         job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
         job_set.block_for_submit()
         job_set.cancel()
         self.assertEqual(job_set.status(), JobStatus.CANCELLED)
         with self.assertRaises(IBMJobInvalidStateError):
             job_set.result(partial=False)
 
+    @skip("Until CompositeJob is fixed")
     def test_creation_date(self):
         """Test retrieving creation date."""
         job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
         job_set.block_for_submit()
         creation_date = job_set.creation_date()
         self.assertTrue(creation_date)
         self.assertIsNotNone(creation_date.tzinfo)
         self.assertEqual(creation_date, job_set.sub_jobs()[0].creation_date())
 
+    @skip("Until CompositeJob is fixed")
     def test_time_per_step_done(self):
         """Test retrieving time per step when job is done."""
         job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
         job_set.wait_for_final_state()
         time_per_step = job_set.time_per_step()
         self.assertTrue(time_per_step)
         self.assertIn("COMPLETED", time_per_step)
         self.assertEqual(time_per_step["CREATING"], job_set.creation_date())
         status_samples = ["CREATING", "QUEUED", "RUNNING", "COMPLETED"]
         for i in range(0, len(status_samples) - 1):
             self.assertLessEqual(
                 time_per_step[status_samples[i]], time_per_step[status_samples[i + 1]]
             )
 
+    @skip("Until CompositeJob is fixed")
     def test_time_per_step_running(self):
         """Test retrieving time per step when job is running."""
         self._set_fake_client(
             BaseFakeAccountClient(
                 job_class=[BaseFakeJob, FixedStatusFakeJob],
                 job_kwargs={"fixed_status": ApiJobStatus.RUNNING},
             )
@@ -547,14 +572,15 @@
         self.assertEqual(time_per_step["CREATING"], job_set.creation_date())
         status_samples = ["CREATING", "QUEUED", "RUNNING"]
         for i in range(0, len(status_samples) - 1):
             self.assertLessEqual(
                 time_per_step[status_samples[i]], time_per_step[status_samples[i + 1]]
             )
 
+    @skip("Until CompositeJob is fixed")
     def test_time_per_step_error(self):
         """Test retrieving time per step when job failed."""
         self._set_fake_client(
             BaseFakeAccountClient(job_class=[BaseFakeJob, FailedFakeJob])
         )
         job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
         job_set.wait_for_final_state()
@@ -566,14 +592,15 @@
         self.assertEqual(time_per_step["CREATING"], job_set.creation_date())
         status_samples = ["CREATING", "VALIDATING", "ERROR_VALIDATING_JOB"]
         for i in range(0, len(status_samples) - 1):
             self.assertLessEqual(
                 time_per_step[status_samples[i]], time_per_step[status_samples[i + 1]]
             )
 
+    @skip("Until CompositeJob is fixed")
     def test_queue_info(self):
         """Test retrieving queue information."""
         ts1 = datetime.now() + timedelta(minutes=5)
         ts2 = datetime.now() + timedelta(minutes=10)
         sub_tests = [  # Queue positions and expected position/completion time.
             ([2, 5], (5, ts2)),
             ([2, None], None),
@@ -600,14 +627,15 @@
                     self.assertEqual(queue_info.position, expected[0])
                     ts_local = expected[1].replace(tzinfo=timezone.utc)
                     ts_local = ts_local.astimezone(tz.tzlocal())
                     self.assertEqual(queue_info.estimated_complete_time, ts_local)
                 else:
                     self.assertIsNone(queue_info)
 
+    @skip("Until CompositeJob is fixed")
     def test_scheduling_mode(self):
         """Test job scheduling mode."""
         sub_tests = [
             ("fairshare", "fairshare"),
             ("dedicated", "dedicated"),
             ("dedicated_once", "fairshare"),
         ]
@@ -615,39 +643,43 @@
             with self.subTest(mode=mode):
                 self._set_fake_client(BaseFakeAccountClient(run_mode=mode))
                 job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
                 while job_set.status() not in [JobStatus.RUNNING, JobStatus.DONE]:
                     time.sleep(1)
                 self.assertEqual(job_set.scheduling_mode(), expected)
 
+    @skip("Until CompositeJob is fixed")
     def test_client_version(self):
         """Test job client version information."""
         job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
         job_set.block_for_submit()
         client_version = job_set.client_version
         self.assertTrue(client_version)
         self.assertEqual(client_version, job_set.sub_jobs()[0].client_version)
         rjob_set = self.fake_provider.backend.job(job_set.job_id())
         self.assertEqual(rjob_set.client_version, client_version)
 
+    @skip("Until CompositeJob is fixed")
     def test_job_error(self):
         """Test retrieving an invalid job."""
         with self.assertRaises(IBMJobNotFoundError):
             self.fake_provider.backend.job(IBM_COMPOSITE_JOB_ID_PREFIX + "1234")
 
+    @skip("Until CompositeJob is fixed")
     def test_missing_required_fields(self):
         """Test response data is missing required fields."""
         self._set_fake_client(
             BaseFakeAccountClient(job_class=[BaseFakeJob, MissingFieldFakeJob])
         )
         job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
         job_set.wait_for_final_state()
         self.assertEqual(job_set.status(), JobStatus.ERROR)
         self.assertIn("Unexpected return value received", job_set.error_message())
 
+    @skip("Until CompositeJob is fixed")
     def test_refresh_job_result(self):
         """Test re-retrieving job result via refresh."""
         job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
         result = job_set.result()
 
         self.assertTrue(result)
         cached_result = copy.deepcopy(result.to_dict())
@@ -655,14 +687,15 @@
         self.assertNotEqual(cached_result, result.to_dict())
 
         # Re-retrieve result via refresh.
         result = job_set.result(refresh=True)
         self.assertNotEqual(result.results[0].header.name, "modified_result")
         self.assertDictEqual(cached_result, result.to_dict())
 
+    @skip("Until CompositeJob is fixed")
     def test_wait_for_final_state(self):
         """Test waiting for job to reach final state."""
 
         def final_state_callback(c_job_id, c_status, c_job, **kwargs):
             """Job status query callback function."""
             self.assertEqual(c_job_id, job_set.job_id())
             self.assertNotIn(c_status, JOB_FINAL_STATES)
@@ -704,20 +737,22 @@
                 job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
                 job_set.wait_for_final_state(
                     timeout=10, wait=wait_time, callback=final_state_callback
                 )
                 self.assertEqual(job_set.status(), JobStatus.DONE)
                 self.assertTrue(callback_info["called"])
 
+    @skip("Until CompositeJob is fixed")
     def test_wait_for_final_state_timeout(self):
         """Test waiting for job to reach final state times out."""
         job_set = self.fake_backend.run([self._qc] * 2, max_circuits_per_job=1)
         with self.assertRaises(IBMJobTimeoutError):
             job_set.wait_for_final_state(timeout=0.1)
 
+    @skip("Until CompositeJob is fixed")
     def test_retry_failed_submit(self):
         """Test retrying failed job submit."""
         max_circs = self.fake_backend.configuration().max_experiments
         circs = []
         count = 3
         for _ in range(max_circs * (count - 1) + 1):
             circs.append(random_circuit(num_qubits=2, depth=3, measure=True))
@@ -743,14 +778,15 @@
                 circ_idx = 0
                 for sub_job in job_set.sub_jobs():
                     for job_circ in sub_job.circuits():
                         self.assertEqual(job_circ, circs[circ_idx])
                         circ_idx += 1
                 self.assertEqual(job_set.circuits(), circs)
 
+    @skip("Until CompositeJob is fixed")
     def test_retry_failed_jobs(self):
         """Test retrying failed jobs."""
         max_circs = 3
         num_jobs = 3
         circs = []
         for _ in range(max_circs * (num_jobs - 1) + 1):
             circs.append(random_circuit(num_qubits=2, depth=3, measure=True))
@@ -786,14 +822,15 @@
                 circ_idx = 0
                 for sub_job in job_set.sub_jobs():
                     for job_circ in sub_job.circuits():
                         self.assertEqual(job_circ, circs[circ_idx])
                         circ_idx += 1
                 self.assertEqual(job_set.circuits(), circs)
 
+    @skip("Until CompositeJob is fixed")
     def test_sub_job(self):
         """Test retrieving a single sub job."""
         max_circs = 3
         num_jobs = 3
         circs = []
         for _ in range(max_circs * (num_jobs - 1) + 1):
             circs.append(random_circuit(num_qubits=2, depth=3, measure=True))
@@ -813,14 +850,15 @@
         # pylint: disable=arguments-differ
         super().setUpClass()
         cls.dependencies = dependencies
         cls.sim_backend = cls.dependencies.provider.get_backend("ibmq_qasm_simulator")
         cls._qc = transpile(ReferenceCircuits.bell(), backend=cls.sim_backend)
         cls.last_week = datetime.now() - timedelta(days=7)
 
+    @skip("Until CompositeJob is fixed")
     def test_job(self):
         """Test retrieving a composite job."""
         tags = ["test_job_set"]
 
         circs_counts = [3, 4]
         for count in circs_counts:
             with self.subTest(count=count):
```

### Comparing `qiskit-ibm-provider-0.5.2/test/integration/test_filter_backends.py` & `qiskit-ibm-provider-0.5.3/test/integration/test_filter_backends.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/integration/test_ibm_integration.py` & `qiskit-ibm-provider-0.5.3/test/integration/test_ibm_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/integration/test_ibm_job.py` & `qiskit-ibm-provider-0.5.3/test/integration/test_ibm_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,14 @@
         self.assertTrue(job1.result())
         self.assertTrue(job2.result())
 
         job_list = self.provider.backend.jobs(
             backend_name=backend_name,
             limit=5,
             skip=0,
-            legacy=True,
         )
         job_ids = [job.job_id() for job in job_list]
         self.assertTrue(job1.job_id() in job_ids)
         self.assertTrue(job2.job_id() in job_ids)
 
     def test_retrieve_single_legacy_job(self):
         """Test retrieving a single legacy job."""
```

### Comparing `qiskit-ibm-provider-0.5.2/test/integration/test_ibm_job_attributes.py` & `qiskit-ibm-provider-0.5.3/test/integration/test_ibm_job_attributes.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/integration/test_ibm_provider.py` & `qiskit-ibm-provider-0.5.3/test/integration/test_ibm_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/integration/test_ibm_qasm_simulator.py` & `qiskit-ibm-provider-0.5.3/test/integration/test_ibm_qasm_simulator.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/integration/test_jupyter.py` & `qiskit-ibm-provider-0.5.3/test/integration/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/integration/test_proxies.py` & `qiskit-ibm-provider-0.5.3/test/integration/test_proxies.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/integration/test_serialization.py` & `qiskit-ibm-provider-0.5.3/test/integration/test_serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Test serializing and deserializing data sent to the server."""
 
 from typing import Set, Any, Dict, Optional
-from unittest import SkipTest, skipIf
+from unittest import SkipTest, skipIf, skip
 
 import dateutil.parser
 from qiskit import transpile, schedule, QuantumCircuit
 from qiskit.circuit import Parameter
 from qiskit.test.reference_circuits import ReferenceCircuits
 from qiskit.version import VERSION as terra_version
 
@@ -39,14 +39,15 @@
         super().setUpClass()
         cls.dependencies = dependencies
         cls.sim_backend = cls.dependencies.provider.get_backend(
             "ibmq_qasm_simulator",
         )
         cls.bell = transpile(ReferenceCircuits.bell(), backend=cls.sim_backend)
 
+    @skip("See Terra issue #9488")
     def test_pulse_qobj(self):
         """Test serializing pulse qobj data."""
         backends = self.dependencies.provider.backends(
             operational=True, open_pulse=True, instance=self.dependencies.instance
         )
         if not backends:
             self.skipTest("Need pulse backends.")
@@ -133,14 +134,15 @@
         good_keys = (
             "results.metadata.input_qubit_map",
             "results.metadata.active_input_qubits",
         )
 
         self._verify_data(result.to_dict(), good_keys=good_keys)
 
+    @skip("See Terra issue #9488")
     def test_pulse_job_result(self):
         """Test deserializing a pulse job result."""
         backends = self.dependencies.provider.backends(
             open_pulse=True, operational=True, instance=self.dependencies.instance
         )
         if not backends:
             raise SkipTest("Skipping pulse test since no pulse backend found.")
```

### Comparing `qiskit-ibm-provider-0.5.2/test/integration/test_websocket_integration.py` & `qiskit-ibm-provider-0.5.3/test/integration/test_websocket_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/jobtestcase.py` & `qiskit-ibm-provider-0.5.3/test/jobtestcase.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/proxy_server.py` & `qiskit-ibm-provider-0.5.3/test/proxy_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/unit/mock/fake_account_client.py` & `qiskit-ibm-provider-0.5.3/test/unit/mock/fake_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/unit/mock/fake_provider.py` & `qiskit-ibm-provider-0.5.3/test/unit/mock/fake_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/unit/test_account.py` & `qiskit-ibm-provider-0.5.3/test/unit/test_account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/unit/test_backend.py` & `qiskit-ibm-provider-0.5.3/test/unit/test_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/unit/test_ibm_job_states.py` & `qiskit-ibm-provider-0.5.3/test/unit/test_ibm_job_states.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/unit/test_ibm_logger.py` & `qiskit-ibm-provider-0.5.3/test/unit/test_ibm_logger.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/unit/test_serialization.py` & `qiskit-ibm-provider-0.5.3/test/unit/test_serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/unit/test_websocket.py` & `qiskit-ibm-provider-0.5.3/test/unit/test_websocket.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py` & `qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/control_flow_test_case.py` & `qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/scheduling/control_flow_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py` & `qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/test_scheduler.py` & `qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/scheduling/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/test_utils.py` & `qiskit-ibm-provider-0.5.3/test/unit/transpiler/passes/scheduling/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,25 +25,37 @@
     def test_patch_measure(self):
         """Test if schedules circuits with c_if after measure with a common clbit.
         See: https://github.com/Qiskit/qiskit-terra/issues/7654"""
 
         durations = DynamicCircuitInstructionDurations(
             [
                 ("x", None, 200),
+                ("sx", (0,), 200),
                 ("measure", None, 1000),
                 ("measure", (0, 1), 1200),
                 ("reset", None, 800),
             ]
         )
 
         self.assertEqual(durations.get("x", (0,)), 200)
         self.assertEqual(durations.get("measure", (0,)), 1160)
         self.assertEqual(durations.get("measure", (0, 1)), 1360)
         self.assertEqual(durations.get("reset", (0,)), 1160)
 
+        short_odd_durations = DynamicCircuitInstructionDurations(
+            [
+                ("sx", (0,), 112),
+                ("measure", None, 1000),
+                ("reset", None, 800),
+            ]
+        )
+
+        self.assertEqual(short_odd_durations.get("measure", (0,)), 1224)
+        self.assertEqual(short_odd_durations.get("reset", (0,)), 1224)
+
     def test_patch_disable(self):
         """Test if schedules circuits with c_if after measure with a common clbit.
         See: https://github.com/Qiskit/qiskit-terra/issues/7654"""
 
         durations = DynamicCircuitInstructionDurations(
             [("x", None, 200), ("measure", None, 1000), ("measure", (0, 1), 1200)],
             enable_patching=False,
```

### Comparing `qiskit-ibm-provider-0.5.2/test/unit/utils/ws_handler.py` & `qiskit-ibm-provider-0.5.3/test/unit/utils/ws_handler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/utils.py` & `qiskit-ibm-provider-0.5.3/test/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.2/test/ws_server.py` & `qiskit-ibm-provider-0.5.3/test/ws_server.py`

 * *Files identical despite different names*

