# Comparing `tmp/pibble-0.5.0.tar.gz` & `tmp/pibble-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pibble-0.5.0.tar", last modified: Wed May  3 22:26:54 2023, max compression
+gzip compressed data, was "pibble-0.5.1.tar", last modified: Wed May  3 22:34:46 2023, max compression
```

## Comparing `pibble-0.5.0.tar` & `pibble-0.5.1.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6485 2023-05-03 22:26:54.502891 pibble-0.5.0/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5960 2023-05-03 22:26:54.000000 pibble-0.5.0/README.md
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     8891 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/__main__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3374 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/client/apachethrift/
--rw-------   0 benjamin  (1000) benjamin  (1000)     6195 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/apachethrift/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1340 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/client/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    14230 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/file/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9726 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/file/hdfs.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    12782 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/file/local.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    19652 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4132 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/client/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4728 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16837 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2312 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/jsonapi.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/client/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11386 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4766 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10690 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6689 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/soap.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7333 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/configuration.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6101 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/exceptions.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/helpers/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/helpers/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15706 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/helpers/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    20612 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/helpers/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    24691 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/helpers/googlerpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13415 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/helpers/store.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13868 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/helpers/wrappers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/meta/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/meta/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9492 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/meta/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2952 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/meta/helpers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/middleware/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/middleware/apachethrift/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/apachethrift/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/apachethrift/screening.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/middleware/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3730 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/database/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/middleware/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      454 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/file/temp.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/middleware/googlerpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/googlerpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/googlerpc/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/googlerpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/googlerpc/metadata.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3703 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/middleware/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/middleware/webservice/authentication/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/authentication/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/authentication/basic.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/authentication/bearer.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13472 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/authentication/digest.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/authentication/header.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    17704 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/authentication/oauth.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3256 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/limit.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/protocol/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/protocol/__init__.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19486 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/protocol/apachethrift.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2451 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2080 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/server/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15640 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5453 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/server/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2393 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7311 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/awslambda.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    38899 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/server/webservice/drivers/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/drivers/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1489 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/drivers/driver_cherrypy.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2194 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/drivers/driver_gunicorn.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1078 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/drivers/driver_werkzeug.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16024 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/handler.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3164 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/jsonapi.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      969 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/server/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4247 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6457 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    12004 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    17061 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/soap.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/server/webservice/template/
--rw-------   0 benjamin  (1000) benjamin  (1000)     9717 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/template/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9201 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/template/extensions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9770 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/template/loader.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7797 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/database/dedupe.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10529 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/database/engine.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/database/exceptions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    26274 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/database/orm.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2694 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/database/util.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/ext/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/ext/cms/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/cms/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/database/interface.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/database/menu.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/database/view.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1366 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/middleware.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/cms/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6759 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/server/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3012 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/server/extension.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/dam/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/dam/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/dam/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/dam/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/dam/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/dam/database/files.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/dam/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/dam/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/dam/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/rest/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/rest/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/rest/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/rest/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/rest/database/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/rest/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/rest/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15690 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/rest/server/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7342 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/rest/server/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/session/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/session/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/session/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/session/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/session/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/session/database/session.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/session/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/session/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5207 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/session/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/user/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/user/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/client/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      985 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/user/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/database/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/database/notification.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5865 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/database/permission.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      611 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/database/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/user/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    25034 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/hooks/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/hooks/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6037 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/hooks/aws.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/media/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/media/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10388 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/media/thumbnail.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/resources/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/resources/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10655 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/resources/retriever.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/scripts/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/scripts/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1909 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/scripts/importcheck.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1726 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/scripts/templatefiles.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/setup.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/util/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     8357 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/encryption.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16171 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/files.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    32821 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/helpers.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/imaging.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6330 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/log.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1701 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/numeric.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    27116 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/strings.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/web/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/web/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3227 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/web/scraper.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble.egg-info/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6485 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble.egg-info/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5627 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble.egg-info/SOURCES.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble.egg-info/dependency_links.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble.egg-info/entry_points.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1936 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble.egg-info/requires.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble.egg-info/top_level.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-05-03 22:26:54.502891 pibble-0.5.0/setup.cfg
--rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-03 22:26:54.000000 pibble-0.5.0/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6485 2023-05-03 22:34:46.371166 pibble-0.5.1/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5960 2023-05-03 22:34:46.000000 pibble-0.5.1/README.md
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.359166 pibble-0.5.1/pibble/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     8955 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/__main__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.363166 pibble-0.5.1/pibble/api/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3374 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.363166 pibble-0.5.1/pibble/api/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.363166 pibble-0.5.1/pibble/api/client/apachethrift/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6195 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/apachethrift/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1340 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.363166 pibble-0.5.1/pibble/api/client/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    14230 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/file/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9726 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/file/hdfs.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    12782 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/file/local.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    19652 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4132 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.363166 pibble-0.5.1/pibble/api/client/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4728 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16837 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2312 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/webservice/jsonapi.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.363166 pibble-0.5.1/pibble/api/client/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11386 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4766 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10690 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6689 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/webservice/soap.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7333 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/webservice/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/client/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/configuration.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6101 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/exceptions.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.363166 pibble-0.5.1/pibble/api/helpers/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/helpers/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15706 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/helpers/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    20612 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/helpers/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    24691 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/helpers/googlerpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13415 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/helpers/store.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13868 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/helpers/wrappers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.363166 pibble-0.5.1/pibble/api/meta/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/meta/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9492 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/meta/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2952 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/meta/helpers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.363166 pibble-0.5.1/pibble/api/middleware/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.363166 pibble-0.5.1/pibble/api/middleware/apachethrift/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/apachethrift/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/apachethrift/screening.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.363166 pibble-0.5.1/pibble/api/middleware/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3730 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/database/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.363166 pibble-0.5.1/pibble/api/middleware/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      454 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/file/temp.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.363166 pibble-0.5.1/pibble/api/middleware/googlerpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/googlerpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/googlerpc/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/googlerpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/googlerpc/metadata.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3703 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.367166 pibble-0.5.1/pibble/api/middleware/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/webservice/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.367166 pibble-0.5.1/pibble/api/middleware/webservice/authentication/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/webservice/authentication/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/webservice/authentication/basic.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/webservice/authentication/bearer.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13472 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/webservice/authentication/digest.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/webservice/authentication/header.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    17704 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/webservice/authentication/oauth.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3256 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/webservice/limit.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/middleware/webservice/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.367166 pibble-0.5.1/pibble/api/protocol/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/protocol/__init__.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19486 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/protocol/apachethrift.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.367166 pibble-0.5.1/pibble/api/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2451 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2080 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.367166 pibble-0.5.1/pibble/api/server/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15640 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5453 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.367166 pibble-0.5.1/pibble/api/server/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2393 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7311 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/awslambda.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    38899 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.367166 pibble-0.5.1/pibble/api/server/webservice/drivers/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/drivers/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1489 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/drivers/driver_cherrypy.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2194 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/drivers/driver_gunicorn.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1078 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/drivers/driver_werkzeug.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16024 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/handler.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3164 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/jsonapi.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      969 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.367166 pibble-0.5.1/pibble/api/server/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4247 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6457 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    12004 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    17061 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/soap.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.367166 pibble-0.5.1/pibble/api/server/webservice/template/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9717 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/template/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9201 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/template/extensions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9770 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/api/server/webservice/template/loader.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.367166 pibble-0.5.1/pibble/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7797 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/database/dedupe.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10529 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/database/engine.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/database/exceptions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    26274 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/database/orm.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2694 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/database/util.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.367166 pibble-0.5.1/pibble/ext/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/ext/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.367166 pibble-0.5.1/pibble/ext/cms/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/ext/cms/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.367166 pibble-0.5.1/pibble/ext/cms/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/cms/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/cms/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/cms/database/interface.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/cms/database/menu.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/cms/database/view.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1366 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/cms/middleware.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.367166 pibble-0.5.1/pibble/ext/cms/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/cms/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6759 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/cms/server/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3012 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/cms/server/extension.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.367166 pibble-0.5.1/pibble/ext/dam/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/dam/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/ext/dam/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/dam/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/dam/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/dam/database/files.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/ext/dam/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/dam/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/dam/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/ext/rest/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/rest/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/ext/rest/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/rest/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/rest/database/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/ext/rest/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/rest/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15690 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/rest/server/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7342 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/rest/server/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/ext/session/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/session/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/ext/session/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/session/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/session/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/session/database/session.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/ext/session/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/session/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5207 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/session/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/ext/user/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/user/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/ext/user/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/user/client/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      985 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/user/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/ext/user/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/user/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/user/database/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/user/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/user/database/notification.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5865 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/user/database/permission.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      611 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/user/database/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/ext/user/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/user/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    25034 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/ext/user/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/hooks/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/hooks/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6037 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/hooks/aws.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/media/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/media/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10388 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/media/thumbnail.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/resources/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/resources/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10655 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/resources/retriever.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/scripts/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/scripts/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1909 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/scripts/importcheck.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1726 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/scripts/templatefiles.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/util/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/util/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     8357 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/util/encryption.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16171 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/util/files.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    32821 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/util/helpers.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/util/imaging.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6330 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/util/log.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1701 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/util/numeric.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    27116 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble/util/strings.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.371166 pibble-0.5.1/pibble/web/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/web/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3227 2023-05-03 22:34:45.000000 pibble-0.5.1/pibble/web/scraper.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:34:46.359166 pibble-0.5.1/pibble.egg-info/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6485 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble.egg-info/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5627 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble.egg-info/SOURCES.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble.egg-info/dependency_links.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble.egg-info/entry_points.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1936 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble.egg-info/requires.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-05-03 22:34:46.000000 pibble-0.5.1/pibble.egg-info/top_level.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-05-03 22:34:46.371166 pibble-0.5.1/setup.cfg
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-03 22:34:46.000000 pibble-0.5.1/setup.py
```

### Comparing `pibble-0.5.0/PKG-INFO` & `pibble-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.5.0
+Version: 0.5.1
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
```

### Comparing `pibble-0.5.0/README.md` & `pibble-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/__main__.py` & `pibble-0.5.1/pibble/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 import logging
 import code
 import requests
 import multiprocessing
 import time
 import traceback
 
-from typing import Optional
+from typing import Optional, List
 
-from pibble.api.meta.helpers import MetaFactory
+from pibble.api.meta.helpers import MetaFactory, MetaService
 from pibble.util.log import (
     logger,
     LevelUnifiedLoggingContext,
     DebugUnifiedLoggingContext,
     ConfigurationLoggingContext,
 )
 from pibble.util.files import load_json
 
 
 class MetaServerProcess(multiprocessing.Process):
-    def __init__(self, service):
+    def __init__(self, service: MetaService) -> None:
         super(MetaServerProcess, self).__init__()
         self.service = service
         self.name = self.service.name
 
-    def run(self):
+    def run(self) -> None:
         self.service.serve()
 
 
 @click.group(name="pibble")
 def main() -> None:
     """
     Pibble Framework command-line tools.
@@ -80,15 +80,15 @@
 
 
 @main.command(short_help="Start multiple servers based on configurations.")
 @click.argument("configuration", nargs=-1)
 @click.option(
     "--debug", is_flag=True, help="Turn on debug unified logging.", default=False
 )
-def servers(configuration: List[str], debug: bool = False):
+def servers(configuration: List[str], debug: bool = False) -> None:
     """
     Starts servers, synchronously, using a configuration file.
 
     All servers will be ran at the same time, and stopped at the same time.
     If any server errors, all will be stopped.
 
     The configuration file format is specified by its extension (.yml/.yaml being YAML, .json being JSON). No other formats are accepted.
@@ -168,15 +168,15 @@
     configuration: str,
     command: Optional[str] = None,
     arg: Optional[List[str]] = None,
     json: Optional[str] = None,
     wrapper: bool = False,
     long: bool = False,
     debug: bool = False,
-):
+) -> None:
     """
     Initiates a client from a configuration file.
 
     The configuration file format is specified by its extension (.yml/.yaml being YAML, .json being JSON). No other formats are accepted.
 
     Use -c/--command to pass a command into the client after instantiation. See -h/--help for other options concerning command usage. Not passing in a command will enter into an interactive shell.
     """
```

### Comparing `pibble-0.5.0/pibble/api/base.py` & `pibble-0.5.1/pibble/api/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/apachethrift/__init__.py` & `pibble-0.5.1/pibble/api/client/apachethrift/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/apachethrift/wrapper.py` & `pibble-0.5.1/pibble/api/client/apachethrift/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/base.py` & `pibble-0.5.1/pibble/api/client/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/file/base.py` & `pibble-0.5.1/pibble/api/client/file/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/file/ftp.py` & `pibble-0.5.1/pibble/api/client/file/ftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/file/hdfs.py` & `pibble-0.5.1/pibble/api/client/file/hdfs.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/file/local.py` & `pibble-0.5.1/pibble/api/client/file/local.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/file/sftp.py` & `pibble-0.5.1/pibble/api/client/file/sftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/googlerpc.py` & `pibble-0.5.1/pibble/api/client/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/webservice/apachethrift.py` & `pibble-0.5.1/pibble/api/client/webservice/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/webservice/base.py` & `pibble-0.5.1/pibble/api/client/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/webservice/jsonapi.py` & `pibble-0.5.1/pibble/api/client/webservice/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/webservice/rpc/base.py` & `pibble-0.5.1/pibble/api/client/webservice/rpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/webservice/rpc/jsonrpc.py` & `pibble-0.5.1/pibble/api/client/webservice/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/webservice/rpc/xmlrpc.py` & `pibble-0.5.1/pibble/api/client/webservice/rpc/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/webservice/soap.py` & `pibble-0.5.1/pibble/api/client/webservice/soap.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/webservice/wrapper.py` & `pibble-0.5.1/pibble/api/client/webservice/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/client/wrapper.py` & `pibble-0.5.1/pibble/api/client/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/configuration.py` & `pibble-0.5.1/pibble/api/configuration.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/exceptions.py` & `pibble-0.5.1/pibble/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/helpers/apachethrift.py` & `pibble-0.5.1/pibble/api/helpers/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/helpers/authentication.py` & `pibble-0.5.1/pibble/api/helpers/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/helpers/googlerpc.py` & `pibble-0.5.1/pibble/api/helpers/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/helpers/store.py` & `pibble-0.5.1/pibble/api/helpers/store.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/helpers/wrappers.py` & `pibble-0.5.1/pibble/api/helpers/wrappers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/meta/base.py` & `pibble-0.5.1/pibble/api/meta/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/meta/helpers.py` & `pibble-0.5.1/pibble/api/meta/helpers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/middleware/apachethrift/base.py` & `pibble-0.5.1/pibble/api/middleware/apachethrift/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/middleware/apachethrift/screening.py` & `pibble-0.5.1/pibble/api/middleware/apachethrift/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/middleware/database/orm.py` & `pibble-0.5.1/pibble/api/middleware/database/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/middleware/googlerpc/authentication.py` & `pibble-0.5.1/pibble/api/middleware/googlerpc/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/middleware/googlerpc/base.py` & `pibble-0.5.1/pibble/api/middleware/googlerpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/middleware/googlerpc/metadata.py` & `pibble-0.5.1/pibble/api/middleware/googlerpc/metadata.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/middleware/screening.py` & `pibble-0.5.1/pibble/api/middleware/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/middleware/webservice/authentication/basic.py` & `pibble-0.5.1/pibble/api/middleware/webservice/authentication/basic.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/middleware/webservice/authentication/bearer.py` & `pibble-0.5.1/pibble/api/middleware/webservice/authentication/bearer.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/middleware/webservice/authentication/digest.py` & `pibble-0.5.1/pibble/api/middleware/webservice/authentication/digest.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/middleware/webservice/authentication/header.py` & `pibble-0.5.1/pibble/api/middleware/webservice/authentication/header.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/middleware/webservice/authentication/oauth.py` & `pibble-0.5.1/pibble/api/middleware/webservice/authentication/oauth.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/middleware/webservice/base.py` & `pibble-0.5.1/pibble/api/middleware/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/middleware/webservice/limit.py` & `pibble-0.5.1/pibble/api/middleware/webservice/limit.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/middleware/webservice/screening.py` & `pibble-0.5.1/pibble/api/middleware/webservice/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/protocol/apachethrift.py` & `pibble-0.5.1/pibble/api/protocol/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/apachethrift.py` & `pibble-0.5.1/pibble/api/server/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/base.py` & `pibble-0.5.1/pibble/api/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/file/ftp.py` & `pibble-0.5.1/pibble/api/server/file/ftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/file/sftp.py` & `pibble-0.5.1/pibble/api/server/file/sftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/googlerpc.py` & `pibble-0.5.1/pibble/api/server/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/apachethrift.py` & `pibble-0.5.1/pibble/api/server/webservice/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/awslambda.py` & `pibble-0.5.1/pibble/api/server/webservice/awslambda.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/base.py` & `pibble-0.5.1/pibble/api/server/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/drivers/driver_cherrypy.py` & `pibble-0.5.1/pibble/api/server/webservice/drivers/driver_cherrypy.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/drivers/driver_gunicorn.py` & `pibble-0.5.1/pibble/api/server/webservice/drivers/driver_gunicorn.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/drivers/driver_werkzeug.py` & `pibble-0.5.1/pibble/api/server/webservice/drivers/driver_werkzeug.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/handler.py` & `pibble-0.5.1/pibble/api/server/webservice/handler.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/jsonapi.py` & `pibble-0.5.1/pibble/api/server/webservice/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/orm.py` & `pibble-0.5.1/pibble/api/server/webservice/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/rpc/base.py` & `pibble-0.5.1/pibble/api/server/webservice/rpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/rpc/jsonrpc.py` & `pibble-0.5.1/pibble/api/server/webservice/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/rpc/xmlrpc.py` & `pibble-0.5.1/pibble/api/server/webservice/rpc/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/soap.py` & `pibble-0.5.1/pibble/api/server/webservice/soap.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/template/__init__.py` & `pibble-0.5.1/pibble/api/server/webservice/template/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/template/extensions.py` & `pibble-0.5.1/pibble/api/server/webservice/template/extensions.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/api/server/webservice/template/loader.py` & `pibble-0.5.1/pibble/api/server/webservice/template/loader.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/database/dedupe.py` & `pibble-0.5.1/pibble/database/dedupe.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/database/engine.py` & `pibble-0.5.1/pibble/database/engine.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/database/orm.py` & `pibble-0.5.1/pibble/database/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/database/util.py` & `pibble-0.5.1/pibble/database/util.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/cms/database/__init__.py` & `pibble-0.5.1/pibble/ext/cms/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/cms/database/interface.py` & `pibble-0.5.1/pibble/ext/cms/database/interface.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/cms/database/menu.py` & `pibble-0.5.1/pibble/ext/cms/database/menu.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/cms/database/view.py` & `pibble-0.5.1/pibble/ext/cms/database/view.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/cms/middleware.py` & `pibble-0.5.1/pibble/ext/cms/middleware.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/cms/server/base.py` & `pibble-0.5.1/pibble/ext/cms/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/cms/server/extension.py` & `pibble-0.5.1/pibble/ext/cms/server/extension.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/dam/database/files.py` & `pibble-0.5.1/pibble/ext/dam/database/files.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/rest/server/base.py` & `pibble-0.5.1/pibble/ext/rest/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/rest/server/user.py` & `pibble-0.5.1/pibble/ext/rest/server/user.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/session/database/session.py` & `pibble-0.5.1/pibble/ext/session/database/session.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/session/server/base.py` & `pibble-0.5.1/pibble/ext/session/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/user/client/base.py` & `pibble-0.5.1/pibble/ext/user/client/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/user/database/__init__.py` & `pibble-0.5.1/pibble/ext/user/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/user/database/authentication.py` & `pibble-0.5.1/pibble/ext/user/database/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/user/database/notification.py` & `pibble-0.5.1/pibble/ext/user/database/notification.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/user/database/permission.py` & `pibble-0.5.1/pibble/ext/user/database/permission.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/user/database/user.py` & `pibble-0.5.1/pibble/ext/user/database/user.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/ext/user/server/base.py` & `pibble-0.5.1/pibble/ext/user/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/hooks/aws.py` & `pibble-0.5.1/pibble/hooks/aws.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/media/thumbnail.py` & `pibble-0.5.1/pibble/media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/resources/retriever.py` & `pibble-0.5.1/pibble/resources/retriever.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/scripts/importcheck.py` & `pibble-0.5.1/pibble/scripts/importcheck.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/scripts/templatefiles.py` & `pibble-0.5.1/pibble/scripts/templatefiles.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/setup.py` & `pibble-0.5.1/pibble/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
 version_minor = "5"
-version_patch = "0"
+version_patch = "1"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
```

### Comparing `pibble-0.5.0/pibble/util/encryption.py` & `pibble-0.5.1/pibble/util/encryption.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/util/files.py` & `pibble-0.5.1/pibble/util/files.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/util/helpers.py` & `pibble-0.5.1/pibble/util/helpers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/util/imaging.py` & `pibble-0.5.1/pibble/util/imaging.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/util/log.py` & `pibble-0.5.1/pibble/util/log.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/util/numeric.py` & `pibble-0.5.1/pibble/util/numeric.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/util/strings.py` & `pibble-0.5.1/pibble/util/strings.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble/web/scraper.py` & `pibble-0.5.1/pibble/web/scraper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble.egg-info/PKG-INFO` & `pibble-0.5.1/pibble.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.5.0
+Version: 0.5.1
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
```

### Comparing `pibble-0.5.0/pibble.egg-info/SOURCES.txt` & `pibble-0.5.1/pibble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/pibble.egg-info/requires.txt` & `pibble-0.5.1/pibble.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pibble-0.5.0/setup.py` & `pibble-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
 version_minor = "5"
-version_patch = "0"
+version_patch = "1"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
```

