# Comparing `tmp/pibble-0.4.9.tar.gz` & `tmp/pibble-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pibble-0.4.9.tar", last modified: Mon May  1 00:10:08 2023, max compression
+gzip compressed data, was "pibble-0.5.0.tar", last modified: Wed May  3 22:26:54 2023, max compression
```

## Comparing `pibble-0.4.9.tar` & `pibble-0.5.0.tar`

### file list

```diff
@@ -1,208 +1,214 @@
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.989380 pibble-0.4.9/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6435 2023-05-01 00:10:08.989380 pibble-0.4.9/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5960 2023-05-01 00:10:08.000000 pibble-0.4.9/README.md
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.973380 pibble-0.4.9/pibble/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     8891 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/__main__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.973380 pibble-0.4.9/pibble/api/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3287 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.973380 pibble-0.4.9/pibble/api/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/client/apachethrift/
--rw-------   0 benjamin  (1000) benjamin  (1000)     6189 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/apachethrift/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1326 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/client/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    14182 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/file/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9703 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/file/hdfs.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    12462 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/file/local.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    19644 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4126 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/client/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4698 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16829 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2330 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/jsonapi.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/client/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11322 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4770 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10558 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6564 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/soap.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7325 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/configuration.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6085 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/exceptions.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/helpers/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/helpers/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15593 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/helpers/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    20508 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/helpers/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    24123 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/helpers/googlerpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13134 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/helpers/store.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13916 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/helpers/wrappers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/meta/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/meta/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9353 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/meta/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2958 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/meta/helpers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/middleware/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/middleware/apachethrift/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/apachethrift/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/apachethrift/screening.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/middleware/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3112 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/database/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/middleware/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      438 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/file/temp.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/middleware/googlerpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/googlerpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/googlerpc/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/googlerpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/googlerpc/metadata.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3027 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/middleware/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/middleware/webservice/authentication/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/authentication/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/authentication/basic.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/authentication/bearer.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13466 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/authentication/digest.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/authentication/header.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    17694 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/authentication/oauth.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3248 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/limit.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/protocol/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/protocol/__init__.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19471 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/protocol/apachethrift.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2443 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1983 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/server/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15450 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5445 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/server/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2377 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7264 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/awslambda.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    41732 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15532 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/handler.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3182 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/jsonapi.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/server/webservice/mixin/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/mixin/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      718 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/mixin/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      987 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/server/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4212 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6486 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11970 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16833 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/soap.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/server/webservice/template/
--rw-------   0 benjamin  (1000) benjamin  (1000)     9667 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/template/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9195 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/template/extensions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9764 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/template/loader.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7772 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/database/dedupe.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10216 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/database/engine.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/database/exceptions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    26389 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/database/orm.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2667 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/database/util.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/ext/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/ext/cms/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/cms/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/database/interface.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/database/menu.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/database/view.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/cms/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6382 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/server/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2998 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/server/extension.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      350 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/server/mixin.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/dam/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/dam/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/dam/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/dam/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/dam/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/dam/database/files.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/dam/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/dam/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/dam/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/rest/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/rest/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/rest/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/rest/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/rest/database/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/rest/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/rest/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15691 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/rest/server/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7707 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/rest/server/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/session/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/session/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/session/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/session/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/session/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/session/database/session.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/session/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/session/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5026 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/session/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/user/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/user/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/client/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      963 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/user/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/database/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/database/notification.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5865 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/database/permission.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      611 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/database/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/user/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    24969 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/hooks/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/hooks/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5971 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/hooks/aws.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/media/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/media/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10234 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/media/thumbnail.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/resources/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/resources/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10649 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/resources/retriever.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2694 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/setup.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.989380 pibble-0.4.9/pibble/util/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     8375 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/encryption.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16134 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/files.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    32731 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/helpers.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/imaging.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6330 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/log.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1610 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/numeric.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    27059 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/strings.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.989380 pibble-0.4.9/pibble/web/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/web/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/web/scraper.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.973380 pibble-0.4.9/pibble.egg-info/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6435 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble.egg-info/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5413 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble.egg-info/SOURCES.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble.egg-info/dependency_links.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble.egg-info/entry_points.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1872 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble.egg-info/requires.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble.egg-info/top_level.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-05-01 00:10:08.989380 pibble-0.4.9/setup.cfg
--rw-------   0 benjamin  (1000) benjamin  (1000)     2694 2023-05-01 00:10:08.000000 pibble-0.4.9/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6485 2023-05-03 22:26:54.502891 pibble-0.5.0/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5960 2023-05-03 22:26:54.000000 pibble-0.5.0/README.md
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     8891 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/__main__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3374 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/client/apachethrift/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6195 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/apachethrift/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1340 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/client/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    14230 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/file/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9726 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/file/hdfs.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    12782 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/file/local.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    19652 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4132 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/client/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4728 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16837 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2312 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/jsonapi.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/client/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11386 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4766 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10690 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6689 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/soap.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7333 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/webservice/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/client/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/configuration.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6101 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/exceptions.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/helpers/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/helpers/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15706 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/helpers/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    20612 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/helpers/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    24691 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/helpers/googlerpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13415 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/helpers/store.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13868 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/helpers/wrappers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/meta/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/meta/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9492 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/meta/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2952 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/meta/helpers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/middleware/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/middleware/apachethrift/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/apachethrift/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/apachethrift/screening.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble/api/middleware/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3730 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/database/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/middleware/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      454 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/file/temp.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/middleware/googlerpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/googlerpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/googlerpc/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/googlerpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/googlerpc/metadata.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3703 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/middleware/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/middleware/webservice/authentication/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/authentication/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/authentication/basic.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/authentication/bearer.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13472 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/authentication/digest.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/authentication/header.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    17704 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/authentication/oauth.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3256 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/limit.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/middleware/webservice/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/protocol/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/protocol/__init__.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19486 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/protocol/apachethrift.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2451 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2080 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/api/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/server/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15640 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5453 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/server/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2393 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7311 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/awslambda.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    38899 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/server/webservice/drivers/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/drivers/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1489 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/drivers/driver_cherrypy.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2194 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/drivers/driver_gunicorn.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1078 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/drivers/driver_werkzeug.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16024 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/handler.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3164 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/jsonapi.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      969 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/server/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4247 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6457 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    12004 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    17061 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/soap.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/api/server/webservice/template/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9717 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/template/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9201 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/template/extensions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9770 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/api/server/webservice/template/loader.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7797 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/database/dedupe.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10529 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/database/engine.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/database/exceptions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    26274 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/database/orm.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2694 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/database/util.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/ext/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.498891 pibble-0.5.0/pibble/ext/cms/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/cms/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/database/interface.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/database/menu.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/database/view.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1366 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/middleware.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/cms/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6759 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/server/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3012 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/cms/server/extension.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/dam/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/dam/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/dam/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/dam/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/dam/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/dam/database/files.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/dam/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/dam/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/dam/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/rest/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/rest/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/rest/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/rest/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/rest/database/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/rest/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/rest/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15690 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/rest/server/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7342 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/rest/server/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/session/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/session/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/session/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/session/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/session/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/session/database/session.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/session/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/session/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5207 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/session/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/user/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/user/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/client/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      985 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/user/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/database/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/database/notification.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5865 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/database/permission.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      611 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/database/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/ext/user/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    25034 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/ext/user/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/hooks/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/hooks/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6037 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/hooks/aws.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/media/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/media/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10388 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/media/thumbnail.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/resources/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/resources/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10655 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/resources/retriever.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/scripts/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/scripts/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1909 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/scripts/importcheck.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1726 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/scripts/templatefiles.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/util/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     8357 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/encryption.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16171 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/files.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    32821 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/helpers.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/imaging.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6330 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/log.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1701 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/numeric.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    27116 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble/util/strings.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.502891 pibble-0.5.0/pibble/web/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/web/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3227 2023-05-03 22:26:53.000000 pibble-0.5.0/pibble/web/scraper.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 22:26:54.494892 pibble-0.5.0/pibble.egg-info/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6485 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble.egg-info/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5627 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble.egg-info/SOURCES.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble.egg-info/dependency_links.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble.egg-info/entry_points.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1936 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble.egg-info/requires.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-05-03 22:26:54.000000 pibble-0.5.0/pibble.egg-info/top_level.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-05-03 22:26:54.502891 pibble-0.5.0/setup.cfg
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-03 22:26:54.000000 pibble-0.5.0/setup.py
```

### Comparing `pibble-0.4.9/PKG-INFO` & `pibble-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.4.9
+Version: 0.5.0
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
 Provides-Extra: mssql
 Provides-Extra: thrift
 Provides-Extra: grpc
 Provides-Extra: browser
 Provides-Extra: imaging
 Provides-Extra: cherrypy
+Provides-Extra: gunicorn
+Provides-Extra: werkzeug
 Provides-Extra: build
 Provides-Extra: all
 
 # pibble
 The Pibble framework turbocharges Python web applications with a huge array of features and easy-to-use interface.
 
 ## Installation
```

### Comparing `pibble-0.4.9/README.md` & `pibble-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/__main__.py` & `pibble-0.5.0/pibble/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,25 +80,25 @@
 
 
 @main.command(short_help="Start multiple servers based on configurations.")
 @click.argument("configuration", nargs=-1)
 @click.option(
     "--debug", is_flag=True, help="Turn on debug unified logging.", default=False
 )
-def servers(configuration: list[str], debug: bool = False):
+def servers(configuration: List[str], debug: bool = False):
     """
     Starts servers, synchronously, using a configuration file.
 
     All servers will be ran at the same time, and stopped at the same time.
     If any server errors, all will be stopped.
 
     The configuration file format is specified by its extension (.yml/.yaml being YAML, .json being JSON). No other formats are accepted.
     """
 
-    services: list[MetaServerProcess] = []
+    services: List[MetaServerProcess] = []
 
     for config in configuration:
         factory = MetaFactory.from_file(config)
         meta_service = factory("server")
         services.append(MetaServerProcess(meta_service))
 
     if debug:
@@ -163,15 +163,15 @@
 )
 @click.option(
     "--debug", is_flag=True, help="Turn on debug unified logging.", default=False
 )
 def client(
     configuration: str,
     command: Optional[str] = None,
-    arg: Optional[list[str]] = None,
+    arg: Optional[List[str]] = None,
     json: Optional[str] = None,
     wrapper: bool = False,
     long: bool = False,
     debug: bool = False,
 ):
     """
     Initiates a client from a configuration file.
```

### Comparing `pibble-0.4.9/pibble/api/base.py` & `pibble-0.5.0/pibble/api/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import os
-from typing import Any
+from typing import Any, Union, List
 
 from pibble.api.configuration import APIConfiguration
 from pibble.api.helpers.store import APISessionStore, UnconfiguredAPISessionStore
 from pibble.api.exceptions import ConfigurationError
 from pibble.util.log import logger, ConfigurationLoggingContext
 from pibble.util.strings import pretty_print, get_uuid
 
 
 class APIBase:
     """
     A base class for servers and clients to inherit from.
     """
 
-    def __init__(self):
+    session: Union[UnconfiguredAPISessionStore, APISessionStore]
+
+    def __init__(self) -> None:
         logger.debug("Initializing API base.")
         self.configuration = APIConfiguration()
         self.configuration.put("session_key", get_uuid())
         self.session = UnconfiguredAPISessionStore()
 
     def on_configure(self) -> None:
         """
@@ -79,12 +81,12 @@
                             cls.__name__
                         )
                     )
                     cls.on_configure(self)
                 except Exception as ex:
                     raise ConfigurationError(str(ex))
 
-    def listMethods(self) -> list[str]:
+    def listMethods(self) -> List[str]:
         """
         Should be extended for function-based servers or clients.
         """
         raise NotImplementedError()
```

### Comparing `pibble-0.4.9/pibble/api/client/apachethrift/__init__.py` & `pibble-0.5.0/pibble/api/client/apachethrift/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import functools
 
-from typing import Callable, Any
+from typing import Callable, Any, List
 
 from thrift.transport import TSocket
 from thrift.transport import TTransport
 from thrift.protocol import TBinaryProtocol
 
 from pibble.api.client.base import APIClientBase
 
@@ -27,15 +27,15 @@
 
     def on_configure(self) -> None:
         """
         Instantiate the service.
         """
         self.thrift = ApacheThriftService(self.configuration)
 
-    def listMethods(self) -> list[str]:
+    def listMethods(self) -> List[str]:
         """
         List methods in the interface.
         """
         return [
             func
             for func in dir(self.thrift.interface)
             if callable(getattr(self.thrift.interface, func))
```

### Comparing `pibble-0.4.9/pibble/api/client/apachethrift/wrapper.py` & `pibble-0.5.0/pibble/api/client/apachethrift/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/api/client/base.py` & `pibble-0.5.0/pibble/api/client/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
-from typing import Any
+from typing import Any, List
 
 from pibble.util.log import logger
 from pibble.api.base import APIBase
 
 
 class APIClientBase(APIBase):
     """
     A base client class, from which all implementing clients will inherit.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         logger.debug("Initializing API Client Base.")
         super(APIClientBase, self).__init__()
 
     def __enter__(self) -> APIClientBase:
         """
         A small context manager to use the close() function.
         """
@@ -35,14 +35,14 @@
     def close(self) -> None:
         """
         Closes a client. This may or may not be meaningful, depending on the
         client type (namely, whether or not a persistent client is created).
         """
         pass
 
-    def listMethods(self) -> list[str]:
+    def listMethods(self) -> List[str]:
         """
         Lists methods, if available. Implementing clients should override these.
 
         :raises NotImplementedError: When the implementing class does not override.
         """
         raise NotImplementedError()
```

### Comparing `pibble-0.4.9/pibble/api/client/file/base.py` & `pibble-0.5.0/pibble/api/client/file/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class ContentIterator:
     """
     A simple wrapper to make sure contents are properly iterable.
     """
 
-    def __init__(self, contents: Any):
+    def __init__(self, contents: Any) -> None:
         if any(
             [
                 isinstance(contents, cls)
                 for cls in [io.TextIOBase, io.BufferedIOBase, io.RawIOBase, io.IOBase]
             ]
         ):
             self.iterable = True
@@ -71,15 +71,15 @@
 
 
 class FileTransferAPIClientBase(APIClientBase):
     """
     A base class for file transfer clients.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         logger.debug("Initializing File Transfer API Client Base.")
         super(FileTransferAPIClientBase, self).__init__()
         self.cwd = ""
 
     # Directory Operations
 
     def changeDirectory(self, path: str, **kwargs: Any) -> None:
@@ -205,18 +205,18 @@
         if type(start) is str:
             fmt = lambda part: part
             buf = ""
         else:
             fmt = lambda part: bytearray(part)
             buf = bytearray()  # type: ignore
 
-        buf += fmt(start)
+        buf += fmt(start)  # type: ignore
 
         for chunk in iterator:
-            buf += fmt(chunk)
+            buf += fmt(chunk)  # type: ignore
         return buf
 
     def checksumFile(self, path: str, **kwargs: Any) -> str:
         """
         Checksums a file.
 
         Some implementations will be able to do this without needing to get the whole
```

### Comparing `pibble-0.4.9/pibble/api/client/file/ftp.py` & `pibble-0.5.0/pibble/api/client/file/ftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ftplib
 import os
 import datetime
 
-from typing import Iterator, Iterable, Optional, Any, Union
+from typing import Iterator, Iterable, Optional, Any, Union, Mapping
 
 from pibble.api.exceptions import (
     NotFoundError,
     BadRequestError,
 )
 from pibble.api.client.file.base import (
     FileTransferAPIClientBase,
@@ -49,15 +49,15 @@
         try:
             self.ftp.quit()
         except:
             pass
 
     # Helpers
 
-    def convertFacts(self, path, facts) -> RemoteObject:
+    def convertFacts(self, path: str, facts: Mapping) -> RemoteObject:
         """
         Converts an MLSx response to a RemoteObject.
 
         :param path str: The path of the remote file.
         :param facts dict: A dictionary of facts.
         :returns RemoteObject: The converted object.
         """
```

### Comparing `pibble-0.4.9/pibble/api/client/file/hdfs.py` & `pibble-0.5.0/pibble/api/client/file/hdfs.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/api/client/file/local.py` & `pibble-0.5.0/pibble/api/client/file/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     import pwd
 except ImportError:
     pass
 
 from multiprocessing import Process, Pipe
 from multiprocessing.connection import Connection
 
-from typing import Callable, Optional, Iterable, Any
+from typing import Callable, Optional, Iterable, Any, cast
 
 from pibble.api.client.file.base import (
     FileTransferAPIClientBase,
     RemoteObject,
     ContentIterator,
 )
 from pibble.api.exceptions import (
@@ -26,26 +26,26 @@
 )
 from pibble.util.strings import encode
 from pibble.util.log import logger
 from pibble.util.helpers import is_binary_file
 from pibble.util.numeric import r8d2o, o2r8d
 
 
-def UserContext(fn) -> Callable:
+def UserContext(fn: Callable) -> Callable:
     """
     Executes a function under the context of a user (or no user.)
 
     Returns a callable suitable for decoration.
     """
 
     if os.name == "nt":
         # No user context available for windows.
         return lambda *args, **kwargs: fn(*args, **kwargs)
 
-    def callable(*args: Any, **kwargs: Any) -> None:
+    def callable(*args: Any, **kwargs: Any) -> Any:
         user = kwargs.get("user", None)
         demote = False
         uid = None
         if user is not None:
             uid = pwd.getpwnam(user).pw_uid  # type: ignore
             if uid != os.getuid():  # type: ignore
                 demote = True
@@ -116,28 +116,33 @@
         :param path str: A directory path.
         :param permission int: Any radix-8 permission integer. Default None.
         :param owner str: The owner of the file. Default None.
         :param group str: The group of the file. Default None.
         :returns RemoteObject: The new directory.
         """
         path = self.absPath(path)
-        os.makedirs(path, r8d2o(permission))
+        if permission:
+            permission = r8d2o(permission)
+        else:
+            permission = 0o700
+
+        os.makedirs(path, permission)
 
         if os.name != "nt":
             if owner is not None:
                 uid = pwd.getpwnam(owner).pw_uid  # type: ignore
             else:
                 uid = -1
             if group is not None:
                 gid = pwd.getpwnam(group).pw_uid  # type: ignore
             else:
                 gid = -1
 
             os.chown(path, uid, gid)  # type: ignore
-        return self.getPath(path)
+        return cast(RemoteObject, self.getPath(path))
 
     @UserContext
     def listDirectory(self, path: str, **kwargs: Any) -> Iterable[RemoteObject]:
         """
         Lists the contents of a directory.
 
         :param path str: A directory path.
@@ -171,24 +176,24 @@
         :param permission int: Any radix-8 permission integer. Default None.
         :param owner str: The owner of the file. Default None.
         :param group str: The group of the file. Default None.
         :returns RemoteObject: The newly written remote file.
         """
         path = self.absPath(path)
         if os.path.exists(path) and not overwrite:
-            return self.getPath(path)
+            return cast(RemoteObject, self.getPath(path))
         else:
             with open(path, "wb") as fp:
                 for part in ContentIterator(contents):
                     fp.write(encode(part))
             if permission is not None:
                 self.setPathPermission(path, permission)
             if owner is not None or group is not None:
                 self.setPathOwner(path, owner, group)
-        return self.getPath(path)
+        return cast(RemoteObject, self.getPath(path))
 
     @UserContext
     def appendFile(self, path: str, contents: Any, **kwargs: Any) -> RemoteObject:
         """
         Appends contents to a file. Some implementations may not have a method
         specifically for this, so a base method is provided to do so.
 
@@ -196,15 +201,15 @@
         :param contents object: Either a unicode string, bytes-like object or iterable.
         :returns RemoteObject: The newly modified remote file.
         """
         path = self.absPath(path)
         with open(path, "ab") as fp:
             for part in ContentIterator(contents):
                 fp.write(encode(part))
-        return self.getPath(path)
+        return cast(RemoteObject, self.getPath(path))
 
     @UserContext
     def readFile(self, path: str, **kwargs: Any) -> Iterable[bytes]:
         """
         Reads the contents of a file.
 
         This should return an iterator to gradually the read the file.
@@ -276,19 +281,19 @@
         :param dest str: The destination path.
         :returns RemoteObject: The newly moved file.
         :raises `pibble.api.exceptions.NotFoundError`: When src is not found.
         """
         src = self.absPath(src)
         dest = self.absPath(dest)
         if os.path.exists(dest) and not overwrite:
-            return self.getPath(dest)
+            return cast(RemoteObject, self.getPath(dest))
         if not os.path.exists(src):
             raise NotFoundError("Cannot find file {0}".format(src))
         os.rename(src, dest)
-        return self.getPath(dest)
+        return cast(RemoteObject, self.getPath(dest))
 
     @UserContext
     def deletePath(self, path: str, **kwargs: Any) -> bool:
         """
         Delete a path.
 
         :param path str: Either a file or directory path.
@@ -311,15 +316,15 @@
         :param path str: Either a file or directory path.
         :param permission: Any radix-8 permission integer.
         :returns RemoteObject: The updated path.
         :raises `pibble.api.exceptions.NotFoundError`: When the path is not found.
         """
         node = self.getPath(path)
         os.chmod(node.path, r8d2o(permission))
-        return self.getPath(path)
+        return cast(RemoteObject, self.getPath(path))
 
     @UserContext
     def copyPath(
         self, src: str, dest: str, overwrite: Optional[bool] = False, **kwargs: Any
     ) -> RemoteObject:
         """
         Copies a path from src to dest.
@@ -328,22 +333,22 @@
         :param dest str: The path to the destination, either a file or directory.
         :param overwrite bool: Whether or not to overwrite when calling writeFile.
         :returns RemoteObject: The newly copied file.
         :raises `pibble.api.exceptions.NotFoundError`: When src is not found.
         """
         dest = self.absPath(dest)
         if os.path.exists(dest) and not overwrite:
-            return self.getPath(dest)
+            return cast(RemoteObject, self.getPath(dest))
 
         node = self.getPath(src)
         if node.otype == RemoteObject.DIRECTORY:
             shutil.copytree(node.path, dest)
         else:
             shutil.copy(node.path, dest)
-        return self.getPath(dest)
+        return cast(RemoteObject, self.getPath(dest))
 
     def setPathOwner(
         self,
         path: str,
         owner: Optional[str] = None,
         group: Optional[str] = None,
         **kwargs: Any
@@ -369,8 +374,8 @@
                 else:
                     uid = -1
                 if group is not None:
                     gid = pwd.getpwnam(group).pw_uid  # type: ignore
                 else:
                     gid = -1
                 os.chown(path, uid, gid)  # type: ignore
-        return self.getPath(path)
+        return cast(RemoteObject, self.getPath(path))
```

### Comparing `pibble-0.4.9/pibble/api/client/file/sftp.py` & `pibble-0.5.0/pibble/api/client/file/sftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
                 "Error connecting to {0}:{1}. {2}".format(self.host, self.port, str(ex))
             )
 
         self.sftp = cast(
             paramiko.SFTPClient, paramiko.SFTPClient.from_transport(self.transport)
         )
 
-    def close(self):
+    def close(self) -> None:
         """
         Closes the active SFTP connection.
         """
         ignore_exceptions(self.sftp.close)
         ignore_exceptions(self.transport.close)
 
     # Helper Functions
```

### Comparing `pibble-0.4.9/pibble/api/client/googlerpc.py` & `pibble-0.5.0/pibble/api/client/googlerpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import grpc
 
-from typing import Callable, Any
+from typing import Callable, Any, List
 from functools import partial
 
 from pibble.api.client.base import APIClientBase
 from pibble.api.helpers.googlerpc import (
     GRPCConfiguration,
     GRPCRequest,
     GRPCResponse,
@@ -113,15 +113,15 @@
         Allows for client.method calls.
         """
         try:
             return self[key]
         except KeyError:
             raise AttributeError(key)
 
-    def listMethods(self) -> list[str]:
+    def listMethods(self) -> List[str]:
         """
         Lists all methods present in the stub.
         """
         return [
             method
             for method in dir(self.client)
             if not method.startswith("_") and callable(getattr(self.client, method))
```

### Comparing `pibble-0.4.9/pibble/api/client/webservice/apachethrift.py` & `pibble-0.5.0/pibble/api/client/webservice/apachethrift.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from functools import partial
-from typing import Callable, Any
+from typing import Callable, Any, List
 
 from pibble.util.log import logger
 from pibble.util.helpers import resolve
 from pibble.api.client.webservice.base import WebServiceAPIClientBase
 from pibble.api.helpers.apachethrift import (
     TTransitiveMemoryBuffer,
     ApacheThriftService,
 )
-from pibble.api.protocol.apachethrift import TJSONProtocol
+from pibble.api.protocol.apachethrift import TJSONProtocol  # type: ignore
 
 
 class ApacheThriftWebClient(WebServiceAPIClientBase):
     """
     A client for thrift web services.
 
     Whenever possible, you should use the regular client and server, as there is significant overhead
@@ -28,15 +28,15 @@
 
     See :class:`pibble.api.helpers.thrift.ThriftService` for required service arguments.
     See superclass :class:`pibble.api.client.webservice.base.WebServiceAPIClientBase` for additional required arguments.
     """
 
     BUFFER_SIZE = 2**15
 
-    def __init__(self):
+    def __init__(self) -> None:
         super(ApacheThriftWebClient, self).__init__()
 
         # Generate input and output protocols.
         # These protocols essentially just write binary data to a bytearray.
         self.input_transport = TTransitiveMemoryBuffer()
         self.input_protocol = TJSONProtocol(self.input_transport)
 
@@ -48,15 +48,15 @@
 
         # Instantiate the client with the transports we made.
         self.client = self.thrift.service.Client(
             self.input_protocol, self.output_protocol
         )
         self.interface = self.thrift.service.Iface()
 
-    def listMethods(self) -> list[str]:
+    def listMethods(self) -> List[str]:
         """
         Lists methods in the interface.
         """
         return [
             method
             for method in dir(self.interface)
             if callable(getattr(self.interface, method)) and not method.startswith("_")
```

### Comparing `pibble-0.4.9/pibble/api/client/webservice/base.py` & `pibble-0.5.0/pibble/api/client/webservice/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import os
 from io import IOBase
-from typing import Optional, Callable, Any, Union, Type, cast
+from typing import Optional, Callable, Any, Union, Type, Dict, List, cast
 
 from pibble.util.helpers import url_join, resolve
 from pibble.util.log import logger
-from pibble.util.strings import FlexibleStringer
+from pibble.util.strings import Serializer
 
 from pibble.api.exceptions import (
     NotFoundError,
     UnsupportedMethodError,
     AuthenticationError,
     PermissionError,
     BadRequestError,
@@ -41,15 +41,15 @@
     retry: bool
     http_session: Union[Session, SessionWrapper]
 
     session_class: Type[Union[Session, SessionWrapper]] = Session
     request_class: Type[Union[Request, RequestWrapper]] = Request
     response_class: Type[Union[Response, ResponseWrapper]] = Response
 
-    def __init__(self):
+    def __init__(self) -> None:
         super(APIClientBase, self).__init__()
         self.headers = {"Accept-Encoding": "gzip"}
 
     def on_configure(self) -> None:
         """
         Builds the configuration.
         """
@@ -114,15 +114,15 @@
         :param request Request: The request before it goes out.
         :param response Response: The response before it goes out.
         """
         if not hasattr(self, "serializer"):
             if "client.serializer" in self.configuration:
                 self.serializer = self.configuration["client.serializer"]
             else:
-                self.serializer = FlexibleStringer.serialize
+                self.serializer = Serializer.serialize
             if type(self.serializer) in [str, bytes] and not callable(self.serializer):
                 try:
                     self.serializer = resolve(self.serializer)
                 except ImportError:
                     raise ConfigurationError(
                         "Cannot resolve serializer name {0}.".format(self.serializer)
                     )
@@ -162,17 +162,17 @@
                     )
                 )
 
     def query(
         self,
         method: str,
         url: str = "/",
-        parameters: dict[str, Any] = {},
-        headers: dict[str, Any] = {},
-        files: dict[str, IOBase] = {},
+        parameters: Dict[str, Any] = {},
+        headers: Dict[str, Any] = {},
+        files: Dict[str, IOBase] = {},
         data: Any = {},
         **kwargs: Any,
     ) -> Union[Response, ResponseWrapper]:
         """
         Sends a request using method "METHOD", with a couple caveats:
           * ``parameters`` is only used in GET, DELETE, HEAD, and OPTIONS
           * ``files`` and ``data`` is only used in PUT, POST, and PATCH
@@ -241,17 +241,17 @@
             self.raise_for_status(response)
         return response
 
     def download(
         self,
         method: str,
         url: str = "/",
-        parameters: dict[str, Any] = {},
-        headers: dict[str, Any] = {},
-        files: dict[str, IOBase] = {},
+        parameters: Dict[str, Any] = {},
+        headers: Dict[str, Any] = {},
+        files: Dict[str, IOBase] = {},
         data: Any = {},
         filename: Optional[str] = None,
         directory: Optional[str] = None,
         **kwargs: Any,
     ) -> str:
         """
         Uses query(), but streams the result to a local file.
@@ -296,73 +296,73 @@
             ):
                 fh.write(chunk)
         return abs_path
 
     def get(
         self,
         url: str = "/",
-        parameters: dict[str, Any] = {},
-        headers: dict[str, Any] = {},
+        parameters: Dict[str, Any] = {},
+        headers: Dict[str, Any] = {},
         **kwargs: Any,
     ) -> Union[Response, ResponseWrapper]:
         """
         Sends a GET request. See :func:`pibble.api.client.webservice.base.WebServiceAPIClientBase.query`
         """
         return self.query(
             "GET", url=url, parameters=parameters, headers=headers, **kwargs
         )
 
     def delete(
         self,
         url: str = "/",
-        parameters: dict[str, Any] = {},
-        headers: dict[str, Any] = {},
+        parameters: Dict[str, Any] = {},
+        headers: Dict[str, Any] = {},
         **kwargs: Any,
     ) -> Union[Response, ResponseWrapper]:
         """
         Sends a DELETE request. See :func:`pibble.api.client.webservice.base.WebServiceAPIClientBase.query`
         """
         return self.query(
             "DELETE", url=url, parameters=parameters, headers=headers, **kwargs
         )
 
     def head(
         self,
         url: str = "/",
-        parameters: dict[str, Any] = {},
-        headers: dict[str, Any] = {},
+        parameters: Dict[str, Any] = {},
+        headers: Dict[str, Any] = {},
         **kwargs: Any,
     ) -> Union[Response, ResponseWrapper]:
         """
         Sends a HEAD request. See :func:`pibble.api.client.webservice.base.WebServiceAPIClientBase.query`
         """
         return self.query(
             "HEAD", url=url, parameters=parameters, headers=headers, **kwargs
         )
 
     def options(
         self,
         url: str = "/",
-        parameters: dict[str, Any] = {},
-        headers: dict[str, Any] = {},
+        parameters: Dict[str, Any] = {},
+        headers: Dict[str, Any] = {},
         **kwargs: Any,
     ) -> Union[Response, ResponseWrapper]:
         """
         Sends an OPTIONS request. See :func:`pibble.api.client.webservice.base.WebServiceAPIClientBase.query`
         """
         return self.query(
             "OPTIONS", url=url, parameters=parameters, headers=headers, **kwargs
         )
 
     def post(
         self,
         url: str = "/",
-        parameters: dict[str, Any] = {},
-        headers: dict[str, Any] = {},
-        files: dict[str, IOBase] = {},
+        parameters: Dict[str, Any] = {},
+        headers: Dict[str, Any] = {},
+        files: Dict[str, IOBase] = {},
         data: Any = {},
         **kwargs: Any,
     ) -> Union[Response, ResponseWrapper]:
         """
         Sends a POST request. See :func:`pibble.api.client.webservice.base.WebServiceAPIClientBase.query`
         """
         return self.query(
@@ -374,17 +374,17 @@
             headers=headers,
             **kwargs,
         )
 
     def put(
         self,
         url: str = "/",
-        parameters: dict[str, Any] = {},
-        headers: dict[str, Any] = {},
-        files: dict[str, IOBase] = {},
+        parameters: Dict[str, Any] = {},
+        headers: Dict[str, Any] = {},
+        files: Dict[str, IOBase] = {},
         data: Any = {},
         **kwargs: Any,
     ) -> Union[Response, ResponseWrapper]:
         """
         Sends a PUT request. See :func:`pibble.api.client.webservice.base.WebServiceAPIClientBase.query`
         """
         return self.query(
@@ -396,28 +396,28 @@
             headers=headers,
             **kwargs,
         )
 
     def patch(
         self,
         url: str = "/",
-        parameters: dict[str, Any] = {},
-        headers: dict[str, Any] = {},
-        files: dict[str, IOBase] = {},
+        parameters: Dict[str, Any] = {},
+        headers: Dict[str, Any] = {},
+        files: Dict[str, IOBase] = {},
         data: Any = {},
         **kwargs: Any,
     ) -> Union[Response, ResponseWrapper]:
         """
         Sends a PATCH request. See :func:`pibble.api.client.webservice.base.WebServiceAPIClientBase.query`
         """
         return self.query(
             "PATCH", url=url, data=data, files=files, headers=headers, **kwargs
         )
 
-    def listMethods(self) -> list[str]:
+    def listMethods(self) -> List[str]:
         """
         Unless overridden, this will list the default functions.
         """
         return [
             "get",
             "post",
             "put",
```

### Comparing `pibble-0.4.9/pibble/api/client/webservice/jsonapi.py` & `pibble-0.5.0/pibble/api/client/webservice/jsonapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 import json
 
 from io import IOBase
 from requests import Response
-from typing import Any, Union
+from typing import Any, Union, Dict
 
-from pibble.util.strings import FlexibleStringer
+from pibble.util.strings import Serializer
 from pibble.api.helpers.wrappers import ResponseWrapper
 from pibble.api.client.webservice.base import WebServiceAPIClientBase
 
 __all__ = ["JSONWebServiceAPIClient"]
 
 
 class JSONWebServiceAPIClient(WebServiceAPIClientBase):
     def post(
         self,
         url: str = "/",
-        parameters: dict[str, Any] = {},
-        headers: dict[str, Any] = {},
-        files: dict[str, IOBase] = {},
+        parameters: Dict[str, Any] = {},
+        headers: Dict[str, Any] = {},
+        files: Dict[str, IOBase] = {},
         data: Any = {},
         **kwargs: Any,
     ) -> Union[Response, ResponseWrapper]:
         """
         Sends a POST request. See :func:`pibble.api.client.webservice.base.WebServiceAPIClientBase.query`
         """
         if data:
-            formatted_data = json.dumps(data, default=FlexibleStringer.serialize)
+            formatted_data = json.dumps(data, default=Serializer.serialize)
             headers["Content-Type"] = "application/vnd.api+json"
         else:
             formatted_data = None
         return super(JSONWebServiceAPIClient, self).post(
             url, parameters, headers, files, formatted_data, **kwargs
         )
 
     def put(
         self,
         url: str = "/",
-        parameters: dict[str, Any] = {},
-        headers: dict[str, Any] = {},
-        files: dict[str, IOBase] = {},
+        parameters: Dict[str, Any] = {},
+        headers: Dict[str, Any] = {},
+        files: Dict[str, IOBase] = {},
         data: Any = {},
         **kwargs: Any,
     ) -> Union[Response, ResponseWrapper]:
         if data:
-            formatted_data = json.dumps(data, default=FlexibleStringer.serialize)
+            formatted_data = json.dumps(data, default=Serializer.serialize)
             headers["Content-Type"] = "application/vnd.api+json"
         else:
             formatted_data = None
         return super(JSONWebServiceAPIClient, self).put(
             url, parameters, headers, files, formatted_data, **kwargs
         )
 
     def patch(
         self,
         url: str = "/",
-        parameters: dict[str, Any] = {},
-        headers: dict[str, Any] = {},
-        files: dict[str, IOBase] = {},
+        parameters: Dict[str, Any] = {},
+        headers: Dict[str, Any] = {},
+        files: Dict[str, IOBase] = {},
         data: Any = {},
         **kwargs: Any,
     ) -> Union[Response, ResponseWrapper]:
         if data:
-            formatted_data = json.dumps(data, default=FlexibleStringer.serialize)
+            formatted_data = json.dumps(data, default=Serializer.serialize)
             headers["Content-Type"] = "application/vnd.api+json"
         else:
             formatted_data = None
         return super(JSONWebServiceAPIClient, self).patch(
             url, parameters, headers, files, formatted_data, **kwargs
         )
```

### Comparing `pibble-0.4.9/pibble/api/client/webservice/rpc/base.py` & `pibble-0.5.0/pibble/api/client/webservice/rpc/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Callable, Any, Type, Optional
+from typing import Callable, Any, Type, Optional, List, Dict
 
 from pibble.util.log import logger
 from pibble.util.strings import pretty_print
 from pibble.api.exceptions import BadRequestError, UnsupportedMethodError
 from pibble.api.client.webservice.base import WebServiceAPIClientBase
 
 
@@ -13,27 +13,29 @@
     A base class for RPC Clients.
 
     This class does not care about any arguments of its own constructor, it merely passes it to its parent class.
     After parent initialization, it performs its own initialization, generating the system methods, and calling
     the server to ask for its definition.
     """
 
-    def __init__(self):
+    methods: List[RPCClientBase.RPCMethod]
+
+    def __init__(self) -> None:
         super(RPCClientBase, self).__init__()
         if not self.configuration.has("client.path"):
             self.configuration["client.path"] = "/RPC2"
         self.methods = [
             RPCClientBase.RPCMethod(self, "system.listMethods", [[list]]),
             RPCClientBase.RPCMethod(self, "system.methodHelp", [[str, str]]),
             RPCClientBase.RPCMethod(self, "system.methodSignature", [[list, str]]),
         ]
         self.introspected = False
         self.introspection_failed = False
 
-    def listMethods(self) -> list[str]:
+    def listMethods(self) -> List[str]:
         """
         Lists the methods in the client.
         """
         return [method.name for method in self.methods]
 
     def on_configure(self) -> None:
         """
@@ -163,15 +165,15 @@
         """
 
         def __init__(
             self,
             client: RPCClientBase,
             name: str,
             arguments: Optional[list] = None,
-            named_arguments: Optional[dict[str, Any]] = None,
+            named_arguments: Optional[Dict[str, Any]] = None,
         ):
             self.client = client
             self.name = name
             self.arguments = arguments
             self.named_arguments = named_arguments
 
         def __call__(self, *args: Any, **kwargs: Any) -> Any:
```

### Comparing `pibble-0.4.9/pibble/api/client/webservice/rpc/jsonrpc.py` & `pibble-0.5.0/pibble/api/client/webservice/rpc/jsonrpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 from pibble.api.client.webservice.rpc.base import RPCClientBase
 from pibble.api.exceptions import (
     BadRequestError,
     BadResponseError,
     UnknownError,
     UnsupportedMethodError,
 )
-from pibble.util.strings import FlexibleStringer
+from pibble.util.strings import Serializer
 
 
 class JSONRPCClient(RPCClientBase):
     """
     An implementation of a JSON RPC client.
 
     We can't do an all-encompassing doctest here, as it relies on an externally reachable server.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         super(JSONRPCClient, self).__init__()
         self.headers["Content-Type"] = "application/json"
         self.request_id = 1
 
     @staticmethod
     def map_typename(typename: str) -> Type:
         """
@@ -77,15 +77,15 @@
             base["params"] = list(args)
         if kwargs:
             base["params"] = kwargs
         elif args and kwargs:
             raise BadRequestError(
                 "Cannot pass both positional and named arguments into a JSONRPC method request."
             )
-        return json.dumps(base, default=FlexibleStringer.serialize)
+        return json.dumps(base, default=Serializer.serialize)
 
     def format_response(self, response: str) -> Any:
         """
         Takes a response from the RPC server, and returns its contents.
 
         >>> from pibble.api.client.webservice.rpc.jsonrpc import JSONRPCClient
         >>> import json
@@ -122,8 +122,8 @@
                 )
             else:
                 raise UnknownError(
                     "An unhandled fault code ({0}) was received. Message: {1}".format(
                         code, msg
                     )
                 )
-        return FlexibleStringer.parse(body.get("result", None))
+        return Serializer.deserialize(body.get("result", None))
```

### Comparing `pibble-0.4.9/pibble/api/client/webservice/rpc/xmlrpc.py` & `pibble-0.5.0/pibble/api/client/webservice/rpc/xmlrpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import sys
+import base64
 import datetime
 import lxml.etree as ET
 from lxml.builder import E
 from pibble.api.client.webservice.rpc.base import RPCClientBase
 from pibble.api.exceptions import (
     BadRequestError,
     BadResponseError,
     UnknownError,
     UnsupportedMethodError,
 )
-from typing import Type, Any
+from typing import Type, Any, Optional
 
 
 class XMLRPCClient(RPCClientBase):
     """
     An implementation of an XML RPC client.
 
     We can't do an all-encompassing doctest here, as it relies on an externally reachable server.
@@ -36,16 +38,16 @@
         b'<param><value><struct><member><value><boolean>0</boolean></value><name>bar</name></member></struct></value></param>'
 
         :param parameter object: Any value of the acceptable list of value types (see :class:`pibble.api.client.webservice.rpc.xmlrpc.XMLRPCClient`)
         :return lxml.etree._Element: The <parameter/> element.
         :raises pibble.api.exceptions.BadRequestError: When the parameter is not a known RPC type.
         """
 
-        def _format_parameter(value, name=None):
-            def _format_value(p):
+        def _format_parameter(value: Any, name: Optional[str] = None) -> ET._Element:
+            def _format_value(p: Any) -> ET._Element:
                 if isinstance(p, bool):
                     return E.value(E.boolean("1" if p else "0"))
                 elif isinstance(p, int):
                     return E.value(E.int(str(p)))
                 elif isinstance(p, str):
                     return E.value(E.string(p))
                 elif isinstance(p, bytes):
@@ -68,15 +70,15 @@
                     )
                 raise BadRequestError(
                     "Cannot encode type {0} into XMLRPC response.".format(
                         type(p).__name__
                     )
                 )
 
-            def _format_name(n):
+            def _format_name(n: Any) -> ET._Element:
                 return E.name(str(n))
 
             if name is not None:
                 return (_format_value(value), _format_name(name))
             return (_format_value(value),)
 
         return E.param(*_format_parameter(parameter))
@@ -171,15 +173,15 @@
         :raises pibble.api.exceptions.BadRequestError: When the type of the value is incorrect.
         """
 
         def parse_parameter(param_node: ET._Element) -> Any:
             value = param_node.find("value")
             value_node = value[0]
 
-            def _parse_value(value_node):
+            def _parse_value(value_node: ET._Element) -> Any:
                 if value_node.tag == "value":
                     return _parse_value(value_node[0])
                 elif value_node.tag == "int" or value_node.tag == "i4":
                     return int(value_node.text)
                 elif value_node.tag == "boolean":
                     return int(value_node.text) == 1
                 elif value_node.tag == "double":
```

### Comparing `pibble-0.4.9/pibble/api/client/webservice/soap.py` & `pibble-0.5.0/pibble/api/client/webservice/soap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 import lxml.etree as ET
 
-from typing import Callable, Any, Optional, Union
+from typing import Callable, Any, Optional, Union, Dict, List, cast
 from functools import partial
 from requests import Request, Response
 
 from zeep import Client
 from zeep.transports import Transport
 from zeep.wsdl.definitions import Operation, AbstractMessage
 
 from pibble.api.helpers.wrappers import RequestWrapper, ResponseWrapper
 from pibble.api.client.webservice.base import WebServiceAPIClientBase
 from pibble.util.helpers import url_join
 
 
 class SOAPError(Exception):
-    def __init__(self, response: Any):
+    def __init__(self, response: Union[Response, ResponseWrapper]) -> None:
         self.response = response
         super(Exception, self).__init__(self.response.text)
 
 
 class SOAPClient(WebServiceAPIClientBase):
     """
     A SOAP client using the Zeep library.
@@ -29,44 +29,44 @@
     break in using middleware if we so desire.
 
     :param wsdl str: The WSDL (web service description language) documentation as a URI.
     """
 
     soap: Client
 
-    def __init__(self):
+    def __init__(self) -> None:
         super(SOAPClient, self).__init__()
 
     def on_configure(self) -> None:
         host = self.configuration["client.host"]
         scheme = self.configuration.get("client.scheme", "http")
         port = int(
             self.configuration.get("client.port", 80 if scheme == "http" else 443)
         )
         path = self.configuration.get("client.path", "/")
         url = url_join("{0}://{1}:{2}/".format(scheme, host, port), path)
-        self.soap = Client(url, transport=SOAPClient.ZeepTransport(self))
+        self.soap = Client(url, transport=SOAPClient.ZeepTransport(self))  # type: ignore
 
     def _get_operation(self, method: str) -> Operation:
         """
         Gets an operation from the service.
 
         This returns the WSDL node that zeep retrieves.
 
         :param method str: The method name.
         :raises KeyError: When the operation is undefined.
         """
         for service in self.soap.wsdl.services.values():
             for port in service.ports.values():
                 for operation in port.binding._operations.values():
                     if operation.name == method:
-                        return operation
+                        return cast(Operation, operation)
         raise KeyError("Unknown or disallowed method {0}".format(method))
 
-    def listMethods(self) -> list[str]:
+    def listMethods(self) -> List[str]:
         """
         Lists methods in the service.
         """
         return [
             method
             for method in dir(self.soap.service)
             if not method.startswith("_")
@@ -77,23 +77,23 @@
         """
         Returns a string which shows input/output for a particular method.
 
         :param method str: The method name.
         :raises KeyError: When the operation is undefined.
         """
 
-        def elementHelp(name, element: ET._Element) -> str:
+        def elementHelp(name: str, element: ET._Element) -> str:
             if hasattr(element.type, "elements"):
                 return "{0} - {1}\n{2}".format(
                     name, element.type.name, elementsHelp(element.type.elements)
                 )
             else:
                 return "{0} - {1}".format(name, element.type)
 
-        def elementsHelp(elements: list[ET._Element], indent: int = 2) -> str:
+        def elementsHelp(elements: List[ET._Element], indent: int = 2) -> str:
             return "\n".join(
                 [
                     "\n".join(
                         [
                             "{0}{1}".format(" " * indent, line)
                             for line in elementHelp(name, element).splitlines()
                         ]
@@ -158,28 +158,28 @@
             raise SOAPError(response)
 
     class ZeepTransport(Transport):
         """
         A small extension of the zeep transport which includes middleware processing.
         """
 
-        def __init__(self, client: SOAPClient):
-            super(SOAPClient.ZeepTransport, self).__init__()
+        def __init__(self, client: SOAPClient) -> None:
+            super(SOAPClient.ZeepTransport, self).__init__()  # type: ignore
             self.client = client
 
         def get(
-            self, address: str, params: dict[str, Any], headers: dict[str, Any]
+            self, address: str, params: Dict[str, Any], headers: Dict[str, Any]
         ) -> Union[Response, ResponseWrapper]:
             try:
                 return self.client.get(address, parameters=params, headers=headers)
             except SOAPError as ex:
                 return ex.response
 
         def post(
-            self, address: str, message: AbstractMessage, headers: dict[str, Any]
+            self, address: str, message: AbstractMessage, headers: Dict[str, Any]
         ) -> Union[Response, ResponseWrapper]:
             try:
                 return self.client.post(address, data=message, headers=headers)
             except SOAPError as ex:
                 return ex.response
 
         def _load_remote_data(self, url: str) -> bytes:
```

### Comparing `pibble-0.4.9/pibble/api/client/webservice/wrapper.py` & `pibble-0.5.0/pibble/api/client/webservice/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
 
 class WebServiceAPILambdaClientSessionWrapper(SessionWrapper):
     """
     This session actually issues a lambda request to a docker container running a lambda app.
     """
 
-    def on_configure(self):
+    def on_configure(self) -> None:
         """
         On configure, build a client to the docker image.
         """
 
     def send(self, request: RequestWrapper, **kwargs: Any) -> ResponseWrapper:
         """
         Build a request to the lambda client.
```

### Comparing `pibble-0.4.9/pibble/api/client/wrapper.py` & `pibble-0.5.0/pibble/api/client/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/api/configuration.py` & `pibble-0.5.0/pibble/api/configuration.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/api/exceptions.py` & `pibble-0.5.0/pibble/api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 try:
     from thrift.Thrift import TApplicationException
 except ImportError:
     TApplicationException: Type = Exception  # type: ignore[no-redef]
 
 
-class ApacheThriftError(TApplicationException):
+class ApacheThriftError(TApplicationException):  # type: ignore
     """
     An exception wrapping around TApplicationExceptions, to pass up to the thrift server layer.
 
     :param cause Exception: The exception to wrap.
     """
 
     def __init__(self, cause: Exception):
```

### Comparing `pibble-0.4.9/pibble/api/helpers/apachethrift.py` & `pibble-0.5.0/pibble/api/helpers/apachethrift.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 from pibble.util.log import logger
 from pibble.util.strings import decode, encode
 from pibble.util.helpers import find_executable, resolve
 
 from thrift.transport import TTransport, TSocket
 from thrift.protocol import TBinaryProtocol
 
-from typing import Type, Optional, Any, Union
+from typing import Type, Optional, Any, Union, List
+from types import ModuleType
 
 
 class ApacheThriftHandler:
     """
     A meta class from which handlers should inherit.
 
     :param configuration pibble.api.configuration.APIConfiguration: The configuration. If passed as a dict, will be instantiated to APIConfiguration.
@@ -36,15 +37,15 @@
     def __init__(self, configuration: Union[dict, APIConfiguration]):
         if isinstance(configuration, dict):
             self.configuration = APIConfiguration(**configuration)
         else:
             self.configuration = configuration
 
 
-class ApacheThriftBufferedTransportFactory(TTransport.TBufferedTransportFactory):
+class ApacheThriftBufferedTransportFactory(TTransport.TBufferedTransportFactory):  # type: ignore
     """
     A small class that wraps around the buffered transport factory.
 
     The point of this is to retrieve the socket so we can do logic based on the local or remote
     address. Normally this is hidden to the handler.
 
     :param client thrift.TSocket.TSocket: The input/output socket used by the transport factory.
@@ -180,15 +181,15 @@
             )
             if not isinstance(response.response, ApacheThriftError):
                 raise ApacheThriftError(response.response)
             raise response.response
         return response.response
 
 
-class TTransitiveMemoryBuffer(TTransport.TTransportBase):
+class TTransitiveMemoryBuffer(TTransport.TTransportBase):  # type: ignore
     """
     A class for holding thrift messages in memory until read.
 
     Basically just a wrapper around a bytearray(). This is implemented
     because TMemoryBuffer() is read OR write, not both.
 
     >>> from pibble.api.helpers.apachethrift import TTransitiveMemoryBuffer
@@ -325,15 +326,15 @@
                     "Importing thrift IDL {0} namespace {1}".format(
                         self.thrift_file, self.namespace
                     )
                 )
                 sys.path.append(os.path.join(tmpdir, "gen-py"))
                 module = __import__(self.namespace, locals(), globals())
 
-                def recurse(module, fromlist=[]):
+                def recurse(module: ModuleType, fromlist: List[str] = []) -> None:
                     for submodule_name in getattr(module, "__all__", []):
                         logger.debug(
                             "Importing thrift IDL {0} namespace {1}".format(
                                 self.thrift_file,
                                 ".".join(fromlist + [module.__name__, submodule_name]),
                             )
                         )
@@ -437,10 +438,10 @@
             )
 
     class ApacheThriftServiceError:
         """
         Wraps around an error to keep track of when it happened.
         """
 
-        def __init__(self, error):
+        def __init__(self, error: str) -> None:
             self.error = error
             self.time = datetime.datetime.now()
```

### Comparing `pibble-0.4.9/pibble/api/helpers/authentication.py` & `pibble-0.5.0/pibble/api/helpers/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import sqlalchemy
 import binascii
 import os
 import hashlib
 import bcrypt
 
 try:
@@ -130,33 +132,33 @@
 
     def __getitem__(self, username: str) -> str:
         """
         Gets the password for a user.
 
         Not all implementations will provide a means for this (nor should they).
         """
-        return self.driver._getPassword(username)
+        return str(self.driver._getPassword(username))
 
 
 class APIAuthenticationSourceDriver:
     """
     A superclass that derived classes should inherit.
 
     Defines only one interface method, `validate(username, password)`, which
     returns True if valid, or false otherwise.
     """
 
-    def __init__(self, encryption: str, configuration: APIConfiguration):
+    def __init__(self, encryption: str, configuration: APIConfiguration) -> None:
         self.encryption = encryption
         self.configuration = configuration
 
     @staticmethod
     def get_implementation(
         CONFIGURATION_PREFIX: str, encryption: str, configuration: APIConfiguration
-    ):
+    ) -> APIAuthenticationSourceDriver:
         drivername = configuration["{0}.driver".format(CONFIGURATION_PREFIX)]
         for cls in APIAuthenticationSourceDriver.__subclasses__():
             if getattr(cls, "AUTHENTICATION_DRIVERNAME", None) == drivername:
                 return cls(encryption, configuration)
         raise ConfigurationError("Unknown authentication driver {0}".format(drivername))
 
     def _encryptPassword(self, password: str, stored: str) -> str:
@@ -164,15 +166,15 @@
         Encrypts a plaintext password based on the provided algorithm.
         """
         if self.encryption == "crypt":
             if os.name == "nt":
                 raise ConfigurationError("Crypt is not supported on Windows.")
             return crypt.crypt(password, stored)  # type: ignore
         else:
-            return getattr(hashlib, self.encryption)(encode(password)).hexdigest()
+            return str(getattr(hashlib, self.encryption)(encode(password)).hexdigest())
 
     def _comparePassword(self, username: str, password: str) -> bool:
         """
         Compares a password using the configured method.
         """
         try:
             stored = self._getPassword(username)
@@ -239,21 +241,21 @@
         self.engine = next(iter(self.factory[self.database_type]))
         self.metadata = sqlalchemy.MetaData(self.engine)
 
         self.table = sqlalchemy.Table(
             self.tablename, self.metadata, autoload=True, autoload_with=self.engine
         )
 
-    def _getPassword(self, username):
+    def _getPassword(self, username: str) -> str:
         row = self.engine.execute(
             self.table.select().where(self.table.c[self.username] == username)
         ).first()
         if not row:
             raise KeyError(f"Cannot find password for username {username}")
-        return row[self.password]
+        return str(row[self.password])
 
 
 class RSAKeyAuthenticationSourceDriver(APIAuthenticationSourceDriver):
     """
     RSA key check authentication.
 
     Optional configuration:
```

### Comparing `pibble-0.4.9/pibble/api/helpers/googlerpc.py` & `pibble-0.5.0/pibble/api/helpers/googlerpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,60 +2,72 @@
 
 import sys
 import os
 import tempfile
 import shutil
 import copy
 
-from typing import Optional, Type, Callable, Any, Iterator, Iterable, Union
+from typing import (
+    Optional,
+    Type,
+    Callable,
+    Any,
+    Iterator,
+    Iterable,
+    Union,
+    List,
+    Dict,
+    cast,
+)
 from types import ModuleType
 
 from google.protobuf import symbol_database as SDB
 from google.protobuf.message import Message
 
 from grpc_tools import protoc
 
 from pibble.util.log import logger
 from pibble.api.exceptions import ConfigurationError, UnsupportedMethodError
+from pibble.api.configuration import APIConfiguration
 
 
 class GRPCRequest:
-    fields: dict[str, Any]
+    fields: Dict[str, Any]
 
-    def __init__(self, service: GRPCService, method: str, **kwargs: Any):
+    def __init__(self, service: GRPCService, method: str, **kwargs: Any) -> None:
         self.service = service
         self.method = method
         for descriptor_method in self.service.descriptor.methods:
             if descriptor_method.name == self.method:
                 self.descriptor = descriptor_method
                 break
         if not hasattr(self, "descriptor"):
             raise UnsupportedMethodError("Unknown method '{0}'.".format(method))
         self.input = self.descriptor.input_type
         self.output = self.descriptor.output_type
         self.kwargs = kwargs
         self.fields = {}
 
     def __call__(self) -> Message:
-        return self.input._concrete_class(**self.fields)
+        return cast(Message, self.input._concrete_class(**self.fields))
 
 
 class GRPCResponse:
-    fields: dict[str, Any]
+    fields: Dict[str, Any]
 
-    def __init__(self, request: GRPCRequest):
+    def __init__(self, request: GRPCRequest) -> None:
         self.request = request
         self.fields = {}
 
-    def load(self, message):
+    def load(self, message: Any) -> None:
         for field in self.request.output.fields:
             self.fields[field.name] = getattr(message, field.name)
 
     def __call__(self) -> Message:
-        return self.request.output._concrete_class(**self.fields)
+        return cast(Message, self.request.output._concrete_class(**self.fields))
 
 
 class GRPCConfiguration:
     """
     Finally, this class reads an API configuration and appropriately retrieves the
     necessary parts of a service.
 
@@ -68,15 +80,15 @@
     Optional Configuration:
       - grpc.namespace - The namespace of the service. If not provided, the first service matching the service name will be taken. This can increase import time.
       - grpc.proto - The name of the .proto file that defines the service. When used in conjunction with namespace, this can greatly reduce searching time.
 
     :param configuration pibble.api.configuration.APIConfiguration: The API configuration.
     """
 
-    def __init__(self, configuration):
+    def __init__(self, configuration: APIConfiguration) -> None:
         self.configuration = configuration
 
         compile_directory = configuration.get("grpc.compile", None)
         directory = configuration.get("grpc.directory", None)
         service_name = configuration.get("grpc.service", None)
         service_namespace = configuration.get("grpc.namespace", None)
         service_proto = configuration.get("grpc.proto", None)
@@ -121,32 +133,32 @@
         qualified_name: str,
         name: str,
         namespace: str,
         descriptor: Any,
         servicer: Type,
         stub: Type,
         assigner: Callable,
-    ):
+    ) -> None:
         self.qualified_name = qualified_name
         self.name = name
         self.namespace = namespace
         self.descriptor = descriptor
         self.servicer = servicer
         self.assigner = assigner
         self.stub = stub
-        self.messages = GRPCService.GRPCMessages()
+        self.messages = GRPCService.GRPCMessages()  # type: ignore
 
-    def addMessage(self, message: Any) -> None:
+    def addMessage(self, message: Any) -> Any:
         """
         Adds messages to the message list after inspecting the descriptor for them.
 
         :param message `google.protobuf.pyext._message.MessageDescriptor`: the message description, compiled by protoc.
         """
         try:
-            added = self.messages.add(message)
+            added = self.messages.add(message)  # type: ignore
         except Exception as ex:
             raise AttributeError(
                 "Error adding message {0} to {1}: {2}".format(
                     message.name, self.name, str(ex)
                 )
             )
         if added:
@@ -156,55 +168,57 @@
         return added
 
     class GRPCMessages:
         """
         This class holds the message objects added to a service.
         """
 
-        def __init__(self):
+        messages: List[GRPCMessage]
+
+        def __init__(self) -> None:
             self.messages = []
 
-        def _find_by_name(self, name):
+        def _find_by_name(self, name: str) -> List[GRPCMessage]:
             """
             Finds by a name.
 
             :param str name: The name of the message to find.
             :returns list: All messages matching this name. It's possible to have multiple.
             :raises KeyError: When a message cannot be found.
             """
             messages = [message for message in self.messages if message.name == name]
             if not messages:
                 raise KeyError(name)
             return messages
 
-        def _find_by_qualified_name(self, qualified_name):
+        def _find_by_qualified_name(self, qualified_name: str) -> GRPCMessage:
             """
             Finds by a qualified name. Unlike `_find_by_name`, this can only have one result.
 
             :param str qualifier_name: The fully qualified message to find.
             :returns `pibble.api.helpers.googlerpc.GRPCService.GRPCMessages.GRPCMessage`: The message object.
             """
             for message in self.messages:
                 if message.qualified_name == qualified_name:
                     return message
             raise KeyError(qualified_name)
 
-        def get(self, name, namespace=None):
+        def get(self, name: str, namespace: Optional[str] = None) -> GRPCMessage:
             """
             Retrieves an item by name or qualified name.
 
             :param name str: The name. Required.
             :param namespace str: The namespace of the item. Optional.
             """
             if namespace is None:
                 return self[name]
             else:
                 return self._find_by_qualified_name("{0}.{1}".format(namespace, name))
 
-        def __getitem__(self, item):
+        def __getitem__(self, item: str) -> GRPCMessage:
             """
             Retrieves an unqualified message name.
 
             :param item str: The item name.
             :raises KeyError: When not found, or ambiguous.
             """
             message = self._find_by_name(item)
@@ -212,28 +226,28 @@
                 raise KeyError(
                     "Name {0} is ambiguous, use `.get()` instead and pass one of {1}.".format(
                         item, ", ".join([msg.namespace for msg in message])
                     )
                 )
             return message[0]
 
-        def __getattr__(self, item):
+        def __getattr__(self, item: str) -> GRPCMessage:
             """
             A wrapper around self[item].
             """
             try:
                 return self[item]
             except KeyError as ex:
                 raise AttributeError(str(ex))
 
-        def add(self, message):
+        def add(self, message: Any) -> bool:
             """
             Adds a message to this list. Called by the parent class.
             """
-            namespace = ".".join(os.path.splitext(message.file.name)[0].split("/"))
+            namespace = ".".join(os.path.splitext(message.file.name)[0].split("/"))  # type: ignore
             qualified_name = "{0}.{1}".format(namespace, message.name)
             try:
                 existing = self._find_by_qualified_name(qualified_name)
                 return False
             except KeyError:
                 self.messages.append(
                     GRPCService.GRPCMessages.GRPCMessage(self, message)
@@ -290,39 +304,39 @@
                         [
                             "{0} = {1}".format(name, usage)
                             for name, usage in field_descriptions
                         ]
                     ),
                 )
 
-            def __call__(self, *args, **kwargs) -> Any:
+            def __call__(self, *args: Any, **kwargs: Any) -> Any:
                 return self.cls(*args, **kwargs)
 
 
 class GRPCServiceExplorer:
     """
     This is the final destination of importing an entire gRPC module,
     i.e., a categorized and aliased list of the important services present
     within a gRPC module.
 
     :param module `pibble.api.helpers.googlerpc.GRPCModuleExplorer`: the module to search through.
     """
 
-    services: list[GRPCService]
+    services: List[GRPCService]
 
-    def __init__(self, module: GRPCModuleExplorer):
+    def __init__(self, module: GRPCModuleExplorer) -> None:
         self.module = module
         self.services = []
 
     def find(
         self,
         service_name: str,
         namespace: Optional[str] = "",
         proto: Optional[str] = None,
-    ):
+    ) -> GRPCService:
         """
         Finds a service by name.
 
         :param service_name str: The name of the service.
         :param namespace str: The namespace to search through. This can be empty, if it's not namespaced.
         :param proto_file str: The proto file, optional. If it is unknown, all proto files will be looked through.
         :returns `pibble.api.helpers.googlerpc.GRPCService`: The final imported service.
@@ -365,15 +379,15 @@
                         namespace,
                         proto_service,
                         getattr(imported, "{0}Servicer".format(name)),
                         getattr(imported, "{0}Stub".format(name)),
                         getattr(imported, "add_{0}Servicer_to_server".format(name)),
                     )
 
-                    def inspect_message(message):
+                    def inspect_message(message: Any) -> None:
                         if grpc_service.addMessage(message):
                             for field in message.fields:
                                 if field.message_type:
                                     inspect_message(field.message_type)
 
                     for method in proto_service.methods:
                         if method.input_type:
@@ -396,15 +410,15 @@
 class GRPCModule:
     """
     This class holds a module, including its path and fromlist.
 
     It is not actually imported until the `.module()` function is called.
     """
 
-    def __init__(self, name: str, fromlist: list[str]):
+    def __init__(self, name: str, fromlist: List[str]):
         self.name = name
         self.fromlist = fromlist
 
         if self.name.endswith("pb2"):
             self.proto = "_".join(name.split("_")[:-1])
         elif self.name.endswith("pb2_grpc"):
             self.proto = "_".join(name.split("_")[:-2])
@@ -438,18 +452,18 @@
 class GRPCModuleExplorer:
     """
     This class holds all modules and submodules represented in a gRPC module.
 
     Submodules are, in turn, also GRPCModules, allowing for chaining of __getattr__ calls.
     """
 
-    modules: dict[str, GRPCModule]
-    submodules: dict[str, GRPCModuleExplorer]
+    modules: Dict[str, GRPCModule]
+    submodules: Dict[str, GRPCModuleExplorer]
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.modules = {}
         self.submodules = {}
 
     def find(self, path: str) -> Union[GRPCModule, GRPCModuleExplorer]:
         """
         Finds a module by dot-separated path.
 
@@ -459,15 +473,15 @@
         if len(path_parts) == 1:
             return self[path]
         result = self[path_parts[0]]
         if not isinstance(result, GRPCModuleExplorer):
             raise TypeError(f"{path} is a module, not a submodule.")
         return result.find(".".join(path_parts[1:]))
 
-    def add(self, path: str, fromlist: list[str] = []):
+    def add(self, path: str, fromlist: List[str] = []) -> None:
         """
         This adds a .py file from the module into this object.
 
         This is invoking the __import__ machinery, and likely shouldn't be used except when
         being called from GRPCImporter.module.
 
         :param path str: The path of this file.
@@ -561,15 +575,17 @@
     def __enter__(self) -> GRPCModuleExplorer:
         logger.info("Recursively importing gRPC Module at {0}".format(self.directory))
         self.path = copy.deepcopy(sys.path)
         sys.path.append(self.directory)
 
         module = GRPCModuleExplorer()
 
-        def recurse(module, path, fromlist=[]):
+        def recurse(
+            module: GRPCModuleExplorer, path: str, fromlist: List[str] = []
+        ) -> None:
             for subpath in os.listdir(path):
                 if os.path.isdir(os.path.join(path, subpath)):
                     recurse(
                         module.submodule(subpath),
                         os.path.join(path, subpath),
                         fromlist + [subpath],
                     )
```

### Comparing `pibble-0.4.9/pibble/api/helpers/store.py` & `pibble-0.5.0/pibble/api/helpers/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import sqlalchemy
 
 from pibble.database.engine import EngineFactory
 from pibble.database.util import row_to_dict
 from pibble.api.exceptions import ConfigurationError
 from pibble.api.configuration import APIConfiguration
-from pibble.util.strings import FlexibleStringer
+from pibble.util.strings import Serializer
 from pibble.util.helpers import resolve
 from pibble.util.log import logger
 
-from typing import Any, Callable
+from typing import Any, Callable, Optional, Dict
 
 
 class NoDefaultProvided:
     pass
 
 
 class APISessionStore:
@@ -27,29 +27,29 @@
     In general, this should NOT be used to store or retrieve data relevant to the actual service being provided, and should simply store metadata.
 
     Required configuration:
       1. ``session.store.driver``: The driver type.
 
     Optional configuration:
       2. ``session.store.scope``: A scope value. Defaults to None.
-      3. ``session.store.serializer``: How values are serialized. Defaults to ``FlexibleStringer.serialize``.
-      4. ``session.store.deserializer``: How values are deserialized. Defaults to ``FlexibleStringer.deserialize``.
+      3. ``session.store.serializer``: How values are serialized. Defaults to ``Serializer.serialize``.
+      4. ``session.store.deserializer``: How values are deserialized. Defaults to ``Serializer.deserialize``.
 
     :param configuration pibble.api.configuration.APIConfiguration: The configuration for the server or client.
     """
 
     CONFIGURATION_PREFIX = "session.store"
 
     def __init__(self, configuration: APIConfiguration):
         self.serializer = configuration.get(
             "{0}.serializer".format(self.CONFIGURATION_PREFIX),
-            FlexibleStringer.serialize,
+            Serializer.serialize,
         )
         self.deserializer = configuration.get(
-            "{0}.deserializer".format(self.CONFIGURATION_PREFIX), FlexibleStringer.parse
+            "{0}.deserializer".format(self.CONFIGURATION_PREFIX), Serializer.deserialize
         )
         self.scope = configuration.get(
             "{0}.scope".format(self.CONFIGURATION_PREFIX), None
         )
 
         if self.scope is None:
             self.scope = "null"
@@ -191,33 +191,39 @@
 
 
 class UnconfiguredAPISessionStore(APISessionStore):
     """
     A session store for non-configured APIs.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.driver = MemoryAPISessionStore(None, None)
 
 
 class APISessionStoreDriver:
     """
     An extendable class for session stores.
 
     Implemented classes ***must*** override the ``get(key)`` and ``set(key, value)`` functions.
     Implementing classes ***must*** set the DRIVERNAME class variable.
     """
 
     DRIVERNAME = ""
 
-    def __init__(self, configuration_prefix: str, configuration: APIConfiguration):
+    def __init__(
+        self,
+        configuration_prefix: Optional[str],
+        configuration: Optional[APIConfiguration],
+    ) -> None:
         self.configuration_prefix = configuration_prefix
         self.configuration = configuration
 
     def get_configuration(self, key: str, default: Any = NoDefaultProvided()) -> Any:
+        if self.configuration is None:
+            raise KeyError("Unconfigured session store.")
         result = self.configuration.get(f"{self.configuration_prefix}.{key}", default)
         if isinstance(result, NoDefaultProvided):
             raise KeyError(key)
         return result
 
     @staticmethod
     def get_implementation(
@@ -274,15 +280,19 @@
         Does nothing.
         """
 
 
 class DatabaseAPISessionStore(APISessionStoreDriver):
     DRIVERNAME = "database"
 
-    def __init__(self, configuration_prefix: str, configuration: APIConfiguration):
+    def __init__(
+        self,
+        configuration_prefix: Optional[str],
+        configuration: Optional[APIConfiguration],
+    ) -> None:
         """
         A driver for database-backed session stores.
 
         Required configuration:
           1. ``session.store.database.type`` The database type - sqlite, postgresql, mssql, etc.
           2. ``session.store.database.connection`` The connection parameters. See :class:``pibble.database.engine.EngineFactory``.
           3. ``session.store.database.table`` The tablename to select from.
@@ -319,15 +329,15 @@
                 self.metadata,
                 sqlalchemy.Column(self.scope, sqlalchemy.String(32), primary_key=True),
                 sqlalchemy.Column(self.key, sqlalchemy.String(32), primary_key=True),
                 sqlalchemy.Column(self.value, sqlalchemy.String(512)),
             )
             self.metadata.create_all()
 
-    def _where(self, scope: str, key: str):
+    def _where(self, scope: str, key: str) -> Any:
         return sqlalchemy.and_(
             self.table.c[self.key] == key, self.table.c[self.scope] == scope
         )
 
     def get(self, scope: str, key: str) -> Any:
         row = self.engine.execute(
             self.table.select().where(self._where(scope, key))
@@ -362,17 +372,21 @@
 
 class MemoryAPISessionStore(APISessionStoreDriver):
     """
     An implementation for storing data in memory. Uses a simple dictionary.
     """
 
     DRIVERNAME = "memory"
-    memory: dict[str, dict[str, Any]]
+    memory: Dict[str, Dict[str, Any]]
 
-    def __init__(self, configuration_prefix: str, configuration: APIConfiguration):
+    def __init__(
+        self,
+        configuration_prefix: Optional[str],
+        configuration: Optional[APIConfiguration],
+    ) -> None:
         super(MemoryAPISessionStore, self).__init__(configuration_prefix, configuration)
         self.memory = {}
 
     def get(self, scope: str, key: str) -> Any:
         return self.memory[scope][key]
 
     def set(self, scope: str, key: str, value: Any) -> None:
```

### Comparing `pibble-0.4.9/pibble/api/helpers/wrappers.py` & `pibble-0.5.0/pibble/api/helpers/wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 import json
 import zlib
 import tempfile
 import datetime
 
-from typing import Any, Union, Iterator, Optional, Literal
+from typing import Any, Union, Iterator, Optional, Literal, List
 from urllib.parse import urlencode
 from http.cookies import SimpleCookie
 
 from pibble.api.client.base import APIClientBase
 from pibble.api.server.base import APIServerBase
 from pibble.util.strings import decode, encode, parse_url_encoded, parse_multipart
 from pibble.util.helpers import (
@@ -30,31 +30,31 @@
     pass
 
 
 class POSTWrapper:
     """
     Used for the request.POST wrapper provided by webob.
 
-    >>> wrapper = POSTWrapper('email=benjamin%40pibbledata.com&password=mypassword')
+    >>> wrapper = POSTWrapper('email=benjamin%40pibble.com&password=mypassword')
     >>> wrapper['email']
-    'benjamin@pibbledata.com'
+    'benjamin@pibble.com'
     >>> wrapper['password']
     'mypassword'
     """
 
     def __init__(self, body: str, content_type: Optional[str] = None):
         self.body = body
         if content_type is not None and "json" in content_type:
             self.decoded = json.loads(body, cls=FlexibleJSONDecoder)
         elif content_type is not None and "multi" in content_type:
             self.decoded = parse_multipart(f"Content-Type: {content_type}\r\n{body}")
         else:
             self.decoded = parse_url_encoded(body)
 
-    def __getitem__(self, key: str) -> str:
+    def __getitem__(self, key: str) -> Any:
         """
         Allows for POST[x] calls.
         """
         if isinstance(self.decoded, dict):
             return self.decoded[key]
         raise ValueError("No key-value pairs present.")
 
@@ -71,15 +71,15 @@
         """
         Allows for 'x in POST' calls.
         """
         if not isinstance(self.decoded, dict):
             raise ValueError("No key-value pairs present.")
         return key in self.decoded
 
-    def get(self, key: str, default: Any = NoDefault) -> str:
+    def get(self, key: str, default: Any = NoDefault) -> Any:
         """
         Allows a dict-list .get().
         """
         try:
             return self[key]
         except KeyError:
             if default is NoDefault:
@@ -250,15 +250,15 @@
         if getattr(self, "client", None) is not None:
             base = getattr(self.client, "base", "")
             if self.url.startswith(base):
                 return self.url[len(base) :]
         return self.url
 
     @property
-    def content_type(self) -> Optional[str]:
+    def content_type(self) -> Any:
         """
         Gets the content-type header.
         """
         return self.headers.get("content-type", None)
 
     @property
     def content_length(self) -> int:
@@ -283,15 +283,15 @@
     client: Optional[APIClientBase]
     server: Optional[APIServerBase]
     status_code: int
     headers: CaseInsensitiveDict
     content_length: int
     app_iter: Iterator[bytes]  # server sending response
     body: bytes
-    content_cache: list[bytes]
+    content_cache: List[bytes]
 
     def __init__(self) -> None:
         self.headers = CaseInsensitiveDict()
         self.content_cache = []
 
     def iter_content(self, chunk_size: int = 8192) -> Iterator[bytes]:
         """
@@ -387,40 +387,40 @@
         if hasattr(self, "body"):
             return self.body
         elif hasattr(self, "app_iter"):
             return b"".join([chunk for chunk in self.iter_content()])
         return b""
 
     @property
-    def content_type(self) -> Optional[str]:
+    def content_type(self) -> Any:
         return self.headers.get("content-type", None)
 
     @content_type.setter
     def content_type(self, new_content_type: str) -> None:
         self.headers["content-type"] = new_content_type
 
     @property
-    def content_encoding(self) -> Optional[str]:
+    def content_encoding(self) -> Any:
         return self.headers.get("content-encoding", None)
 
     @content_encoding.setter
     def content_encoding(self, new_content_encoding: str) -> None:
         self.headers["content-encoding"] = new_content_encoding
 
     @property
-    def location(self) -> Optional[str]:
+    def location(self) -> Any:
         return self.headers.get("location", None)
 
     @location.setter
     def location(self, new_location: str) -> None:
         self.headers["location"] = new_location
 
     def json(self) -> Any:
         """
-        Loads the text as JSON. Doesn't use the FlexibleStringer, since this is
+        Loads the text as JSON. Doesn't use the Serializer, since this is
         emulating a requests.Response in this context.
         """
         return json.loads(self.text)
 
     def __str__(self) -> str:
         stringified = f"ResponseWrapper<{self.status_code}>"
         if self.status_code < 400:
```

### Comparing `pibble-0.4.9/pibble/api/meta/base.py` & `pibble-0.5.0/pibble/api/meta/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,23 @@
+from __future__ import annotations
+
 from re import sub
 from functools import partial
-from typing import Type, Callable, Any, Optional, Sequence, Mapping, Union, cast
+from typing import (
+    Type,
+    Callable,
+    Any,
+    Optional,
+    Sequence,
+    Mapping,
+    Union,
+    Dict,
+    List,
+    cast,
+)
 
 from pibble.api.base import APIBase
 from pibble.api.server.webservice.base import MethodBasedWebServiceAPIServerBase
 from pibble.util.helpers import resolve
 
 
 class MetaTestClass:
@@ -134,15 +147,15 @@
 
     @instance.deleter
     def instance(self) -> None:
         if self._class_instance is not None:
             self._class_instance.destroy()
             self._class_instance = None
 
-    def listMethods(self) -> list[str]:
+    def listMethods(self) -> List[str]:
         """
         Lists methods in the underlying layer.
         """
         functions = [func for func in self.functions.keys()]
         has_list_methods = getattr(self.instance, "listMethods", None) is not None
         if has_list_methods:
             try:
@@ -198,15 +211,17 @@
 class MetaServiceFactory:
     """
     The MetaServiceFactory simply stores and creates metaservices.
 
     See :class:`pibble.api.meta.base.MetaService` for more information.
     """
 
-    def __init__(self):
+    services: Dict[str, MetaService]
+
+    def __init__(self) -> None:
         self.services = {}
 
     def __getattr__(self, name: str) -> MetaService:
         """
         A helpful syntax for getting services.
 
         >>> from pibble.api.meta.base import MetaServiceFactory
@@ -218,17 +233,17 @@
         """
 
         return self.services[name]
 
     def define(
         self,
         name: str,
-        classes: list[Union[Type, str]],
+        classes: List[Union[Type, str]],
         configuration: dict = {},
-        functions: dict[str, Callable] = {},
+        functions: Dict[str, Callable] = {},
     ) -> MetaService:
         """
         Defines a service.
 
         >>> from pibble.api.meta.base import MetaServiceFactory
         >>> factory = MetaServiceFactory()
         >>> factory.define("myclass", ["pibble.api.base.APIBase", "pibble.api.meta.base.MetaTestClass"])
```

### Comparing `pibble-0.4.9/pibble/api/meta/helpers.py` & `pibble-0.5.0/pibble/api/meta/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import os
 
 from pibble.util.files import load_yaml, load_json
-from pibble.util.strings import FlexibleStringer
+from pibble.util.strings import Serializer
 
 from pibble.api.configuration import APIConfiguration
 from pibble.api.meta.base import MetaService, MetaFunction
 
 __all__ = ["MetaFactory"]
 
 
@@ -21,15 +21,15 @@
     :raises IOError: When there is an issue reading the configuration file.
     """
 
     def __init__(self, configuration: dict):
         if "configuration" not in configuration:
             raise KeyError("Missing keyword 'configuration.'")
 
-        self.configuration = FlexibleStringer.parse(configuration)
+        self.configuration = Serializer.deserialize(configuration)
         if "cwd" not in self.configuration:
             self.configuration["cwd"] = os.getcwd()
         self.api_configuration = APIConfiguration(**self.configuration["configuration"])
 
     @staticmethod
     def from_file(configuration_file: str) -> MetaFactory:
         """
```

### Comparing `pibble-0.4.9/pibble/api/middleware/apachethrift/base.py` & `pibble-0.5.0/pibble/api/middleware/apachethrift/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/api/middleware/apachethrift/screening.py` & `pibble-0.5.0/pibble/api/middleware/apachethrift/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/api/middleware/database/orm.py` & `pibble-0.5.0/pibble/api/middleware/database/orm.py`

 * *Files 17% similar despite different names*

```diff
@@ -47,15 +47,22 @@
         Either open or a close a database session, depending on client or server.
         """
         if hasattr(self, "orm"):
             if isinstance(request, RequestsRequest):
                 # Client parsing a response, close database
                 if hasattr(self, "database"):
                     logger.debug("Closing client ORM session.")
-                    self.database.close()
+                    try:
+                        self.database.close()
+                    except Exception as ex:
+                        logger.debug(
+                            "Ignoring exception during database close {0}: {1}".format(
+                                type(ex).__name__, ex
+                            )
+                        )
             elif isinstance(request, WebobRequest) or isinstance(
                 request, RequestWrapper
             ):
                 # Server parsing a request, open database
                 logger.debug("Opening server ORM session.")
                 self.database = self.orm.session(expire_on_commit=False)
 
@@ -76,8 +83,15 @@
                 self.database = self.orm.session(expire_on_commit=False)
             elif isinstance(request, WebobRequest) or isinstance(
                 request, RequestWrapper
             ):
                 # Server preparing a response, close database
                 if hasattr(self, "database"):
                     logger.debug("Closing server ORM session.")
-                    self.database.close()
+                    try:
+                        self.database.close()
+                    except Exception as ex:
+                        logger.debug(
+                            "Ignoring exception during database close {0}: {1}".format(
+                                type(ex).__name__, ex
+                            )
+                        )
```

### Comparing `pibble-0.4.9/pibble/api/middleware/googlerpc/authentication.py` & `pibble-0.5.0/pibble/api/middleware/googlerpc/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/api/middleware/googlerpc/base.py` & `pibble-0.5.0/pibble/api/middleware/googlerpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/api/middleware/googlerpc/metadata.py` & `pibble-0.5.0/pibble/api/middleware/googlerpc/metadata.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/api/middleware/webservice/authentication/basic.py` & `pibble-0.5.0/pibble/api/middleware/webservice/authentication/basic.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/api/middleware/webservice/authentication/bearer.py` & `pibble-0.5.0/pibble/api/middleware/webservice/authentication/bearer.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/api/middleware/webservice/authentication/digest.py` & `pibble-0.5.0/pibble/api/middleware/webservice/authentication/digest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import datetime
 import uuid
 import hashlib
 
-from typing import Optional, Union
+from typing import Optional, Union, List
 
 from webob import (
     Request as WebobRequest,
     Response as WebobResponse,
 )
 from requests import (
     Request as RequestsRequest,
@@ -261,15 +261,15 @@
     """
     A class to hold a list of nonces.
 
     :param ttl int: The time a nonce is valid, in seconds.
     :param max_uses int: The number of times a nonce can be used before a new one must be generated.
     """
 
-    nonces: list[NonceList.Nonce]
+    nonces: List[NonceList.Nonce]
 
     def __init__(self, ttl: int = 60 * 60 * 24, max_uses: int = 25):
         self.ttl = ttl
         self.max_uses = max_uses
         self.nonces = []
 
     def clear(self) -> None:
```

### Comparing `pibble-0.4.9/pibble/api/middleware/webservice/authentication/header.py` & `pibble-0.5.0/pibble/api/middleware/webservice/authentication/header.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/api/middleware/webservice/authentication/oauth.py` & `pibble-0.5.0/pibble/api/middleware/webservice/authentication/oauth.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from pibble.api.helpers.store import APISessionStore
 
 from pibble.api.exceptions import (
     AuthorizationError,
     ConfigurationError,
 )
 
-from pibble.util.strings import FlexibleStringer
+from pibble.util.strings import Serializer
 from pibble.util.log import logger
 
 
 class OAuthAuthenticationMiddleware(WebServiceAPIMiddlewareBase):
     """
     Middleware for OAuth authentication.
 
@@ -249,15 +249,15 @@
             refresh_token = self.session.get("oauth_refresh_token", None)
             expires_at = self.session.get(
                 "oauth_expires_at",
                 datetime.datetime.now() - datetime.timedelta(seconds=30),
             )
 
             if not isinstance(expires_at, datetime.datetime):
-                expires_at = FlexibleStringer.parse(expires_at)
+                expires_at = Serializer.deserialize(expires_at)
 
             if expires_at <= datetime.datetime.now() and refresh_token:
                 logger.debug("OAuth2 (authorization_code) expired, refreshing.")
                 refreshed = self.requests_session.refresh_token(
                     self.configuration.get("authentication.oauth.refresh_url", None),
                     client_id=self.configuration["authentication.oauth.client_id"],
                     client_secret=self.configuration[
@@ -326,15 +326,15 @@
             token_type = self.session.get("oauth_token_type", "Bearer")
             expires_at = self.session.get(
                 "oauth_expires_at",
                 datetime.datetime.now() - datetime.timedelta(seconds=30),
             )
 
             if not isinstance(expires_at, datetime.datetime):
-                expires_at = FlexibleStringer.parse(expires_at)
+                expires_at = Serializer.deserialize(expires_at)
             expires_in = int((expires_at - datetime.datetime.now()).total_seconds())
 
             if access_token is not None:
                 logger.info(
                     "OAuth2 (authorization_code) found stored access information, will set authentication to re-use credentials."
                 )
 
@@ -376,15 +376,15 @@
                 )
             )
             self.session["oauth_state"] = 0
             return self.OAuth2ClientWebAuthentication(request, response)
 
     def OAuth2ClientLegacyAuthentication(
         self, request: RequestsRequest, response: RequestsResponse
-    ):
+    ) -> None:
         """
         OAuth2 Legacy (password) authentication flow.
 
         No states.
         """
 
         if type(self.requests_session) is not OAuth2Session:
@@ -401,15 +401,15 @@
                 password=self.configuration["authentication.oauth.password"],
                 client_id=self.configuration["authentication.oauth.client_id"],
                 client_secret=self.configuration["authentication.oauth.client_secret"],
             )
 
     def OAuth2ClientBackendAuthentication(
         self, request: RequestsRequest, response: RequestsResponse
-    ):
+    ) -> None:
         """
         OAuth Backend (client_credentials) authentication flow.
         """
         if type(self.requests_session) is not OAuth2Session:
             logger.info("OAuth2 (client_credentials) initialization authentication.")
             self.requests_session = OAuth2Session(
                 client=BackendApplicationClient(
@@ -434,12 +434,12 @@
         if "refresh_token" in token:
             self.session["oauth_refresh_token"] = token["refresh_token"]
 
     def GetOAuthTokenData(self) -> dict:
         return {
             "access_token": self.session.get("oauth_access_token", None),
             "token_type": self.session.get("oauth_token_type", None),
-            "expires_at": FlexibleStringer.parse(
+            "expires_at": Serializer.deserialize(
                 self.session.get("oauth_expires_at", None)
             ),
             "refresh_token": self.session.get("oauth_refresh_token", None),
         }
```

### Comparing `pibble-0.4.9/pibble/api/middleware/webservice/base.py` & `pibble-0.5.0/pibble/api/middleware/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/api/middleware/webservice/limit.py` & `pibble-0.5.0/pibble/api/middleware/webservice/limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
 
     rate_reset: datetime.datetime
     rate_quota: int
     rate_limit: int
     rate_period: int
 
-    def on_configure(self):
+    def on_configure(self) -> None:
         """
         On configuration, initialize rate quotas.
         """
         self.rate_limit = self.configuration.get("server.rate.limit", 60)
         self.rate_period = self.configuration.get("server.rate.period", 60)
 
     def parse(
```

### Comparing `pibble-0.4.9/pibble/api/middleware/webservice/screening.py` & `pibble-0.5.0/pibble/api/middleware/webservice/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/api/protocol/apachethrift.py` & `pibble-0.5.0/pibble/api/protocol/apachethrift.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# type: ignore
 #
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements. See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership. The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
```

### Comparing `pibble-0.4.9/pibble/api/server/apachethrift.py` & `pibble-0.5.0/pibble/api/server/apachethrift.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     See :class:`pibble.api.helpers.thrift.ApacheThriftService` for required arguments for the thrift service.
     """
 
     SIMPLE = 0
     THREADED = 1
     FORKING = 2
 
-    def __init__(self):
+    def __init__(self) -> None:
         super(ApacheThriftServer, self).__init__()
 
     def on_configure(self) -> None:
         """
         Builds the server.
         """
```

### Comparing `pibble-0.4.9/pibble/api/server/base.py` & `pibble-0.5.0/pibble/api/server/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,73 @@
+from __future__ import annotations
+
 from multiprocessing import Process
 from pibble.api.base import APIBase
 from pibble.util.helpers import Pause
 from pibble.util.log import logger
 
 
 class APIServerProcess(Process):
     """
     A small class that will run the server process in the background.
     """
 
-    def __init__(self, server):
+    def __init__(self, server: APIServerBase) -> None:
         super(APIServerProcess, self).__init__()
         self.server = server
 
-    def run(self):
+    def run(self) -> None:
         try:
             self.server.serve()
         except Exception as ex:
             logger.critical("{0}(): {1}".format(type(ex).__name__, str(ex)))
             raise
 
 
 class APIServerBase(APIBase):
     """
     A base server class, from which all server implementations will inherit.
     """
 
-    def __init__(self):
+    _process: APIServerProcess
+
+    def __init__(self) -> None:
         super(APIServerBase, self).__init__()
 
-    def serve(self):
+    def serve(self) -> None:
         """
         The main serve() method will _synchronously_ perform the server functions.
 
         There is no base serving ability, so implementing classes _must_ override this.
         """
         raise NotImplementedError()
 
-    def running(self):
+    def running(self) -> bool:
         """
         Determines if the server is currently running (when used asynchronously.)
         """
         return hasattr(self, "_process") and self._process.is_alive()
 
-    def start(self):
+    def start(self) -> None:
         """
         Starts the server, which will serve asynchronously.
         """
-        if getattr(self, "_process", None) is not None:
+        if hasattr(self, "_process"):
             if self._process.is_alive():
                 logger.warning(
                     "start() was called while process is still alive. Ignoring."
                 )
                 return
-            self._process = None
+            del self._process
         self._process = APIServerProcess(self)
         self._process.start()
         Pause.milliseconds(250)
 
-    def stop(self):
+    def stop(self) -> None:
         """
         Stops the server.
         """
-        if getattr(self, "_process", None) is not None:
+        if hasattr(self, "_process"):
             self._process.terminate()
             self._process.join()
             self._process.close()
-            self._process = None
+            del self._process
```

### Comparing `pibble-0.4.9/pibble/api/server/file/ftp.py` & `pibble-0.5.0/pibble/api/server/file/ftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/api/server/file/sftp.py` & `pibble-0.5.0/pibble/api/server/file/sftp.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,57 +14,57 @@
     SFTPServer as ParamikoSFTPServer,
     SFTPHandle as ParamikoSFTPHandle,
     SFTPAttributes,
     RSAKey,
     Transport,
 )
 
-from typing import Callable, Any, Union
+from typing import Callable, Any, Union, Optional, List
 
 from pibble.util.log import logger
 from pibble.api.server.base import APIServerBase
 from pibble.api.exceptions import AuthenticationError
 from pibble.api.configuration import APIConfiguration
 from pibble.api.helpers.authentication import APIAuthenticationSource
 
 
 class SFTPRequest:
     """
     A wrapper around each request for processing.
     """
 
-    def __init__(self, server: APIServerBase, fn: Callable, *args: Any):
+    def __init__(self, server: APIServerBase, fn: Callable, *args: Any) -> None:
         self.server = server
         self.fn = fn
         self.args = args
 
     def __call__(self) -> Any:
         return self.fn(self.server, *self.args)
 
 
 class SFTPResponse:
     """
     A wrapper around each response for processing.
     """
 
-    def __init__(self, request, response):
+    def __init__(self, request: Any, response: Any) -> None:
         self.request = request
         self.response = response
 
-    def __call__(self):
+    def __call__(self) -> Any:
         return self.response
 
 
 class SFTPProcessor:
     """
     A wrapper around requests and responses for processing.
     """
 
     def wrap(self, fn: Callable) -> Callable:
-        def wrapper(stub, *args: Any):
+        def wrapper(stub: Any, *args: Any) -> Any:
             request = SFTPRequest(stub, fn, *args)
             stub.server.server.parse_all(request)
             response = SFTPResponse(request, request())
             stub.server.server.prepare_all(response)
             return response()
 
         return wrapper
@@ -75,15 +75,18 @@
     This is the server instantiated for the paramiko transport.
 
     Adapted from https://github.com/rspivak/sftpserver
 
     See :class:pibble.api.server.file.sftp.ParamikoSFTPServer for more information.
     """
 
-    def __init__(self, server):
+    publickey: Optional[APIAuthenticationSource]
+    password: Optional[APIAuthenticationSource]
+
+    def __init__(self, server: Any) -> None:
         super(StubServer, self).__init__()
         self.server = server
         self.configuration = self.server.configuration
         if isinstance(self.configuration.get("authentication.driver", None), list):
             if "rsa" in self.configuration["authentication.driver"]:
                 rsa_configuration = APIConfiguration(
                     authentication=self.configuration["authentication"]
@@ -112,33 +115,33 @@
         allowed = []
         if self.publickey is not None:
             allowed.append("publickey")
         if self.password is not None:
             allowed.append("password")
         return ",".join(allowed)
 
-    def check_auth_publickey(self, username: str, key) -> int:
+    def check_auth_publickey(self, username: str, key: Any) -> Any:
         if self.publickey is not None:
             try:
                 self.publickey.validate(username, key)
                 return AUTH_SUCCESSFUL
             except AuthenticationError:
                 pass
         return AUTH_FAILED
 
-    def check_auth_password(self, username: str, password: str) -> int:
+    def check_auth_password(self, username: str, password: str) -> Any:
         if self.password is not None:
             try:
                 self.password.validate(username, password)
                 return AUTH_SUCCESSFUL
             except AuthenticationError:
                 pass
         return AUTH_FAILED
 
-    def check_channel_request(self, kind: Any, chanid: int) -> int:
+    def check_channel_request(self, kind: Any, chanid: int) -> Any:
         return OPEN_SUCCEEDED
 
 
 class SFTPStubHandler(ParamikoSFTPHandle):
     """
     This is the handler instantiated for the paramiko transport.
 
@@ -149,15 +152,15 @@
 
     def stat(self) -> Union[SFTPAttributes, int]:
         try:
             return SFTPAttributes.from_stat(os.fstat(self.readfile.fileno()))  # type: ignore
         except OSError as e:
             return ParamikoSFTPServer.convert_errno(e.errno)
 
-    def chattr(self, attr: Union[SFTPAttributes, int]) -> int:
+    def chattr(self, attr: Union[SFTPAttributes, int]) -> Any:
         try:
             ParamikoSFTPServer.set_file_attr(self.filename, attr)  # type: ignore
             return SFTP_OK
         except OSError as e:
             return ParamikoSFTPServer.convert_errno(e.errno)
 
 
@@ -169,15 +172,15 @@
 
     See :class:pibble.api.server.file.sftp.ParamikoSFTPServer for more information.
     """
 
     processor = SFTPProcessor()
     _root = os.getcwd()
 
-    def __init__(self, server):
+    def __init__(self, server: Any) -> None:
         super(SFTPStubServer, self).__init__(server)
         self.server = server
         self._root = server.configuration.get("server.sftp.root.directory", os.getcwd())
         self._relative = server.configuration.get("server.sftp.root.relative", True)
 
     def _realpath(self, path: str) -> str:
         if os.path.isabs(path) and not self._relative:
@@ -185,15 +188,15 @@
         else:
             _path = os.path.join(self._root, self.canonicalize(path.strip("/")))
         if os.path.commonprefix([self._root, _path]) != self._root:
             raise OSError(errno.EACCES, "Access denied.")
         return _path
 
     @processor.wrap
-    def list_folder(self, path: str) -> Union[list[SFTPAttributes], int]:
+    def list_folder(self, path: str) -> Union[List[SFTPAttributes], int]:
         try:
             path = self._realpath(path)
             out = []
             flist = os.listdir(path)
             for fname in flist:
                 attr = SFTPAttributes.from_stat(os.stat(os.path.join(path, fname)))
                 attr.filename = fname
@@ -255,63 +258,63 @@
         fobj = SFTPStubHandler(flags)
         fobj.filename = path  # type: ignore
         fobj.readfile = f  # type: ignore
         fobj.writefile = f  # type: ignore
         return fobj
 
     @processor.wrap
-    def remove(self, path: str) -> int:
+    def remove(self, path: str) -> Any:
         try:
             path = self._realpath(path)
             os.remove(path)
         except OSError as e:
             return ParamikoSFTPServer.convert_errno(e.errno)
         return SFTP_OK
 
     @processor.wrap
-    def rename(self, oldpath: str, newpath: str) -> int:
+    def rename(self, oldpath: str, newpath: str) -> Any:
         try:
             oldpath = self._realpath(oldpath)
             newpath = self._realpath(newpath)
             os.rename(oldpath, newpath)
         except OSError as e:
             return ParamikoSFTPServer.convert_errno(e.errno)
         return SFTP_OK
 
     @processor.wrap
-    def mkdir(self, path: str, attr: SFTPAttributes) -> int:
+    def mkdir(self, path: str, attr: SFTPAttributes) -> Any:
         try:
             path = self._realpath(path)
             os.mkdir(path)
             if attr is not None:
                 ParamikoSFTPServer.set_file_attr(path, attr)
         except OSError as e:
             return ParamikoSFTPServer.convert_errno(e.errno)
         return SFTP_OK
 
     @processor.wrap
-    def rmdir(self, path: str) -> int:
+    def rmdir(self, path: str) -> Any:
         try:
             path = self._realpath(path)
             os.rmdir(path)
         except OSError as e:
             return ParamikoSFTPServer.convert_errno(e.errno)
         return SFTP_OK
 
     @processor.wrap
-    def chattr(self, path: str, attr: SFTPAttributes) -> int:
+    def chattr(self, path: str, attr: SFTPAttributes) -> Any:
         try:
             path = self._realpath(path)
             ParamikoSFTPServer.set_file_attr(path, attr)
         except OSError as e:
             return ParamikoSFTPServer.convert_errno(e.errno)
         return SFTP_OK
 
     @processor.wrap
-    def symlink(self, target_path: str, path: str) -> int:
+    def symlink(self, target_path: str, path: str) -> Any:
         try:
             path = self._realpath(path)
             if (len(target_path) > 0) and (target_path[0] == "/"):
                 target_path = os.path.join(self._root, target_path[1:])
                 if target_path[:2] == "//":
                     target_path = target_path[1:]
             else:
```

### Comparing `pibble-0.4.9/pibble/api/server/googlerpc.py` & `pibble-0.5.0/pibble/api/server/googlerpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     Optional configuration:
       1. ``server.threads`` The number of threads to run the server on. Defaults to 10.
 
     See :class:`pibble.api.helpers.GRPC.GRPCService` for required arguments for the GRPC service.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         super(GRPCAPIServer, self).__init__()
 
     def on_configure(self) -> None:
         """
         Builds the server.
         """
```

### Comparing `pibble-0.4.9/pibble/api/server/webservice/apachethrift.py` & `pibble-0.5.0/pibble/api/server/webservice/apachethrift.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from thrift.transport import TTransport
 
 from typing import Any
 
 from pibble.api.server.webservice.base import WebServiceAPIServerBase
 from pibble.api.server.webservice.handler import WebServiceAPIHandlerRegistry
-from pibble.api.protocol.apachethrift import TJSONProtocol
+from pibble.api.protocol.apachethrift import TJSONProtocol  # type: ignore
 from pibble.api.exceptions import ApacheThriftError
 from pibble.api.helpers.apachethrift import (
     ApacheThriftService,
     ApacheThriftServerHandler,
 )
 
 handlers = WebServiceAPIHandlerRegistry()
```

### Comparing `pibble-0.4.9/pibble/api/server/webservice/awslambda.py` & `pibble-0.5.0/pibble/api/server/webservice/awslambda.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypedDict, Optional, Union, cast
+from typing import TypedDict, Optional, Union, Dict, List, Any, cast
 from base64 import b64decode
 from urllib.parse import parse_qs
 
 from pibble.util.log import logger
 from pibble.util.strings import encode
 
 from pibble.api.exceptions import ConfigurationError
@@ -13,32 +13,32 @@
 
 
 class LambdaRequestContextV1(TypedDict):
     accountId: str
     apiId: str
     domainName: str
     httpMethod: str
-    identity: Optional[dict]
+    identity: Optional[Dict[str, Any]]
     path: str
     protocol: str
     requestId: str
     requestTime: str
     requestTimeEpoch: int
     resourcePath: str
     stage: str
 
 
 class LambdaRequestPayloadV1(TypedDict):
     resource: str
     path: str
     httpMethod: str
-    headers: dict[str, str]
-    multiValueHeaders: Optional[dict[str, list[str]]]
-    queryStringParameters: Optional[dict[str, str]]
-    multiValueQueryStringParameters: Optional[dict[str, list[str]]]
+    headers: Dict[str, str]
+    multiValueHeaders: Optional[Dict[str, List[str]]]
+    queryStringParameters: Optional[Dict[str, str]]
+    multiValueQueryStringParameters: Optional[Dict[str, List[str]]]
     requestContext: LambdaRequestContextV1
     body: Optional[str]
     isBase64Encoded: Optional[bool]
 
 
 # V2
 
@@ -50,44 +50,44 @@
     sourceIp: str
     userAgent: str
 
 
 class LambdaRequestContextV2(TypedDict):
     accountId: str
     apiId: str
-    authentication: Optional[dict]
-    authorizer: Optional[dict]
+    authentication: Optional[Dict[str, Any]]
+    authorizer: Optional[Dict[str, Any]]
     domainName: str
     http: LambdaRequestContextV2HTTP
     requestId: str
     routeKey: str
     stage: str
     time: str
     timeEpoch: int
 
 
 class LambdaRequestPayloadV2(TypedDict):
     routeKey: str
     rawPath: str
     rawQueryString: str
-    cookies: Optional[list[str]]
-    headers: dict[str, str]
-    queryStringParameters: Optional[dict[str, str]]
+    cookies: Optional[List[str]]
+    headers: Dict[str, str]
+    queryStringParameters: Optional[Dict[str, str]]
     requestContext: LambdaRequestContextV2
     body: Optional[str]
     isBase64Encoded: Optional[bool]
 
 
 # Common
 
 
 class LambdaResponseDict(TypedDict):
     statusCode: int
-    headers: dict[str, str]
-    multiValueHeaders: dict[str, list[str]]
+    headers: Dict[str, str]
+    multiValueHeaders: Dict[str, List[str]]
     body: str
 
 
 class LambdaContext:
     function_name: str
     function_version: str
     invoked_function_arn: str
@@ -106,23 +106,23 @@
         self,
         event: Union[LambdaRequestPayloadV1, LambdaRequestPayloadV2],
         context: Optional[LambdaContext] = None,
     ) -> LambdaResponseDict:
         logger.debug(f"Receiving lambda request {event}")
         try:
             # Declare base variables to parse from differing payload
-            parameters: dict[str, Union[str, list[str]]] = {}
+            parameters: Dict[str, Union[str, List[str]]] = {}
             body: Optional[bytes] = None
             user_agent: Optional[str] = None
             http_method: str = ""
             remote_addr: str = ""
             path: str = ""
 
             # Common between payload types
-            headers: dict[str, str] = event["headers"]
+            headers: Dict[str, str] = event["headers"]
 
             if event.get("body", None) is not None:
                 body_str = cast(str, event["body"])
                 if event.get("isBase64Encoded", False):
                     body = b64decode(body_str)
                 else:
                     body = encode(body_str)
@@ -139,15 +139,15 @@
 
                 http_method = payload_v2["requestContext"]["http"]["method"]
                 path = payload_v2["requestContext"]["http"]["path"]
                 user_agent = payload_v2["requestContext"]["http"]["userAgent"]
                 remote_addr = payload_v2["requestContext"]["http"]["sourceIp"]
 
                 if payload_v2.get("cookies", None) is not None:
-                    headers["cookie"] = ";".join(cast(list[str], payload_v2["cookies"]))
+                    headers["cookie"] = ";".join(cast(List[str], payload_v2["cookies"]))
 
                 if payload_v2.get("rawQueryString", None) is not None:
                     parsed_parameters = parse_qs(payload_v2["rawQueryString"])
                     parameters.update(
                         dict(
                             [
                                 (
@@ -166,15 +166,15 @@
                 payload_v1 = cast(LambdaRequestPayloadV1, event)
 
                 http_method = payload_v1["httpMethod"]
                 path = payload_v1["path"]
 
                 if payload_v1.get("multiValueQueryStringParameters", None) is not None:
                     payload_params = cast(
-                        dict[str, list[str]],
+                        Dict[str, List[str]],
                         payload_v1["multiValueQueryStringParameters"],
                     )
                     parameters.update(
                         dict(
                             [
                                 (
                                     key,
```

### Comparing `pibble-0.4.9/pibble/api/server/webservice/base.py` & `pibble-0.5.0/pibble/api/server/webservice/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,43 @@
 from __future__ import annotations
 
 import io
 import os
 import re
-import ssl
 import logging
 import mimetypes
 
-from multiprocessing import cpu_count
 from traceback import format_exc
 
 from typing import (
     Optional,
     Any,
     Callable,
-    Iterable,
     Type,
     Tuple,
     Union,
-    TYPE_CHECKING,
+    List,
+    Dict,
     cast,
+    TYPE_CHECKING,
 )
 
 from webob import Request, Response
 
-from werkzeug.serving import run_simple as WerkzeugRun
-
-try:
-    from gunicorn.app.base import Application as GunicornApplication
-except ImportError:
-    GunicornApplication = object
-
 from pibble.util.strings import decode, truncate
 from pibble.util.log import logger
 from pibble.util.helpers import CompressedIterator
 from pibble.util.files import FileIterator
 from pibble.api.server.base import APIServerBase
-from pibble.api.server.webservice.mixin.base import WebServiceAPIServerMixinBase
 from pibble.api.server.webservice.handler import (
     WebServiceAPIHandlerRegistry,
     WebServiceAPIHandler,
+    WebServiceAPIBoundHandler,
 )
+from pibble.api.middleware.webservice.base import WebServiceAPIMiddlewareBase
 
 from pibble.api.exceptions import (
     BadRequestError,
     BadResponseError,
     NotFoundError,
     UnsupportedMethodError,
     AuthenticationError,
@@ -68,45 +61,14 @@
     # wouldn't be available at runtime. That means these are all valid
     # type to notate, and will be appropriately checked when necessary. Neat!
     from _typeshed.wsgi import StartResponse, WSGIEnvironment, WSGIApplication
 
 TEXT_CONTENT_TYPE = re.compile(r"^(text|application).*$")
 
 
-class CustomApplication(GunicornApplication):
-    """
-    A simple extension of the gunicorn application base
-    to work with the webservice.
-    """
-
-    def __init__(self, application: WSGIApplication, options: dict):
-        self.options = options
-        self.application = application
-        super(CustomApplication, self).__init__()
-
-    def load_config(self) -> None:
-        config = dict(
-            [
-                (key, self.options[key])
-                for key in self.options
-                if key in self.cfg.settings and self.options[key] is not None
-            ]
-        )
-        for key in config:
-            logger.debug(
-                "Setting Gunicorn configuration key {0} = {1}".format(
-                    key.lower(), config[key]
-                )
-            )
-            self.cfg.set(key.lower(), config[key])
-
-    def load(self) -> WSGIApplication:
-        return self.application
-
-
 class WebServiceAPIServerBase(APIServerBase):
     """
     A web service API base, useful for extension or mixins.
 
     To add functionality to the web service, use a :class:`pibble.api.server.webservice.handler.WebServiceAPIHandlerRegistry` to register methods and paths.
     """
 
@@ -123,17 +85,17 @@
         PermissionError: 403,
         NotFoundError: 404,
         UnsupportedMethodError: 405,
         TooManyRequestsError: 429,
         NotImplementedError: 501,
     }
 
-    class_handlers: list[WebServiceAPIHandlerRegistry]
+    class_handlers: List[WebServiceAPIHandlerRegistry]
 
-    def __init__(self):
+    def __init__(self) -> None:
         super(WebServiceAPIServerBase, self).__init__()
         self.class_handlers = []
         self.register_all_handlers()
 
     def format_exception(
         self,
         exception: Exception,
@@ -166,27 +128,29 @@
 
         Used for middleware that registers handlers.
         """
         for cls in reversed(type(self).mro()):
             if (
                 (
                     WebServiceAPIServerBase in cls.mro()
-                    or WebServiceAPIServerMixinBase in cls.mro()
+                    or WebServiceAPIMiddlewareBase in cls.mro()
                 )
                 and hasattr(cls, "get_handlers")
                 and "get_handlers" in cls.__dict__
             ):
                 logger.debug("Registering handlers in class {0}".format(cls.__name__))
                 self.class_handlers.append(cls.get_handlers())
 
     def prepare_all(
         self,
         request: Optional[Union[Request, RequestWrapper]] = None,
         response: Optional[Union[Response, ResponseWrapper]] = None,
-        handler: Optional[WebServiceAPIHandler] = None,
+        handler: Optional[
+            Union[WebServiceAPIHandler, WebServiceAPIBoundHandler]
+        ] = None,
     ) -> None:
         """
         Runs all ``prepare()`` methods.
 
         :param request Request: The request before processing.
         :param response Response: The response before processing.
         """
@@ -200,15 +164,17 @@
                     )
                     cls.prepare(self, request, response)
 
     def parse_all(
         self,
         request: Optional[Union[Request, RequestWrapper]] = None,
         response: Optional[Union[Response, ResponseWrapper]] = None,
-        handler: Optional[WebServiceAPIHandler] = None,
+        handler: Optional[
+            Union[WebServiceAPIHandler, WebServiceAPIBoundHandler]
+        ] = None,
     ) -> None:
         """
         Runs all ``parse()`` methods.
 
         :param request Request: The request after processing.
         :param response Response: The response after processing.
         """
@@ -247,15 +213,15 @@
             raise NotFoundError(
                 f"No view with name {view_name} (tried {tried_handlers})"
             )
         return path
 
     def _find_handler_by_request(
         self, request: Union[Request, RequestWrapper]
-    ) -> WebServiceAPIHandler:
+    ) -> Union[WebServiceAPIHandler, WebServiceAPIBoundHandler]:
         """
         Finds a handler by the request object.
 
         Will iterate through handlers in method resolution order to find the highest priority
         handler that matches a given a request, based on whatever criteria the handler
         has.
 
@@ -450,17 +416,15 @@
     def wsgi(self) -> WSGIApplication:
         """
         Returns an "application" function, almost all wsgi servers expect this.
 
         :return function: The application to pass into your wsgi server of choice.
         """
 
-        def application(
-            environ: WSGIEnvironment, start_response: StartResponse
-        ) -> Iterable[bytes]:
+        def application(environ: WSGIEnvironment, start_response: StartResponse) -> Any:
             try:
                 request = Request(environ)
                 response = Response()
                 self.handle_request(request, response)
                 return response(environ, start_response)
             except Exception as ex:
                 logger.error(
@@ -478,90 +442,52 @@
         Serves the API through varying means.
 
         This is provided as a shortcut option, and not intended for use in production.
         """
         try:
             driver = self.configuration["server.driver"]
             host = self.configuration["server.host"]
-            port = self.configuration["server.port"]
+            port = int(self.configuration["server.port"])
             secure = self.configuration.get("server.secure", False)
             cert = self.configuration.get("server.cert", None)
             key = self.configuration.get("server.key", None)
+            workers = self.configuration.get("server.workers", None)
 
             logger.debug(
                 "Attempting to run development server process using driver {0} on {1}://{2}:{3}.".format(
                     driver, "https" if secure else "http", host, port
                 )
             )
 
-            if driver == "cherrypy":
-                import cherrypy
+            run_driver: Optional[Callable] = None
 
-                cherrypy.tree.graft(self.wsgi(), "/")
-                cherrypy.server.unsubscribe()
-                server = cherrypy._cpserver.Server()
-                server.socket_host = host
-                server.socket_port = port
-                server.thread_pool = self.configuration.get("server.threads", 30)
-
-                if secure and cert is not None and key is not None:
-                    server.ssl_module = "pyopenssl"
-                    server.ssl_certificate = cert
-                    server.ssl_private_key = key
-                elif secure:
-                    logger.warning(
-                        "No SSL certificate/key specified. If this server is being proxied through another service that provides SSL context, this is okay - otherwise connections will fail."
-                    )
-
-                server.subscribe()
-                cherrypy.engine.start()
-                cherrypy.engine.block()
+            if driver == "cherrypy":
+                from pibble.api.server.webservice.drivers.driver_cherrypy import (
+                    run_cherrypy,
+                )
 
+                run_driver = run_cherrypy
             elif driver == "werkzeug":
-                context = None
-
-                if secure and cert is not None and key is not None:
-                    context = ssl.SSLContext(ssl.PROTOCOL_SSLv23)
-                    logger.info(
-                        "Loading SSL Certificate Chain, certfile {0}, keyfile {1}.".format(
-                            cert, key
-                        )
-                    )
-                elif secure:
-                    logger.warning(
-                        "No SSL certificate/key specified. If this server is being proxied through another service that provides SSL context, this is okay - otherwise connections will fail."
-                    )
+                from pibble.api.server.webservice.drivers.driver_werkzeug import (
+                    run_werkzeug,
+                )
 
-                WerkzeugRun(host, int(port), self.wsgi(), ssl_context=context)
+                run_driver = run_werkzeug
             elif driver == "gunicorn":
-                options = {
-                    "bind": "{0}:{1}".format(host, port),
-                    "workers": int(
-                        self.configuration.get("server.workers", cpu_count() * 2 + 1)
-                    ),
-                }
-
-                if secure and cert is not None and key is not None:
-                    options["keyfile"] = key
-                    options["certfile"] = cert
-                    logger.info(
-                        "Loading SSL Certificate Chain, certfile {0}, keyfile {1}.".format(
-                            cert, key
-                        )
-                    )
-                elif secure:
-                    logger.warning(
-                        "No SSL certificate/key specified. If this server is being proxied through another service that provides SSL context, this is okay - otherwise connections will fail."
-                    )
+                from pibble.api.server.webservice.drivers.driver_gunicorn import (
+                    run_gunicorn,
+                )
 
-                CustomApplication(self.wsgi(), options).run()
-            else:
+                run_driver = run_gunicorn
+
+            if run_driver is None:
                 raise ConfigurationError(
                     "Server driver {0} not supported.".format(driver)
                 )
+            run_driver(self.wsgi(), host, port, secure, cert, key, workers)
         except KeyError as ex:
             raise ConfigurationError(str(ex))
         finally:
             if destroy_on_stop:
                 self.destroy()
 
 
@@ -569,15 +495,17 @@
     """
     A base class for method-based servers, i.e. RPC and SOAP.
 
     This handles storing methods and allows for some nice and easy-to-use syntax for
     implementing servers.
     """
 
-    def __init__(self):
+    methods: List[MethodBasedWebServiceAPIServerBase.WebServiceMethod]
+
+    def __init__(self) -> None:
         super(MethodBasedWebServiceAPIServerBase, self).__init__()
         self.methods = []
 
     def _find_method_by_function(
         self, fn: Callable
     ) -> Optional[MethodBasedWebServiceAPIServerBase.WebServiceMethod]:
         """
@@ -964,23 +892,23 @@
         A class to hold the method, name, signature, etc.
 
         Not meant to be instantiated outside of the parent class.
         """
 
         def __init__(
             self,
-            method,
-            name: Optional[str] = None,
+            method: Callable,
+            name: str,
             docstring: Optional[str] = None,
-            signature: Optional[list[list[Type]]] = [],
+            signature: Optional[List[List[Type]]] = [],
             response_signature: Optional[Type] = None,
             registered: bool = False,
-            named_signature: Optional[dict[str, Type]] = None,
-            response_named_signature: Optional[dict[str, Type]] = None,
-        ):
+            named_signature: Optional[Dict[str, Type]] = None,
+            response_named_signature: Optional[Dict[str, Type]] = None,
+        ) -> None:
             self.method = method
             self.name = name
             self.docstring = docstring
             self.signature = signature
             self.response_signature = response_signature
             self.named_signature = named_signature
             self.response_named_signature = response_named_signature
```

### Comparing `pibble-0.4.9/pibble/api/server/webservice/handler.py` & `pibble-0.5.0/pibble/api/server/webservice/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from re import compile, Pattern
 from urllib.parse import unquote
-from typing import Optional, Callable, Any, Type, Iterable, Union
+from typing import Optional, Callable, Any, Type, Iterable, Union, List
 from webob import Request, Response
 
 from collections import defaultdict
 
 from pibble.util.helpers import resolve
 from pibble.util.log import logger
 from pibble.api.exceptions import NotFoundError
@@ -19,16 +19,16 @@
     Small class to hold handlers.
     """
 
     def __init__(
         self,
         function: Callable,
         pattern: Optional[Union[str, Pattern]] = None,
-        methods: list[str] = [],
-        bypass: list[Union[str, Type]] = [],
+        methods: List[str] = [],
+        bypass: List[Union[str, Type]] = [],
         reverse: Optional[tuple[str, str]] = None,
         format_response: bool = False,
         download_response: bool = False,
         cache_response: Optional[int] = None,
         compress_response: bool = False,
     ):
         self.function = function
@@ -37,14 +37,19 @@
         self.bypass = bypass
         self.reverse = reverse
         self.compress_response = compress_response
         self.format_response = format_response
         self.download_response = download_response
         self.cache_response = cache_response
 
+    def get_pattern(self) -> Optional[Pattern]:
+        if isinstance(self.pattern, str):
+            return compile(self.pattern)
+        return self.pattern
+
     def bind(self, **kwargs: Any) -> WebServiceAPIBoundHandler:
         return WebServiceAPIBoundHandler(self, **kwargs)
 
     def __repr__(self) -> str:
         return "{0} {1}: {2}{3}".format(
             ", ".join(self.methods),
             self.pattern,
@@ -112,40 +117,45 @@
         @handlers.path("/user(/(?P<username>\w+))?")
         @handlers.methods("GET"):
         def get_user(request, response, username = None):
           # Handles getting either all users (username is None) or an individual user
           pass
     """
 
-    def __init__(self):
+    handlers: List[WebServiceAPIHandler]
+
+    def __init__(self) -> None:
         self.handlers = []
 
     def _find_handler_by_function(self, fn: Callable) -> WebServiceAPIHandler:
         """
         Retrieves a handler by a function.
 
         :param fn callable: The function to check for.
         :returns WebServiceAPIHandler: The handler to return.
         """
         for handler in self.handlers:
             if handler.function is fn:
                 return handler
         raise NotFoundError(f"Cannot find function {fn}")
 
-    def _find_handler_by_request(self, method: str, path: str) -> WebServiceAPIHandler:
+    def _find_handler_by_request(
+        self, method: str, path: str
+    ) -> Union[WebServiceAPIHandler, WebServiceAPIBoundHandler]:
         """
         Retrieves the handler matching a method and path.
 
         :param method str: The method - GET, PUT, POST, etc.
         :param path str: The request path.
         :returns WebServiceAPIHandler: The method that handles the request.
         """
         for handler in self.handlers:
-            if handler.pattern is not None:
-                match = handler.pattern.match(path)
+            handler_pattern = handler.get_pattern()
+            if handler_pattern is not None:
+                match = handler_pattern.match(path)
                 if match and method.upper() in handler.methods:
                     logger.debug(
                         "Handler {0} matched on path {1} and method {2}".format(
                             handler.function.__name__, path, method.upper()
                         )
                     )
                     groups = match.groupdict()
@@ -225,15 +235,15 @@
             else:
               # Get one user
 
         :param pattern str: A regular expression pattern. Can be string or regular express (`r""`).
         :returns function: Returns the wrapper function. The inner wrapper function returns the function itself, so they can be composed.
         """
 
-        def wrap(fn):
+        def wrap(fn: Callable) -> Callable:
             self.create_or_modify_handler(
                 fn,
                 pattern=pattern if isinstance(pattern, Pattern) else compile(pattern),
             )
             return fn
 
         return wrap
@@ -250,65 +260,65 @@
           def make_user(self, request, response):
             # Make a user
 
         :param methods tuple: Any number of HTTP methods, all strings. Should be capitalized, like GET, PUT, POST, etc.
         :returns function: Returns the wrapper function. The inner wrapper function returns the function itself, so they can be composed.
         """
 
-        def wrap(fn):
+        def wrap(fn: Callable) -> Callable:
             self.create_or_modify_handler(
                 fn, methods=[method.upper() for method in methods]
             )
             return fn
 
         return wrap
 
     def format(self) -> Callable[[Callable], Callable]:
         """
         Indicates that the results of the request should be formatted by calling the format_response()
         handler. This, by default, is false.
         """
 
-        def wrap(fn):
+        def wrap(fn: Callable) -> Callable:
             self.create_or_modify_handler(fn, format_response=True)
             return fn
 
         return wrap
 
     def download(self) -> Callable[[Callable], Callable]:
         """
         Indicates that the results of the request is a file path, and that file path should be iterated
         over for the response in a streaming fashion.
         """
 
-        def wrap(fn):
+        def wrap(fn: Callable) -> Callable:
             self.create_or_modify_handler(fn, download_response=True)
             return fn
 
         return wrap
 
     def compress(self) -> Callable[[Callable], Callable]:
         """
         Indicates that the results of the request should be compressed (using zlib.)
         """
 
-        def wrap(fn):
+        def wrap(fn: Callable) -> Callable:
             self.create_or_modify_handler(fn, compress_response=True)
             return fn
 
         return wrap
 
     def cache(
         self, cache_time: Optional[int] = 31536000
     ) -> Callable[[Callable], Callable]:
         """
         Indicates that the results of the request should be cacheed (using http headers.)
         """
 
-        def wrap(fn):
+        def wrap(fn: Callable) -> Callable:
             self.create_or_modify_handler(fn, cache_response=cache_time)
             return fn
 
         return wrap
 
     def reverse(self, name: str, path: str = "/") -> Callable[[Callable], Callable]:
         """
@@ -353,43 +363,20 @@
           news_url = handlers.resolve("Articles", category = "news") # /article/news
           article_url = handlers.resolve("Articles", category = "news", id = 21) # /article/news/21
 
         :param name str: The name of the string.
         :param path str: A formatting string.
         """
 
-        def wrap(fn):
+        def wrap(fn: Callable) -> Callable:
             self.create_or_modify_handler(fn, reverse=(name, path))
             return fn
 
         return wrap
 
-    def resolve(self, view_name: str, **kwargs: Any) -> str:
-        """
-        Resolves a URL name with URL arguments defined by **kwargs. See reverse() above
-        for more details.
-
-        :see
-        :param name str: The name of the view to find.
-        :param kwargs dict: Any number of URL arguments to pass in.
-        """
-        for handler in self.handlers:
-            if handler.reverse is not None and handler.reverse[0] == view_name:
-                format_dict = defaultdict(lambda: "")  # type: ignore
-                format_dict.update(kwargs)
-                resolved = handler.reverse[1].format_map(format_dict)
-                while resolved.find("//") != -1:
-                    resolved = resolved.replace("//", "/")
-                while resolved and resolved[-1] == "/":
-                    resolved = resolved[:-1]
-                if not resolved:
-                    return "/"
-                return resolved
-        raise NotFoundError("No view with name {0}".format(view_name))
-
     def bypass(self, *classes: Union[str, Type]) -> Callable[[Callable], Callable]:
         """
         Marks a handler to pybass parsing or preparing requests/responses.
 
         Example usage::
 
           handler = WebServiceAPIHandlerRegistry()
@@ -400,20 +387,43 @@
             # Handle an insecure request
 
         :param classes tuple: Any number of class names to ignore. These can be fully qualified strings, like `pibble.api.middleware.webservice.authentication.basic.BasicAuthenticationMiddleware` or an actual class.
         :returns function: Returns the wrapper function.
         """
         classlist = [cls if isinstance(cls, type) else resolve(cls) for cls in classes]
 
-        def wrap(fn):
+        def wrap(fn: Callable) -> Callable:
             self.create_or_modify_handler(fn, bypass=classlist)
             return fn
 
         return wrap
 
+    def resolve(self, view_name: str, **kwargs: Any) -> str:
+        """
+        Resolves a URL name with URL arguments defined by **kwargs. See reverse() above
+        for more details.
+
+        :see
+        :param name str: The name of the view to find.
+        :param kwargs dict: Any number of URL arguments to pass in.
+        """
+        for handler in self.handlers:
+            if handler.reverse is not None and handler.reverse[0] == view_name:
+                format_dict = defaultdict(lambda: "")  # type: ignore
+                format_dict.update(kwargs)
+                resolved = handler.reverse[1].format_map(format_dict)
+                while resolved.find("//") != -1:
+                    resolved = resolved.replace("//", "/")
+                while resolved and resolved[-1] == "/":
+                    resolved = resolved[:-1]
+                if not resolved:
+                    return "/"
+                return resolved
+        raise NotFoundError("No view with name {0}".format(view_name))
+
     def __iter__(self) -> Iterable[WebServiceAPIHandler]:
         self.index = 0
         while True:
             try:
                 yield next(self)
             except StopIteration:
                 return
```

### Comparing `pibble-0.4.9/pibble/api/server/webservice/jsonapi.py` & `pibble-0.5.0/pibble/api/server/webservice/jsonapi.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from webob import Request, Response
 
 from typing import Any, Optional
 
 from pibble.database.orm import ORMObject
 from pibble.api.server.webservice.base import WebServiceAPIServerBase
-from pibble.util.strings import FlexibleStringer
+from pibble.util.strings import Serializer
 
 
 class JSONWebServiceAPIServer(WebServiceAPIServerBase):
     """
     A small extension of the API Server base for JSONAPI's.
 
     Parses JSON requests, and formats per JSONAPI spec.
@@ -46,15 +46,15 @@
             )
         }
 
         if hasattr(response, "meta"):
             response_meta.update(response.meta)
 
         return json.dumps(
-            {"meta": response_meta, "data": result}, default=FlexibleStringer.serialize
+            {"meta": response_meta, "data": result}, default=Serializer.serialize
         )
 
     def format_exception(
         self,
         exception: Exception,
         request: Request,
         response: Response,
@@ -77,28 +77,28 @@
                     {
                         "status": str(error_code),
                         "title": type(exception).__name__,
                         "detail": str(exception),
                     }
                 ]
             },
-            default=FlexibleStringer.serialize,
+            default=Serializer.serialize,
         )
 
     def parse(
         self,
         request: Optional[Request] = None,
         response: Optional[Response] = None,
     ) -> None:
         """
         Parses the request and sets content type on the response.
         """
         if request is not None:
             if request.body:
                 try:
-                    setattr(request, "parsed", FlexibleStringer.parse(request.json))
+                    setattr(request, "parsed", Serializer.deserialize(request.json))
                 except json.JSONDecodeError:
                     setattr(request, "parsed", {})
             else:
                 setattr(request, "parsed", {})
         if response is not None:
             response.content_type = "application/vnd.api+json"
```

### Comparing `pibble-0.4.9/pibble/api/server/webservice/orm.py` & `pibble-0.5.0/pibble/api/server/webservice/orm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from webob import Request, Response
 from typing import Any
 
-from pibble.util.strings import FlexibleStringer
+from pibble.util.strings import Serializer
 from pibble.api.server.webservice.base import WebServiceAPIServerBase
 from pibble.api.middleware.database.orm import ORMMiddlewareBase
 
 
 class ORMWebServiceAPIServer(WebServiceAPIServerBase, ORMMiddlewareBase):
     """
     Overrides format_response to perform a format() on the results.
@@ -14,19 +14,19 @@
     def format_response(
         self,
         result: Any,
         request: Request,
         response: Response,
     ) -> str:
         if isinstance(result, list):
-            return FlexibleStringer.serialize(
+            return Serializer.serialize(
                 [
                     r.format(include=request.GET.getall("include"))
                     for r in result
                     if r is not None
                 ]
             )
         if result is not None:
-            return FlexibleStringer.serialize(
+            return Serializer.serialize(
                 result.format(include=request.GET.getall("include"))
             )
         return ""
```

### Comparing `pibble-0.4.9/pibble/api/server/webservice/rpc/base.py` & `pibble-0.5.0/pibble/api/server/webservice/rpc/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 from pibble.api.server.webservice.base import MethodBasedWebServiceAPIServerBase
 from pibble.api.server.webservice.handler import WebServiceAPIHandlerRegistry
 from pibble.api.exceptions import (
     UnsupportedMethodError,
     ConfigurationError,
 )
-from typing import Type, Optional, Union
+from typing import Type, Optional, Union, List, Dict
 
 
 handlers = WebServiceAPIHandlerRegistry()
 
 
 class RPCServerBase(MethodBasedWebServiceAPIServerBase):
     """
     A base server for RPC classes.
 
     This will handle function registration and dispatching. Inherited classes are responsible for parsing and formatting requests and responses.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         super(RPCServerBase, self).__init__()
         self.register_introspection_functions()
 
     @classmethod
     def get_handlers(cls) -> WebServiceAPIHandlerRegistry:
         return handlers
 
@@ -46,25 +46,25 @@
         self.sign_request(str)(fn2)
         self.sign_response(list)(fn2)
 
         fn3 = self.register("system.methodHelp")(self.method_help)
         self.sign_request(str)(fn3)
         self.sign_response(str)(fn3)
 
-    def list_methods(self) -> list[str]:
+    def list_methods(self) -> List[str]:
         """
         Returns a list of all methods.
 
         :returns list: A list of function names.
         """
-        return [method.name for method in self.methods]
+        return [method.name for method in self.methods if method.name]
 
     def method_signature(
         self, fn_name: str
-    ) -> Optional[Union[list[list[Type]], list[dict[str, Type]]]]:
+    ) -> Optional[Union[List[List[Type]], List[Dict[str, Type]]]]:
         """
         Returns the signature of a method.
 
         Returns None if no signature is known or it takes no parameters.
 
         :param fn_name str: The function to return.
         :returns list: A list of lists of types.
@@ -75,15 +75,15 @@
             raise UnsupportedMethodError("{0} does not exist.".format(fn_name))
         if fn.named_signature:
             return [fn.named_signature]
         elif not fn.signature:
             raise ConfigurationError(
                 "Method {0} is missing a signature.".format(fn_name)
             )
-        signatures: list[list[Type]] = []
+        signatures: List[List[Type]] = []
         for signature in fn.signature:
             if fn.response_signature is not None:
                 signatures.append([fn.response_signature] + signature)
             else:
                 signatures.append(signature)
         if not fn.signature and fn.response_signature:
             signatures = [[fn.response_signature]]
```

### Comparing `pibble-0.4.9/pibble/api/server/webservice/rpc/jsonrpc.py` & `pibble-0.5.0/pibble/api/server/webservice/rpc/jsonrpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 from typing import Type, Any, Optional
 
 from webob import Request, Response
 
 from pibble.api.server.webservice.rpc.base import RPCServerBase
 from pibble.api.exceptions import UnsupportedMethodError, BadRequestError
-from pibble.util.strings import FlexibleStringer, decode
+from pibble.util.strings import Serializer, decode
 
 
-class JSONRPCFlexibleStringer(FlexibleStringer):
+class JSONRPCSerializer(Serializer):
     SERIALIZE_FORMATS = {
-        **FlexibleStringer.SERIALIZE_FORMATS,
+        **Serializer.SERIALIZE_FORMATS,
         **{type: lambda p, **k: JSONRPCServer.map_typename(p)},
     }
 
 
 class JSONRPCServer(RPCServerBase):
     """
     An implementation of the RPC server for parsing and returning XMLRPC objects.
@@ -103,18 +103,18 @@
             )
         if "method" not in request:
             raise BadRequestError("Missing method name in request.")
         params = request.get("params", None)
         if params is None:
             return request["method"], [], {}
         elif type(params) is dict:
-            params = FlexibleStringer.parse(params)
+            params = Serializer.deserialize(params)
             return request["method"], [], params
         elif type(params) is list:
-            params = FlexibleStringer.parse(params)
+            params = Serializer.deserialize(params)
             return request["method"], params, {}
         else:
             raise BadRequestError(
                 "Bad 'params' format. Must be object or array, got {0} instead.".format(
                     type(params).__name__
                 )
             )
@@ -129,22 +129,22 @@
         """
         if result is not None:
             id = json.loads(request.body).get("id", None)
             if id is not None:
                 return decode(
                     json.dumps(
                         {"jsonrpc": "2.0", "result": result, "id": id},
-                        default=JSONRPCFlexibleStringer.serialize,
+                        default=JSONRPCSerializer.serialize,
                     )
                 )
         return ""
 
     def format_exception(
         self, exception: Exception, request: Request, response: Response
-    ):
+    ) -> str:
         """
         Formats an exception into a dict.
 
         :param ex exception: The exception thrown.
         :returns str: The formatted exception response.
         """
         code = -32500
@@ -153,10 +153,10 @@
         if isinstance(exception, UnsupportedMethodError):
             code = -32601
         if isinstance(exception, BadRequestError):
             code = -32600
         return decode(
             json.dumps(
                 {"jsonrpc": "2.0", "code": code, "message": str(exception)},
-                default=JSONRPCFlexibleStringer.serialize,
+                default=JSONRPCSerializer.serialize,
             )
         )
```

### Comparing `pibble-0.4.9/pibble/api/server/webservice/rpc/xmlrpc.py` & `pibble-0.5.0/pibble/api/server/webservice/rpc/xmlrpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         if typename is None:
             raise TypeError(
                 "Cannot determine typename from type '{0}'.".format(_type.__name__)
             )
         return typename
 
     @staticmethod
-    def format_parameter(parameter) -> ET._Element:
+    def format_parameter(parameter: Any) -> ET._Element:
         """
         Formats a single datum into a <parameter/> node.
 
         >>> import lxml.etree as ET
         >>> import datetime
         >>> from pibble.api.server.webservice.rpc.xmlrpc import XMLRPCServer
         >>> ET.tostring(XMLRPCServer.format_parameter("foo"))
@@ -118,15 +118,15 @@
                     )
                 raise BadRequestError(
                     "Cannot encode type {0} into XMLRPC response.".format(
                         type(p).__name__
                     )
                 )
 
-            def _format_name(n: Any) -> str:
+            def _format_name(n: Any) -> ET._Element:
                 return E.name(str(n))
 
             if name is not None:
                 return (_format_value(value), _format_name(name))
             return (_format_value(value),)
 
         return E.param(*_format_parameter(parameter))
@@ -181,15 +181,15 @@
             kwargs = parameters[0]
             parameters = []
         else:
             kwargs = {}
         return method_name, parameters, kwargs
 
     @staticmethod
-    def parse_parameters(node: ET._Element):
+    def parse_parameters(node: ET._Element) -> Any:
         """
         Takes the <params/> node from a request, then returns a list of the parsed parameters.
 
         >>> import lxml.etree as ET
         >>> from lxml.builder import E
         >>> from pibble.api.server.webservice.rpc.xmlrpc import XMLRPCServer
         >>> XMLRPCServer.parse_parameters(E.params(E.param(E.value(E.int("4")))))
@@ -238,30 +238,30 @@
                     "Unknown value type '{0}'.".format(value_node.tag)
                 )
 
             return _parse_value(value_node)
 
         return [parse_parameter(param) for param in node]
 
-    def format_response(self, result: Any, request: Request, response: Response):
+    def format_response(self, result: Any, request: Request, response: Response) -> str:
         """
         Formats a method response from the dispatcher.
 
         :param response object: The response from the method.
         :returns str: The <methodResponse/> node.
         """
         if result is None:
             return decode(ET.tostring(E.methodResponse(E.params())))
         return decode(
             ET.tostring(E.methodResponse(XMLRPCServer.format_parameters(result)))
         )
 
     def format_exception(
         self, exception: Exception, request: Request, response: Response
-    ):
+    ) -> str:
         """
         Formats an exception into a <fault/> node.
 
         :param ex exception: The exception thrown.
         :return str: The <fault/> node.
         """
         code = -32500
```

### Comparing `pibble-0.4.9/pibble/api/server/webservice/soap.py` & `pibble-0.5.0/pibble/api/server/webservice/soap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import datetime
 
 from lxml import etree as ET
 from lxml.builder import ElementMaker
 
-from typing import Type, Optional, Any, Iterator, Tuple
+from typing import Type, Optional, Any, Iterator, Tuple, List, Dict, cast
 
 from webob import Request, Response
 
 from pibble.api.server.webservice.base import MethodBasedWebServiceAPIServerBase
 from pibble.api.server.webservice.handler import WebServiceAPIHandlerRegistry
 from pibble.api.exceptions import (
     UnsupportedMethodError,
     BadRequestError,
     ConfigurationError,
     NotFoundError,
 )
-from pibble.util.strings import decode, encode, FlexibleStringer
+from pibble.util.strings import decode, encode, Serializer
 from pibble.util.log import logger
 
 
 class MultiNamespaceElementBuilder:
     """
     A helper class for generating XML elements in multiple namespaces at once.
 
@@ -94,22 +94,22 @@
         xmlnsxsd = "{0}{1}.xsd".format(path, name)
 
         nsmap = {"xsd": "http://www.w3.org/2001/XMLSchema"}
 
         E = MultiNamespaceElementBuilder(**nsmap)
 
         def _get_types() -> Iterator[ET._Element]:
-            def _list_node(name: str, lst: list[Type]) -> Iterator[ET._Element]:
+            def _list_node(name: str, lst: List[Type]) -> Iterator[ET._Element]:
                 for node in _dict_node(
                     name,
                     dict(zip(["listIndex{0}".format(i) for i in range(len(lst))], lst)),
                 ):
                     yield node
 
-            def _dict_node(name: str, dct: dict[str, Type]) -> Iterator[ET._Element]:
+            def _dict_node(name: str, dct: Dict[str, Type]) -> Iterator[ET._Element]:
                 if len(dct.keys()) == 1:
                     key = list(dct.keys())[0]
                     yield E.xsd.element(
                         E.xsd.complexType(
                             E.xsd.all(
                                 E.xsd.element(name=key, type=self.get_type(dct[key]))
                             ),
@@ -327,38 +327,40 @@
             raise UnsupportedMethodError("{0} does not exist.".format(method))
 
         if fn.signature:
             for i, arg in enumerate(args):
                 if (
                     type(fn.signature[0][i]) is type and fn.signature[0][i] is not str
                 ) or not isinstance(fn.signature[0][i], str):
-                    args[i] = FlexibleStringer.parse(arg)
+                    args[i] = Serializer.deserialize(arg)
         elif fn.named_signature:
             for key in kwargs:
                 if key not in fn.named_signature:
                     raise BadRequestError(
                         "Method {0} does not understand keyword argument {1}.".format(
                             method, key
                         )
                     )
                 if (
                     type(fn.named_signature[key]) is type
                     and fn.named_signature[key] is not str
                 ) or not isinstance(fn.named_signature[key], str):
-                    kwargs[key] = FlexibleStringer.parse(kwargs[key])
+                    kwargs[key] = Serializer.deserialize(kwargs[key])
 
         return method, args, kwargs
 
     def format_response(self, result: Any, request: Request, response: Response) -> str:
         """
         Takes a result and formats it in the appropriate XSD object
         as generated during initial request.
         """
         method = request.soap_method
         fn = self._find_method_by_name(method)
+        if not fn or not fn.registered:
+            raise UnsupportedMethodError("{0} does not exist.".format(method))
         ssl = self.configuration.get("server.secure", False)
         name = self.configuration.get("server.name", "SOAPServer")
         hostname = self.configuration.get("server.hostname", "127.0.0.1")
         path = "{protocol}://{hostname}:{port}{path}".format(
             protocol="https" if ssl else "http",
             hostname=hostname,
             path=self.configuration.get("server.path", "/"),
@@ -372,33 +374,34 @@
             "soapenv": "http://schemas.xmlsoap.org/soap/envelope/",
             "tns": xmlns,
             "xsd1": xmlnsxsd,
         }
 
         E = MultiNamespaceElementBuilder(**nsmap)
 
-        def _get_node(method, result):
-            if fn.response_signature:
-                if fn.response_signature is not list:
+        def _get_node(method: str, result: Any) -> ET._Element:
+            if fn.response_signature:  # type: ignore
+                if fn.response_signature is not list:  # type: ignore
                     result = [result]
                 return E.xsd1(
                     "{0}Response".format(method),
                     *[
                         E.xsd1("listIndex{0}".format(i), str(part))
                         for i, part in enumerate(result)
                     ],
                 )
-            elif fn.response_named_signature:
+            elif fn.response_named_signature:  # type: ignore
                 return E.xsd1(
                     "{0}Response".format(method),
                     *[E.xsd1(key, str(result[key])) for key in result],
                 )
 
-        return ET.tostring(
-            E.soapenv.Envelope(E.soapenv.Body(_get_node(method, result)))
+        return cast(
+            str,
+            ET.tostring(E.soapenv.Envelope(E.soapenv.Body(_get_node(method, result)))),
         )
 
     @handlers.path("/(?P<service_name>\w*)\.(?P<request_type>\w*)")
     @handlers.methods("GET")
     def wsdl(
         self, request: Request, response: Response, service_name: str, request_type: str
     ) -> str:
```

### Comparing `pibble-0.4.9/pibble/api/server/webservice/template/__init__.py` & `pibble-0.5.0/pibble/api/server/webservice/template/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import io
 import logging
 import traceback
 
-from typing import Optional, Callable, Any
+from typing import Optional, Callable, Any, List
 from webob import Request, Response
 
 from pibble.util.helpers import CompressedIterator
 from pibble.util.strings import truncate
 from pibble.util.log import logger
 from pibble.api.exceptions import ConfigurationError
 from pibble.api.server.base import APIServerBase
@@ -25,29 +25,29 @@
     A small extension to the base handler to allow for template responses.
     """
 
     def __init__(
         self,
         function: Callable,
         template: Optional[str] = None,
-        errors: Optional[list[int]] = [],
+        errors: Optional[List[int]] = [],
         **kwargs: Any,
     ):
         super(TemplateHandler, self).__init__(function, **kwargs)
         self.template = template
         self.errors = errors
 
     def __call__(
         self,
         server: APIServerBase,
         request: Request,
         response: Response,
         *args: Any,
         **kwargs: Any,
-    ) -> str:
+    ) -> Any:
         if self.template is not None and isinstance(server, TemplateServer):
             response.content_type = (
                 "text/html"  # Push default now, this could be changed in handler
             )
             server.prepare_context_all(request, response)
             try:
                 context = self.function(server, request, response, *args, **kwargs)
@@ -91,15 +91,15 @@
         - Template hanlders will look for <filename> in the handler registry template directories.
           * Directories are traversed in the order they were passed to the registry.
         - When a template is not found, it is considered a configuration error.
         - Templates use Jinja2 to render.
         - Templates are **always** given a variable of `csrf_token`. They can be ignored if so desired.
         """
 
-        def wrap(fn):
+        def wrap(fn: Callable) -> Callable:
             self.create_or_modify_handler(fn, template=filename)
             return fn
 
         return wrap
 
     def errors(self, *codes: int) -> Callable[[Callable], Callable]:
         """
@@ -107,15 +107,15 @@
 
         When a response has an error code, the TemplateServer can intercept and respond with an
         error handler. This is generally also a template handler, but needn't be.
 
         :param codes tuple: Any number of error codes to handle.
         """
 
-        def wrap(fn):
+        def wrap(fn: Callable) -> Callable:
             self.create_or_modify_handler(fn, errors=[int(code) for code in codes])
             return fn
 
         return wrap
 
     def create_handler(self, fn: Callable, **kwargs: Any) -> TemplateHandler:
         """
@@ -129,15 +129,15 @@
 
 
 class TemplateServer(WebServiceAPIServerBase):
     """
     This is a small extension on the base server to add error handlers and template loaders.
     """
 
-    class_handlers: list[WebServiceAPIHandlerRegistry]
+    class_handlers: List[WebServiceAPIHandlerRegistry]
 
     def on_configure(self) -> None:
         """
         Create the template loader.
 
         This does not require any actual configuration, but see :class:pibble.api.server.webservice.html.server.TemplateServerTemplateLoader for optional keys.
         """
```

### Comparing `pibble-0.4.9/pibble/api/server/webservice/template/extensions.py` & `pibble-0.5.0/pibble/api/server/webservice/template/extensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import math
 import jinja2.exceptions
 
 from jinja2 import nodes
 from jinja2.ext import Extension
 from jinja2.parser import Parser
 
-from typing import Callable, Any, Union
+from typing import Callable, Any, Union, List
 
 from pibble.api.base import APIBase
 from pibble.api.configuration import APIConfiguration
 
 
 class ExtensionBase:
     getConfiguration: Callable[[], APIConfiguration]
@@ -38,15 +38,15 @@
     """
 
     tags = {"context_extension_base"}
 
     def parse(self, parser: Parser) -> nodes.Node:
         line = next(parser.stream).lineno
         context = nodes.ContextReference()
-        args: list[Any] = [context]
+        args: List[Any] = [context]
 
         while True:
             try:
                 args.append(parser.parse_expression())
             except jinja2.exceptions.TemplateSyntaxError:
                 break
```

### Comparing `pibble-0.4.9/pibble/api/server/webservice/template/loader.py` & `pibble-0.5.0/pibble/api/server/webservice/template/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import jinja2
 
 from jinja2.ext import Extension
-from typing import Optional, Callable, Any, Type, Union
+from typing import Optional, Callable, Any, Type, Union, Dict
 
 from pibble.api.exceptions import ConfigurationError
 from pibble.api.configuration import APIConfiguration
 from pibble.api.base import APIBase
 
 from pibble.util.log import logger
 from pibble.util.helpers import resolve
@@ -83,15 +83,15 @@
         self.extensions = [
             extension if isinstance(extension, type) else resolve(extension)
             for extension in self.extensions
         ]
 
         # Add in Lambdas
 
-        lambdas: dict[str, Callable] = {}
+        lambdas: Dict[str, Callable] = {}
         lambdas["getServer"] = lambda *args: self.server
         lambdas["getConfiguration"] = lambda *args: self.configuration
 
         self.extensions = [
             type("{0}Extension".format(extension.__name__), (extension,), lambdas)
             for extension in self.extensions
         ]
@@ -141,15 +141,15 @@
         ]
     ) -> None:
         """
         Adds an extension after initial creation.
 
         :param extensions list<Extension>: Either a jinja2.ext.Extension or any of the extensions in the template extension directory.
         """
-        lambdas: dict[str, Callable] = {}
+        lambdas: Dict[str, Callable] = {}
         lambdas["getServer"] = lambda *args: self.server
         lambdas["getConfiguration"] = lambda *args: self.configuration
         for extension in extensions:
             extension = type(
                 "{0}Extension".format(extension.__name__), (extension,), lambdas
             )
```

### Comparing `pibble-0.4.9/pibble/database/dedupe.py` & `pibble-0.5.0/pibble/database/dedupe.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 except ImportError:
     sys.stderr.write(f"Dedupe package missing. Run `pip install dedupe` to get it.\r\n")
     sys.stderr.flush()
     raise
 
 import sqlalchemy
 
-from typing import Any
+from typing import Any, List, Dict
 from statistics import median
 from pibble.util.log import logger
 from pibble.database.engine import EngineFactory
 from pibble.database.util import row_to_dict
 
 from sqlalchemy.sql.type_api import TypeEngine as SQLAlchemyType
 
@@ -31,20 +31,20 @@
     """
 
     STEP_SIZE = 30000
 
     def __init__(
         self,
         database_type: str,
-        database_params: dict[str, Any],
+        database_params: Dict[str, Any],
         tablename: str,
         unique_key: str,
         unique_key_type: SQLAlchemyType,
-        fields: list[str],
-    ):
+        fields: List[str],
+    ) -> None:
         self.settings_file = os.path.join(os.getcwd(), "{0}.settings".format(tablename))
         self.training_file = os.path.join(os.getcwd(), "{0}.training".format(tablename))
 
         self.database_type = database_type
         self.database_params = database_params
         self.tablename = tablename
         self.unique_key = unique_key
@@ -57,15 +57,15 @@
         """
         Runs the deduplicator to completion.
         """
         self.gather()
         self.train()
         self.cluster()
 
-    def sample(self, row) -> dict[str, Any]:
+    def sample(self, row: Any) -> Dict[str, Any]:
         """
         A helper method to turn a row into a "sample", expected by dedupe.
 
         Notably this turns it into a dictionary, and turns empty strings into "None".
         """
         row_dict = row_to_dict(row)
         return dict(
```

### Comparing `pibble-0.4.9/pibble/database/engine.py` & `pibble-0.5.0/pibble/database/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 import os
 
 try:
     import pyodbc
 except ImportError:
     pyodbc = None
 
-from typing import Any
+from typing import Any, List, Dict, cast
+from typing_extensions import Self
 
 from sqlalchemy.engine.url import URL
 from sqlalchemy.engine.base import Engine as EngineBase
 from pibble.util.log import logger
 
 from sqlalchemy.schema import DropTable
 from sqlalchemy.ext.compiler import compiles
 
 os.environ["TDSVER"] = "8.0"
 
 
-@compiles(DropTable, "postgresql")
-def _compile_drop_table(element, compiler, **kwargs):
+@compiles(DropTable, "postgresql")  # type: ignore
+def _compile_drop_table(element: Any, compiler: Any, **kwargs: Any) -> Any:
     return compiler.visit_drop_table(element) + " CASCADE"
 
 
 class Engine:
     """
     An 'engine' class, made to wrap around SQLAlchemy's engine creation.
 
@@ -39,34 +40,38 @@
     :param username str: A username to use for authentication. This authentication is handled by the driver, so the method varies.
     :param password str: A password to use for authentication.
     :param database str: An initial database to connect to. If ommitted, the engine will connect to "default" initially.
     """
 
     KNOWN_KEYS = ["drivername", "username", "password", "host", "port", "database"]
 
-    engines: dict[str, EngineBase]
+    engines: Dict[str, EngineBase]
 
     def __init__(self, name: str, **connection_params: Any):
         self.name = name
         self.connection_params = {}
         for key in connection_params:
             if key in Engine.KNOWN_KEYS:
                 self.connection_params[key] = connection_params[key]
             else:
                 if "query" not in self.connection_params:
                     self.connection_params["query"] = {}
                 self.connection_params["query"][key] = connection_params[key]
         self.engines = {}
         if "database" in self.connection_params:
             self._default_database = str(self.connection_params.pop("database"))
+            if self.connection_params["drivername"].startswith(
+                "sqlite"
+            ) and self._default_database.startswith("~"):
+                self._default_database = os.path.expanduser(self._default_database)
         else:
             self._default_database = "default"
         self._create_engine(self._default_database)
 
-    def __iter__(self):
+    def __iter__(self) -> Self:
         self._iterkeys = list(self.engines.keys())
         self._iterindex = 0
         return self
 
     def __next__(self) -> EngineBase:
         if self._iterindex > len(self._iterkeys):
             raise StopIteration
@@ -100,15 +105,15 @@
         self.engines[database_name] = sqlalchemy.create_engine(conn_string)
         if "pyodbc" in self.connection_params["drivername"]:
             if pyodbc is None:
                 raise OSError(
                     "Failed to import PyODBC. This server/container likely needs ODBC configuration."
                 )
 
-            def decode_sketchy_utf16(raw_bytes):
+            def decode_sketchy_utf16(raw_bytes: bytes) -> str:
                 s = raw_bytes.decode("utf-16le", "ignore")
                 try:
                     n = s.index("\u0000")
                     s = s[:n]  # respect null terminator
                 except ValueError:
                     pass
                 return s
@@ -140,28 +145,28 @@
         self.engines = {}
 
 
 class NoEngine:
     def __init__(self, name: str):
         self.name = name
 
-    def __getattr__(self, key):
+    def __getattr__(self, key: str) -> Any:
         raise NotImplementedError(
             "The engine for database type {0} is not configured.".format(self.name)
         )
 
 
 class EngineFactory:
     """
     The EngineFactory is used to create Engines. See :class:pibble.database.engine.Engine
 
     :param kwargs dict: A dictionary containing "key" => "configuration" pairs, where "configuration" is a dictionary containing necessary configuration keys.
     """
 
-    DEFAULTS: dict[str, dict[str, Any]] = {
+    DEFAULTS: Dict[str, Dict[str, Any]] = {
         "postgres": {
             "drivername": "postgresql+psycopg2",
             "database": "default",
         },
         "impala": {
             "drivername": "impala",
             "auth_mechanism": "NOSASL",
@@ -180,18 +185,18 @@
         "sqlite": {"drivername": "sqlite", "database": ":memory:"},
         "mysql": {
             "drivername": "mysql",
             "database": "default",
         },
     }
 
-    configuration: dict[str, dict[str, Any]]
-    stores: list[EngineStore]
+    configuration: Dict[str, Dict[str, Any]]
+    stores: List[EngineStore]
 
-    def __init__(self, **kwargs: dict[str, Any]):
+    def __init__(self, **kwargs: Dict[str, Any]):
         self.configuration = {}
         for key in EngineFactory.DEFAULTS:
             self.configuration[key] = {**EngineFactory.DEFAULTS[key]}
         for key in kwargs:
             self.configuration[key].update(kwargs[key])
         self.stores = []
 
@@ -238,25 +243,22 @@
 
         :param engine pibble.database.engine.Engine: The engine to dispose of.
         """
         self.stores = [store for store in self.stores if store.engine is not engine]
         engine.dispose()
 
     def __getitem__(self, key: str) -> Engine:
-        return getattr(self, key)
+        return cast(Engine, getattr(self, key))
 
-    def __delitem__(self, key) -> None:
+    def __delitem__(self, key: str) -> None:
         return delattr(self, key)
 
-    def __getattr__(self, key) -> Engine:
+    def __getattr__(self, key: str) -> Engine:
         return self.get(key)
 
-    def __delattr__(self, key) -> None:
-        self.dispose(key)
-
     def __enter__(self) -> EngineFactory:
         return self
 
     def __exit__(self, *args: Any) -> None:
         _stores = self.stores
         self.stores = []
         for store in _stores:
```

### Comparing `pibble-0.4.9/pibble/database/orm.py` & `pibble-0.5.0/pibble/database/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,44 +7,37 @@
 from traceback import format_exc
 
 from pibble.api.exceptions import PermissionError, BadRequestError
 from pibble.api.configuration import APIConfiguration
 
 from pibble.util.log import logger
 from pibble.util.helpers import resolve
-from pibble.util.strings import FlexibleStringer, decode
+from pibble.util.strings import Serializer, decode
 from pibble.util.encryption import AESCipher
 
 from pibble.database.engine import EngineFactory
 
-from typing import Optional, Type, Iterator, Any, Callable, Union, cast
+from typing import Optional, Type, Iterator, Any, Callable, Union, List, Dict, cast
 
 from sqlalchemy import Column, Integer, String, Sequence, ForeignKey
 
 from sqlalchemy.exc import InvalidRequestError
 
 from sqlalchemy.orm import sessionmaker, relationship
 from sqlalchemy.orm.session import Session
 from sqlalchemy.orm.state import InstanceState
 from sqlalchemy.orm.attributes import InstrumentedAttribute
 from sqlalchemy.orm.collections import InstrumentedList
 
-from sqlalchemy.schema import DropTable
 from sqlalchemy.engine import Dialect, Engine
-from sqlalchemy.ext.compiler import compiles
 from sqlalchemy.ext.declarative import declarative_base
 
 FILE_CHUNK_SIZE = 1000
 
 
-@compiles(DropTable, "postgresql")
-def _compile_drop_table(element, compiler, **kwargs):
-    return compiler.visit_drop_table(element) + " CASCADE"
-
-
 class ORMSession:
     """
     A context manager for sessions.
 
     Most of the time, function calls will be passed to the underlying session object.
 
     Should not be instantiated manually. Call ORM.session() to instantiate.
@@ -129,17 +122,17 @@
 
     This should be treated identically to a sqlalchemy declarative base object.
 
     :see: https://docs.sqlalchemy.org/en/13/orm/index.html
     """
 
     __tablename__: str
-    __hidden_columns__: list[str]
-    __hidden_relationships__: list[str]
-    __default_hidden_columns__: list[str]
+    __hidden_columns__: List[str]
+    __hidden_relationships__: List[str]
+    __default_hidden_columns__: List[str]
 
     @classmethod
     def Relationship(cls, **kwargs: Any) -> InstrumentedAttribute:
         """
         Declare a relationship within a class structure.
 
         Usage is like so::
@@ -189,42 +182,42 @@
         to build a foreign key to that class.
         """
         return ForeignKey("{0}.{1}".format(cls.__tablename__, column), **kwargs)
 
     @classmethod
     def Hide(
         cls,
-        columns: Optional[Union[list[str], str]] = [],
-        relationships: Optional[Union[list[str], str]] = [],
+        columns: Optional[Union[List[str], str]] = [],
+        relationships: Optional[Union[List[str], str]] = [],
     ) -> None:
         """
         Configures columns and relationships that will
         not be passed through in a format() call.
         """
-        existing_columns: list[str] = []
+        existing_columns: List[str] = []
         existing_columns.extend(getattr(cls, "__hidden_columns__", []))
         if not isinstance(columns, list):
-            columns = cast(list[str], [columns])
+            columns = cast(List[str], [columns])
         existing_columns.extend(columns)
         setattr(cls, "__hidden_columns__", existing_columns)
 
-        existing_relationships: list[str] = []
+        existing_relationships: List[str] = []
         existing_relationships.extend(getattr(cls, "__hidden_relationships__", []))
         if not isinstance(relationships, list):
-            relationships = cast(list[str], [relationships])
+            relationships = cast(List[str], [relationships])
         existing_relationships.extend(relationships)
         setattr(cls, "__hidden_relationships__", existing_relationships)
 
     @classmethod
-    def DefaultHide(cls, *columns: str):
+    def DefaultHide(cls, *columns: str) -> None:
         """
         Configures columns that will, by default, not be passed through
         in a format() call, but can be requested.
         """
-        existing_columns: list[str] = []
+        existing_columns: List[str] = []
         existing_columns.extend(getattr(cls, "__default_hidden_columns__", []))
         existing_columns.extend(columns)
         setattr(cls, "__default_hidden_columns__", existing_columns)
 
     @staticmethod
     def _is_sqlalchemy_data(value: Any) -> bool:
         """
@@ -280,15 +273,15 @@
 
         response = {
             "type": type(self).__name__.replace("Declarative", ""),
             "attributes": attributes,
         }
 
         if "include" in kwargs and kwargs["include"]:
-            include: dict[str, Optional[list[Optional[ORMObjectBase]]]] = {}
+            include: Dict[str, Optional[List[Optional[ORMObjectBase]]]] = {}
             include_paths = kwargs["include"]
             hidden_relationships = getattr(self, "__hidden_relationships__", [])
 
             if not isinstance(include_paths, list):
                 include_paths = [include_paths]
 
             for include_path in include_paths:
@@ -329,15 +322,15 @@
                 else:
                     formatter = lambda i: i.format()
 
                 if included_item is None:
                     include[include_path] = None
                 else:
                     include[include_path] = [
-                        None if item is None else formatter(item)
+                        None if item is None else formatter(item)  # type: ignore
                         for item in included_item
                     ]
             response["include"] = include
 
         see = getattr(self, "__see_also__", [])
         if see:
             response["see"] = [
@@ -351,32 +344,32 @@
     def solidify(self) -> ORMSolidifiedObject:
         """
         Returns the "solidified" object (removing sqlalchemy state.)
         """
         return ORMSolidifiedObject(**self.get_attributes())
 
     @classmethod
-    def _declared_functions(cls) -> dict[str, Callable]:
+    def _declared_functions(cls) -> Dict[str, Callable]:
         """
         Gets the functions that will pass through into the results of the session queries.
         """
         return {
             "format": cls.format,
             "solidify": cls.solidify,
             "see": cls.see,
             "get_attributes": cls.get_attributes,
         }
 
     @classmethod
-    def _declared_dict(cls, orm) -> dict[str, Any]:
+    def _declared_dict(cls, orm: ORM) -> Dict[str, Any]:
         """
         Gets class variables necessary to declare an object inherited a declarative base.
         """
         _declared = cls._declared_functions()
-        _declared["__orm__"] = orm
+        _declared["__orm__"] = orm  # type: ignore
         _vars = vars(cls)
         for mapped in _vars:
             if isinstance(_vars[mapped], sqlalchemy.Column):
                 setattr(_vars[mapped], "__orm__", orm)
                 setattr(_vars[mapped].type, "__orm__", orm)
             _declared[mapped] = _vars[mapped]
         return _declared
@@ -393,15 +386,15 @@
                 logger.info(
                     "Ignoring subclass {0} due to lack of __tablename__ attribute. If this is not intentional, declare a __tablename__ to migrate this subclass.".format(
                         subcls.__name__
                     )
                 )
 
 
-class ORMEncryptedStringType(sqlalchemy.types.TypeDecorator):
+class ORMEncryptedStringType(sqlalchemy.types.TypeDecorator):  # type: ignore
     """
     Using `pibble.util.AESCipher`, encrypt values on their way into the database,
     and decrypt values on their way out of the database. Use the same way you'd use sqlalchemy.String.
 
     See the class in pibble.util for additional info, but the gist is that you
     should either pass a static password (string) and salt (string, 8 bytes base64-encoded),
     or a key (string, 32 bytes base64-encoded) as the seed for the cipher. If you don't
@@ -415,15 +408,15 @@
     def process_bind_param(self, value: str, dialect: Dialect) -> str:
         return decode(self.__orm__.cipher.encrypt(value))
 
     def process_result_value(self, value: str, dialect: Dialect) -> str:
         return decode(self.__orm__.cipher.decrypt(value))
 
 
-class ORMEncryptedTextType(sqlalchemy.types.TypeDecorator):
+class ORMEncryptedTextType(sqlalchemy.types.TypeDecorator):  # type: ignore
     """
     Using `pibble.util.AESCipher`, encrypt values on their way into the database,
     and decrypt values on their way out of the database. Use the same way you'd use sqlalchemy.String.
 
     See the class in pibble.util for additional info, but the gist is that you
     should either pass a static password (string) and salt (string, 8 bytes base64-encoded),
     or a key (string, 32 bytes base64-encoded) as the seed for the cipher. If you don't
@@ -437,41 +430,41 @@
     def process_bind_param(self, value: str, dialect: Dialect) -> str:
         return decode(self.__orm__.cipher.encrypt(value))
 
     def process_result_value(self, value: str, dialect: Dialect) -> str:
         return decode(self.__orm__.cipher.decrypt(value))
 
 
-class ORMVariadicType(sqlalchemy.types.TypeDecorator):
+class ORMVariadicType(sqlalchemy.types.TypeDecorator):  # type: ignore
     """
-    Using `pibble.util.FlexibleStringer` and `pibble.util.FlexibleStringer`, serialize values
+    Using `pibble.util.Serializer` and `pibble.util.Serializer`, serialize values
     on their way into the databased, and deserialize them on their way out.
     """
 
     impl = sqlalchemy.String
 
     def process_bind_param(self, value: Any, dialect: Dialect) -> str:
-        return FlexibleStringer.serialize(value)
+        return Serializer.serialize(value)
 
     def process_result_value(self, value: str, dialect: Dialect) -> Any:
-        return FlexibleStringer.parse(value)
+        return Serializer.deserialize(value)
 
 
-class ORMEncryptedVariadicType(sqlalchemy.types.TypeDecorator):
+class ORMEncryptedVariadicType(sqlalchemy.types.TypeDecorator):  # type: ignore
     """
     Combines the encrypted and variadic types.
     """
 
     impl = sqlalchemy.String
 
     def process_bind_param(self, value: Any, dialect: Dialect) -> str:
-        return decode(self.__orm__.cipher.encrypt(FlexibleStringer.serialize(value)))
+        return decode(self.__orm__.cipher.encrypt(Serializer.serialize(value)))
 
     def process_result_value(self, value: str, dialect: Dialect) -> Any:
-        return FlexibleStringer.parse(decode(self.__orm__.cipher.decrypt(value)))
+        return Serializer.deserialize(decode(self.__orm__.cipher.decrypt(value)))
 
 
 class ORMObject:
     """
     A small class to make isinstance() easier on classes extending the declarative_base()
     """
 
@@ -505,31 +498,31 @@
     >>> session.get().query(builder.user).first().id
     1
 
     :param engine sqlalchemy.Engine: The engine to use with this ORM.
     :param base type: The type to check for subclasses of. Note that subclass checking is not recursive.
     """
 
-    bases: list[Type[ORMObjectBase]]
-    models: dict[str, Type]
+    bases: List[Type[ORMObjectBase]]
+    models: Dict[str, Type]
 
     def __init__(
         self,
         engine: Engine,
         migrate: bool = False,
         force: bool = False,
-        base: Union[Type[ORMObjectBase], list[Type[ORMObjectBase]]] = ORMObjectBase,
+        base: Union[Type[ORMObjectBase], List[Type[ORMObjectBase]]] = ORMObjectBase,
         cipher: Optional[AESCipher] = AESCipher(),
     ):
         self.engine = engine
         self.bases = []
         self.models = {}
 
         if type(base) is not list:
-            base = cast(list[Type[ORMObjectBase]], [base])
+            base = cast(List[Type[ORMObjectBase]], [base])
 
         for object_base in base:
             if type(object_base) is not type:
                 object_base = resolve(object_base)
             self.bases.append(object_base)
 
         self.declarative_base = declarative_base(self.engine)
@@ -565,27 +558,27 @@
         try:
             table = sqlalchemy.Table(tablename, metadata, autoload=True)
             logger.info("Removing existing table {0}.".format(tablename))
             table.drop()
         except sqlalchemy.exc.NoSuchTableError:
             pass
 
-    def __getattr__(self, name) -> Type:
+    def __getattr__(self, name: str) -> Type:
         if name in self.models:
-            return self.models[name]
+            return self.models[name]  # type: ignore
         raise AttributeError(f"Model {name} not defined.")
 
     def extend(
         self,
         name: str,
-        clsdict: dict[str, Any],
+        clsdict: Dict[str, Any],
         cls: Type = ORMObject,
         force: bool = False,
         create: bool = True,
-    ):
+    ) -> Type:
         """
         Extends the underlying ORM layer with the object itself. Likely won't be
         called directly by implementing applications. If the ORM was instantiated
         with an ORMObjectBase base class which had declared subclasses at the time
         of instantiation, those subclasses will be automatically bound to the underlying
         layer. This is only necessary to be used *after* initial instantiation. This
         is most useful for mix-ins that need an ORM model.
@@ -683,15 +676,15 @@
 
 class ORMBuilder(ORM):
     """
     A simple helper for building an ORM programmatically.
     """
 
     def __init__(
-        self, engine_type: str, engine_kwargs: dict[str, Any] = {}, **kwargs: Any
+        self, engine_type: str, engine_kwargs: Dict[str, Any] = {}, **kwargs: Any
     ):
         self.engine_type = engine_type
         self.engine_kwargs = engine_kwargs
         self.init_kwargs = kwargs
         super(ORMBuilder, self).__init__(
             EngineFactory.singleton(self.engine_type, **self.engine_kwargs),
             **self.init_kwargs,
```

### Comparing `pibble-0.4.9/pibble/database/util.py` & `pibble-0.5.0/pibble/database/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sqlalchemy.types
 
 from sqlalchemy.sql.type_api import TypeEngine as SQLAlchemyType
 
-from typing import Type, Any
+from typing import Type, Any, Iterator
 from pandas import Timestamp
 from numpy import int64, float64
 from datetime import datetime, date, time, timedelta
 from decimal import Decimal
 
 
 def sqlalchemy_type_from_python_type(python_type: Type) -> SQLAlchemyType:
@@ -53,15 +53,15 @@
     >>> rp = RowProxy(foo = "bar", bar = "baz")
     >>> [r for r in rp]
     ['bar', 'baz']
 
     :param kwargs dict: Any number of keywords arguments.
     """
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Any]:
         return iter(self.values())
 
 
 def row_to_dict(row: Any) -> dict:
     """
     Turns a row into a dictionary. See :class:pibble.database.util.RowProxy for why this is necessary.
```

### Comparing `pibble-0.4.9/pibble/ext/cms/database/__init__.py` & `pibble-0.5.0/pibble/ext/cms/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/ext/cms/database/interface.py` & `pibble-0.5.0/pibble/ext/cms/database/interface.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/ext/cms/database/menu.py` & `pibble-0.5.0/pibble/ext/cms/database/menu.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/ext/cms/database/view.py` & `pibble-0.5.0/pibble/ext/cms/database/view.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/ext/cms/server/base.py` & `pibble-0.5.0/pibble/ext/cms/server/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,70 @@
+from typing import Optional
+
 from pibble.util.log import logger
+from pibble.api.exceptions import ConfigurationError
 from pibble.api.server.webservice.template import (
     TemplateServer,
     TemplateServerHandlerRegistry,
 )
 from pibble.api.middleware.database.orm import ORMMiddlewareBase
 from pibble.ext.dam.server.base import DAMServerBase
 
-from pibble.ext.cms.database.base import CMSExtensionObjectBase
-from pibble.ext.cms.server.mixin import CMSExtensionContextMixin
+from pibble.ext.cms.middleware import CMSExtensionContextMiddleware
+from pibble.ext.cms.database import *
 
 
 handlers = TemplateServerHandlerRegistry()
 
 
 class CMSServerBase(
-    TemplateServer, DAMServerBase, CMSExtensionContextMixin, ORMMiddlewareBase
+    TemplateServer, DAMServerBase, CMSExtensionContextMiddleware, ORMMiddlewareBase
 ):
     @classmethod
     def get_handlers(cls) -> TemplateServerHandlerRegistry:
         return handlers
 
-    def migrate_taxonomies(self):
+    def migrate_taxonomies(self) -> None:
+        """
+        Updates configured taxonomies in database at runtime
+        """
         with self.orm.session() as session:
             taxonomies = session.query(self.orm.Taxonomy).all()
 
             for taxonomy in self.configuration["cms.taxonomies"]:
                 if "name" not in taxonomy:
                     raise ConfigurationError("Taxonomies require a name.")
 
                 name = taxonomy["name"]
-                existing = [t for t in taxonomies if t.name == name]
+                existing_list: list[Taxonomy] = [
+                    t for t in taxonomies if t.name == name
+                ]
+                existing: Optional[Taxonomy] = (
+                    None if not existing_list else existing_list[0]
+                )
 
-                if existing:
+                if existing is not None:
                     logger.debug(f"Found existing taxonomy {name}, updating.")
-                    existing = existing[0]
                     existing.label = taxonomy.get("label", name)
                     existing.hierarchical = taxonomy.get("hierarchical", False)
                 else:
                     logger.debug(f"Creating new taxonomy {name}.")
                     taxonomy_object = self.orm.Taxonomy(
                         name=name,
                         label=taxonomy.get("label", name),
                         active=True,
                         hierarchical=taxonomy.get("hierarchical", False),
                     )
                     session.add(taxonomy_object)
                     session.commit()
 
-    def migrate_interfaces(self):
+    def migrate_interfaces(self) -> None:
+        """
+        Updates configured interfaces in database at runtime
+        """
         with self.orm.session() as session:
             interfaces = session.query(self.orm.Interface).all()
             for interface in self.configuration["cms.interfaces"]:
                 if "name" not in interface:
                     raise ConfigurationError("Interfaces require a name.")
 
                 name = interface["name"]
@@ -103,19 +116,17 @@
                             )
                         )
 
                 for parameter in interface_object.parameters:
                     configured = [p for p in parameters if p.name == parameter["name"]]
 
                     if configured:
-                        parameter.ptype = configured[0]["ptype"]
-                        parameter.required = configured[0].get("required", False)
-                        parameter.label = configured[0].get(
-                            "label", configured[0]["name"]
-                        )
+                        parameter["ptype"] = configured[0].ptype  # type: ignore
+                        parameter["required"] = configured[0].required  # type: ignore
+                        parameter["label"] = configured[0].label  # type: ignore
                     else:
                         session.remove(parameter)
 
                 for parameter in parameters:
                     if parameter["name"] not in [
                         p.name for p in interface_object.parameters
                     ]:
@@ -128,15 +139,15 @@
                                 required=parameter.get("required", False),
                                 values=parameter.get("values", []),
                             )
                         )
 
             session.commit()
 
-    def on_configure(self):
+    def on_configure(self) -> None:
         """
         Look for configured views, update database if necessary.
         """
         self.orm.extend_base(
             CMSExtensionObjectBase,
             force=self.configuration.get("orm.force", False),
             create=self.configuration.get("orm.create", True),
```

### Comparing `pibble-0.4.9/pibble/ext/cms/server/extension.py` & `pibble-0.5.0/pibble/ext/cms/server/extension.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     This can be used as follows::
       <a href="{% resolve "Articles" %}">All Articles</a>
 
     """
 
     tags = {"resolve"}
 
-    def __call__(self, *args: Any):
+    def __call__(self, *args: Any) -> str:
         if not args:
             raise ValueError("View name is required.")
         view = str(args[0])
         kwargs = args[1] if len(args) == 2 else {}
         logger.debug(
             "Resolving statement for view {0} with arguments {1}".format(view, kwargs)
         )
@@ -75,15 +75,15 @@
         <a href="{{ resolve("Articles", id = article.id) }}">{{ article.name }}</a>
       {% endfor %}
 
     """
 
     name = "resolve"
 
-    def __call__(self, *args: Any):
+    def __call__(self, *args: Any) -> str:
         if not args:
             raise ValueError("View name is required.")
         view = str(args[0])
         kwargs = args[1] if len(args) == 2 else {}
         logger.debug(
             "Resolving function for view {0} with arguments {1}".format(view, kwargs)
         )
```

### Comparing `pibble-0.4.9/pibble/ext/dam/database/files.py` & `pibble-0.5.0/pibble/ext/dam/database/files.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/ext/rest/server/base.py` & `pibble-0.5.0/pibble/ext/rest/server/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     NotFoundError,
     PermissionError,
 )
 from pibble.api.server.webservice.handler import WebServiceAPIHandlerRegistry
 from pibble.api.server.webservice.orm import ORMWebServiceAPIServer
 from pibble.database.orm import ORMSession, ORMObjectBase
 from pibble.util.log import logger
-from pibble.util.strings import FlexibleStringer, pretty_print, pretty_print_sentence
+from pibble.util.strings import Serializer, pretty_print, pretty_print_sentence
 
 from webob import Request, Response
 
-from typing import Any, Callable
+from typing import Any, Callable, List
 
 DEFAULT_LIMIT = 100
 
 
 handlers = WebServiceAPIHandlerRegistry()
 
 
@@ -104,37 +104,37 @@
             )
 
         def apply_filters(
             query: Query,
             obj: ORMObjectBase,
             column: str,
             value: str,
-            filter_func: Callable[[QueryableAttribute, str], None],
+            filter_func: Callable[[QueryableAttribute, str], Any],
         ) -> Query:
             or_split = column.split("|")
             and_split = column.split("+")
             value_or_split = value.split("|")
 
             def apply_column(column: str) -> ColumnElement:
                 negate = False
                 if column[0] == "!":
                     column = column[1:]
                     negate = True
                 if len(value_or_split) > 1:
                     condition = or_(
                         *[
                             filter_func(
-                                getattr(obj, column), FlexibleStringer.parse(value_part)
+                                getattr(obj, column), Serializer.deserialize(value_part)
                             )
                             for value_part in value_or_split
                         ]
                     )
                 else:
                     condition = filter_func(
-                        getattr(obj, column), FlexibleStringer.parse(value)
+                        getattr(obj, column), Serializer.deserialize(value)
                     )
                 if negate:
                     return not_(condition)
                 return condition
 
             if len(or_split) > 1:
                 query = query.filter(
@@ -187,31 +187,31 @@
         return query, count
 
     @classmethod
     def get_scoped_handler(
         cls,
         handler_classname: str,
         handler_root: str,
-        handler_parent: list[str],
+        handler_parent: List[str],
         handler_scope: str,
         **scope: Any,
-    ) -> Callable[[RESTExtensionServerBase, Request, Response], list[ORMObjectBase]]:
+    ) -> Callable[[RESTExtensionServerBase, Request, Response], List[ORMObjectBase]]:
         """
         Returns a rest handler that has been properly handler_scoped to be callable when registering
         with a handler registry.
 
         See the handler_root class for descriptions, as they correspond to the configuration values.
         """
 
         def rest_handler(
             self: RESTExtensionServerBase,
             request: Request,
             response: Response,
             **kwargs: Any,
-        ) -> list[ORMObjectBase]:
+        ) -> List[ORMObjectBase]:
             method = request.method.upper()
 
             if hasattr(self, "database"):
                 session = self.database
                 autoclose = False
             elif not hasattr(self, "orm"):
                 raise ConfigurationError(
@@ -320,17 +320,17 @@
             return result
 
         return rest_handler
 
     def bind_rest_handler(
         self,
         handler_classname: str,
-        handler_methods: list[str],
+        handler_methods: List[str],
         handler_root: str,
-        handler_parent: list[str],
+        handler_parent: List[str],
         handler_scope: str,
         handler_regex: str,
         **scope: Any,
     ) -> None:
         """
         Builds the scoped handler, then binds it to the handler registry.
```

### Comparing `pibble-0.4.9/pibble/ext/rest/server/user.py` & `pibble-0.5.0/pibble/ext/rest/server/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,164 @@
-from pibble.util.log import logger
+from typing import Callable, Any, List, Dict, Literal
+from typing_extensions import Self
+
+from webob import Request, Response
+
 from pibble.api.exceptions import PermissionError, BadRequestError
 from pibble.ext.user.server.base import (
     UserExtensionServer,
     UserExtensionHandlerRegistry,
 )
 from pibble.ext.rest.server.base import RESTExtensionServerBase
+from pibble.ext.user.database import *
 
 handlers = UserExtensionHandlerRegistry()
 
 
 class UserRESTExtensionServerBase(UserExtensionServer, RESTExtensionServerBase):
     @classmethod
-    def get_handlers(cls):
+    def get_handlers(cls) -> UserExtensionHandlerRegistry:
         return handlers
 
+    def grant_permission_to_group(
+        self, permission: Permission, user_permission_group: UserPermissionGroup
+    ) -> None:
+        """
+        Grants a permission to a user group, if it does not already have it.
+        """
+        existing = (
+            self.database.query(self.orm.PermissionGroupPermission)
+            .filter(
+                self.orm.PermissionGroupPermission.group_id
+                == user_permission_group.group_id
+            )
+            .filter(self.orm.PermissionGroupPermission.permission_id == permission.id)
+            .one_or_none()
+        )
+
+        if not existing:
+            self.database.add(
+                self.orm.PermissionGroupPermission(
+                    permission_id=permission.id,
+                    group_id=user_permission_group.group_id,
+                )
+            )
+            self.database.commit()
+
+    def grant_permission_to_user(self, permission: Permission, user: User) -> None:
+        """
+        Grants a permission to a user, if they do not already have it.
+        """
+        existing = (
+            self.database.query(self.orm.UserPermission)
+            .filter(self.orm.UserPermission.user_id == user.id)
+            .filter(self.orm.UserPermission.permission_id == permission.id)
+            .one_or_none()
+        )
+
+        if not existing:
+            self.database.add(
+                self.orm.UserPermission(
+                    permission_id=permission.id,
+                    user_id=user.id,
+                )
+            )
+            self.database.commit()
+
+    def grant_permission_after_create(
+        self,
+        user: User,
+        grant_type: Literal["user", "group"],
+        action: Literal["create", "read", "update", "delete"],
+        object_name: str,
+        explicit_scope_attribute: str,
+        explicit_scope_value: str,
+    ) -> None:
+        """
+        Grants a permission after creation.
+        """
+        permission = (
+            self.database.query(self.orm.Permission)
+            .filter(self.orm.Permission.action == action)
+            .filter(self.orm.Permission.object_name == object_name)
+            .filter(
+                self.orm.Permission.explicit_scope_attribute == explicit_scope_attribute
+            )
+            .filter(self.orm.Permission.explicit_scope_value == explicit_scope_value)
+            .one_or_none()
+        )
+
+        if not permission:
+            permission = self.orm.Permission(
+                action=action,
+                object_name=object_name,
+                scope_type="explicit",
+                explicit_scope_attribute=explicit_scope_attribute,
+                explicit_scope_value=explicit_scope_value,
+            )
+            self.database.add(permission)
+            self.database.commit()
+
+        if grant_type == "group":
+            for user_permission_group in user.permission_groups:  # type: ignore
+                self.grant_permission_to_group(permission, user_permission_group)
+        elif grant_type == "user":
+            self.grant_permission_to_user(permission, user)
+
+    def grant_after(
+        self,
+        user: User,
+        handler_classname: str,
+        handler_scope: str,
+        grant_items: List[Any],
+        grants: Dict[str, List[str]],
+    ) -> None:
+        """
+        Grants configured permissions after creation.
+        """
+        to_grant: List[Dict[str, str]] = []
+
+        for grant_type in grants:
+            for grant_action in grants[grant_type]:
+                for grant_item in grant_items:
+                    scope_value = getattr(grant_item, handler_scope)
+                    permission_data = {
+                        "grant_type": grant_type,
+                        "object_name": handler_classname,
+                        "action": grant_action,
+                        "explicit_scope_attribute": handler_scope,
+                        "explicit_scope_value": scope_value,
+                    }
+                    to_grant.append(permission_data)
+
+        for permission_datum in to_grant:
+            self.grant_permission_after_create(user, **permission_datum)  # type: ignore[arg-type]
+
     @classmethod
     def get_scoped_handler(
-        cls, handler_classname, handler_root, handler_parent, handler_scope, **scope
-    ):
+        cls,
+        handler_classname: str,
+        handler_root: str,
+        handler_parent: List[str],
+        handler_scope: str,
+        **scope: Any
+    ) -> Callable[..., Any]:
+        """
+        Builds the callable handler.
+        """
         handler = RESTExtensionServerBase.get_scoped_handler(
             handler_classname, handler_root, handler_parent, handler_scope, **scope
         )
 
-        def user_rest_scoped_handler(self, request=None, response=None, **kwargs):
+        def user_rest_scoped_handler(
+            self: Self,
+            request: Request = None,
+            response: Response = None,
+            **kwargs: Any
+        ) -> Any:
             action = {
                 "POST": "create",
                 "GET": "read",
                 "DELETE": "delete",
                 "PUT": "update",
             }.get(request.method, None)
 
@@ -48,102 +180,29 @@
                 )
                 if not permission:
                     raise PermissionError(
                         "User {0} is not authorized to {1} on {2}.".format(
                             request.token.user.email, action, handler_classname
                         )
                     )
-            try:
-                result = handler(self, request, response, **kwargs)
-                if action:
-                    after = scope.get("actions", {}).get(action, {})
-                    results = result
-                    if not isinstance(results, list):
-                        results = [results]
-
-                    if "grant" in after:
-                        for grant_type in after["grant"]:
-                            for grant_action in after["grant"][grant_type]:
-                                for result in results:
-                                    scope_value = getattr(result, handler_scope)
-
-                                    permission_data = {
-                                        "scope_type": "explicit",
-                                        "object_name": handler_classname,
-                                        "action": grant_action,
-                                        "explicit_scope_attribute": handler_scope,
-                                        "explicit_scope_value": scope_value,
-                                    }
-
-                                    granted_permission = (
-                                        self.database.query(self.orm.Permission)
-                                        .filter_by(**permission_data)
-                                        .one_or_none()
-                                    )
-
-                                    if not granted_permission:
-                                        granted_permission = self.orm.Permission(
-                                            **permission_data
-                                        )
-                                        self.database.add(granted_permission)
-                                        self.database.commit()
-
-                                    if grant_type == "group":
-                                        for (
-                                            user_group
-                                        ) in request.token.user.permission_groups:
-                                            if (
-                                                self.database.query(
-                                                    self.orm.PermissionGroupPermission
-                                                )
-                                                .filter(
-                                                    self.orm.PermissionGroupPermission.group_id
-                                                    == user_group.group_id
-                                                )
-                                                .filter(
-                                                    self.orm.PermissionGroupPermission.permission_id
-                                                    == permission.id
-                                                )
-                                                .one_or_none()
-                                            ):
-                                                logger.debug(
-                                                    f"REST handler adding permission to group {user_group.group.label} after action '{action}'. Permission permits '{grant_action}' on {handler_classname} for scope {handler_scope} = {scope_value}"
-                                                )
-                                                self.database.add(
-                                                    self.orm.PermissionGroupPermission(
-                                                        group_id=user_group.group_id,
-                                                        permission_id=granted_permission.id,
-                                                    )
-                                                )
-                                                self.database.commit()
-
-                                    elif grant_type == "user":
-                                        if (
-                                            not self.database.query(
-                                                self.orm.UserPermission
-                                            )
-                                            .filter(
-                                                self.orm.UserPermission.user_id
-                                                == request.token.user.id
-                                            )
-                                            .filter(
-                                                Self.orm.UserPermission.permission_id
-                                                == granted_permission.id
-                                            )
-                                            .one_or_none()
-                                        ):
-                                            logger.debug(
-                                                f"REST handler adding permission to user {request.token.user.email} after action '{action}'. Permission permits '{grant_action}' on {handler_classname} for scope {handler_scope} = {scope_value}"
-                                            )
-
-                                            self.database.add(
-                                                self.orm.UserPermission(
-                                                    user_id=request.token.user.id,
-                                                    permission_id=granted_permission.id,
-                                                )
-                                            )
-                                            self.database.commit()
-            except:
-                raise
-            return result
+
+            handler_result = handler(self, request, response, **kwargs)
+
+            if action:
+                after = scope.get("actions", {}).get(action, {})
+                if isinstance(handler_result, list):
+                    results = handler_result
+                else:
+                    results = [handler_result]  # type: ignore[unreachable]
+
+                if "grant" in after:
+                    self.grant_after(
+                        request.token.user,
+                        handler_classname,
+                        handler_scope,
+                        results,
+                        after["grant"],
+                    )
+
+            return handler_result
 
         return user_rest_scoped_handler
```

### Comparing `pibble-0.4.9/pibble/ext/session/database/session.py` & `pibble-0.5.0/pibble/ext/session/database/session.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/ext/session/server/base.py` & `pibble-0.5.0/pibble/ext/session/server/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 
-from typing import Any, Optional
+from typing import Any, Optional, cast
 
 from webob import Request, Response
 
 from pibble.util.strings import get_uuid
 from pibble.database.orm import ORMSession, ORM
 from pibble.api.server.webservice.orm import ORMWebServiceAPIServer
 from pibble.api.exceptions import ConfigurationError
@@ -30,23 +30,29 @@
         try:
             return self[key]
         except KeyError:
             if default is NoDefaultProvided:
                 raise
             return default
 
-    def _get_session_datum(self, key: str) -> SessionDatum:
-        return (
+    def _get_session_datum(self, key: str) -> Optional[SessionDatum]:
+        """
+        Gets the underlying session datum
+        """
+        result = (
             self.database.query(self.orm.SessionDatum)
             .filter(
                 self.orm.SessionDatum.session_token == self.cookie,
                 self.orm.SessionDatum.key == key,
             )
             .one_or_none()
         )
+        if result is None:
+            return None
+        return cast(SessionDatum, result)
 
     def __getitem__(self, key: str) -> Any:
         result = self._get_session_datum(key)
         if not result:
             raise KeyError(key)
         return result.value
 
@@ -92,15 +98,15 @@
                 response.status_code = 301
                 response.location = "/"
 
     """
 
     def parse(
         self, request: Optional[Request] = None, response: Optional[Response] = None
-    ):
+    ) -> None:
         if request is not None and not hasattr(request, "session"):
             cookie = request.cookies.get(self.session_cookie_name, None)
 
             if cookie:
                 result = (
                     self.database.query(self.orm.Session)
                     .filter(self.orm.Session.token == cookie)
@@ -133,9 +139,9 @@
             raise ConfigurationError("No ORM configured, cannot use session extension.")
         self.orm.extend_base(
             SessionExtensionObjectBase,
             force=self.configuration.get("orm.force", False),
             create=self.configuration.get("orm.create", True),
         )
         self.session_cookie_name = self.configuration.get(
-            "session.cookie", "pibbledata_session"
+            "session.cookie", "pibble_session"
         )
```

### Comparing `pibble-0.4.9/pibble/ext/user/client/base.py` & `pibble-0.5.0/pibble/ext/user/client/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from typing import Any
 from pibble.util.log import logger
 from pibble.api.client.webservice.base import WebServiceAPIClientBase
 
 
 class UserExtensionClientBase(WebServiceAPIClientBase):
     """
     A small class that adds the 'login' method to get a token and set authorization.
     """
 
-    def login(self, email: str, password: str) -> dict:
+    def login(self, email: str, password: str) -> Any:
         """
         Logs in, in accordance with the schema set by `UserExtensionServerBase`.
 
         :param email str: The email address of the user to log in as.
         :param password str: The password of the user to log in as.
         :returns dict: The login response.
         """
```

### Comparing `pibble-0.4.9/pibble/ext/user/database/__init__.py` & `pibble-0.5.0/pibble/ext/user/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/ext/user/database/authentication.py` & `pibble-0.5.0/pibble/ext/user/database/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/ext/user/database/notification.py` & `pibble-0.5.0/pibble/ext/user/database/notification.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/ext/user/database/permission.py` & `pibble-0.5.0/pibble/ext/user/database/permission.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/ext/user/database/user.py` & `pibble-0.5.0/pibble/ext/user/database/user.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/ext/user/server/base.py` & `pibble-0.5.0/pibble/ext/user/server/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,25 +41,25 @@
     def __init__(
         self,
         fn: Callable,
         secured: bool = False,
         object_name: Optional[str] = None,
         action: Optional[str] = None,
         secondary_action: Optional[str] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         super(UserExtensionHandler, self).__init__(fn, **kwargs)
         self.secured = secured
         self.object_name = object_name
         self.action = action
         self.secondary_action = secondary_action
 
     def _check_permissions(
         self, server: UserExtensionServerBase, request: Request, **kwargs: Any
-    ):
+    ) -> None:
         if getattr(self, "secured", False):
             if not getattr(request, "token", None):
                 raise AuthenticationError("Invalid or no credentials supplied.")
 
             if self.object_name is not None and self.action is not None:
                 server.assert_user_permission(
                     request,
@@ -88,15 +88,15 @@
         object_name: Optional[Union[str, Type]] = None,
         action: Optional[str] = None,
         secondary_action: Optional[str] = None,
     ) -> Callable[[Callable], Callable]:
         if type(object_name) is type:
             object_name = object_name.__name__
 
-        def wrap(fn: Callable):
+        def wrap(fn: Callable) -> Callable:
             self.create_or_modify_handler(
                 fn,
                 secured=True,
                 object_name=cast(str, object_name),
                 action=action,
                 secondary_action=secondary_action,
             )
@@ -223,15 +223,15 @@
             )
 
         return permission_query.all()
 
     def check_user_permission(
         self,
         user: User,
-        object_name: str,
+        subject: Any,
         action: str,
         secondary_action: Optional[str] = None,
         **kwargs: Any,
     ) -> bool:
         """
         Check a user's permission to perform an individual action.
 
@@ -242,28 +242,27 @@
         :param kwargs dict: All values passed into the check_permission function. See it for details.
         :returns boolean: Whether or not a user has permission to do the requested scoped action.
         """
 
         if user.superuser:
             return True
 
-        if type(object_name) is type:
-            object_name = object_name.__name__
+        object_name = getattr(subject, "__name__", str(subject))
 
         logger.debug(
             "Checking permissions on user {0} for object {1}, action {2}, secondary action {3}".format(
                 user.email, object_name, action, secondary_action
             )
         )
 
         for permission in self.find_permissions_by_user(
             user, object_name, action=action, secondary_action=secondary_action
         ):
             if self.check_permission(user, permission, **kwargs):
-                return permission
+                return True
         return False
 
     def assert_user_permission(
         self,
         request: Request,
         object_name: str,
         action: str,
@@ -532,15 +531,15 @@
         )
 
         user.last_login = datetime.datetime.now()
 
         self.database.add(token)
         self.database.commit()
 
-        return token
+        return cast(AuthenticationToken, token)
 
     def bypass_login(self, request: Request, response: Response) -> AuthenticationToken:
         """
         Generates a 'noauth' authentication token.
         """
         user = (
             self.database.query(self.orm.User)
@@ -560,15 +559,15 @@
         )
 
         user.last_login = datetime.datetime.now()
 
         self.database.add(token)
         self.database.commit()
 
-        return token
+        return cast(AuthenticationToken, token)
 
 
 handlers = UserExtensionHandlerRegistry()
 
 
 class UserExtensionServer(UserExtensionServerBase):
     """
@@ -591,28 +590,28 @@
     @handlers.path("^/self$")
     def get_self(self, request: Request, response: Response) -> User:
         user = (
             self.database.query(self.orm.User)
             .filter(self.orm.User.id == request.token.user_id)
             .one()
         )
-        return user
+        return cast(User, user)
 
 
 class UserExtensionTemplateServer(UserExtensionServerBase, TemplateServer):
     """
     This avoids default handler registration and adds cookies, since the template server
     will likely be acting through a browser.
     """
 
     def on_configure(self) -> None:
         """
         On configure, grab the cookie name from config.
         """
-        self.cookie = self.configuration.get("user.cookie", "pibbledata_token")
+        self.cookie = self.configuration.get("user.cookie", "pibble_token")
 
     def set_token_cookie(self, response: Response, token: AuthenticationToken) -> None:
         """
         Sets the cookie on the response object that contains the token.
         """
         response.set_cookie(
             self.cookie,
```

### Comparing `pibble-0.4.9/pibble/hooks/aws.py` & `pibble-0.5.0/pibble/hooks/aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 import json
 import yaml
 import logging
 import traceback
 
-from typing import Optional, Union
+from typing import Optional, Union, Any, cast
 
 from pibble.util.helpers import qualify, resolve, FlexibleJSONDecoder
 from pibble.resources.retriever import Retriever
 from pibble.database.orm import ORMBuilder
 from pibble.api.meta.helpers import MetaFactory, MetaService
 from pibble.api.server.webservice.awslambda import (
     LambdaRequestPayloadV1,
@@ -37,15 +37,15 @@
     """
     Checks if the debug environment variable is set.
     """
     debug_str = os.environ.get("PIBBLEDEBUG", None)
     return isinstance(debug_str, str) and debug_str.lower()[0] in ["t", "y", "1"]
 
 
-def get_config_from_file(config_file: str) -> dict:
+def get_config_from_file(config_file: str) -> Any:
     """
     Loads config from a file.
 
     Supports any protocol supported by the retriever (file, http, s3, ftp, sftp, etc.)
     """
     logger.debug(f"Retrieving configuration file {config_file}")
     retriever = Retriever.get(config_file)
@@ -144,15 +144,17 @@
                         "event": event,
                     }
                 ),
             }
     if service is not None:
         try:
             logger.debug("Service loaded, handling lambda request.")
-            return service.handle_lambda_request(event, context)
+            return cast(
+                LambdaResponseDict, service.handle_lambda_request(event, context)
+            )
         except Exception as ex:
             if debug_mode():
                 return {
                     "statusCode": 500,
                     "multiValueHeaders": {},
                     "headers": {"Content-Type": "application/json"},
                     "body": json.dumps(
```

### Comparing `pibble-0.4.9/pibble/media/thumbnail.py` & `pibble-0.5.0/pibble/media/thumbnail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import re
 import subprocess
 
 from typing import Optional, Any
+from pibble.util.strings import decode
 from pibble.util.log import logger
 
 try:
     from PIL import ImageChops, Image
 except ImportError:
     logger.warning(
         "Cannot import imaging libraries. Make sure to install with the [imaging] option selected if imaging functionality is required."
@@ -81,15 +82,15 @@
     making this method a synchronous subprocess call.
     """
     logger.debug(f"Calling subprocess with args {args}, kwargs {kwargs}.")
     p = subprocess.Popen(*args, **kwargs)
     out, err = p.communicate()
     if p.returncode != 0:
         raise Exception(err)
-    return out
+    return str(decode(out))
 
 
 def TrimImage(image: Image.Image) -> Image.Image:
     """
     Trims an image - i.e., removes empty background space around the 'content'
     of the image.
 
@@ -116,17 +117,21 @@
     an image of that input.
 
     :param filename str: The filename to build an image from. Supports audio, video,
         common productivity document formats, web formats, and image formats. Also
         supports photoshop uses PSDFile.
     """
 
-    EXECUTABLES = ["ffmpeg", "libreoffice", "chromedrivert"]
+    EXECUTABLES = ["ffmpeg", "libreoffice", "chromedriver"]
 
-    def __init__(self, filename):
+    ffmpeg: Optional[str]
+    libreoffice: Optional[str]
+    chromedriver: Optional[str]
+
+    def __init__(self, filename: str) -> None:
         self.filename = filename
         self.ffmpeg = None
         self.libreoffice = None
         self.chromedriver = None
         self._find_executables("ffmpeg", "libreoffice", "chromedriver")
 
     def build(
```

### Comparing `pibble-0.4.9/pibble/resources/retriever.py` & `pibble-0.5.0/pibble/resources/retriever.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import os
 import boto3
 
 from io import IOBase
 from urllib.parse import urlparse, ParseResult
-from typing import Optional, Iterator, Type, Sequence, Union
+from typing import Optional, Iterator, Type, Sequence, Union, List, Dict
 
 from pibble.util.log import logger
 
 from pibble.api.meta.base import MetaService
 from pibble.api.client.webservice.base import WebServiceAPIClientBase
 
 from pibble.api.middleware.webservice.authentication.basic import (
@@ -111,15 +111,15 @@
             configuration_dict["client"]["port"] = str(self.url.port)
 
         api_configuration = APIConfiguration(**configuration_dict)
 
         if self.configuration is not None:
             api_configuration.update(**self.configuration)
 
-        classes: list[Type] = [WebServiceAPIClientBase]
+        classes: List[Type] = [WebServiceAPIClientBase]
         if self.configuration is not None:
             authentication_type = api_configuration.get("authentication.type", None)
             if authentication_type == "oauth":
                 classes.append(OAuthAuthenticationMiddleware)
             elif authentication_type == "basic":
                 classes.append(BasicAuthenticationMiddleware)
             elif authentication_type == "digest":
@@ -143,15 +143,15 @@
             if BasicAuthenticationMiddleware not in classes:
                 classes.append(BasicAuthenticationMiddleware)
 
         self.client = MetaService(
             "HTTPRetrieverClient", classes, api_configuration.configuration
         )
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[bytes]:
         kwargs = {}
         if self.url.params:
             kwargs["parameters"] = self.url.params
 
         with self.client.get(self.url.path, stream=True, **kwargs) as response:
             for chunk in response.iter_content(chunk_size=self.CHUNK_SIZE):
                 yield chunk
@@ -174,15 +174,15 @@
         elif self.url.path:
             self.file_path = self.url.path
         else:
             raise IOError("No path found at URL {0}".format(self.url))
         if not os.path.exists(self.file_path):
             raise NotFoundError("Could not find file at {0}".format(self.file_path))
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[bytes]:
         fp = open(self.file_path, "rb")
         try:
             while True:
                 data = fp.read(self.CHUNK_SIZE)
                 if not data:
                     break
                 yield data
@@ -196,15 +196,15 @@
     """
 
     SCHEMES = ["ftp", "ftps"]
 
     def __init__(self, url: ParseResult, configuration: Optional[dict] = None):
         super(FTPRetriever, self).__init__(url, configuration)
 
-        client_config: dict[str, Union[dict, str, int, None]] = {
+        client_config: Dict[str, Union[dict, str, int, None]] = {
             "host": self.url.hostname,
             "secure": self.url.scheme == "ftps",
             "ftp": {
                 "username": self.url.username,
                 "password": self.url.password,
                 "chunksize": self.CHUNK_SIZE,
             },
@@ -212,52 +212,49 @@
 
         if self.url.port:
             client_config["port"] = self.url.port
 
         self.client = FTPClient()
         self.client.configure(client=client_config)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[bytes]:
         for chunk in self.client.readFile(self.url.path):
             yield chunk.encode("UTF-8")
 
 
 class SFTPRetriever(Retriever):
     """
     Gets data from SFTP (FTP over SSH.)
     """
 
     SCHEMES = ["sftp"]
 
     def __init__(self, url: ParseResult, configuration: Optional[dict] = None):
         super(SFTPRetriever, self).__init__(url, configuration)
 
-        client_config: dict[str, Union[dict, str, int, None]] = {
+        client_config: Dict[str, Union[dict, str, int, None]] = {
             "host": self.url.hostname,
             "sftp": {
                 "username": self.url.username,
                 "password": self.url.password,
                 "chunksize": self.CHUNK_SIZE,
             },
         }
 
         if self.url.port:
             client_config["port"] = self.url.port
 
         self.client_config = client_config
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[bytes]:
         client = SFTPClient()
         client.configure(client=self.client_config)
         try:
             for chunk in client.readFile(self.url.path):
-                if isinstance(chunk, str):
-                    yield chunk.encode("UTF-8")
-                else:
-                    yield chunk
+                yield chunk.encode("UTF-8")
         finally:
             logger.warning("Closing client.")
             try:
                 client.close()
             except:
                 pass
 
@@ -269,15 +266,15 @@
 
     SCHEMES = ["s3"]
 
     def __init__(self, url: ParseResult, configuration: Optional[dict] = None):
         super(S3Retriever, self).__init__(url, configuration)
         self.s3 = boto3.client("s3")
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[bytes]:
         logger.debug(
             f"Getting data from S3 bucket {self.url.hostname},key {self.url.path[1:]}"
         )
         data = self.s3.get_object(Bucket=self.url.hostname, Key=self.url.path[1:])
         for chunk in data["Body"].iter_chunks(chunk_size=self.CHUNK_SIZE):
             yield chunk
```

### Comparing `pibble-0.4.9/pibble/setup.py` & `pibble-0.5.0/pibble/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
-version_minor = "4"
-version_patch = "9"
+version_minor = "5"
+version_patch = "0"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
-    "gunicorn>=20.0,<21.0",
     "jinja2>=3.1,<3.2",
     "lxml>=4.9,<5.0",
     "mimeparse>=0.1",
     "mypy>=1.2,<1.3",
     "openpyxl>=3.1,<4.0",
     "pandas>=2.0,<3.0",
     "paramiko>=3.1,<4.0",
@@ -27,29 +26,30 @@
     "requests>=2.28,<3.0",
     "requests-oauthlib>=1.3,<2.0",
     "semantic-version>=2.10,<3.0",
     "sqlalchemy>=1.4,<2.0",
     "sshpubkeys>=3.3,<4.0",
     "termcolor>=2.2,<3.0",
     "webob>=1.8,<2.0",
-    "werkzeug>=2.2,<3.0",
     "wsgitypes>=0.0.4",
     "xlrd>=2.0,<3.0",
     "zeep>=4.2,<5.0",
 ]
 
 extras_require = {
     "mysql": ["mysqlclient>=2.1,<2.2"],
     "postgresql": ["psycopg2-binary>=2.9,<3.0"],
     "mssql": ["pyodbc>=4.0,<5.0", "sqlalchemy-pyodbc-mssql>=0.1"],
     "thrift": ["thrift>=0.16,<1.0"],
     "grpc": ["grpcio<1.49", "grpcio-tools<1.49"],
     "browser": ["selenium>=4.8,<5.0"],
     "imaging": ["pdf2image>=1.16,<2.0", "pillow>=9.5,<10.0", "psd-tools>=1.9,<2.0"],
     "cherrypy": ["cherrypy>=18.8,<19.0"],
+    "gunicorn": ["gunicorn>=20.0,<21.0"],
+    "werkzeug": ["werkzeug>=2.2,<3.0"],
     "build": [
         "sphinx>=6.2,<6.3",
         "sphinx-rtd-theme>=1.2,<1.3",
         "types-PyYAML>=6.0.12,<6.1",
         "types-chardet>=5.0.4,<6.0",
         "types-requests>=2.29,<3.0",
         "types-termcolor>=1.1.6,<1.2",
@@ -72,15 +72,15 @@
 
 setup(
     name=package_name,
     author="Benjamin Paine",
     author_email="painebenjamin@gmail.com",
     version=f"{version_major}.{version_minor}.{version_patch}",
     packages=find_packages("."),
-    package_data={"pibble": []},
+    package_data={"pibble": ["py.typed"]},
     license="gpl-3.0",
     description="A framework for developing webapps quickly and easily using Python",
     long_description=open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"), "r"
     ).read(),
     long_description_content_type="text/markdown",
     entry_points={
```

### Comparing `pibble-0.4.9/pibble/util/encryption.py` & `pibble-0.5.0/pibble/util/encryption.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from hashlib import sha256, pbkdf2_hmac
 
 from Crypto import Random
 from Crypto.Cipher import AES
 from Crypto.Cipher._mode_cbc import CbcMode as CBCModeCipher
 from Crypto.Protocol.KDF import PBKDF2
 
-from typing import Optional, Tuple, Union, cast
+from typing import Optional, Tuple, Union
 
 from pibble.util.strings import encode, decode
 
 __all__ = ["Password", "AESCipher"]
 
 
 class Password:
@@ -167,15 +167,15 @@
                 # Likely due to new thread
                 Random.atfork()
                 return AESCipher.random(size, False)
             else:
                 raise
 
     @property
-    def b64key(self):
+    def b64key(self) -> bytes:
         """
         Simply encodes the current key in base64. Necessary if you're going to store it later.
 
         >>> from pibble.util.encryption import AESCipher
         >>> from base64 import b64encode
         >>> key = AESCipher.random(AESCipher.KEY_SIZE)
         >>> assert AESCipher(key=key).b64key == b64encode(key)
@@ -189,15 +189,15 @@
         Gets the cipher.
 
         :param iv str: The initialization vector - should be BLOCK_SIZE bytes.
         :returns tuple: A 2-tuple of [initialization vector, cipher].
         """
         if iv is None:
             iv = self.random(AES.block_size)
-        return iv, cast(CBCModeCipher, AES.new(self.key, AES.MODE_CBC, iv))
+        return iv, AES.new(self.key, AES.MODE_CBC, iv)
 
     def encrypt(self, raw: str, iv: Optional[bytes] = None) -> str:
         """
         Encrypts a string and returns the base64 representation.
 
         >>> from pibble.util.encryption import AESCipher
         >>> iv = b'0' * AESCipher.BLOCK_SIZE
```

### Comparing `pibble-0.4.9/pibble/util/files.py` & `pibble-0.5.0/pibble/util/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 __all__ = [
     "TempfileContext",
     "FileIterator",
     "ConfigParser",
     "SpreadsheetParser",
     "IncludeLoader",
     "load_yaml",
+    "load_json",
 ]
 
 
 class IncludeLoader(yaml.SafeLoader):
     """
     This loader allows !include directives in yaml files.
 
@@ -85,15 +86,15 @@
         """
         filename = self.construct_scalar(node)
         if not isinstance(filename, str):
             return None
         if not filename.startswith("/"):
             filename = os.path.join(self._root, filename)
         with open(filename, "r") as fp:
-            return yaml.load(fp, Loader=IncludeLoader)
+            return yaml.load(fp, Loader=IncludeLoader)  # type: ignore
 
 
 IncludeLoader.add_constructor("!include", IncludeLoader.include)
 
 
 def load_yaml(path: str) -> Any:
     """
@@ -125,15 +126,15 @@
     """
     with open(path, "w") as fp:
         fp.write(yaml.dump(to_dump, default_flow_style=False))
 
 
 def load_json(path: str) -> Union[dict, list, str, int, float, bool, None]:
     """
-    Loads a JSON file, using the FlexibleStringer.
+    Loads a JSON file, using the Serializer.
 
     >>> from pibble.util.files import TempfileContext, load_json
     >>> import datetime
     >>> context = TempfileContext()
     >>> context.start()
     >>> path = next(context)
     >>> _ = open(path, "w").write('{"str_key": "abc", "int_key": 4, "float_key": 5.5, "date_key": "2020-01-01", "datetime_key": "2020-01-01T01:00:00"}')
@@ -141,15 +142,15 @@
     {'str_key': 'abc', 'int_key': 4, 'float_key': 5.5, 'date_key': datetime.date(2020, 1, 1), 'datetime_key': datetime.datetime(2020, 1, 1, 1, 0)}
     >>> context.stop()
 
     :param path str: The path to the file to read:
 
     """
     with open(path, "r") as fp:
-        return json.loads(fp.read(), cls=FlexibleJSONDecoder)
+        return json.loads(fp.read(), cls=FlexibleJSONDecoder)  # type: ignore
 
 
 def dump_json(path: str, to_dump: Union[dict, list]) -> None:
     """
     Dumps JSON to a file.
 
     >>> from pibble.util.files import TempfileContext, dump_json
@@ -352,15 +353,15 @@
         self,
         file_path: Union[Iterable[dict], IOBase, str],
         parse: Optional[bool] = None,
         **kwargs: Any,
     ) -> None:
         """
         :param file_path str: The path to the spreadsheet file. Also allows for other IO types.
-        :param parse bool: Whether or not to parse the values using FlexibleStringer.
+        :param parse bool: Whether or not to parse the values using Serializer.
         """
         self.path = file_path
         self.parse = parse
         self.kwargs = kwargs
 
         logger.info(
             "Instantiating spreadsheet iterator on file path {0}".format(str(file_path))
@@ -411,28 +412,28 @@
         return faux
 
     def listIterator(self, include_columns: Optional[bool] = False) -> Iterator[list]:
         """
         Iterates over the spreadsheet in a list.
 
         :param include_columns bool: Whether or not to include columns (i.e. yield them first.). Default false.
-        :returns Iterator[list[Any]]: The iterator over the contents.
+        :returns Iterator[List[Any]]: The iterator over the contents.
         """
         data = self.read(self.path, **self.kwargs)
         if include_columns:
             yield data.columns
         for row in data.values:
             yield row
 
     def dictIterator(self, safe_names: Optional[bool] = False) -> Iterator[dict]:
         """
         Iterates over the spreadsheet in a dict.
 
         :param safe_names bool: Whether ot not to rename column keys to their 'safe' versions. Default false.
-        :returns Iterator[dict[Any]]: The iterator over the contents.
+        :returns Iterator[Dict[Any]]: The iterator over the contents.
         """
         data = self.read(self.path, **self.kwargs)
         columns = data.columns
         if safe_names:
             columns = [safe_name(col) for col in columns]
         self.columns = columns
         for row in data.values:
@@ -442,15 +443,15 @@
         """
         Same as ``listIterator``, but chunks the reading.
 
         Doesn't work for all file types - specifically XML-based types (XLSX)
         can't be read iteratively.
 
         :param chunk_size int: The number of rows to get at once. Default 100.
-        :returns Iterator[list[Any]]: The iterator over the contents.
+        :returns Iterator[List[Any]]: The iterator over the contents.
         """
         for chunk in self.read(self.path, chunksize=chunk_size, **self.kwargs):
             for row in chunk.values:
                 yield row
 
     def chunkedDictIterator(
         self, chunk_size: int = 100, safe_names: Optional[bool] = False
@@ -458,15 +459,15 @@
         """
         Same as ``dictIterator``, but chunks the reading.
 
         Doesn't work for all file types - specifically XML-based types (XLSX)
         can't be read iteratively.
 
         :param chunk_size int: The number of rows to get at once. Default 100.
-        :returns Iterator[dict[Any]]: The iterator over the contents.
+        :returns Iterator[Dict[Any]]: The iterator over the contents.
         """
         if self.read is pd.read_excel:
             # Can't do it
             for row in self.dictIterator(safe_names):
                 yield row
         else:
             for chunk in self.read(self.path, chunksize=chunk_size, **self.kwargs):
```

### Comparing `pibble-0.4.9/pibble/util/helpers.py` & `pibble-0.5.0/pibble/util/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,38 +16,47 @@
     import pwd
 except ImportError:
     pass
 
 from logging import DEBUG
 from distutils import spawn
 
-from typing import Type, Callable, Optional, Iterable, Iterator, Any, Tuple, Union
+from typing import (
+    Type,
+    Callable,
+    Optional,
+    Iterable,
+    Iterator,
+    Any,
+    Tuple,
+    Union,
+    Dict,
+    List,
+)
 from types import FunctionType
 
 from pandas import DataFrame
 from io import StringIO
 
 from numpy import ndarray
 from difflib import unified_diff
 from time import sleep
 from datetime import date, datetime
 from openpyxl import load_workbook
 
 from pibble.util.log import logger
-from pibble.util.strings import truncate, decode, FlexibleStringer
+from pibble.util.strings import truncate, decode, Serializer
 
 __all__ = [
     "url_join",
     "find_executable",
     "qualify",
     "resolve",
     "expect_exception",
     "ignore_exceptions",
-    "human_size",
-    "human_file_size",
     "is_binary",
     "is_binary_file",
     "openpyxl_dataframe",
     "Assertion",
     "CompressedIterator",
     "DecompressedIterator",
     "AttributeDictionary",
@@ -122,15 +131,15 @@
     :param obj object: The object to qualify.
     :returns str: The string name of the object.
     """
     if obj.__class__ in [FunctionType, type]:
         return f"{obj.__module__}.{obj.__name__}"
     module = obj.__module__ if hasattr(obj, "__module__") else obj.__class__.__module__
     if module is None or module == str.__class__.__module__:
-        return obj.__class__.__name__
+        return str(obj.__class__.__name__)
     return f"{module}.{obj.__class__.__name__}"
 
 
 def resolve(qualified_name: Any, local: dict = {}) -> Any:
     """
     Attempts to resolve a name through imports.
 
@@ -640,15 +649,15 @@
         Sleeps for <n> milliseconds.
 
         :param n int | float: The number of milliseconds to wait for.
         """
         sleep(n / 1000)
 
     @staticmethod
-    def until(dt: Union[date, datetime]):
+    def until(dt: Union[date, datetime]) -> None:
         """
         Allows for sleeping until a certain datetime.
 
         :param dt date | datetime: The date or time to wait until/
         """
         while True:
             diff = (dt - datetime.now()).total_seconds()
@@ -675,24 +684,24 @@
     def __init__(self) -> None:
         """
         Initialize IOs for stdout and stderr.
         """
         self.stdout = StringIO()
         self.stderr = StringIO()
 
-    def __enter__(self):
+    def __enter__(self) -> None:
         """
         When entering context, steal system streams.
         """
         self._stdout = sys.stdout
         self._stderr = sys.stderr
         sys.stdout = self.stdout
         sys.stderr = self.stderr
 
-    def __exit__(self, *args):
+    def __exit__(self, *args: Any) -> None:
         """
         When exiting context, return system streams.
         """
         if hasattr(self, "_stdout"):
             sys.stdout = self._stdout
         if hasattr(self, "_stderr"):
             sys.stderr = self._stderr
@@ -733,15 +742,15 @@
         >>> type(p)
         <class 'subprocess.Popen'>
         >>> p.communicate()
         (b'hello\\n', b'')
         >>> p.returncode
         0
         """
-        subprocess_kwargs: dict[str, Any] = {
+        subprocess_kwargs: Dict[str, Any] = {
             "stdout": subprocess.PIPE,
             "stderr": subprocess.PIPE,
         }
         if user is not None and os.name != "nt":
             # Set the env for the subprocess
             user_pw = pwd.getpwnam(user)  # type: ignore
             env = os.environ.copy()
@@ -756,27 +765,27 @@
                 env.update({"PWD": cwd})
             else:
                 env.update({"PWD": os.getcwd()})
 
             subprocess_kwargs["env"] = env
 
             # Generate a demote function as pre-executable
-            def demote(user_id, group_id):
-                def wrapper():
+            def demote(user_id: int, group_id: int) -> Callable[[], None]:
+                def wrapper() -> None:
                     os.setsid()
                     os.setgid(group_id)
                     os.setuid(user_id)
 
                 return wrapper
 
             subprocess_kwargs["preexec_fn"] = demote(user_pw.pw_uid, user_pw.pw_gid)
         if cwd:
             subprocess_kwargs["cwd"] = cwd
 
-        subprocess_command: Union[list[str], str] = [self.executable] + list(args)
+        subprocess_command: Union[List[str], str] = [self.executable] + list(args)
         if shell:
             subprocess_command = shlex.join(subprocess_command)
             subprocess_kwargs["shell"] = True
         logger.debug(
             "Executing subprocess command {0}, kwargs {1}".format(
                 subprocess_command, subprocess_kwargs
             )
@@ -893,15 +902,15 @@
 
 class PythonRunner(ProcessRunner):
     """
     Extends the ProcessRunner to allow calling python modules
     or scripts from within python itself.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         super(PythonRunner, self).__init__(sys.executable)
 
     def module(
         self,
         module: str,
         *args: str,
         sync: bool = True,
@@ -1039,26 +1048,26 @@
         self, string: str, *args: Any
     ) -> Union[dict, list, str, int, float, bool, None]:
         """
         The function called by the decoder - will be passed the raw string of the JSON text.
 
         :param string str: The contents of the JSON to be decoded.
         :returns Any: The decoded value - see the flexible stringer for more details.
-        :see: class:`pibble.helpers.strings.FlexibleStringer`
+        :see: class:`pibble.helpers.strings.Serializer`
         """
-        return FlexibleStringer.parse(string)
+        return Serializer.deserialize(string)  # type: ignore
 
 
 class FlexibleJSONEncoder(json.JSONEncoder):
     """
     Extends the base JSONEncoder to allow for more string formats (incl. dates/times.)
     """
 
     def encode(self, to_encode: Any) -> str:
         """
         The function called by the encoder - will be passed anything, and respond with a string.
 
         :param to_encode Any: The object to encode to a string.
         :returns str: The stringified object.
-        :see: class:`funllib.helpers.strings.FlexibleStringer`
+        :see: class:`funllib.helpers.strings.Serializer`
         """
-        return FlexibleStringer.serialize(to_encode)
+        return Serializer.serialize(to_encode)
```

### Comparing `pibble-0.4.9/pibble/util/imaging.py` & `pibble-0.5.0/pibble/util/imaging.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/util/log.py` & `pibble-0.5.0/pibble/util/log.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.9/pibble/util/numeric.py` & `pibble-0.5.0/pibble/util/numeric.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from math import log, ceil
+from typing import Union
 
-__all__ = ["r8d2o", "o2r8d"]
+__all__ = ["r8d2o", "o2r8d", "human_size"]
 
 
-def r8d2o(value):
+def r8d2o(value: int) -> int:
     """
     Converts a radix-8 decimal value to a proper octal value.
 
     Probably called exactly in one scenario - to turn octal permission values
     from decimal (e.g. 755) to octal (decimal 493, or 0o755).
 
     >>> from pibble.util.numeric import r8d2o
@@ -23,15 +24,15 @@
     o = 0
     for i in range(1, magnitude + 1):
         n = (value // (10 ** (magnitude - i))) % 10
         o |= n << ((magnitude - i) * 3)
     return o
 
 
-def o2r8d(value):
+def o2r8d(value: int) -> int:
     """
     Converts an octal integer to its radix-8 decimal value.
 
     Opposite of r8d20.
 
     >>> from pibble.util.numeric import o2r8d
     >>> o2r8d(493)
@@ -45,15 +46,15 @@
     """
     r8d = 0
     for i in range(ceil(value.bit_length() / 3)):
         r8d += ((value & 0b111 << (i * 3)) >> (i * 3)) * (10**i)
     return r8d
 
 
-def human_size(size):
+def human_size(size: Union[int, float]) -> str:
     """
     Returns a human-readable size, based on a number of bytes.
 
     >>> from pibble.util.numeric import human_size
     >>> human_size(42)
     '42 B'
     >>> human_size(2**10)
@@ -61,10 +62,10 @@
     """
     suffixes = ["B", "KB", "MB", "GB", "TB"]
     suffix_index = 0
     while size > 1000:
         size /= 1000.0
         suffix_index += 1
     if suffix_index == 0:
-        return "{0:d} {1:s}".format(size, suffixes[suffix_index])
+        return "{0:.0f} {1:s}".format(size, suffixes[suffix_index])
     else:
         return "{0:.2f} {1:s}".format(size, suffixes[suffix_index])
```

### Comparing `pibble-0.4.9/pibble/util/strings.py` & `pibble-0.5.0/pibble/util/strings.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import base64
 import string
 import hashlib
 
 import email.parser
 
 from re import compile, sub, split
-from typing import Any, TypedDict, Optional, Union, Tuple, cast
+from typing import Any, TypedDict, Optional, Union, Tuple, Dict, List, cast
 from random import choice, shuffle
 from uuid import uuid4, UUID
 from json import dumps, loads, JSONDecodeError
 from numpy import nan, isnan
 from datetime import datetime, date, time
 from chardet import detect
 from urllib.parse import unquote
@@ -34,27 +34,27 @@
 def try_json_dict_parse(to_parse: str) -> Union[dict, str]:
     """
     Tries to parse JSON to a dict, but returns the string
     if it fails.
     """
     try:
         loaded = loads(to_parse)
-        return dict([(key, FlexibleStringer.parse(loaded[key])) for key in loaded])
+        return dict([(key, Serializer.deserialize(loaded[key])) for key in loaded])
     except JSONDecodeError:
         return to_parse
 
 
 def try_json_list_parse(to_parse: str) -> Union[list, str]:
     """
     Tries to parse JSON to a list, but returns the string
     if it fails.
     """
     try:
         loaded = loads(to_parse)
-        return [FlexibleStringer.parse(i) for i in loaded]
+        return [Serializer.deserialize(i) for i in loaded]
     except JSONDecodeError:
         return to_parse
 
 
 def serialize_image(image: Image.Image, **kwargs: Any) -> str:
     """
     Serializes an image to a base64 Data URI.
@@ -66,39 +66,38 @@
 
 
 def deserialize_image(image_string: str, **kwargs: Any) -> Image.Image:
     """
     Deserializes an image from a base64 Data URI.
     """
     image_bytestring = image_string.split(",")[1]
-    logger.debug(image_bytestring)
     image_bytes = base64.b64decode(image_bytestring)
     return Image.open(io.BytesIO(image_bytes))
 
 
-class FlexibleStringer:
+class Serializer:
     """
     A class that takes a string and attempts to parse it into an object by matching
     it with a regular expression, and vice-versa.
 
-    >>> from pibble.util.strings import FlexibleStringer
+    >>> from pibble.util.strings import Serializer
     >>> from datetime import datetime
-    >>> FlexibleStringer.parse("4")
+    >>> Serializer.deserialize("4")
     4
-    >>> FlexibleStringer.parse("4.0")
+    >>> Serializer.deserialize("4.0")
     4.0
-    >>> FlexibleStringer.parse("true")
+    >>> Serializer.deserialize("true")
     True
-    >>> FlexibleStringer.parse("2018-01-01T00:00:00")
+    >>> Serializer.deserialize("2018-01-01T00:00:00")
     datetime.datetime(2018, 1, 1, 0, 0)
-    >>> FlexibleStringer.serialize(4)
+    >>> Serializer.serialize(4)
     '4'
-    >>> FlexibleStringer.serialize(False)
+    >>> Serializer.serialize(False)
     'false'
-    >>> FlexibleStringer.serialize(datetime(2018, 1, 1))
+    >>> Serializer.serialize(datetime(2018, 1, 1))
     '2018-01-01T00:00:00'
 
     :param parameter str: The string to attempt to parse.
     :returns object: Either the parameter itself, or the parsed version of it.
     """
 
     PARSE_FORMATS = {
@@ -176,25 +175,25 @@
         float: lambda p, **k: str(p),
         dict: lambda p, **k: dump_json(p, **k),
         list: lambda p, **k: dump_json(p, **k),
         bool: lambda p, **k: "true" if p else "false",
     }
 
     @classmethod
-    def parse(cls, parameter: Any, permissive: bool = False) -> Any:
+    def deserialize(cls, parameter: Any, permissive: bool = False) -> Any:
         try:
             if isinstance(parameter, list):
-                return [cls.parse(p) for p in parameter]
+                return [cls.deserialize(p) for p in parameter]
             elif isinstance(parameter, dict):
-                return dict([(p, cls.parse(parameter[p])) for p in parameter])
+                return dict([(p, cls.deserialize(parameter[p])) for p in parameter])
             elif isinstance(parameter, str):
                 test_parameter = parameter.strip().replace("\n", "")
                 for pattern in cls.PARSE_FORMATS:
                     if bool(pattern.match(test_parameter)):
-                        return cls.PARSE_FORMATS[pattern](test_parameter)
+                        return cls.PARSE_FORMATS[pattern](test_parameter)  # type: ignore
         except Exception as ex:
             if permissive:
                 logger.warning(
                     "Couldn't parse parameter {0}, ignoring.".format(parameter)
                 )
                 pass
             else:
@@ -203,15 +202,15 @@
                 )
         return parameter
 
     @classmethod
     def serialize(cls, parameter: Any, **kwargs: Any) -> str:
         for typename in cls.SERIALIZE_FORMATS:
             if type(parameter) is typename:
-                return cls.SERIALIZE_FORMATS[typename](parameter, **kwargs)
+                return cls.SERIALIZE_FORMATS[typename](parameter, **kwargs)  # type: ignore
         return str(parameter)
 
 
 class RandomWordGenerator(object):
     """
     A simple class to generate a random word. Reads from /usr/share/dict/words.
 
@@ -316,17 +315,15 @@
             return None
         elif type(_obj) is list:
             return [_fix_nan(_o) for _o in _obj]
         elif type(_obj) is dict:
             return dict([(_key, _fix_nan(_obj[_key])) for _key in _obj])
         return _obj
 
-    return dumps(
-        _fix_nan(obj), allow_nan=False, default=FlexibleStringer.serialize, **kwargs
-    )
+    return dumps(_fix_nan(obj), allow_nan=False, default=Serializer.serialize, **kwargs)
 
 
 def random_string(
     length: int = 32,
     use_uppercase: bool = True,
     use_lowercase: bool = True,
     use_digits: bool = True,
@@ -421,15 +418,15 @@
         (SENTENCE_CASE, "SENTENCE"),
     ]:
         if bool(test.match(string)):
             return name
     return "UNKNOWN"
 
 
-def guess_string_parts(string: str) -> list[str]:
+def guess_string_parts(string: str) -> List[str]:
     """
     Using guess_case, splits a string into it's constituent parts.
 
     >>> from pibble.util.strings import guess_string_parts
     >>> guess_string_parts('MyString')
     ['my', 'string']
     >>> guess_string_parts('myString')
@@ -441,15 +438,15 @@
     >>> guess_string_parts('my string')
     ['my', 'string']
     """
 
     string = sub(r"[^A-Za-z0-9_\-\ ]", "", string.strip())
     case = guess_case(string)
 
-    def _regex_split_capture(_regex: str, _string: str) -> list[str]:
+    def _regex_split_capture(_regex: str, _string: str) -> List[str]:
         _split = split(_regex, _string)
         parts = []
         for i in range(len(_split)):
             if i == 0 or i % 2 == 1:
                 parts.append(_split[i])
             else:
                 parts[-1] += _split[i]
@@ -556,25 +553,25 @@
 
 def safe_name(string: Any, permissive: Optional[bool] = True) -> str:
     """
     Makes a 'Safe' name from a string.
     """
     if not isinstance(string, str):
         if permissive:
-            return string
+            return string  # type: ignore
         raise ValueError("save_name called on {0}".format(type(string)))
     return sub(r"\W+", "_", string).strip("_")
 
 
 class Encoding(TypedDict):
     confidence: float
     encoding: str
 
 
-def detect_encoding(obj: Union[bytes, list, dict]) -> list[Encoding]:
+def detect_encoding(obj: Union[bytes, list, dict]) -> List[Encoding]:
     """
     Detects the encoding of a bytestring based upon the characters present in it. Uses chardet to achieve this.
 
     :param obj object: The object to detect the encoding of. Generally a string, but can be a list or dict as well.
     :returns list: A list of encodings, of the form {"confidence": x, "encoding": y}. Higher confidence means it is more likely.
     :raises TypeError: When obj is not a string, bytestring, list or dict.
     """
@@ -649,23 +646,23 @@
         raise TypeError(
             "Cannot decode object of type '{0}'.".format(type(obj).__name__)
         )
 
     if isinstance(obj, str):
         return obj
     try:
-        return _decode(obj, encoding)
+        return _decode(obj, encoding)  # type: ignore
     except UnicodeDecodeError:
         detected_encodings = detect_encoding(obj)
         for detected_encoding in sorted(
             detected_encodings,
             key=lambda detected_encoding: detected_encoding["confidence"],
         ):
             try:
-                return _decode(obj, detected_encoding["encoding"])
+                return _decode(obj, detected_encoding["encoding"])  # type: ignore
             except UnicodeDecodeError:
                 continue
         try:
             logger.error("Failed in decoding the following value: {!r}".format(obj))
         except:
             pass
         raise ValueError(
@@ -713,26 +710,26 @@
                 [(_encode(key, encoding), _encode(obj[key], encoding)) for key in obj]
             )
         raise TypeError(
             "Cannot encode object of type '{0}'.".format(type(obj).__name__)
         )
 
     try:
-        return _encode(obj, encoding)
+        return _encode(obj, encoding)  # type: ignore
     except UnicodeEncodeError:
         if isinstance(obj, str):
             raise ValueError("Cannot encode as {0}".format(encoding))
         detected_encodings = detect_encoding(obj)
 
         for detected_encoding in sorted(
             detected_encodings,
             key=lambda detected_encoding: detected_encoding["confidence"],
         ):
             try:
-                return _encode(obj, detected_encoding["encoding"])
+                return _encode(obj, detected_encoding["encoding"])  # type: ignore
             except UnicodeEncodeError:
                 continue
         try:
             logger.error("Failed in encoding the following value: {!r}".format(obj))
         except:
             pass
         raise ValueError(
@@ -786,15 +783,15 @@
         return ""
     elif len(lst) == 1:
         return lst[0]
     else:
         return "{0} and {1}".format(", ".join(lst[:-1]), lst[-1])
 
 
-def parse_url_encoded(encoded: str) -> Union[str, dict[str, Any]]:
+def parse_url_encoded(encoded: str) -> Union[str, Dict[str, Any]]:
     """
     Parses a urlencoded string and returns either the string, or a dictionary of parameters.
 
     >>> parse_url_encoded("Hello%20Neighbor")
     'Hello Neighbor'
     >>> parse_url_encoded("username=foo&password=bar")
     {'username': 'foo', 'password': 'bar'}
@@ -821,27 +818,27 @@
         self.limit = len(content)
 
     @property
     def file(self) -> io.BytesIO:
         return io.BytesIO(self.content)
 
 
-def parse_multipart(encoded: Union[str, bytes]) -> dict[str, Union[str, MultipartFile]]:
+def parse_multipart(encoded: Union[str, bytes]) -> Dict[str, Union[str, MultipartFile]]:
     """
     Parses a multipart payload.
     """
 
     parser = email.parser.BytesParser()
     if isinstance(encoded, str):
         message = parser.parsebytes(encoded.strip().encode("utf-8"))
     else:
         message = parser.parsebytes(encoded.strip())
     if not message.is_multipart():
         return {}
-    parsed: dict[str, Union[str, MultipartFile]] = {}
+    parsed: Dict[str, Union[str, MultipartFile]] = {}
     for part in message.get_payload():
         name = str(part.get_param("name", header="content-disposition"))
         value = part.get_payload(decode=True)
         filename = part.get_filename()
         if filename:
             parsed[name] = MultipartFile(filename, value)
         else:
```

### Comparing `pibble-0.4.9/pibble/web/scraper.py` & `pibble-0.5.0/pibble/web/scraper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 
+from typing import List, Any
+
 from pibble.util.log import logger
 from pibble.util.strings import pretty_print
 from pibble.util.helpers import find_executable
 
 from urllib.parse import urlparse
 
 try:
@@ -40,35 +42,35 @@
             logger.debug(
                 "Initializing web scraper with chrome driver {0}, arguments {1}".format(
                     chromedriver, pretty_print(*self.arguments)
                 )
             )
             options = Options()
             for argument in self.arguments:
-                options.add_argument(argument)
+                options.add_argument(argument)  # type: ignore
             self._driver = Chrome(chrome_options=options)
         return self._driver
 
-    def crawl(self, url: str) -> list[str]:
+    def crawl(self, url: str) -> List[str]:
         """
         Starting from one URL, find all internal links on that URL. Then recursively
         find the URLs on those internal links, and return the set of all found URLs.
 
         :param url str: The starting URL.
         :returns list: All URLs found, sorted.
         """
         urls_crawled = set()
         crawled_domain = urlparse(url).netloc
         driver = self.driver()
 
-        def crawl_url(url):
+        def crawl_url(url: str) -> None:
             urls_crawled.add(url)
             logger.debug("Crawling URL {0}".format(url))
             driver.get(url)
-            for link in driver.find_elements_by_tag_name("a"):
+            for link in driver.find_elements_by_tag_name("a"):  # type: ignore
                 href = link.get_attribute("href")
                 if href:
                     parsed = urlparse(href)
                     if parsed.netloc == crawled_domain:
                         url_to_crawl = (
                             parsed._replace(fragment="")._replace(query="").geturl()
                         )
@@ -77,16 +79,16 @@
 
         crawl_url(url)
         driver.close()
         crawled = list(urls_crawled)
         crawled.sort()
         return crawled
 
-    def __enter__(self):
+    def __enter__(self) -> Chrome:
         return self.driver()
 
-    def __exit__(self, *args):
+    def __exit__(self, *args: Any) -> None:
         if hasattr(self, "_driver"):
             try:
                 self._driver.close()
             except:
                 pass
```

### Comparing `pibble-0.4.9/pibble.egg-info/PKG-INFO` & `pibble-0.5.0/pibble.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.4.9
+Version: 0.5.0
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
 Provides-Extra: mssql
 Provides-Extra: thrift
 Provides-Extra: grpc
 Provides-Extra: browser
 Provides-Extra: imaging
 Provides-Extra: cherrypy
+Provides-Extra: gunicorn
+Provides-Extra: werkzeug
 Provides-Extra: build
 Provides-Extra: all
 
 # pibble
 The Pibble framework turbocharges Python web applications with a huge array of features and easy-to-use interface.
 
 ## Installation
```

### Comparing `pibble-0.4.9/pibble.egg-info/SOURCES.txt` & `pibble-0.5.0/pibble.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,18 @@
 pibble/api/server/webservice/apachethrift.py
 pibble/api/server/webservice/awslambda.py
 pibble/api/server/webservice/base.py
 pibble/api/server/webservice/handler.py
 pibble/api/server/webservice/jsonapi.py
 pibble/api/server/webservice/orm.py
 pibble/api/server/webservice/soap.py
-pibble/api/server/webservice/mixin/__init__.py
-pibble/api/server/webservice/mixin/base.py
+pibble/api/server/webservice/drivers/__init__.py
+pibble/api/server/webservice/drivers/driver_cherrypy.py
+pibble/api/server/webservice/drivers/driver_gunicorn.py
+pibble/api/server/webservice/drivers/driver_werkzeug.py
 pibble/api/server/webservice/rpc/__init__.py
 pibble/api/server/webservice/rpc/base.py
 pibble/api/server/webservice/rpc/jsonrpc.py
 pibble/api/server/webservice/rpc/xmlrpc.py
 pibble/api/server/webservice/template/__init__.py
 pibble/api/server/webservice/template/extensions.py
 pibble/api/server/webservice/template/loader.py
@@ -98,23 +100,23 @@
 pibble/database/dedupe.py
 pibble/database/engine.py
 pibble/database/exceptions.py
 pibble/database/orm.py
 pibble/database/util.py
 pibble/ext/__init__.py
 pibble/ext/cms/__init__.py
+pibble/ext/cms/middleware.py
 pibble/ext/cms/database/__init__.py
 pibble/ext/cms/database/base.py
 pibble/ext/cms/database/interface.py
 pibble/ext/cms/database/menu.py
 pibble/ext/cms/database/view.py
 pibble/ext/cms/server/__init__.py
 pibble/ext/cms/server/base.py
 pibble/ext/cms/server/extension.py
-pibble/ext/cms/server/mixin.py
 pibble/ext/dam/__init__.py
 pibble/ext/dam/database/__init__.py
 pibble/ext/dam/database/base.py
 pibble/ext/dam/database/files.py
 pibble/ext/dam/server/__init__.py
 pibble/ext/dam/server/base.py
 pibble/ext/rest/__init__.py
@@ -142,14 +144,17 @@
 pibble/ext/user/server/base.py
 pibble/hooks/__init__.py
 pibble/hooks/aws.py
 pibble/media/__init__.py
 pibble/media/thumbnail.py
 pibble/resources/__init__.py
 pibble/resources/retriever.py
+pibble/scripts/__init__.py
+pibble/scripts/importcheck.py
+pibble/scripts/templatefiles.py
 pibble/util/__init__.py
 pibble/util/encryption.py
 pibble/util/files.py
 pibble/util/helpers.py
 pibble/util/imaging.py
 pibble/util/log.py
 pibble/util/numeric.py
```

### Comparing `pibble-0.4.9/pibble.egg-info/requires.txt` & `pibble-0.5.0/pibble.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 bcrypt<4.1,>=4.0
 boto3<2.0,>=1.26
 chardet<5.2,>=5.1
 click<9.0,>=8.0
 configparser<5.4,>=5.3
-gunicorn<21.0,>=20.0
 jinja2<3.2,>=3.1
 lxml<5.0,>=4.9
 mimeparse>=0.1
 mypy<1.3,>=1.2
 openpyxl<4.0,>=3.1
 pandas<3.0,>=2.0
 paramiko<4.0,>=3.1
@@ -18,15 +17,14 @@
 requests<3.0,>=2.28
 requests-oauthlib<2.0,>=1.3
 semantic-version<3.0,>=2.10
 sqlalchemy<2.0,>=1.4
 sshpubkeys<4.0,>=3.3
 termcolor<3.0,>=2.2
 webob<2.0,>=1.8
-werkzeug<3.0,>=2.2
 wsgitypes>=0.0.4
 xlrd<3.0,>=2.0
 zeep<5.0,>=4.2
 
 [all]
 mysqlclient<2.2,>=2.1
 psycopg2-binary<3.0,>=2.9
@@ -36,14 +34,16 @@
 grpcio<1.49
 grpcio-tools<1.49
 selenium<5.0,>=4.8
 pdf2image<2.0,>=1.16
 pillow<10.0,>=9.5
 psd-tools<2.0,>=1.9
 cherrypy<19.0,>=18.8
+gunicorn<21.0,>=20.0
+werkzeug<3.0,>=2.2
 sphinx<6.3,>=6.2
 sphinx-rtd-theme<1.3,>=1.2
 types-PyYAML<6.1,>=6.0.12
 types-chardet<6.0,>=5.0.4
 types-requests<3.0,>=2.29
 types-termcolor<1.2,>=1.1.6
 types-pytz>=2023.3
@@ -81,14 +81,17 @@
 [cherrypy]
 cherrypy<19.0,>=18.8
 
 [grpc]
 grpcio<1.49
 grpcio-tools<1.49
 
+[gunicorn]
+gunicorn<21.0,>=20.0
+
 [imaging]
 pdf2image<2.0,>=1.16
 pillow<10.0,>=9.5
 psd-tools<2.0,>=1.9
 
 [mssql]
 pyodbc<5.0,>=4.0
@@ -98,7 +101,10 @@
 mysqlclient<2.2,>=2.1
 
 [postgresql]
 psycopg2-binary<3.0,>=2.9
 
 [thrift]
 thrift<1.0,>=0.16
+
+[werkzeug]
+werkzeug<3.0,>=2.2
```

### Comparing `pibble-0.4.9/setup.py` & `pibble-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
-version_minor = "4"
-version_patch = "9"
+version_minor = "5"
+version_patch = "0"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
-    "gunicorn>=20.0,<21.0",
     "jinja2>=3.1,<3.2",
     "lxml>=4.9,<5.0",
     "mimeparse>=0.1",
     "mypy>=1.2,<1.3",
     "openpyxl>=3.1,<4.0",
     "pandas>=2.0,<3.0",
     "paramiko>=3.1,<4.0",
@@ -27,29 +26,30 @@
     "requests>=2.28,<3.0",
     "requests-oauthlib>=1.3,<2.0",
     "semantic-version>=2.10,<3.0",
     "sqlalchemy>=1.4,<2.0",
     "sshpubkeys>=3.3,<4.0",
     "termcolor>=2.2,<3.0",
     "webob>=1.8,<2.0",
-    "werkzeug>=2.2,<3.0",
     "wsgitypes>=0.0.4",
     "xlrd>=2.0,<3.0",
     "zeep>=4.2,<5.0",
 ]
 
 extras_require = {
     "mysql": ["mysqlclient>=2.1,<2.2"],
     "postgresql": ["psycopg2-binary>=2.9,<3.0"],
     "mssql": ["pyodbc>=4.0,<5.0", "sqlalchemy-pyodbc-mssql>=0.1"],
     "thrift": ["thrift>=0.16,<1.0"],
     "grpc": ["grpcio<1.49", "grpcio-tools<1.49"],
     "browser": ["selenium>=4.8,<5.0"],
     "imaging": ["pdf2image>=1.16,<2.0", "pillow>=9.5,<10.0", "psd-tools>=1.9,<2.0"],
     "cherrypy": ["cherrypy>=18.8,<19.0"],
+    "gunicorn": ["gunicorn>=20.0,<21.0"],
+    "werkzeug": ["werkzeug>=2.2,<3.0"],
     "build": [
         "sphinx>=6.2,<6.3",
         "sphinx-rtd-theme>=1.2,<1.3",
         "types-PyYAML>=6.0.12,<6.1",
         "types-chardet>=5.0.4,<6.0",
         "types-requests>=2.29,<3.0",
         "types-termcolor>=1.1.6,<1.2",
@@ -72,15 +72,15 @@
 
 setup(
     name=package_name,
     author="Benjamin Paine",
     author_email="painebenjamin@gmail.com",
     version=f"{version_major}.{version_minor}.{version_patch}",
     packages=find_packages("."),
-    package_data={"pibble": []},
+    package_data={"pibble": ["py.typed"]},
     license="gpl-3.0",
     description="A framework for developing webapps quickly and easily using Python",
     long_description=open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"), "r"
     ).read(),
     long_description_content_type="text/markdown",
     entry_points={
```

