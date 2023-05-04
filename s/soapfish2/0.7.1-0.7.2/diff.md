# Comparing `tmp/soapfish2-0.7.1.tar.gz` & `tmp/soapfish2-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/soapfish2-0.7.1.tar", last modified: Sat May 22 04:24:47 2021, max compression
+gzip compressed data, was "soapfish2-0.7.2.tar", last modified: Thu May  4 17:50:38 2023, max compression
```

## Comparing `soapfish2-0.7.1.tar` & `soapfish2-0.7.2.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/
--rw-r--r--   0 luisza    (1000) luisza    (1002)      961 2018-03-05 05:21:50.000000 soapfish2-0.7.1/AUTHORS.md
--rw-r--r--   0 luisza    (1000) luisza    (1002)     5406 2020-09-05 23:10:08.000000 soapfish2-0.7.1/CHANGES.md
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1258 2018-03-05 05:21:50.000000 soapfish2-0.7.1/CONTRIBUTING.md
--rw-r--r--   0 luisza    (1000) luisza    (1002)     2200 2020-09-05 23:10:08.000000 soapfish2-0.7.1/INFORMATION.md
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1573 2018-03-05 05:21:50.000000 soapfish2-0.7.1/LICENSE
--rw-r--r--   0 luisza    (1000) luisza    (1002)     3030 2020-09-05 23:10:08.000000 soapfish2-0.7.1/LIMITATIONS.md
--rw-r--r--   0 luisza    (1000) luisza    (1002)      182 2020-09-05 23:10:08.000000 soapfish2-0.7.1/MANIFEST.in
--rw-r--r--   0 luisza    (1000) luisza    (1002)    14428 2021-05-22 04:24:47.000000 soapfish2-0.7.1/PKG-INFO
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1718 2020-09-05 23:10:08.000000 soapfish2-0.7.1/README.md
--rw-r--r--   0 luisza    (1000) luisza    (1002)     2954 2018-03-05 05:21:50.000000 soapfish2-0.7.1/TODO.md
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/docs/
--rw-r--r--   0 luisza    (1000) luisza    (1002)     6770 2018-03-05 05:21:50.000000 soapfish2-0.7.1/docs/Makefile
--rw-r--r--   0 luisza    (1000) luisza    (1002)     9249 2020-09-05 23:10:08.000000 soapfish2-0.7.1/docs/conf.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      222 2020-01-02 01:02:00.000000 soapfish2-0.7.1/docs/index.rst
--rw-r--r--   0 luisza    (1000) luisza    (1002)     6705 2018-03-05 05:21:50.000000 soapfish2-0.7.1/docs/make.bat
--rw-r--r--   0 luisza    (1000) luisza    (1002)     4481 2018-03-05 05:21:50.000000 soapfish2-0.7.1/docs/middlewares.rst
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1471 2020-01-02 01:02:00.000000 soapfish2-0.7.1/docs/sslcontext.rst
--rw-r--r--   0 luisza    (1000) luisza    (1002)    13963 2018-03-05 05:21:50.000000 soapfish2-0.7.1/docs/tutorial.rst
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/examples/
--rw-r--r--   0 luisza    (1000) luisza    (1002)     4447 2020-09-05 23:10:08.000000 soapfish2-0.7.1/examples/client.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      592 2018-03-05 05:21:50.000000 soapfish2-0.7.1/examples/flask_stock.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     5209 2018-03-05 05:21:50.000000 soapfish2-0.7.1/examples/ops.wsdl
--rw-r--r--   0 luisza    (1000) luisza    (1002)     4050 2018-03-05 05:21:50.000000 soapfish2-0.7.1/examples/ops.xsd
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/examples/stock/
--rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.1/examples/stock/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     5683 2020-09-05 23:10:08.000000 soapfish2-0.7.1/examples/stock/gen.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      627 2020-09-05 23:10:08.000000 soapfish2-0.7.1/examples/stock/manage.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     5032 2020-09-05 23:10:08.000000 soapfish2-0.7.1/examples/stock/settings.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      222 2020-09-05 23:10:08.000000 soapfish2-0.7.1/examples/stock/urls.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/examples/stock/web/
--rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.1/examples/stock/web/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.1/examples/stock/web/models.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      339 2018-03-05 05:21:50.000000 soapfish2-0.7.1/examples/stock/web/views.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      961 2020-09-05 23:10:08.000000 soapfish2-0.7.1/examples/xml_complex_types.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      348 2020-09-05 23:10:08.000000 soapfish2-0.7.1/examples/xml_parsing.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      271 2020-09-05 23:10:08.000000 soapfish2-0.7.1/examples/xml_rendering.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      106 2020-09-05 23:10:08.000000 soapfish2-0.7.1/pyproject.toml
--rw-r--r--   0 luisza    (1000) luisza    (1002)     2430 2021-05-22 04:24:47.000000 soapfish2-0.7.1/setup.cfg
--rw-r--r--   0 luisza    (1000) luisza    (1002)       38 2020-09-05 23:10:08.000000 soapfish2-0.7.1/setup.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/soapfish/
--rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1166 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/core.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1440 2021-05-22 04:22:44.000000 soapfish2-0.7.1/soapfish/django_.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      736 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/flask_.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/soapfish/lib/
--rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.1/soapfish/lib/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      927 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/lib/attribute_dict.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1268 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/middlewares.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1321 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/namespaces.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     5104 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/py2wsdl.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)    11027 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/py2xsd.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/soapfish/raw/
--rw-r--r--   0 luisza    (1000) luisza    (1002)     5574 2018-03-05 05:21:50.000000 soapfish2-0.7.1/soapfish/raw/wsa.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)     5419 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/soap.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     3041 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/soap11.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     2773 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/soap12.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)    11514 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/soap_dispatch.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/soapfish/templates/
--rw-r--r--   0 luisza    (1000) luisza    (1002)     9621 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/templates/lib.jinja2
--rw-r--r--   0 luisza    (1000) luisza    (1002)     5873 2018-03-05 05:21:50.000000 soapfish2-0.7.1/soapfish/templates/wsdl.jinja2
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1822 2018-03-05 05:21:50.000000 soapfish2-0.7.1/soapfish/templates/xsd.jinja2
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/soapfish/testutil/
--rw-r--r--   0 luisza    (1000) luisza    (1002)      120 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/testutil/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     2508 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/testutil/echo_service.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      849 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/testutil/framework.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1253 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/testutil/generated_symbols.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1441 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/testutil/simpletype_testcase.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     7997 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/utils.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1410 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/wsa.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1281 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/wsdl.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     6825 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/wsdl11.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     3095 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/wsdl12.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     4999 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/wsdl2py.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)    41669 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/xsd.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     6113 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/xsd2py.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     2209 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/xsd_types.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     5714 2020-09-05 23:10:08.000000 soapfish2-0.7.1/soapfish/xsdspec.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/soapfish2.egg-info/
--rw-r--r--   0 luisza    (1000) luisza    (1002)     3615 2021-05-22 04:24:47.000000 soapfish2-0.7.1/soapfish2.egg-info/SOURCES.txt
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/tests/
--rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/__init__.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/tests/assets/
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/tests/assets/generation/
--rw-r--r--   0 luisza    (1000) luisza    (1002)      601 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/attrgroup_usage.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      452 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/attribute_usage.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)     5742 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/default.wsdl
--rw-r--r--   0 luisza    (1000) luisza    (1002)     3897 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/default.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      440 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/enumeration.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      617 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/assets/generation/enumeration2.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      640 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/extension.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      650 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/extension_imported.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      357 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/extension_imported_parent.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      935 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/extension_with_special_chars.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      186 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/implicit_namespace.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      282 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/import_looped.wsdl
--rw-r--r--   0 luisza    (1000) luisza    (1002)      203 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/import_nested.wsdl
--rw-r--r--   0 luisza    (1000) luisza    (1002)      380 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/import_remote.wsdl
--rw-r--r--   0 luisza    (1000) luisza    (1002)      203 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/import_simple.wsdl
--rw-r--r--   0 luisza    (1000) luisza    (1002)      357 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/import_target.wsdl
--rw-r--r--   0 luisza    (1000) luisza    (1002)      392 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/inheritance.wsdl
--rw-r--r--   0 luisza    (1000) luisza    (1002)      446 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/list_param.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      559 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/multi_schema.wsdl
--rw-r--r--   0 luisza    (1000) luisza    (1002)      578 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/reference_complex.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      441 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/reference_simple.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      551 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/restriction.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      318 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/generation/simple_element.xsd
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/tests/assets/include/
--rw-r--r--   0 luisza    (1000) luisza    (1002)      435 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/include/include.wsdl
--rw-r--r--   0 luisza    (1000) luisza    (1002)      237 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/include/schema1.xsd
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/tests/assets/relative/
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/tests/assets/relative/1/
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/tests/assets/relative/1/2/
--rw-r--r--   0 luisza    (1000) luisza    (1002)      472 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/relative/1/2/schema2.xsd
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/tests/assets/relative/1/3/
--rw-r--r--   0 luisza    (1000) luisza    (1002)      239 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/relative/1/3/schema3.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      341 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/relative/1/schema1.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      469 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/relative/relative.wsdl
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/tests/assets/same_namespace/
--rw-r--r--   0 luisza    (1000) luisza    (1002)      545 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/same_namespace/same_namespace.wsdl
--rw-r--r--   0 luisza    (1000) luisza    (1002)      237 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/same_namespace/schema1.xsd
--rw-r--r--   0 luisza    (1000) luisza    (1002)      237 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/assets/same_namespace/schema2.xsd
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/tests/framework/
--rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/framework/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1933 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/framework/django_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1236 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/framework/flask_test.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/tests/generation/
--rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/generation/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     3942 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/generation/code_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     3052 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/generation/wsdl_code_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     3310 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/generation/xsd_attrs_code_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     5387 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/generation/xsd_code_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     3548 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/ops_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1264 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/py2xsd_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      278 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/requirements.txt
--rw-r--r--   0 luisza    (1000) luisza    (1002)      566 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/soap11_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      589 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/soap12_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     8108 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/soap2_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)    18775 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/soap_dispatcher_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     6696 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/soap_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     3634 2020-09-06 00:44:18.000000 soapfish2-0.7.1/tests/utils_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     2156 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/wsgi_soap_application_test.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/tests/xsd/
--rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/xsd/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     3572 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/xsd/date_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      298 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/xsd/decimal_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      669 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/xsd/schema_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     2551 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/xsd/string_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     2227 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/xsd/time_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     2521 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/xsd/xsd_choice_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     2473 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/xsd/xsd_datetime_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1971 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/xsd/xsd_ref_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)    31140 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/xsd_test.py
-drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2021-05-22 04:24:47.000000 soapfish2-0.7.1/tests/xsd_types/
--rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.1/tests/xsd_types/__init__.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      877 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/xsd_types/xsddate_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     2609 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/xsdspec_element_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)     1572 2020-09-05 23:10:08.000000 soapfish2-0.7.1/tests/xsdspec_schema_test.py
--rw-r--r--   0 luisza    (1000) luisza    (1002)      106 2020-09-06 00:40:56.000000 soapfish2-0.7.1/tox.ini
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.693468 soapfish2-0.7.2/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      961 2018-03-05 05:21:50.000000 soapfish2-0.7.2/AUTHORS.md
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     5406 2023-05-04 16:20:17.000000 soapfish2-0.7.2/CHANGES.md
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1258 2018-03-05 05:21:50.000000 soapfish2-0.7.2/CONTRIBUTING.md
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     2200 2023-05-04 16:20:17.000000 soapfish2-0.7.2/INFORMATION.md
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1573 2018-03-05 05:21:50.000000 soapfish2-0.7.2/LICENSE
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     3030 2023-05-04 16:20:17.000000 soapfish2-0.7.2/LIMITATIONS.md
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      182 2023-05-04 16:20:17.000000 soapfish2-0.7.2/MANIFEST.in
+-rw-r--r--   0 luisza    (1000) luisza    (1002)    12388 2023-05-04 17:50:38.693468 soapfish2-0.7.2/PKG-INFO
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1718 2023-05-04 16:20:17.000000 soapfish2-0.7.2/README.md
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     2954 2018-03-05 05:21:50.000000 soapfish2-0.7.2/TODO.md
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.657468 soapfish2-0.7.2/docs/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     6770 2018-03-05 05:21:50.000000 soapfish2-0.7.2/docs/Makefile
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     9249 2023-05-04 16:20:17.000000 soapfish2-0.7.2/docs/conf.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      222 2020-01-02 01:02:00.000000 soapfish2-0.7.2/docs/index.rst
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     6705 2018-03-05 05:21:50.000000 soapfish2-0.7.2/docs/make.bat
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     4481 2018-03-05 05:21:50.000000 soapfish2-0.7.2/docs/middlewares.rst
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1471 2020-01-02 01:02:00.000000 soapfish2-0.7.2/docs/sslcontext.rst
+-rw-r--r--   0 luisza    (1000) luisza    (1002)    13963 2018-03-05 05:21:50.000000 soapfish2-0.7.2/docs/tutorial.rst
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.661468 soapfish2-0.7.2/examples/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     4447 2023-05-04 16:20:17.000000 soapfish2-0.7.2/examples/client.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      592 2018-03-05 05:21:50.000000 soapfish2-0.7.2/examples/flask_stock.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     5209 2018-03-05 05:21:50.000000 soapfish2-0.7.2/examples/ops.wsdl
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     4050 2018-03-05 05:21:50.000000 soapfish2-0.7.2/examples/ops.xsd
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.661468 soapfish2-0.7.2/examples/stock/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.2/examples/stock/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     5683 2023-05-04 16:20:17.000000 soapfish2-0.7.2/examples/stock/gen.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      627 2023-05-04 16:20:17.000000 soapfish2-0.7.2/examples/stock/manage.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     5032 2023-05-04 16:20:17.000000 soapfish2-0.7.2/examples/stock/settings.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      222 2023-05-04 16:20:17.000000 soapfish2-0.7.2/examples/stock/urls.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.661468 soapfish2-0.7.2/examples/stock/web/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.2/examples/stock/web/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.2/examples/stock/web/models.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      339 2018-03-05 05:21:50.000000 soapfish2-0.7.2/examples/stock/web/views.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      961 2023-05-04 16:20:17.000000 soapfish2-0.7.2/examples/xml_complex_types.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      348 2023-05-04 16:20:17.000000 soapfish2-0.7.2/examples/xml_parsing.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      271 2023-05-04 16:20:17.000000 soapfish2-0.7.2/examples/xml_rendering.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      106 2023-05-04 16:20:17.000000 soapfish2-0.7.2/pyproject.toml
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     2430 2023-05-04 17:50:38.693468 soapfish2-0.7.2/setup.cfg
+-rw-r--r--   0 luisza    (1000) luisza    (1002)       38 2023-05-04 16:20:17.000000 soapfish2-0.7.2/setup.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.665468 soapfish2-0.7.2/soapfish/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1166 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/core.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1974 2023-05-04 16:20:53.000000 soapfish2-0.7.2/soapfish/django_.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      736 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/flask_.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.665468 soapfish2-0.7.2/soapfish/lib/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.2/soapfish/lib/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      927 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/lib/attribute_dict.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1268 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/middlewares.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1321 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/namespaces.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     5104 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/py2wsdl.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)    11027 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/py2xsd.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.669468 soapfish2-0.7.2/soapfish/raw/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     5574 2018-03-05 05:21:50.000000 soapfish2-0.7.2/soapfish/raw/wsa.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     5419 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/soap.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     3041 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/soap11.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     2773 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/soap12.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)    11514 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/soap_dispatch.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.669468 soapfish2-0.7.2/soapfish/templates/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     9621 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/templates/lib.jinja2
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     5873 2018-03-05 05:21:50.000000 soapfish2-0.7.2/soapfish/templates/wsdl.jinja2
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1822 2018-03-05 05:21:50.000000 soapfish2-0.7.2/soapfish/templates/xsd.jinja2
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.669468 soapfish2-0.7.2/soapfish/testutil/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      120 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/testutil/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     2508 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/testutil/echo_service.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      849 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/testutil/framework.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1253 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/testutil/generated_symbols.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1441 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/testutil/simpletype_testcase.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     7997 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/utils.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1410 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/wsa.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1281 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/wsdl.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     6825 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/wsdl11.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     3095 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/wsdl12.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     4999 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/wsdl2py.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)    41669 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/xsd.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     6113 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/xsd2py.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     2209 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/xsd_types.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     5714 2023-05-04 16:20:17.000000 soapfish2-0.7.2/soapfish/xsdspec.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.693468 soapfish2-0.7.2/soapfish2.egg-info/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     3615 2023-05-04 17:50:38.000000 soapfish2-0.7.2/soapfish2.egg-info/SOURCES.txt
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.673468 soapfish2-0.7.2/tests/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/__init__.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.653468 soapfish2-0.7.2/tests/assets/
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.681468 soapfish2-0.7.2/tests/assets/generation/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      601 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/attrgroup_usage.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      452 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/attribute_usage.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     5742 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/default.wsdl
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     3897 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/default.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      440 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/enumeration.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      617 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/assets/generation/enumeration2.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      640 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/extension.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      650 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/extension_imported.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      357 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/extension_imported_parent.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      935 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/extension_with_special_chars.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      186 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/implicit_namespace.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      282 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/import_looped.wsdl
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      203 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/import_nested.wsdl
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      380 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/import_remote.wsdl
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      203 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/import_simple.wsdl
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      357 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/import_target.wsdl
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      392 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/inheritance.wsdl
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      446 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/list_param.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      559 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/multi_schema.wsdl
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      578 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/reference_complex.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      441 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/reference_simple.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      551 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/restriction.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      318 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/generation/simple_element.xsd
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.681468 soapfish2-0.7.2/tests/assets/include/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      435 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/include/include.wsdl
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      237 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/include/schema1.xsd
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.681468 soapfish2-0.7.2/tests/assets/relative/
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.681468 soapfish2-0.7.2/tests/assets/relative/1/
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.681468 soapfish2-0.7.2/tests/assets/relative/1/2/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      472 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/relative/1/2/schema2.xsd
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.681468 soapfish2-0.7.2/tests/assets/relative/1/3/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      239 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/relative/1/3/schema3.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      341 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/relative/1/schema1.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      469 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/relative/relative.wsdl
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.685468 soapfish2-0.7.2/tests/assets/same_namespace/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      545 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/same_namespace/same_namespace.wsdl
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      237 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/same_namespace/schema1.xsd
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      237 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/assets/same_namespace/schema2.xsd
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.685468 soapfish2-0.7.2/tests/framework/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/framework/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1933 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/framework/django_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1236 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/framework/flask_test.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.689468 soapfish2-0.7.2/tests/generation/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/generation/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     3942 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/generation/code_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     3052 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/generation/wsdl_code_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     3310 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/generation/xsd_attrs_code_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     5387 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/generation/xsd_code_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     3548 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/ops_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1264 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/py2xsd_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      278 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/requirements.txt
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      566 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/soap11_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      589 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/soap12_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     8108 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/soap2_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)    18775 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/soap_dispatcher_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     6696 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/soap_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     3634 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/utils_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     2156 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/wsgi_soap_application_test.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.689468 soapfish2-0.7.2/tests/xsd/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/xsd/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     3572 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/xsd/date_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      298 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/xsd/decimal_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      669 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/xsd/schema_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     2551 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/xsd/string_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     2227 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/xsd/time_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     2521 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/xsd/xsd_choice_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     2473 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/xsd/xsd_datetime_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1971 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/xsd/xsd_ref_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)    31140 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/xsd_test.py
+drwxr-xr-x   0 luisza    (1000) luisza    (1002)        0 2023-05-04 17:50:38.693468 soapfish2-0.7.2/tests/xsd_types/
+-rw-r--r--   0 luisza    (1000) luisza    (1002)        0 2018-03-05 05:21:50.000000 soapfish2-0.7.2/tests/xsd_types/__init__.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      877 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/xsd_types/xsddate_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     2609 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/xsdspec_element_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)     1572 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tests/xsdspec_schema_test.py
+-rw-r--r--   0 luisza    (1000) luisza    (1002)      106 2023-05-04 16:20:17.000000 soapfish2-0.7.2/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `soapfish2-0.7.1/AUTHORS.md` & `soapfish2-0.7.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/CHANGES.md` & `soapfish2-0.7.2/CHANGES.md`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/CONTRIBUTING.md` & `soapfish2-0.7.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/INFORMATION.md` & `soapfish2-0.7.2/INFORMATION.md`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/LICENSE` & `soapfish2-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/LIMITATIONS.md` & `soapfish2-0.7.2/LIMITATIONS.md`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/PKG-INFO` & `soapfish2-0.7.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,278 +1,19 @@
 Metadata-Version: 2.1
 Name: soapfish2
-Version: 0.7.1
+Version: 0.7.2
 Summary: No official SOAP library for Python
 Home-page: http://soapfish.org/
+Download-URL: http://soapfish.org/releases/
 Author: Damian Powązka
 Author-email: dpowazka@gmail.com
 Maintainer: Felix Schwarz
 Maintainer-email: felix.schwarz@oss.schwarz.eu
 License: BSD-3-Clause
-Download-URL: http://soapfish.org/releases/
-Description: Soapfish
-        ========
-        
-        [![Travis](https://img.shields.io/travis/soapteam/soapfish/master.svg)](https://travis-ci.org/soapteam/soapfish)
-        [![PyPI](https://img.shields.io/pypi/v/soapfish.svg)](https://pypi.org/project/soapfish/)
-        [![PyPI](https://img.shields.io/pypi/l/soapfish.svg)](https://pypi.org/project/soapfish/)
-        [![PyPI](https://img.shields.io/pypi/dm/soapfish.svg)](https://pypi.org/project/soapfish/)
-        [![PyPI](https://img.shields.io/pypi/pyversions/soapfish.svg)](https://pypi.org/project/soapfish/)
-        [![PyPI](https://img.shields.io/pypi/status/soapfish.svg)](https://pypi.org/project/soapfish/)
-        [![PyPI](https://img.shields.io/pypi/wheel/soapfish.svg)](https://pypi.org/project/soapfish/)
-        
-        [![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)
-        
-        **This project is not actively maintained. If you only need a dynamic client using a predefined WSDL rather than
-        generated code, it is recommended that you check out [Zeep](https://pypi.org/project/zeep/).**
-        
-        Introduction
-        ------------
-        
-        Soapfish is a library to use SOAP services in Python. The server-side component can be used with Django, Flask, Pyramid
-        and other frameworks (including plain WSGI). The library can also be used to implement SOAP clients.
-        
-        The library can help parsing/serializing a Python class model from/to XML and a bare-bones SOAP client.
-        
-        Currently the project supports the following:
-        
-        - SOAP 1.1 and 1.2
-        - WSDL 1.1
-        - WS-Addressing
-        
-        Other notable features include:
-        
-        - Support for Python 3.6+
-        - Licensed under the 3-clause BSD license
-        - Code generation utilities to get started quickly
-        - Parsing/serializing a Python class model from/to XML so you can easily work
-          with XML even if you don't use SOAP at all.
-        
-        Authors
-        =======
-        
-        Soapfish was originally written by Damian Powązka while working at Flight Data
-        Services. At that time it was called Soapbox and from February 2012 was
-        maintained by Flight Data Services. The project was forked in November 2013 by
-        Felix Schwarz (based on the last BSD-licensed commit), after which a large
-        number of new features were added by Thomas Recouvreux and Xavier Fernandez
-        from Polyconseil between February and June 2014. Iuri de Silvio from Pricez
-        added some features and fixed numerous bugs during 2015. In early 2016, Flight
-        Data Services retired the unmaintained Soapbox project in favour of Soapfish.
-        
-        **Original Author:**
-        
-        - Damian Powązka (Flight Data Services)
-        
-        **Maintainers:**
-        
-        - Felix Schwarz (sponsored by Rechenzentrum für Berliner Apotheken Stein & Reichwald GmbH)
-        - Nick Pope (Flight Data Services)
-        - Iuri de Silvio (Pricez)
-        
-        **Major Contributors:**
-        
-        - Thomas Recouvreux (Polyconseil)
-        - Xavier Fernandez (Polyconseil)
-        
-        Changes
-        =======
-        
-        0.6.0 (2020-??-??)
-        ------------------
-        
-        Project has been renamed to `soapfish` to distinguish it from the legacy
-        `soapbox` project and allow for publishing the project on PyPI. Note that the
-        rename effectively makes it backwards incompatible with previous releases due
-        to API breakage.
-        
-        Due to lack of time to maintain the original `soapbox` project, `soapbox` been
-        retired by Flight Data Services who now contribute to and recommend the use of
-        the `soapfish` fork.
-        
-        - **Security:**
-          - Fixed potential security issue - pattern restrictions were not applied correctly
-        - **Features:**
-          - Add support for xsd.date (date range currently limited by datetime.date)
-          - Add support relative schema paths (#49)
-          - Add support to string restrictions length, minLength, maxLength, whiteSpace (#67)
-          - Add support for choice indicator in ComplexTypes (#39)
-            - Fixes validation of matching XML documents - previously sequences were always assumed - and code generation from WSDL/XSD.
-            - _Patch contributed by Martin Mrose, tests written by Felix Schwarz_
-          - Implemented a dispatcher for Flask (#53)
-          - Implement service.route function to avoid changes to generated code (#68)
-          - Changed to use `requests` instead of `httplib2`.
-          - Added support for multiple inline schema imports and includes.
-          - Added support for import of other WSDL documents.
-          - Support for reordering of schema imports and includes and handle circular imports.
-        - **Bug Fixes:**
-          - Make xsd.Decimal field accept Python Decimal (#52)
-          - Fix relative imports with remote files. (#96)
-          - Schema validation now also uses imported schemas correctly
-          - Various fixes for `wsdl2py` and `xsd2py` when using Python 3
-          - Fix exception in `SOAPDispatcher` when a handler does not return a `SOAPResponse`
-          - Fix bad WSDL generation due to unresolved type references
-          - Correctly apply pattern restrictions for simple types
-          - Pattern restriction was not correctly serialized when generating schemas
-          - Omit `minOccurs=1` and `maxOccurs=1` in `xsd2py` as these are the default.
-            (The latter produces invalid code because `xsd.Element` doesn't support it.)
-          - Restored ability to validate parsed XML using a soapfish schema in `ComplexType`
-          - Fixed WSDL classes to more closely match the WSDL specifications.
-          - Fixed WSDL classes to correctly define SOAP extensibility elements.
-          - Removed reverse references from WSDL classes.
-          - Fixed query string handling in dispatch to be more robust.
-          - Support importing documents over HTTPS.
-          - Fixed detection of XML schema namespaces.
-          - Attempts to fix handling of remote vs local imports.
-        - **Miscellaneous:**
-          - Renamed `SoapboxRequest` and `SoapboxResponse` to `SOAPRequest` and `SOAPResponse` respectively.
-          - Support Python 3.6+, Django 1.11, 2.2 & 3.0, and Flask 1.0.0+
-          - Improved testing against different versions of Python, Django & Flask.
-          - Improved entry points for generation scripts - additional flags, etc.
-          - Moved to using an external dependency for `iso8601`
-        
-        0.5.1 (2014-06-12)
-        ------------------
-        
-        - **Miscellaneous:**
-          - Downgrade log level on soap action discovery.
-        
-        0.5.0 (2014-06-12)
-        ------------------
-        
-        - **Miscellaneous:**
-          - Make elements inherit from schema namespace
-          - Better logging in soap/stub
-          - soap12: Quotes around action in HTTP header
-        
-        0.4.0 (2014-05-06)
-        ------------------
-        
-        Project forked by Felix Schwarz as `soapbox-bsd` due to licensing incompatibilities.
-        
-        Flight Data Services started using the GPL-incompatible OSL for the `soapbox`
-        project. This fork is based on the last `soapbox` commit still using the
-        original 3-clause BSD license (7d3516fe).  Later on the fork received
-        significant contributions from Thomas Recouvreux and Xavier Fernandez
-        (Polyconseil).
-        
-        - **Features:**
-          - Added support for SOAP 1.2 and WSDL 1.2
-          - Added support for WS-Addressing
-          - Added support for fault actors (Damian Powązka)
-          - Added support for Django >= 1.4
-          - Added compatibility with Python 3
-          - Added framework-agnostic SOAP dispatcher to support virtually any web framework.
-        - **Bug Fixes:**
-          - Preserve `elementFormDefault` attribute in Schema
-          - Many bug fixes for code generation and XML rendering
-        - **Miscellaneous:**
-          - Ability to use custom SOAP headers
-          - Middleware stack to hook into SOAP request processing
-          - Better handling of invalid SOAP requests, e.g. missing bodies, invalid actions.
-        
-        0.3.2 (2012-03-09)
-        ------------------
-        
-        - **Miscellaneous:**
-          - Initial support for variable URL scheme and host
-          - Test suite executes
-        
-        0.3.1 (2012-03-08)
-        ------------------
-        
-        - **Miscellaneous:**
-          - SSL certificate verification
-        
-        0.3.0 (2012-03-02)
-        ------------------
-        
-        - **Features:**
-          - Add option to disable schema validation on parsing:
-            - Set `xsd.VALIDATE_ON_PARSE` to `False`.
-          - Added some initial logging support:
-            - Request logging available at when level set to DEBUG.
-        - **Bug Fixes:**
-          - Allow unicode as a valid type for strings.
-          - Check for Python keywords and prefix with underscore.
-        - **Miscellaneous:**
-          - Python code templates now loaded from external files.
-          - Generated code is now much cleaner.
-          - Generated code is now timestamped.
-          - Code tidying as reported by pyflakes and pep8.
-          - Fixed a number of typographical errors.
-          - Various name improvements to functions.
-          - Updated .hgignore
-        - **Known Issues:**
-          - Generated schema classes can be circular referencing.
-        
-        To Do
-        =====
-        
-        This project is very, very promising:
-        
-        - It is focused on XML and SOAP/WSDL without any compromise. In an ideal world
-          soapfish works with each and every syntax allowed by these technologies.
-        - It allows you to have a representation of arbitrary XML including support
-          for XSD. Parse any XML described by a schema into a nice class-based tree
-          (and the other way round: serialization is possible as well).
-        - Because soapfish supports only SOAP and no other remoting protocol (e.g.
-          ReST-style APIs with JSON) the API is not tied to the lowest common
-          denominator. You should be able implement any given WSDL.
-        
-        Unfortunately we're not there yet.
-        
-        This is a typical open source software and XML/SOAP is usually not perceived
-        as a fun project. So various users added some smaller features which they
-        needed but typically there are many incomplete implementations above the very
-        basic layer (the object model to represent XML/XSD programmatically).
-        On the upside that means there are a lot of ways to improve the code and your
-        contribution and make a big difference.
-        
-        Here some bigger areas which need work:
-        
-        - A much more comprehensive set of unit tests
-        - Implement support for additional web frameworks
-        - XSD schema generation (object graph to XSD file) has most of its logic in a
-          very complex Jinja2 template which shows it limits. For example features like
-          named xs:Elements with embedded anonymous ComplexTypes can not be serialized
-          to XSD currently.
-          However the code internally assumes that the class tree and the XSD
-          representation contain the same information so this can lead to bugs.
-        - The XSD mapping is currently incomplete: Some types in schemas are not
-          implemented at all (e.g. xs:date, xs:gYearMonth). Other types might not be
-          parsed/serialized correctly. Also references to xs:elements are pretty
-          incomplete right now.
-        - Generated code (e.g. WSDL handling or XSD mapping) usually has some syntax
-          errors. Some of them are fixable on their own but often this is because of
-          other missing features (see above). The output should be usable as
-          scaffolding though.
-        
-        Don't worry if the items on the list above seem to big for you. Just start out
-        with something small, write tests and contribute them. Even a small (failing)
-        unit test which demonstrates a current shortcoming is great.
-        
-        You might also check out current skipped unit tests which usually represent
-        missing functionality (though these might not be ideal beginner projects - if
-        they were trivial to implement I would have done that already).
-        
-        All these shortcomings and limitations exist only because of the lack of
-        time and/or awareness about certain XSD features. The goal of this library is
-        to fully implement XSD schemas and potentially SOAP/WSDL so patches (with tests)
-        are always welcome.
-        
-        Specific Items
-        --------------
-        
-        - Fix circular dependency of generated schema classes.
-        
-        See the **TODO** markers in `soapfish/*.py` for a complete list.
-        
 Keywords: soap,wsdl,xsd,xml,schema,web service
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Flask
 Classifier: Framework :: Pyramid
 Classifier: Intended Audience :: Developers
@@ -286,7 +27,267 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Obsoletes: soapbox
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+
+Soapfish
+========
+
+[![Travis](https://img.shields.io/travis/soapteam/soapfish/master.svg)](https://travis-ci.org/soapteam/soapfish)
+[![PyPI](https://img.shields.io/pypi/v/soapfish.svg)](https://pypi.org/project/soapfish/)
+[![PyPI](https://img.shields.io/pypi/l/soapfish.svg)](https://pypi.org/project/soapfish/)
+[![PyPI](https://img.shields.io/pypi/dm/soapfish.svg)](https://pypi.org/project/soapfish/)
+[![PyPI](https://img.shields.io/pypi/pyversions/soapfish.svg)](https://pypi.org/project/soapfish/)
+[![PyPI](https://img.shields.io/pypi/status/soapfish.svg)](https://pypi.org/project/soapfish/)
+[![PyPI](https://img.shields.io/pypi/wheel/soapfish.svg)](https://pypi.org/project/soapfish/)
+
+[![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)
+
+**This project is not actively maintained. If you only need a dynamic client using a predefined WSDL rather than
+generated code, it is recommended that you check out [Zeep](https://pypi.org/project/zeep/).**
+
+Introduction
+------------
+
+Soapfish is a library to use SOAP services in Python. The server-side component can be used with Django, Flask, Pyramid
+and other frameworks (including plain WSGI). The library can also be used to implement SOAP clients.
+
+The library can help parsing/serializing a Python class model from/to XML and a bare-bones SOAP client.
+
+Currently the project supports the following:
+
+- SOAP 1.1 and 1.2
+- WSDL 1.1
+- WS-Addressing
+
+Other notable features include:
+
+- Support for Python 3.6+
+- Licensed under the 3-clause BSD license
+- Code generation utilities to get started quickly
+- Parsing/serializing a Python class model from/to XML so you can easily work
+  with XML even if you don't use SOAP at all.
+
+Authors
+=======
+
+Soapfish was originally written by Damian Powązka while working at Flight Data
+Services. At that time it was called Soapbox and from February 2012 was
+maintained by Flight Data Services. The project was forked in November 2013 by
+Felix Schwarz (based on the last BSD-licensed commit), after which a large
+number of new features were added by Thomas Recouvreux and Xavier Fernandez
+from Polyconseil between February and June 2014. Iuri de Silvio from Pricez
+added some features and fixed numerous bugs during 2015. In early 2016, Flight
+Data Services retired the unmaintained Soapbox project in favour of Soapfish.
+
+**Original Author:**
+
+- Damian Powązka (Flight Data Services)
+
+**Maintainers:**
+
+- Felix Schwarz (sponsored by Rechenzentrum für Berliner Apotheken Stein & Reichwald GmbH)
+- Nick Pope (Flight Data Services)
+- Iuri de Silvio (Pricez)
+
+**Major Contributors:**
+
+- Thomas Recouvreux (Polyconseil)
+- Xavier Fernandez (Polyconseil)
+
+Changes
+=======
+
+0.6.0 (2020-??-??)
+------------------
+
+Project has been renamed to `soapfish` to distinguish it from the legacy
+`soapbox` project and allow for publishing the project on PyPI. Note that the
+rename effectively makes it backwards incompatible with previous releases due
+to API breakage.
+
+Due to lack of time to maintain the original `soapbox` project, `soapbox` been
+retired by Flight Data Services who now contribute to and recommend the use of
+the `soapfish` fork.
+
+- **Security:**
+  - Fixed potential security issue - pattern restrictions were not applied correctly
+- **Features:**
+  - Add support for xsd.date (date range currently limited by datetime.date)
+  - Add support relative schema paths (#49)
+  - Add support to string restrictions length, minLength, maxLength, whiteSpace (#67)
+  - Add support for choice indicator in ComplexTypes (#39)
+    - Fixes validation of matching XML documents - previously sequences were always assumed - and code generation from WSDL/XSD.
+    - _Patch contributed by Martin Mrose, tests written by Felix Schwarz_
+  - Implemented a dispatcher for Flask (#53)
+  - Implement service.route function to avoid changes to generated code (#68)
+  - Changed to use `requests` instead of `httplib2`.
+  - Added support for multiple inline schema imports and includes.
+  - Added support for import of other WSDL documents.
+  - Support for reordering of schema imports and includes and handle circular imports.
+- **Bug Fixes:**
+  - Make xsd.Decimal field accept Python Decimal (#52)
+  - Fix relative imports with remote files. (#96)
+  - Schema validation now also uses imported schemas correctly
+  - Various fixes for `wsdl2py` and `xsd2py` when using Python 3
+  - Fix exception in `SOAPDispatcher` when a handler does not return a `SOAPResponse`
+  - Fix bad WSDL generation due to unresolved type references
+  - Correctly apply pattern restrictions for simple types
+  - Pattern restriction was not correctly serialized when generating schemas
+  - Omit `minOccurs=1` and `maxOccurs=1` in `xsd2py` as these are the default.
+    (The latter produces invalid code because `xsd.Element` doesn't support it.)
+  - Restored ability to validate parsed XML using a soapfish schema in `ComplexType`
+  - Fixed WSDL classes to more closely match the WSDL specifications.
+  - Fixed WSDL classes to correctly define SOAP extensibility elements.
+  - Removed reverse references from WSDL classes.
+  - Fixed query string handling in dispatch to be more robust.
+  - Support importing documents over HTTPS.
+  - Fixed detection of XML schema namespaces.
+  - Attempts to fix handling of remote vs local imports.
+- **Miscellaneous:**
+  - Renamed `SoapboxRequest` and `SoapboxResponse` to `SOAPRequest` and `SOAPResponse` respectively.
+  - Support Python 3.6+, Django 1.11, 2.2 & 3.0, and Flask 1.0.0+
+  - Improved testing against different versions of Python, Django & Flask.
+  - Improved entry points for generation scripts - additional flags, etc.
+  - Moved to using an external dependency for `iso8601`
+
+0.5.1 (2014-06-12)
+------------------
+
+- **Miscellaneous:**
+  - Downgrade log level on soap action discovery.
+
+0.5.0 (2014-06-12)
+------------------
+
+- **Miscellaneous:**
+  - Make elements inherit from schema namespace
+  - Better logging in soap/stub
+  - soap12: Quotes around action in HTTP header
+
+0.4.0 (2014-05-06)
+------------------
+
+Project forked by Felix Schwarz as `soapbox-bsd` due to licensing incompatibilities.
+
+Flight Data Services started using the GPL-incompatible OSL for the `soapbox`
+project. This fork is based on the last `soapbox` commit still using the
+original 3-clause BSD license (7d3516fe).  Later on the fork received
+significant contributions from Thomas Recouvreux and Xavier Fernandez
+(Polyconseil).
+
+- **Features:**
+  - Added support for SOAP 1.2 and WSDL 1.2
+  - Added support for WS-Addressing
+  - Added support for fault actors (Damian Powązka)
+  - Added support for Django >= 1.4
+  - Added compatibility with Python 3
+  - Added framework-agnostic SOAP dispatcher to support virtually any web framework.
+- **Bug Fixes:**
+  - Preserve `elementFormDefault` attribute in Schema
+  - Many bug fixes for code generation and XML rendering
+- **Miscellaneous:**
+  - Ability to use custom SOAP headers
+  - Middleware stack to hook into SOAP request processing
+  - Better handling of invalid SOAP requests, e.g. missing bodies, invalid actions.
+
+0.3.2 (2012-03-09)
+------------------
+
+- **Miscellaneous:**
+  - Initial support for variable URL scheme and host
+  - Test suite executes
+
+0.3.1 (2012-03-08)
+------------------
+
+- **Miscellaneous:**
+  - SSL certificate verification
+
+0.3.0 (2012-03-02)
+------------------
+
+- **Features:**
+  - Add option to disable schema validation on parsing:
+    - Set `xsd.VALIDATE_ON_PARSE` to `False`.
+  - Added some initial logging support:
+    - Request logging available at when level set to DEBUG.
+- **Bug Fixes:**
+  - Allow unicode as a valid type for strings.
+  - Check for Python keywords and prefix with underscore.
+- **Miscellaneous:**
+  - Python code templates now loaded from external files.
+  - Generated code is now much cleaner.
+  - Generated code is now timestamped.
+  - Code tidying as reported by pyflakes and pep8.
+  - Fixed a number of typographical errors.
+  - Various name improvements to functions.
+  - Updated .hgignore
+- **Known Issues:**
+  - Generated schema classes can be circular referencing.
+
+To Do
+=====
+
+This project is very, very promising:
+
+- It is focused on XML and SOAP/WSDL without any compromise. In an ideal world
+  soapfish works with each and every syntax allowed by these technologies.
+- It allows you to have a representation of arbitrary XML including support
+  for XSD. Parse any XML described by a schema into a nice class-based tree
+  (and the other way round: serialization is possible as well).
+- Because soapfish supports only SOAP and no other remoting protocol (e.g.
+  ReST-style APIs with JSON) the API is not tied to the lowest common
+  denominator. You should be able implement any given WSDL.
+
+Unfortunately we're not there yet.
+
+This is a typical open source software and XML/SOAP is usually not perceived
+as a fun project. So various users added some smaller features which they
+needed but typically there are many incomplete implementations above the very
+basic layer (the object model to represent XML/XSD programmatically).
+On the upside that means there are a lot of ways to improve the code and your
+contribution and make a big difference.
+
+Here some bigger areas which need work:
+
+- A much more comprehensive set of unit tests
+- Implement support for additional web frameworks
+- XSD schema generation (object graph to XSD file) has most of its logic in a
+  very complex Jinja2 template which shows it limits. For example features like
+  named xs:Elements with embedded anonymous ComplexTypes can not be serialized
+  to XSD currently.
+  However the code internally assumes that the class tree and the XSD
+  representation contain the same information so this can lead to bugs.
+- The XSD mapping is currently incomplete: Some types in schemas are not
+  implemented at all (e.g. xs:date, xs:gYearMonth). Other types might not be
+  parsed/serialized correctly. Also references to xs:elements are pretty
+  incomplete right now.
+- Generated code (e.g. WSDL handling or XSD mapping) usually has some syntax
+  errors. Some of them are fixable on their own but often this is because of
+  other missing features (see above). The output should be usable as
+  scaffolding though.
+
+Don't worry if the items on the list above seem to big for you. Just start out
+with something small, write tests and contribute them. Even a small (failing)
+unit test which demonstrates a current shortcoming is great.
+
+You might also check out current skipped unit tests which usually represent
+missing functionality (though these might not be ideal beginner projects - if
+they were trivial to implement I would have done that already).
+
+All these shortcomings and limitations exist only because of the lack of
+time and/or awareness about certain XSD features. The goal of this library is
+to fully implement XSD schemas and potentially SOAP/WSDL so patches (with tests)
+are always welcome.
+
+Specific Items
+--------------
+
+- Fix circular dependency of generated schema classes.
+
+See the **TODO** markers in `soapfish/*.py` for a complete list.
```

### Comparing `soapfish2-0.7.1/README.md` & `soapfish2-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/TODO.md` & `soapfish2-0.7.2/TODO.md`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/docs/Makefile` & `soapfish2-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/docs/conf.py` & `soapfish2-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/docs/make.bat` & `soapfish2-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/docs/middlewares.rst` & `soapfish2-0.7.2/docs/middlewares.rst`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/docs/sslcontext.rst` & `soapfish2-0.7.2/docs/sslcontext.rst`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/docs/tutorial.rst` & `soapfish2-0.7.2/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/examples/client.py` & `soapfish2-0.7.2/examples/client.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/examples/flask_stock.py` & `soapfish2-0.7.2/examples/flask_stock.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/examples/ops.wsdl` & `soapfish2-0.7.2/examples/ops.wsdl`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/examples/ops.xsd` & `soapfish2-0.7.2/examples/ops.xsd`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/examples/stock/gen.py` & `soapfish2-0.7.2/examples/stock/gen.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/examples/stock/manage.py` & `soapfish2-0.7.2/examples/stock/manage.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/examples/stock/settings.py` & `soapfish2-0.7.2/examples/stock/settings.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/examples/xml_complex_types.py` & `soapfish2-0.7.2/examples/xml_complex_types.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/setup.cfg` & `soapfish2-0.7.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = soapfish2
-version = 0.7.1
+version = 0.7.2
 url = http://soapfish.org/
 download_url = http://soapfish.org/releases/
 author = Damian Powązka
 author_email = dpowazka@gmail.com
 maintainer = Felix Schwarz
 maintainer_email = felix.schwarz@oss.schwarz.eu
 description = No official SOAP library for Python
```

### Comparing `soapfish2-0.7.1/soapfish/core.py` & `soapfish2-0.7.2/soapfish/core.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/flask_.py` & `soapfish2-0.7.2/soapfish/flask_.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/lib/attribute_dict.py` & `soapfish2-0.7.2/soapfish/lib/attribute_dict.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/middlewares.py` & `soapfish2-0.7.2/soapfish/middlewares.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/namespaces.py` & `soapfish2-0.7.2/soapfish/namespaces.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/py2wsdl.py` & `soapfish2-0.7.2/soapfish/py2wsdl.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/py2xsd.py` & `soapfish2-0.7.2/soapfish/py2xsd.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/raw/wsa.xsd` & `soapfish2-0.7.2/soapfish/raw/wsa.xsd`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/soap.py` & `soapfish2-0.7.2/soapfish/soap.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/soap11.py` & `soapfish2-0.7.2/soapfish/soap11.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/soap12.py` & `soapfish2-0.7.2/soapfish/soap12.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/soap_dispatch.py` & `soapfish2-0.7.2/soapfish/soap_dispatch.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/templates/lib.jinja2` & `soapfish2-0.7.2/soapfish/templates/lib.jinja2`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/templates/wsdl.jinja2` & `soapfish2-0.7.2/soapfish/templates/wsdl.jinja2`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/templates/xsd.jinja2` & `soapfish2-0.7.2/soapfish/templates/xsd.jinja2`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/testutil/echo_service.py` & `soapfish2-0.7.2/soapfish/testutil/echo_service.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/testutil/framework.py` & `soapfish2-0.7.2/soapfish/testutil/framework.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/testutil/generated_symbols.py` & `soapfish2-0.7.2/soapfish/testutil/generated_symbols.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/testutil/simpletype_testcase.py` & `soapfish2-0.7.2/soapfish/testutil/simpletype_testcase.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/utils.py` & `soapfish2-0.7.2/soapfish/utils.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/wsa.py` & `soapfish2-0.7.2/soapfish/wsa.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/wsdl.py` & `soapfish2-0.7.2/soapfish/wsdl.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/wsdl11.py` & `soapfish2-0.7.2/soapfish/wsdl11.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/wsdl12.py` & `soapfish2-0.7.2/soapfish/wsdl12.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/wsdl2py.py` & `soapfish2-0.7.2/soapfish/wsdl2py.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/xsd.py` & `soapfish2-0.7.2/soapfish/xsd.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/xsd2py.py` & `soapfish2-0.7.2/soapfish/xsd2py.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/xsd_types.py` & `soapfish2-0.7.2/soapfish/xsd_types.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish/xsdspec.py` & `soapfish2-0.7.2/soapfish/xsdspec.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/soapfish2.egg-info/SOURCES.txt` & `soapfish2-0.7.2/soapfish2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/assets/generation/attrgroup_usage.xsd` & `soapfish2-0.7.2/tests/assets/generation/attrgroup_usage.xsd`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/assets/generation/default.wsdl` & `soapfish2-0.7.2/tests/assets/generation/default.wsdl`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/assets/generation/default.xsd` & `soapfish2-0.7.2/tests/assets/generation/default.xsd`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/assets/generation/enumeration2.xsd` & `soapfish2-0.7.2/tests/assets/generation/enumeration2.xsd`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/assets/generation/extension.xsd` & `soapfish2-0.7.2/tests/assets/generation/extension.xsd`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/assets/generation/extension_imported.xsd` & `soapfish2-0.7.2/tests/assets/generation/extension_imported.xsd`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/assets/generation/extension_with_special_chars.xsd` & `soapfish2-0.7.2/tests/assets/generation/extension_with_special_chars.xsd`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/assets/generation/multi_schema.wsdl` & `soapfish2-0.7.2/tests/assets/generation/multi_schema.wsdl`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/assets/generation/reference_complex.xsd` & `soapfish2-0.7.2/tests/assets/generation/reference_complex.xsd`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/assets/generation/restriction.xsd` & `soapfish2-0.7.2/tests/assets/generation/restriction.xsd`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/assets/same_namespace/same_namespace.wsdl` & `soapfish2-0.7.2/tests/assets/same_namespace/same_namespace.wsdl`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/framework/django_test.py` & `soapfish2-0.7.2/tests/framework/django_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/framework/flask_test.py` & `soapfish2-0.7.2/tests/framework/flask_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/generation/code_test.py` & `soapfish2-0.7.2/tests/generation/code_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/generation/wsdl_code_test.py` & `soapfish2-0.7.2/tests/generation/wsdl_code_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/generation/xsd_attrs_code_test.py` & `soapfish2-0.7.2/tests/generation/xsd_attrs_code_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/generation/xsd_code_test.py` & `soapfish2-0.7.2/tests/generation/xsd_code_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/ops_test.py` & `soapfish2-0.7.2/tests/ops_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/py2xsd_test.py` & `soapfish2-0.7.2/tests/py2xsd_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/soap11_test.py` & `soapfish2-0.7.2/tests/soap11_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/soap12_test.py` & `soapfish2-0.7.2/tests/soap12_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/soap2_test.py` & `soapfish2-0.7.2/tests/soap2_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/soap_dispatcher_test.py` & `soapfish2-0.7.2/tests/soap_dispatcher_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/soap_test.py` & `soapfish2-0.7.2/tests/soap_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/utils_test.py` & `soapfish2-0.7.2/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/wsgi_soap_application_test.py` & `soapfish2-0.7.2/tests/wsgi_soap_application_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/xsd/date_test.py` & `soapfish2-0.7.2/tests/xsd/date_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/xsd/schema_test.py` & `soapfish2-0.7.2/tests/xsd/schema_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/xsd/string_test.py` & `soapfish2-0.7.2/tests/xsd/string_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/xsd/time_test.py` & `soapfish2-0.7.2/tests/xsd/time_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/xsd/xsd_choice_test.py` & `soapfish2-0.7.2/tests/xsd/xsd_choice_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/xsd/xsd_datetime_test.py` & `soapfish2-0.7.2/tests/xsd/xsd_datetime_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/xsd/xsd_ref_test.py` & `soapfish2-0.7.2/tests/xsd/xsd_ref_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/xsd_test.py` & `soapfish2-0.7.2/tests/xsd_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/xsd_types/xsddate_test.py` & `soapfish2-0.7.2/tests/xsd_types/xsddate_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/xsdspec_element_test.py` & `soapfish2-0.7.2/tests/xsdspec_element_test.py`

 * *Files identical despite different names*

### Comparing `soapfish2-0.7.1/tests/xsdspec_schema_test.py` & `soapfish2-0.7.2/tests/xsdspec_schema_test.py`

 * *Files identical despite different names*

