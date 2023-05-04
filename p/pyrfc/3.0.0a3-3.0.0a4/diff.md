# Comparing `tmp/pyrfc-3.0.0a3.tar.gz` & `tmp/pyrfc-3.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfc-3.0.0a3.tar", last modified: Thu May  4 13:53:34 2023, max compression
+gzip compressed data, was "pyrfc-3.0.0a4.tar", last modified: Thu May  4 16:43:24 2023, max compression
```

## Comparing `pyrfc-3.0.0a3.tar` & `pyrfc-3.0.0a4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:53:34.854441 pyrfc-3.0.0a3/
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:53:34.714288 pyrfc-3.0.0a3/LICENSES/
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10283 2023-04-25 13:34:15.000000 pyrfc-3.0.0a3/LICENSES/Apache-2.0.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)       58 2023-04-25 13:34:15.000000 pyrfc-3.0.0a3/MANIFEST.in
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23719 2023-05-04 13:53:34.847091 pyrfc-3.0.0a3/PKG-INFO
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10452 2023-05-04 13:30:21.000000 pyrfc-3.0.0a3/README.md
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)     1744 2023-05-04 13:52:27.000000 pyrfc-3.0.0a3/pyproject.toml
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)       38 2023-05-04 13:53:34.855564 pyrfc-3.0.0a3/setup.cfg
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)     5747 2023-05-04 13:52:23.000000 pyrfc-3.0.0a3/setup.py
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:53:34.686978 pyrfc-3.0.0a3/src/
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:53:34.811531 pyrfc-3.0.0a3/src/pyrfc/
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     1480 2023-05-04 10:40:57.000000 pyrfc-3.0.0a3/src/pyrfc/__init__.py
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)  2313697 2023-05-04 13:53:29.000000 pyrfc-3.0.0a3/src/pyrfc/_cyrfc.cpp
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)   129762 2023-05-03 12:19:55.000000 pyrfc-3.0.0a3/src/pyrfc/_cyrfc.pyx
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     5675 2023-05-04 07:59:09.000000 pyrfc-3.0.0a3/src/pyrfc/_exception.py
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      317 2023-05-04 09:19:28.000000 pyrfc-3.0.0a3/src/pyrfc/_utils.py
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)    23820 2023-05-03 10:59:40.000000 pyrfc-3.0.0a3/src/pyrfc/csapnwrfc.pxd
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:53:34.840577 pyrfc-3.0.0a3/src/pyrfc.egg-info/
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23719 2023-05-04 13:53:34.000000 pyrfc-3.0.0a3/src/pyrfc.egg-info/PKG-INFO
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      333 2023-05-04 13:53:34.000000 pyrfc-3.0.0a3/src/pyrfc.egg-info/SOURCES.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)        1 2023-05-04 13:53:34.000000 pyrfc-3.0.0a3/src/pyrfc.egg-info/dependency_links.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)        6 2023-05-04 13:53:34.000000 pyrfc-3.0.0a3/src/pyrfc.egg-info/top_level.txt
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 16:43:24.680269 pyrfc-3.0.0a4/
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 16:43:24.531075 pyrfc-3.0.0a4/LICENSES/
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10283 2023-04-25 13:34:15.000000 pyrfc-3.0.0a4/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)       58 2023-04-25 13:34:15.000000 pyrfc-3.0.0a4/MANIFEST.in
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23719 2023-05-04 16:43:24.676281 pyrfc-3.0.0a4/PKG-INFO
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10452 2023-05-04 13:30:21.000000 pyrfc-3.0.0a4/README.md
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)     1744 2023-05-04 16:42:06.000000 pyrfc-3.0.0a4/pyproject.toml
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)       38 2023-05-04 16:43:24.681166 pyrfc-3.0.0a4/setup.cfg
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)     5747 2023-05-04 13:52:23.000000 pyrfc-3.0.0a4/setup.py
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 16:43:24.501148 pyrfc-3.0.0a4/src/
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 16:43:24.637333 pyrfc-3.0.0a4/src/pyrfc/
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     1470 2023-05-04 16:41:48.000000 pyrfc-3.0.0a4/src/pyrfc/__init__.py
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)  2313566 2023-05-04 16:43:19.000000 pyrfc-3.0.0a4/src/pyrfc/_cyrfc.cpp
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)   129747 2023-05-04 16:41:17.000000 pyrfc-3.0.0a4/src/pyrfc/_cyrfc.pyx
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     5670 2023-05-04 16:41:25.000000 pyrfc-3.0.0a4/src/pyrfc/_exception.py
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)      317 2023-05-04 09:19:28.000000 pyrfc-3.0.0a4/src/pyrfc/_utils.py
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)    23820 2023-05-03 10:59:40.000000 pyrfc-3.0.0a4/src/pyrfc/csapnwrfc.pxd
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 16:43:24.665436 pyrfc-3.0.0a4/src/pyrfc.egg-info/
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23719 2023-05-04 16:43:24.000000 pyrfc-3.0.0a4/src/pyrfc.egg-info/PKG-INFO
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)      333 2023-05-04 16:43:24.000000 pyrfc-3.0.0a4/src/pyrfc.egg-info/SOURCES.txt
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)        1 2023-05-04 16:43:24.000000 pyrfc-3.0.0a4/src/pyrfc.egg-info/dependency_links.txt
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)        6 2023-05-04 16:43:24.000000 pyrfc-3.0.0a4/src/pyrfc.egg-info/top_level.txt
```

### Comparing `pyrfc-3.0.0a3/LICENSES/Apache-2.0.txt` & `pyrfc-3.0.0a4/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0.0a3/PKG-INFO` & `pyrfc-3.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfc
-Version: 3.0.0a3
+Version: 3.0.0a4
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
 Author-email: srdjan.boskovic@sap.com
 Maintainer-email: Srdjan Boskovic <srdjan.boskovic@sap.com>
 License: Apache License
         
         Version 2.0, January 2004
```

### Comparing `pyrfc-3.0.0a3/README.md` & `pyrfc-3.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0.0a3/pyproject.toml` & `pyrfc-3.0.0a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["Cython >= 0.29", "setuptools >= 67", "wheel >= 0.40"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrfc"
-version = "3.0.0.a3"
+version = "3.0.0.a4"
 readme = "README.md"
 license = { file = "LICENSES/Apache-2.0.txt" }
 description = "Python bindings for SAP NetWeaver RFC SDK"
 authors = [ { name = "SAP SE"}, { email = "srdjan.boskovic@sap.com" } ]
 maintainers = [ { name = "Srdjan Boskovic", email = "srdjan.boskovic@sap.com" } ]
 requires-python = ">=3.8"
 keywords = ["pyrfc", "sap", "nwrfc", "sapnwrfc", "abap"]
```

### Comparing `pyrfc-3.0.0a3/setup.py` & `pyrfc-3.0.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0.0a3/src/pyrfc/__init__.py` & `pyrfc-3.0.0a4/src/pyrfc/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 __version_info__ = tuple(__version__.split("."))
 
 if os.name == "nt":
     # add SAP NWRFC SDK to DLL pth
     with suppress(Exception):
         os.add_dll_directory(os.path.join(os.environ["SAPNWRFC_HOME"], "lib"))
 
-from pyrfc._exception import (  # noqa F401
+from ._exception import (  # noqa F401
     RFCError,
     RFCLibError,
     CommunicationError,
     LogonError,
     ABAPApplicationError,
     ABAPRuntimeError,
     ExternalAuthorizationError,
     ExternalApplicationError,
     ExternalRuntimeError,
 )
 
 try:
-    from pyrfc._cyrfc import (  # noqa F401
+    from ._cyrfc import (  # noqa F401
         get_nwrfclib_version,
         reload_ini_file,
         set_ini_file_directory,
         set_cryptolib_path,
         set_locale_radix,
         language_iso_to_sap,
         language_sap_to_iso,
```

### Comparing `pyrfc-3.0.0a3/src/pyrfc/_cyrfc.cpp` & `pyrfc-3.0.0a4/src/pyrfc/_cyrfc.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2197,14 +2197,15 @@
 static const char __pyx_k_serve[] = "serve";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_state[] = "state";
 static const char __pyx_k_sysId[] = "sysId";
 static const char __pyx_k_sysid[] = "sysid";
 static const char __pyx_k_trace[] = "trace";
 static const char __pyx_k_upper[] = "upper";
+static const char __pyx_k_utils[] = "_utils";
 static const char __pyx_k_value[] = "value";
 static const char __pyx_k_Server[] = "Server";
 static const char __pyx_k_Thread[] = "Thread";
 static const char __pyx_k_Values[] = "\n Values: ";
 static const char __pyx_k_append[] = "append";
 static const char __pyx_k_cancel[] = "cancel";
 static const char __pyx_k_client[] = "client";
@@ -2296,14 +2297,15 @@
 static const char __pyx_k_but_found[] = ", but found ";
 static const char __pyx_k_call_type[] = "call_type";
 static const char __pyx_k_committed[] = "committed";
 static const char __pyx_k_confirmed[] = "confirmed";
 static const char __pyx_k_direction[] = "direction";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_errorInfo[] = "errorInfo";
+static const char __pyx_k_exception[] = "_exception";
 static const char __pyx_k_func_name[] = "func_name";
 static const char __pyx_k_int_field[] = "int_field";
 static const char __pyx_k_iteritems[] = "iteritems";
 static const char __pyx_k_kernelRel[] = "kernelRel";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_msg_class[] = "msg_class";
 static const char __pyx_k_not_found[] = "not_found";
@@ -2391,15 +2393,14 @@
 static const char __pyx_k_UnitCallType[] = "UnitCallType";
 static const char __pyx_k_confirm_unit[] = "_confirm_unit";
 static const char __pyx_k_destroy_unit[] = "_destroy_unit";
 static const char __pyx_k_kernel_trace[] = "kernel_trace";
 static const char __pyx_k_must_be_in_2[] = "' must be in '";
 static const char __pyx_k_protocolType[] = "protocolType";
 static const char __pyx_k_pyrfc__cyrfc[] = "pyrfc._cyrfc";
-static const char __pyx_k_pyrfc__utils[] = "pyrfc._utils";
 static const char __pyx_k_sapnwrfc_ini[] = "sapnwrfc.ini";
 static const char __pyx_k_sending_date[] = "sending_date";
 static const char __pyx_k_sending_time[] = "sending_time";
 static const char __pyx_k_server_log_2[] = "server_log";
 static const char __pyx_k_staticmethod[] = "staticmethod";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_unit_history[] = "unit_history";
@@ -2458,15 +2459,14 @@
 static const char __pyx_k_ABAPRuntimeError[] = "ABAPRuntimeError";
 static const char __pyx_k_ServerConnection[] = "ServerConnection";
 static const char __pyx_k_Unknown_RFC_type[] = "Unknown RFC type ";
 static const char __pyx_k_currentBusyCount[] = "currentBusyCount";
 static const char __pyx_k_direction_string[] = "'direction' (string) '";
 static const char __pyx_k_func_desc_handle[] = "func_desc_handle";
 static const char __pyx_k_is_not_supported[] = "' is not supported";
-static const char __pyx_k_pyrfc__exception[] = "pyrfc._exception";
 static const char __pyx_k_server_functions[] = "server_functions";
 static const char __pyx_k_set_locale_radix[] = "set_locale_radix";
 static const char __pyx_k_type_description[] = "type_description";
 static const char __pyx_k_RFCTYPE_STRUCTURE[] = "RFCTYPE_STRUCTURE";
 static const char __pyx_k_RFCTYPE_UTCMINUTE[] = "RFCTYPE_UTCMINUTE";
 static const char __pyx_k_RFCTYPE_UTCSECOND[] = "RFCTYPE_UTCSECOND";
 static const char __pyx_k_Server_connection[] = "Server connection";
@@ -2837,14 +2837,15 @@
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_enum;
 static PyObject *__pyx_n_s_enum_names;
 static PyObject *__pyx_n_s_enum_values;
 static PyObject *__pyx_n_s_enumerate;
 static PyObject *__pyx_n_s_errorInfo;
 static PyObject *__pyx_n_s_exc_info;
+static PyObject *__pyx_n_s_exception;
 static PyObject *__pyx_n_s_executed;
 static PyObject *__pyx_kp_u_field;
 static PyObject *__pyx_kp_u_field_name_string;
 static PyObject *__pyx_kp_u_field_name_string_2;
 static PyObject *__pyx_n_s_field_type;
 static PyObject *__pyx_n_u_field_type;
 static PyObject *__pyx_kp_u_field_type_string;
@@ -2976,16 +2977,14 @@
 static PyObject *__pyx_n_u_port;
 static PyObject *__pyx_n_s_prepare;
 static PyObject *__pyx_n_s_print;
 static PyObject *__pyx_n_u_progName;
 static PyObject *__pyx_n_u_program;
 static PyObject *__pyx_n_u_protocolType;
 static PyObject *__pyx_n_s_pyrfc__cyrfc;
-static PyObject *__pyx_n_s_pyrfc__exception;
-static PyObject *__pyx_n_s_pyrfc__utils;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_qualname;
 static PyObject *__pyx_n_s_queue_name;
 static PyObject *__pyx_n_s_queue_names;
 static PyObject *__pyx_n_s_queued;
 static PyObject *__pyx_n_u_queued;
 static PyObject *__pyx_kp_u_raises_ABAPApplicationError;
@@ -3088,14 +3087,15 @@
 static PyObject *__pyx_n_u_unit_history;
 static PyObject *__pyx_n_s_unit_id;
 static PyObject *__pyx_n_u_unit_identifier;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_upper;
 static PyObject *__pyx_n_u_user;
 static PyObject *__pyx_n_s_utcnow;
+static PyObject *__pyx_n_s_utils;
 static PyObject *__pyx_n_s_value;
 static PyObject *__pyx_kp_u_when_filling;
 static PyObject *__pyx_kp_u_when_getting_server_context_for;
 static PyObject *__pyx_kp_u_when_wrapping;
 static PyObject *__pyx_kp_u_with;
 static PyObject *__pyx_n_s_wrap;
 static PyObject *__pyx_kp_u_wrapString_uclen_u_utf8_size_u;
@@ -42663,14 +42663,15 @@
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_enum, __pyx_k_enum, sizeof(__pyx_k_enum), 0, 0, 1, 1},
   {&__pyx_n_s_enum_names, __pyx_k_enum_names, sizeof(__pyx_k_enum_names), 0, 0, 1, 1},
   {&__pyx_n_s_enum_values, __pyx_k_enum_values, sizeof(__pyx_k_enum_values), 0, 0, 1, 1},
   {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
   {&__pyx_n_s_errorInfo, __pyx_k_errorInfo, sizeof(__pyx_k_errorInfo), 0, 0, 1, 1},
   {&__pyx_n_s_exc_info, __pyx_k_exc_info, sizeof(__pyx_k_exc_info), 0, 0, 1, 1},
+  {&__pyx_n_s_exception, __pyx_k_exception, sizeof(__pyx_k_exception), 0, 0, 1, 1},
   {&__pyx_n_s_executed, __pyx_k_executed, sizeof(__pyx_k_executed), 0, 0, 1, 1},
   {&__pyx_kp_u_field, __pyx_k_field, sizeof(__pyx_k_field), 0, 1, 0, 0},
   {&__pyx_kp_u_field_name_string, __pyx_k_field_name_string, sizeof(__pyx_k_field_name_string), 0, 1, 0, 0},
   {&__pyx_kp_u_field_name_string_2, __pyx_k_field_name_string_2, sizeof(__pyx_k_field_name_string_2), 0, 1, 0, 0},
   {&__pyx_n_s_field_type, __pyx_k_field_type, sizeof(__pyx_k_field_type), 0, 0, 1, 1},
   {&__pyx_n_u_field_type, __pyx_k_field_type, sizeof(__pyx_k_field_type), 0, 1, 0, 1},
   {&__pyx_kp_u_field_type_string, __pyx_k_field_type_string, sizeof(__pyx_k_field_type_string), 0, 1, 0, 0},
@@ -42802,16 +42803,14 @@
   {&__pyx_n_u_port, __pyx_k_port, sizeof(__pyx_k_port), 0, 1, 0, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
   {&__pyx_n_s_print, __pyx_k_print, sizeof(__pyx_k_print), 0, 0, 1, 1},
   {&__pyx_n_u_progName, __pyx_k_progName, sizeof(__pyx_k_progName), 0, 1, 0, 1},
   {&__pyx_n_u_program, __pyx_k_program, sizeof(__pyx_k_program), 0, 1, 0, 1},
   {&__pyx_n_u_protocolType, __pyx_k_protocolType, sizeof(__pyx_k_protocolType), 0, 1, 0, 1},
   {&__pyx_n_s_pyrfc__cyrfc, __pyx_k_pyrfc__cyrfc, sizeof(__pyx_k_pyrfc__cyrfc), 0, 0, 1, 1},
-  {&__pyx_n_s_pyrfc__exception, __pyx_k_pyrfc__exception, sizeof(__pyx_k_pyrfc__exception), 0, 0, 1, 1},
-  {&__pyx_n_s_pyrfc__utils, __pyx_k_pyrfc__utils, sizeof(__pyx_k_pyrfc__utils), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
   {&__pyx_n_s_queue_name, __pyx_k_queue_name, sizeof(__pyx_k_queue_name), 0, 0, 1, 1},
   {&__pyx_n_s_queue_names, __pyx_k_queue_names, sizeof(__pyx_k_queue_names), 0, 0, 1, 1},
   {&__pyx_n_s_queued, __pyx_k_queued, sizeof(__pyx_k_queued), 0, 0, 1, 1},
   {&__pyx_n_u_queued, __pyx_k_queued, sizeof(__pyx_k_queued), 0, 1, 0, 1},
   {&__pyx_kp_u_raises_ABAPApplicationError, __pyx_k_raises_ABAPApplicationError, sizeof(__pyx_k_raises_ABAPApplicationError), 0, 1, 0, 0},
@@ -42914,14 +42913,15 @@
   {&__pyx_n_u_unit_history, __pyx_k_unit_history, sizeof(__pyx_k_unit_history), 0, 1, 0, 1},
   {&__pyx_n_s_unit_id, __pyx_k_unit_id, sizeof(__pyx_k_unit_id), 0, 0, 1, 1},
   {&__pyx_n_u_unit_identifier, __pyx_k_unit_identifier, sizeof(__pyx_k_unit_identifier), 0, 1, 0, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_upper, __pyx_k_upper, sizeof(__pyx_k_upper), 0, 0, 1, 1},
   {&__pyx_n_u_user, __pyx_k_user, sizeof(__pyx_k_user), 0, 1, 0, 1},
   {&__pyx_n_s_utcnow, __pyx_k_utcnow, sizeof(__pyx_k_utcnow), 0, 0, 1, 1},
+  {&__pyx_n_s_utils, __pyx_k_utils, sizeof(__pyx_k_utils), 0, 0, 1, 1},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
   {&__pyx_kp_u_when_filling, __pyx_k_when_filling, sizeof(__pyx_k_when_filling), 0, 1, 0, 0},
   {&__pyx_kp_u_when_getting_server_context_for, __pyx_k_when_getting_server_context_for, sizeof(__pyx_k_when_getting_server_context_for), 0, 1, 0, 0},
   {&__pyx_kp_u_when_wrapping, __pyx_k_when_wrapping, sizeof(__pyx_k_when_wrapping), 0, 1, 0, 0},
   {&__pyx_kp_u_with, __pyx_k_with, sizeof(__pyx_k_with), 0, 1, 0, 0},
   {&__pyx_n_s_wrap, __pyx_k_wrap, sizeof(__pyx_k_wrap), 0, 0, 1, 1},
   {&__pyx_kp_u_wrapString_uclen_u_utf8_size_u, __pyx_k_wrapString_uclen_u_utf8_size_u, sizeof(__pyx_k_wrapString_uclen_u_utf8_size_u), 0, 1, 0, 0},
@@ -44151,15 +44151,15 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":17
  * from sys import exc_info, platform
  * import socket
  * from threading import Thread, Timer             # <<<<<<<<<<<<<<
  * 
- * from pyrfc.csapnwrfc cimport *
+ * from .csapnwrfc cimport *
  */
   __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Thread);
   __Pyx_GIVEREF(__pyx_n_s_Thread);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Thread);
   __Pyx_INCREF(__pyx_n_s_Timer);
@@ -44176,46 +44176,46 @@
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Timer, __pyx_t_2) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":20
  * 
- * from pyrfc.csapnwrfc cimport *
- * from pyrfc._exception import *             # <<<<<<<<<<<<<<
- * from pyrfc._utils import enum_names, enum_values
+ * from .csapnwrfc cimport *
+ * from ._exception import *             # <<<<<<<<<<<<<<
+ * from ._utils import enum_names, enum_values
  * 
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s__51);
   __Pyx_GIVEREF(__pyx_n_s__51);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s__51);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_pyrfc__exception, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_exception, __pyx_t_1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_import_star(__pyx_t_2) < 0) __PYX_ERR(0, 20, __pyx_L1_error);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":21
- * from pyrfc.csapnwrfc cimport *
- * from pyrfc._exception import *
- * from pyrfc._utils import enum_names, enum_values             # <<<<<<<<<<<<<<
+ * from .csapnwrfc cimport *
+ * from ._exception import *
+ * from ._utils import enum_names, enum_values             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_enum_names);
   __Pyx_GIVEREF(__pyx_n_s_enum_names);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_enum_names);
   __Pyx_INCREF(__pyx_n_s_enum_values);
   __Pyx_GIVEREF(__pyx_n_s_enum_values);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_enum_values);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_pyrfc__utils, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_utils, __pyx_t_2, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_enum_names); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_enum_names, __pyx_t_2) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_enum_values); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
```

### Comparing `pyrfc-3.0.0a3/src/pyrfc/_cyrfc.pyx` & `pyrfc-3.0.0a4/src/pyrfc/_cyrfc.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from enum import Enum, auto
 from locale import localeconv
 from os.path import isfile, join
 from sys import exc_info, platform
 import socket
 from threading import Thread, Timer
 
-from pyrfc.csapnwrfc cimport *
-from pyrfc._exception import *
-from pyrfc._utils import enum_names, enum_values
+from .csapnwrfc cimport *
+from ._exception import *
+from ._utils import enum_names, enum_values
 
 
 ################################################################################
 # Configuration options
 ################################################################################
 
 # configuration bitmasks, internal use
```

### Comparing `pyrfc-3.0.0a3/src/pyrfc/_exception.py` & `pyrfc-3.0.0a4/src/pyrfc/_exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2013 SAP SE Srdjan Boskovic <srdjan.boskovic@sap.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """:mod:`pyrfc`-specific exception classes."""
 
 from enum import Enum, auto
-from pyrfc._utils import enum_values
+from ._utils import enum_values
 
 
 class RFCError(Exception):
     """Exception base class.
 
     Indicates that there was an error in the Python connector.
     """
```

### Comparing `pyrfc-3.0.0a3/src/pyrfc/csapnwrfc.pxd` & `pyrfc-3.0.0a4/src/pyrfc/csapnwrfc.pxd`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0.0a3/src/pyrfc.egg-info/PKG-INFO` & `pyrfc-3.0.0a4/src/pyrfc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfc
-Version: 3.0.0a3
+Version: 3.0.0a4
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
 Author-email: srdjan.boskovic@sap.com
 Maintainer-email: Srdjan Boskovic <srdjan.boskovic@sap.com>
 License: Apache License
         
         Version 2.0, January 2004
```

