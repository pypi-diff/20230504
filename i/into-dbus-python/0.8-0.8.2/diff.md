# Comparing `tmp/into-dbus-python-0.8.tar.gz` & `tmp/into-dbus-python-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/into-dbus-python-0.8.tar", last modified: Tue Dec  8 01:24:31 2020, max compression
+gzip compressed data, was "into-dbus-python-0.8.2.tar", last modified: Thu May  4 13:08:11 2023, max compression
```

## Comparing `into-dbus-python-0.8.tar` & `into-dbus-python-0.8.2.tar`

### file list

```diff
@@ -1,27 +1,23 @@
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2020-12-08 01:23:55.000000 into-dbus-python-0.8/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    11358 2019-01-17 23:29:41.000000 into-dbus-python-0.8/LICENSE
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      192 2020-12-03 17:59:52.000000 into-dbus-python-0.8/MANIFEST.in
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     9046 2020-12-08 01:24:31.000000 into-dbus-python-0.8/PKG-INFO
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6938 2020-12-07 17:09:41.000000 into-dbus-python-0.8/README.rst
--rwxrwxr-x   0 mulhern   (1000) mulhern   (1000)     1492 2020-12-07 17:09:41.000000 into-dbus-python-0.8/check.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       41 2020-12-07 17:09:41.000000 into-dbus-python-0.8/requirements.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       38 2020-12-08 01:24:31.000000 into-dbus-python-0.8/setup.cfg
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1586 2020-12-07 17:09:41.000000 into-dbus-python-0.8/setup.py
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2020-12-08 01:23:55.000000 into-dbus-python-0.8/src/
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2020-12-08 01:23:55.000000 into-dbus-python-0.8/src/into_dbus_python/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      721 2020-12-07 17:09:41.000000 into-dbus-python-0.8/src/into_dbus_python/__init__.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2493 2020-12-07 17:09:41.000000 into-dbus-python-0.8/src/into_dbus_python/_errors.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4383 2020-12-08 00:49:06.000000 into-dbus-python-0.8/src/into_dbus_python/_signature.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      752 2020-12-08 01:19:55.000000 into-dbus-python-0.8/src/into_dbus_python/_version.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    11596 2020-12-08 00:49:06.000000 into-dbus-python-0.8/src/into_dbus_python/_xformer.py
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2020-12-08 01:24:31.000000 into-dbus-python-0.8/src/into_dbus_python.egg-info/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     9046 2020-12-08 01:24:31.000000 into-dbus-python-0.8/src/into_dbus_python.egg-info/PKG-INFO
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      539 2020-12-08 01:24:31.000000 into-dbus-python-0.8/src/into_dbus_python.egg-info/SOURCES.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        1 2020-12-08 01:24:31.000000 into-dbus-python-0.8/src/into_dbus_python.egg-info/dependency_links.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       45 2020-12-08 01:24:31.000000 into-dbus-python-0.8/src/into_dbus_python.egg-info/requires.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       17 2020-12-08 01:24:31.000000 into-dbus-python-0.8/src/into_dbus_python.egg-info/top_level.txt
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2020-12-08 01:23:55.000000 into-dbus-python-0.8/tests/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        0 2019-01-17 23:29:41.000000 into-dbus-python-0.8/tests/__init__.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3633 2020-12-08 00:49:06.000000 into-dbus-python-0.8/tests/test_deterministic.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    11208 2020-12-08 00:49:06.000000 into-dbus-python-0.8/tests/test_hypothesis.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      710 2020-12-08 01:02:53.000000 into-dbus-python-0.8/tox.ini
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-05-04 13:08:11.461207 into-dbus-python-0.8.2/
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)    11358 2021-06-03 21:47:37.000000 into-dbus-python-0.8.2/LICENSE
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)     7840 2023-05-04 13:08:11.461207 into-dbus-python-0.8.2/PKG-INFO
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     6938 2021-06-03 21:47:37.000000 into-dbus-python-0.8.2/README.rst
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)       81 2023-05-04 01:01:04.000000 into-dbus-python-0.8.2/pyproject.toml
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     1030 2023-05-04 13:08:11.461207 into-dbus-python-0.8.2/setup.cfg
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)      106 2023-05-04 01:01:04.000000 into-dbus-python-0.8.2/setup.py
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-05-04 13:08:11.458206 into-dbus-python-0.8.2/src/
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-05-04 13:08:11.460206 into-dbus-python-0.8.2/src/into_dbus_python/
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)      755 2023-05-04 01:01:04.000000 into-dbus-python-0.8.2/src/into_dbus_python/__init__.py
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     2493 2021-06-03 21:47:37.000000 into-dbus-python-0.8.2/src/into_dbus_python/_errors.py
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)     4369 2023-05-03 19:07:28.000000 into-dbus-python-0.8.2/src/into_dbus_python/_signature.py
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)      753 2023-05-04 02:13:19.000000 into-dbus-python-0.8.2/src/into_dbus_python/_version.py
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)    11572 2023-05-03 19:07:28.000000 into-dbus-python-0.8.2/src/into_dbus_python/_xformer.py
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-05-04 13:08:11.461207 into-dbus-python-0.8.2/src/into_dbus_python.egg-info/
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)     7840 2023-05-04 13:08:11.000000 into-dbus-python-0.8.2/src/into_dbus_python.egg-info/PKG-INFO
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)      490 2023-05-04 13:08:11.000000 into-dbus-python-0.8.2/src/into_dbus_python.egg-info/SOURCES.txt
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)        1 2023-05-04 13:08:11.000000 into-dbus-python-0.8.2/src/into_dbus_python.egg-info/dependency_links.txt
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)       45 2023-05-04 13:08:11.000000 into-dbus-python-0.8.2/src/into_dbus_python.egg-info/requires.txt
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)       17 2023-05-04 13:08:11.000000 into-dbus-python-0.8.2/src/into_dbus_python.egg-info/top_level.txt
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-05-04 13:08:11.461207 into-dbus-python-0.8.2/tests/
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     3856 2021-08-27 19:33:58.000000 into-dbus-python-0.8.2/tests/test_deterministic.py
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)    11206 2023-05-03 19:07:28.000000 into-dbus-python-0.8.2/tests/test_hypothesis.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `into-dbus-python-0.8/LICENSE` & `into-dbus-python-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `into-dbus-python-0.8/PKG-INFO` & `into-dbus-python-0.8.2/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,177 +1,157 @@
-Metadata-Version: 1.1
-Name: into-dbus-python
-Version: 0.8
-Summary: transforms values into properly wrapped dbus-python objects
-Home-page: https://github.com/stratis-storage/into-dbus-python
-Author: Anne Mulhern
-Author-email: amulhern@redhat.com
-License: Apache 2.0
-Description: A transformer to dbus-python types
-        ==================================
-        
-        Facilities for converting an object that inhabits core Python types, e.g.,
-        lists, ints, dicts, to an object that inhabits dbus-python types, e.g.,
-        dbus.Array, dbus.UInt32, dbus.Dictionary based on a specified dbus signature.
-        
-        Motivation
-        ----------
-        
-        The dbus-python library is a library of python bindings for libdbus. It does
-        not provide facilities to ensure that the types of the values that client code
-        places on the D-Bus conform to the required signature. The client code may
-        either be a D-Bus service, so that the values that it places on the D-Bus
-        should conform to the signature that it specifies, or, in some cases, a client
-        of the service, which must conform to the specifications of the service.
-        
-        If a service implements the Introspectable interface on its objects,
-        dbus-python will use the signature information to massage client messages
-        into the correct dbus types. If the Introspectable interface is unavailable,
-        dbus-python will guess the signature by recursively examining the values of
-        the arguments, and will then proceed the same as before. If the signature
-        contains a 'v', indicating a variant type, dbus-python must guess the type
-        of the correspdoning value. dbus-python can be instructed not to make use of
-        dbus introspection by setting the introspect parameter to false in the
-        appropriate methods.
-        
-        This library provides facilities to ensure that values placed on the D-Bus
-        conform to a given signature, by wrapping the values in the appropriate
-        constructors for this signature. It generates correct functions for any
-        valid signature.
-        
-        Usage and Implementation Hints
-        ------------------------------
-        
-        Usage of the library is fairly straightforward::
-        
-           >>> from into_dbus_python import xformers
-           >>> funcs = xformers("adq")
-           >>> len(funcs)
-           2
-        
-        Note that the length of the list of functions is the same as the number of
-        complete types in the signature. Each element in the list of functions is
-        a tuple. ::
-        
-            >>> funcs[0]
-            (<function ToDbusXformer._handleArray.<locals>.the_func at 0x7f4542f2d730>, 'ad')
-        
-        The first element is the function itself, the second is a string which
-        matches the complete type signature for which this function yields values of
-        the correct type. Applying this function yields the actual value ::
-        
-            >>> funcs[0][0]([2.3, 37.5])
-            (dbus.Array([dbus.Double(2.3), dbus.Double(37.5)], signature=dbus.Signature('d')), 0)
-        
-        In this example, the signature was "ad" so the resulting value is a dbus.Array
-        of dbus.Double objects. The signature parameter has the appropriate value;
-        it is just 'd', the symbol for the type of the elements in the array,
-        double. Note that the function also yields a tuple, the converted value and
-        an int, which represents the variant level. Since there was no "v" in the
-        signature, the variant level is 0.
-        
-        The generated functions will fail with an IntoDPError if passed invalid
-        arguments. ::
-        
-            >>> try:
-            ...     funcs[0][0](True)
-            ... except IntoDPError as err:
-            ...     print("bad arg")
-            ...
-            bad arg
-        
-        If any of the functions raises an exception that is not a subtype of
-        IntoDPError this constitutes a bug and is not part of the public API.
-        
-        Conveniences
-        ------------
-        The parser itself returns a list of tuples, of which generally only the first
-        element in the tuple is of interest to the client. The second element, the
-        string matched, is a necessary result for the recursive implementation,
-        but is not generally useful to the client. The resulting functions each
-        return a tuple of the transformed value and the variant level, generally only
-        the transformed value is of interest to the client.
-        
-        For this reason, the library provides a convenience function, xformer(),
-        which takes a signature and returns a function, which takes a list of objects
-        and returns the list, transformed to appropriate dbus types. It can be used
-        in the following way::
-        
-            >>> from into_dbus_python import xformer
-            >>> func = xformer("adq")
-            >>> func([[2.3, 34.0], 3])
-            [dbus.Array([dbus.Double(2.3), dbus.Double(34.0)], signature=dbus.Signature('d')), dbus.UInt16(3)]
-        
-        Note that the function must take a list of values, one for each complete type
-        in the signature. Here, there are two complete types "ad", and "q", and there
-        are two resulting values.
-        
-        If the signature contains a "v", for a variant type, the value must be a pair
-        of a signature and a value that inhabits that type. For example, ::
-        
-            >>> func = xformer("v")
-            >>> func([("aq", [0, 1])])
-            [dbus.Array([dbus.UInt16(0), dbus.UInt16(1)], signature=dbus.Signature('q'), variant_level=1)]
-        
-        Note that the variant level of the constructed Array object is 1. A non-zero
-        variant level in the dbus object indicates that the object is a variant.
-        In this example the variant level is just 1. Further nesting of variants is
-        permitted, the variant level increases by one with each level. ::
-        
-            >>> func([("av", [("q", 0)])])
-            [dbus.Array([dbus.UInt16(0, variant_level=1)], signature=dbus.Signature('v'), variant_level=2)]
-        
-        Here the variant level of the variant element in the array, 0, is 1, but the
-        variant level of the whole array is 2, since the array inhabits a variant type
-        and contains a variant element.
-        
-        Restrictions on Core Types
-        --------------------------
-        The generated functions place as few restrictions as possible on the types
-        of the values to be transformed. Generally speaking, a tuple is as good as a
-        list, since both are iterable. ::
-        
-            >>> func = xformer("adq")
-            >>> func([(2.3, 34.0), 3])
-            [dbus.Array([dbus.Double(2.3), dbus.Double(34.0)], signature=dbus.Signature('d')), dbus.UInt16(3)]
-        
-        However, the inhabitant of a dbus.Dictionary type must be an object with an
-        items() method which yields pairs of keys and values, e.g., a dict.
-        
-        The signature() function
-        ------------------------
-        This library also exposes a function, signature(), which, given a value in
-        dbus-python types, calculates its signature. It has the following relation
-        to the xformer() function.
-        
-        Let S be a signature. Let C be a list of values in Python core types.
-        Let V = xformer(S)(C). Then "".join(signature(v) for v in V) is equal to S.
-        
-        Technical Remarks
-        -----------------
-        
-        This package extends the parser for dbus signatures implemented in the
-        dbus-signature-pyparsing package
-        (https://github.com/stratis-storage/dbus-signature-pyparsing)
-        by adding actions to the individual parsers using the setParseAction() method.
-        
-        The package has undergone significant testing using the Hypothesis testing
-        library (http://hypothesis.works/) and the external Hypothesis strategy
-        implemented in the hs-dbus-signature package
-        (https://github.com/stratis-storage/hs-dbus-signature).
-        
-        Downstream packagers, if incorporating testing into their packaging, are
-        encouraged to use only the tests in the test_deterministic.py module, to
-        avoid testing failures that may arise due to the non-deterministic behavior
-        of Hypothesis tests.
-        
-Platform: Linux
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+A transformer to dbus-python types
+==================================
+
+Facilities for converting an object that inhabits core Python types, e.g.,
+lists, ints, dicts, to an object that inhabits dbus-python types, e.g.,
+dbus.Array, dbus.UInt32, dbus.Dictionary based on a specified dbus signature.
+
+Motivation
+----------
+
+The dbus-python library is a library of python bindings for libdbus. It does
+not provide facilities to ensure that the types of the values that client code
+places on the D-Bus conform to the required signature. The client code may
+either be a D-Bus service, so that the values that it places on the D-Bus
+should conform to the signature that it specifies, or, in some cases, a client
+of the service, which must conform to the specifications of the service.
+
+If a service implements the Introspectable interface on its objects,
+dbus-python will use the signature information to massage client messages
+into the correct dbus types. If the Introspectable interface is unavailable,
+dbus-python will guess the signature by recursively examining the values of
+the arguments, and will then proceed the same as before. If the signature
+contains a 'v', indicating a variant type, dbus-python must guess the type
+of the correspdoning value. dbus-python can be instructed not to make use of
+dbus introspection by setting the introspect parameter to false in the
+appropriate methods.
+
+This library provides facilities to ensure that values placed on the D-Bus
+conform to a given signature, by wrapping the values in the appropriate
+constructors for this signature. It generates correct functions for any
+valid signature.
+
+Usage and Implementation Hints
+------------------------------
+
+Usage of the library is fairly straightforward::
+
+   >>> from into_dbus_python import xformers
+   >>> funcs = xformers("adq")
+   >>> len(funcs)
+   2
+
+Note that the length of the list of functions is the same as the number of
+complete types in the signature. Each element in the list of functions is
+a tuple. ::
+
+    >>> funcs[0]
+    (<function ToDbusXformer._handleArray.<locals>.the_func at 0x7f4542f2d730>, 'ad')
+
+The first element is the function itself, the second is a string which
+matches the complete type signature for which this function yields values of
+the correct type. Applying this function yields the actual value ::
+
+    >>> funcs[0][0]([2.3, 37.5])
+    (dbus.Array([dbus.Double(2.3), dbus.Double(37.5)], signature=dbus.Signature('d')), 0)
+
+In this example, the signature was "ad" so the resulting value is a dbus.Array
+of dbus.Double objects. The signature parameter has the appropriate value;
+it is just 'd', the symbol for the type of the elements in the array,
+double. Note that the function also yields a tuple, the converted value and
+an int, which represents the variant level. Since there was no "v" in the
+signature, the variant level is 0.
+
+The generated functions will fail with an IntoDPError if passed invalid
+arguments. ::
+
+    >>> try:
+    ...     funcs[0][0](True)
+    ... except IntoDPError as err:
+    ...     print("bad arg")
+    ...
+    bad arg
+
+If any of the functions raises an exception that is not a subtype of
+IntoDPError this constitutes a bug and is not part of the public API.
+
+Conveniences
+------------
+The parser itself returns a list of tuples, of which generally only the first
+element in the tuple is of interest to the client. The second element, the
+string matched, is a necessary result for the recursive implementation,
+but is not generally useful to the client. The resulting functions each
+return a tuple of the transformed value and the variant level, generally only
+the transformed value is of interest to the client.
+
+For this reason, the library provides a convenience function, xformer(),
+which takes a signature and returns a function, which takes a list of objects
+and returns the list, transformed to appropriate dbus types. It can be used
+in the following way::
+
+    >>> from into_dbus_python import xformer
+    >>> func = xformer("adq")
+    >>> func([[2.3, 34.0], 3])
+    [dbus.Array([dbus.Double(2.3), dbus.Double(34.0)], signature=dbus.Signature('d')), dbus.UInt16(3)]
+
+Note that the function must take a list of values, one for each complete type
+in the signature. Here, there are two complete types "ad", and "q", and there
+are two resulting values.
+
+If the signature contains a "v", for a variant type, the value must be a pair
+of a signature and a value that inhabits that type. For example, ::
+
+    >>> func = xformer("v")
+    >>> func([("aq", [0, 1])])
+    [dbus.Array([dbus.UInt16(0), dbus.UInt16(1)], signature=dbus.Signature('q'), variant_level=1)]
+
+Note that the variant level of the constructed Array object is 1. A non-zero
+variant level in the dbus object indicates that the object is a variant.
+In this example the variant level is just 1. Further nesting of variants is
+permitted, the variant level increases by one with each level. ::
+
+    >>> func([("av", [("q", 0)])])
+    [dbus.Array([dbus.UInt16(0, variant_level=1)], signature=dbus.Signature('v'), variant_level=2)]
+
+Here the variant level of the variant element in the array, 0, is 1, but the
+variant level of the whole array is 2, since the array inhabits a variant type
+and contains a variant element.
+
+Restrictions on Core Types
+--------------------------
+The generated functions place as few restrictions as possible on the types
+of the values to be transformed. Generally speaking, a tuple is as good as a
+list, since both are iterable. ::
+
+    >>> func = xformer("adq")
+    >>> func([(2.3, 34.0), 3])
+    [dbus.Array([dbus.Double(2.3), dbus.Double(34.0)], signature=dbus.Signature('d')), dbus.UInt16(3)]
+
+However, the inhabitant of a dbus.Dictionary type must be an object with an
+items() method which yields pairs of keys and values, e.g., a dict.
+
+The signature() function
+------------------------
+This library also exposes a function, signature(), which, given a value in
+dbus-python types, calculates its signature. It has the following relation
+to the xformer() function.
+
+Let S be a signature. Let C be a list of values in Python core types.
+Let V = xformer(S)(C). Then "".join(signature(v) for v in V) is equal to S.
+
+Technical Remarks
+-----------------
+
+This package extends the parser for dbus signatures implemented in the
+dbus-signature-pyparsing package
+(https://github.com/stratis-storage/dbus-signature-pyparsing)
+by adding actions to the individual parsers using the setParseAction() method.
+
+The package has undergone significant testing using the Hypothesis testing
+library (http://hypothesis.works/) and the external Hypothesis strategy
+implemented in the hs-dbus-signature package
+(https://github.com/stratis-storage/hs-dbus-signature).
+
+Downstream packagers, if incorporating testing into their packaging, are
+encouraged to use only the tests in the test_deterministic.py module, to
+avoid testing failures that may arise due to the non-deterministic behavior
+of Hypothesis tests.
```

### Comparing `into-dbus-python-0.8/README.rst` & `into-dbus-python-0.8.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: into-dbus-python
+Version: 0.8.2
+Summary: "transforms values into properly wrapped dbus-python objects"
+Home-page: https://github.com/stratis-storage/into-dbus-python
+Author: Anne Mulhern
+Author-email: amulhern@redhat.com
+License: Apache-2.0
+Platform: Linux
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 A transformer to dbus-python types
 ==================================
 
 Facilities for converting an object that inhabits core Python types, e.g.,
 lists, ints, dicts, to an object that inhabits dbus-python types, e.g.,
 dbus.Array, dbus.UInt32, dbus.Dictionary based on a specified dbus signature.
```

### Comparing `into-dbus-python-0.8/src/into_dbus_python/__init__.py` & `into-dbus-python-0.8.2/src/into_dbus_python/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 # limitations under the License.
 """
 Top-level file for xformer.
 """
 
 from ._errors import IntoDPError
 from ._signature import signature
+from ._version import __version__
 from ._xformer import xformer, xformers
```

### Comparing `into-dbus-python-0.8/src/into_dbus_python/_errors.py` & `into-dbus-python-0.8.2/src/into_dbus_python/_errors.py`

 * *Files identical despite different names*

### Comparing `into-dbus-python-0.8/src/into_dbus_python/_signature.py` & `into-dbus-python-0.8.2/src/into_dbus_python/_signature.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,16 +49,15 @@
         return "v"
 
     if isinstance(dbus_object, dbus.Array):
         sigs = frozenset(signature(x) for x in dbus_object)
         len_sigs = len(sigs)
         if len_sigs > 1:
             raise IntoDPSignatureError(
-                "the dbus-python Array object %s has items with varying signatures"
-                % dbus_object,
+                f"the dbus-python Array object {dbus_object} has items with varying signatures",
                 dbus_object,
             )
 
         if len_sigs == 0:
             return "a" + dbus_object.signature
 
         return "a" + list(sigs)[0]
@@ -74,25 +73,25 @@
         len_key_sigs = len(key_sigs)
         len_value_sigs = len(value_sigs)
 
         if len_key_sigs != len_value_sigs:
             # It seems impossible to force a dbus-python Dictionary value
             # to have this property; the Dictionary constructor prevents it.
             raise IntoDPSignatureError(
-                "the dbus-python Dictionary object %s does not have a valid signature"
-                % dbus_object,
+                f"the dbus-python Dictionary object {dbus_object} "
+                f"does not have a valid signature",
                 dbus_object,
             )  # pragma: no cover
 
         if len_key_sigs > 1:
             # It seems impossible to force a dbus-python Dictionary value
             # to have this property; the Dictionary constructor prevents it.
             raise IntoDPSignatureError(
-                "the dbus-python Dictionary object %s has different signatures for different keys"
-                % dbus_object,
+                f"the dbus-python Dictionary object {dbus_object} "
+                f"has different signatures for different keys",
                 dbus_object,
             )  # pragma: no cover
 
         if len_key_sigs == 0:
             return "a{" + dbus_object.signature + "}"
 
         return "a{" + list(key_sigs)[0] + list(value_sigs)[0] + "}"
```

### Comparing `into-dbus-python-0.8/src/into_dbus_python/_version.py` & `into-dbus-python-0.8.2/src/into_dbus_python/_version.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 # limitations under the License.
 """
     Version information.
 
     .. moduleauthor::  mulhern  <amulhern@redhat.com>
 """
 
-__version__ = "0.08"
+__version__ = "0.8.2"
 __version_info__ = tuple(int(x) for x in __version__.split("."))
```

### Comparing `into-dbus-python-0.8/src/into_dbus_python/_xformer.py` & `into-dbus-python-0.8.2/src/into_dbus_python/_xformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                 :type a_list: list of `a
                 :param int variant: variant level of the value
                 :returns: a dbus Array of transformed values
                 :rtype: Array
                 """
                 if isinstance(a_list, dict):
                     raise IntoDPUnexpectedValueError(
-                        "expected a list for an array but found a dict: %s" % a_list,
+                        f"expected a list for an array but found a dict: {a_list}",
                         a_list,
                     )
                 elements = [func(x) for x in a_list]
 
                 return dbus.types.Array(elements, signature=sig, variant_level=variant)
 
             return (the_array_func, "a" + sig)
@@ -196,22 +196,22 @@
             :param int variant: variant index
             :returns: a dbus Struct of transformed values
             :rtype: Struct
             :raises IntoDPRuntimeError:
             """
             if isinstance(a_list, dict):
                 raise IntoDPUnexpectedValueError(
-                    "expected a simple sequence for the fields of a struct but found a dict: %s"
-                    % a_list,
+                    f"expected a simple sequence for the fields of a struct "
+                    f"but found a dict: {a_list}",
                     a_list,
                 )
             if len(a_list) != len(funcs):
                 raise IntoDPUnexpectedValueError(
-                    "expected %u elements for a struct, but found %u"
-                    % (len(funcs), len(a_list)),
+                    f"expected {len(funcs)} elements for a struct, "
+                    f"but found {len(a_list)}",
                     a_list,
                 )
             elements = [f(x) for (f, x) in zip(funcs, a_list)]
             return dbus.types.Struct(
                 elements, signature=signature, variant_level=variant
             )
 
@@ -329,14 +329,13 @@
         :type objects: list of object
 
         :returns: transformed objects
         :rtype: list of object (in dbus types)
         """
         if len(objects) != len(funcs):
             raise IntoDPUnexpectedValueError(
-                "expected %u items to transform but found %u"
-                % (len(funcs), len(objects)),
+                f"expected {len(funcs)} items to transform but found {len(objects)}",
                 objects,
             )
         return [f(a) for (f, a) in zip(funcs, objects)]
 
     return the_func
```

### Comparing `into-dbus-python-0.8/src/into_dbus_python.egg-info/PKG-INFO` & `into-dbus-python-0.8.2/src/into_dbus_python.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,177 +1,179 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: into-dbus-python
-Version: 0.8
-Summary: transforms values into properly wrapped dbus-python objects
+Version: 0.8.2
+Summary: "transforms values into properly wrapped dbus-python objects"
 Home-page: https://github.com/stratis-storage/into-dbus-python
 Author: Anne Mulhern
 Author-email: amulhern@redhat.com
-License: Apache 2.0
-Description: A transformer to dbus-python types
-        ==================================
-        
-        Facilities for converting an object that inhabits core Python types, e.g.,
-        lists, ints, dicts, to an object that inhabits dbus-python types, e.g.,
-        dbus.Array, dbus.UInt32, dbus.Dictionary based on a specified dbus signature.
-        
-        Motivation
-        ----------
-        
-        The dbus-python library is a library of python bindings for libdbus. It does
-        not provide facilities to ensure that the types of the values that client code
-        places on the D-Bus conform to the required signature. The client code may
-        either be a D-Bus service, so that the values that it places on the D-Bus
-        should conform to the signature that it specifies, or, in some cases, a client
-        of the service, which must conform to the specifications of the service.
-        
-        If a service implements the Introspectable interface on its objects,
-        dbus-python will use the signature information to massage client messages
-        into the correct dbus types. If the Introspectable interface is unavailable,
-        dbus-python will guess the signature by recursively examining the values of
-        the arguments, and will then proceed the same as before. If the signature
-        contains a 'v', indicating a variant type, dbus-python must guess the type
-        of the correspdoning value. dbus-python can be instructed not to make use of
-        dbus introspection by setting the introspect parameter to false in the
-        appropriate methods.
-        
-        This library provides facilities to ensure that values placed on the D-Bus
-        conform to a given signature, by wrapping the values in the appropriate
-        constructors for this signature. It generates correct functions for any
-        valid signature.
-        
-        Usage and Implementation Hints
-        ------------------------------
-        
-        Usage of the library is fairly straightforward::
-        
-           >>> from into_dbus_python import xformers
-           >>> funcs = xformers("adq")
-           >>> len(funcs)
-           2
-        
-        Note that the length of the list of functions is the same as the number of
-        complete types in the signature. Each element in the list of functions is
-        a tuple. ::
-        
-            >>> funcs[0]
-            (<function ToDbusXformer._handleArray.<locals>.the_func at 0x7f4542f2d730>, 'ad')
-        
-        The first element is the function itself, the second is a string which
-        matches the complete type signature for which this function yields values of
-        the correct type. Applying this function yields the actual value ::
-        
-            >>> funcs[0][0]([2.3, 37.5])
-            (dbus.Array([dbus.Double(2.3), dbus.Double(37.5)], signature=dbus.Signature('d')), 0)
-        
-        In this example, the signature was "ad" so the resulting value is a dbus.Array
-        of dbus.Double objects. The signature parameter has the appropriate value;
-        it is just 'd', the symbol for the type of the elements in the array,
-        double. Note that the function also yields a tuple, the converted value and
-        an int, which represents the variant level. Since there was no "v" in the
-        signature, the variant level is 0.
-        
-        The generated functions will fail with an IntoDPError if passed invalid
-        arguments. ::
-        
-            >>> try:
-            ...     funcs[0][0](True)
-            ... except IntoDPError as err:
-            ...     print("bad arg")
-            ...
-            bad arg
-        
-        If any of the functions raises an exception that is not a subtype of
-        IntoDPError this constitutes a bug and is not part of the public API.
-        
-        Conveniences
-        ------------
-        The parser itself returns a list of tuples, of which generally only the first
-        element in the tuple is of interest to the client. The second element, the
-        string matched, is a necessary result for the recursive implementation,
-        but is not generally useful to the client. The resulting functions each
-        return a tuple of the transformed value and the variant level, generally only
-        the transformed value is of interest to the client.
-        
-        For this reason, the library provides a convenience function, xformer(),
-        which takes a signature and returns a function, which takes a list of objects
-        and returns the list, transformed to appropriate dbus types. It can be used
-        in the following way::
-        
-            >>> from into_dbus_python import xformer
-            >>> func = xformer("adq")
-            >>> func([[2.3, 34.0], 3])
-            [dbus.Array([dbus.Double(2.3), dbus.Double(34.0)], signature=dbus.Signature('d')), dbus.UInt16(3)]
-        
-        Note that the function must take a list of values, one for each complete type
-        in the signature. Here, there are two complete types "ad", and "q", and there
-        are two resulting values.
-        
-        If the signature contains a "v", for a variant type, the value must be a pair
-        of a signature and a value that inhabits that type. For example, ::
-        
-            >>> func = xformer("v")
-            >>> func([("aq", [0, 1])])
-            [dbus.Array([dbus.UInt16(0), dbus.UInt16(1)], signature=dbus.Signature('q'), variant_level=1)]
-        
-        Note that the variant level of the constructed Array object is 1. A non-zero
-        variant level in the dbus object indicates that the object is a variant.
-        In this example the variant level is just 1. Further nesting of variants is
-        permitted, the variant level increases by one with each level. ::
-        
-            >>> func([("av", [("q", 0)])])
-            [dbus.Array([dbus.UInt16(0, variant_level=1)], signature=dbus.Signature('v'), variant_level=2)]
-        
-        Here the variant level of the variant element in the array, 0, is 1, but the
-        variant level of the whole array is 2, since the array inhabits a variant type
-        and contains a variant element.
-        
-        Restrictions on Core Types
-        --------------------------
-        The generated functions place as few restrictions as possible on the types
-        of the values to be transformed. Generally speaking, a tuple is as good as a
-        list, since both are iterable. ::
-        
-            >>> func = xformer("adq")
-            >>> func([(2.3, 34.0), 3])
-            [dbus.Array([dbus.Double(2.3), dbus.Double(34.0)], signature=dbus.Signature('d')), dbus.UInt16(3)]
-        
-        However, the inhabitant of a dbus.Dictionary type must be an object with an
-        items() method which yields pairs of keys and values, e.g., a dict.
-        
-        The signature() function
-        ------------------------
-        This library also exposes a function, signature(), which, given a value in
-        dbus-python types, calculates its signature. It has the following relation
-        to the xformer() function.
-        
-        Let S be a signature. Let C be a list of values in Python core types.
-        Let V = xformer(S)(C). Then "".join(signature(v) for v in V) is equal to S.
-        
-        Technical Remarks
-        -----------------
-        
-        This package extends the parser for dbus signatures implemented in the
-        dbus-signature-pyparsing package
-        (https://github.com/stratis-storage/dbus-signature-pyparsing)
-        by adding actions to the individual parsers using the setParseAction() method.
-        
-        The package has undergone significant testing using the Hypothesis testing
-        library (http://hypothesis.works/) and the external Hypothesis strategy
-        implemented in the hs-dbus-signature package
-        (https://github.com/stratis-storage/hs-dbus-signature).
-        
-        Downstream packagers, if incorporating testing into their packaging, are
-        encouraged to use only the tests in the test_deterministic.py module, to
-        avoid testing failures that may arise due to the non-deterministic behavior
-        of Hypothesis tests.
-        
+License: Apache-2.0
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+A transformer to dbus-python types
+==================================
+
+Facilities for converting an object that inhabits core Python types, e.g.,
+lists, ints, dicts, to an object that inhabits dbus-python types, e.g.,
+dbus.Array, dbus.UInt32, dbus.Dictionary based on a specified dbus signature.
+
+Motivation
+----------
+
+The dbus-python library is a library of python bindings for libdbus. It does
+not provide facilities to ensure that the types of the values that client code
+places on the D-Bus conform to the required signature. The client code may
+either be a D-Bus service, so that the values that it places on the D-Bus
+should conform to the signature that it specifies, or, in some cases, a client
+of the service, which must conform to the specifications of the service.
+
+If a service implements the Introspectable interface on its objects,
+dbus-python will use the signature information to massage client messages
+into the correct dbus types. If the Introspectable interface is unavailable,
+dbus-python will guess the signature by recursively examining the values of
+the arguments, and will then proceed the same as before. If the signature
+contains a 'v', indicating a variant type, dbus-python must guess the type
+of the correspdoning value. dbus-python can be instructed not to make use of
+dbus introspection by setting the introspect parameter to false in the
+appropriate methods.
+
+This library provides facilities to ensure that values placed on the D-Bus
+conform to a given signature, by wrapping the values in the appropriate
+constructors for this signature. It generates correct functions for any
+valid signature.
+
+Usage and Implementation Hints
+------------------------------
+
+Usage of the library is fairly straightforward::
+
+   >>> from into_dbus_python import xformers
+   >>> funcs = xformers("adq")
+   >>> len(funcs)
+   2
+
+Note that the length of the list of functions is the same as the number of
+complete types in the signature. Each element in the list of functions is
+a tuple. ::
+
+    >>> funcs[0]
+    (<function ToDbusXformer._handleArray.<locals>.the_func at 0x7f4542f2d730>, 'ad')
+
+The first element is the function itself, the second is a string which
+matches the complete type signature for which this function yields values of
+the correct type. Applying this function yields the actual value ::
+
+    >>> funcs[0][0]([2.3, 37.5])
+    (dbus.Array([dbus.Double(2.3), dbus.Double(37.5)], signature=dbus.Signature('d')), 0)
+
+In this example, the signature was "ad" so the resulting value is a dbus.Array
+of dbus.Double objects. The signature parameter has the appropriate value;
+it is just 'd', the symbol for the type of the elements in the array,
+double. Note that the function also yields a tuple, the converted value and
+an int, which represents the variant level. Since there was no "v" in the
+signature, the variant level is 0.
+
+The generated functions will fail with an IntoDPError if passed invalid
+arguments. ::
+
+    >>> try:
+    ...     funcs[0][0](True)
+    ... except IntoDPError as err:
+    ...     print("bad arg")
+    ...
+    bad arg
+
+If any of the functions raises an exception that is not a subtype of
+IntoDPError this constitutes a bug and is not part of the public API.
+
+Conveniences
+------------
+The parser itself returns a list of tuples, of which generally only the first
+element in the tuple is of interest to the client. The second element, the
+string matched, is a necessary result for the recursive implementation,
+but is not generally useful to the client. The resulting functions each
+return a tuple of the transformed value and the variant level, generally only
+the transformed value is of interest to the client.
+
+For this reason, the library provides a convenience function, xformer(),
+which takes a signature and returns a function, which takes a list of objects
+and returns the list, transformed to appropriate dbus types. It can be used
+in the following way::
+
+    >>> from into_dbus_python import xformer
+    >>> func = xformer("adq")
+    >>> func([[2.3, 34.0], 3])
+    [dbus.Array([dbus.Double(2.3), dbus.Double(34.0)], signature=dbus.Signature('d')), dbus.UInt16(3)]
+
+Note that the function must take a list of values, one for each complete type
+in the signature. Here, there are two complete types "ad", and "q", and there
+are two resulting values.
+
+If the signature contains a "v", for a variant type, the value must be a pair
+of a signature and a value that inhabits that type. For example, ::
+
+    >>> func = xformer("v")
+    >>> func([("aq", [0, 1])])
+    [dbus.Array([dbus.UInt16(0), dbus.UInt16(1)], signature=dbus.Signature('q'), variant_level=1)]
+
+Note that the variant level of the constructed Array object is 1. A non-zero
+variant level in the dbus object indicates that the object is a variant.
+In this example the variant level is just 1. Further nesting of variants is
+permitted, the variant level increases by one with each level. ::
+
+    >>> func([("av", [("q", 0)])])
+    [dbus.Array([dbus.UInt16(0, variant_level=1)], signature=dbus.Signature('v'), variant_level=2)]
+
+Here the variant level of the variant element in the array, 0, is 1, but the
+variant level of the whole array is 2, since the array inhabits a variant type
+and contains a variant element.
+
+Restrictions on Core Types
+--------------------------
+The generated functions place as few restrictions as possible on the types
+of the values to be transformed. Generally speaking, a tuple is as good as a
+list, since both are iterable. ::
+
+    >>> func = xformer("adq")
+    >>> func([(2.3, 34.0), 3])
+    [dbus.Array([dbus.Double(2.3), dbus.Double(34.0)], signature=dbus.Signature('d')), dbus.UInt16(3)]
+
+However, the inhabitant of a dbus.Dictionary type must be an object with an
+items() method which yields pairs of keys and values, e.g., a dict.
+
+The signature() function
+------------------------
+This library also exposes a function, signature(), which, given a value in
+dbus-python types, calculates its signature. It has the following relation
+to the xformer() function.
+
+Let S be a signature. Let C be a list of values in Python core types.
+Let V = xformer(S)(C). Then "".join(signature(v) for v in V) is equal to S.
+
+Technical Remarks
+-----------------
+
+This package extends the parser for dbus signatures implemented in the
+dbus-signature-pyparsing package
+(https://github.com/stratis-storage/dbus-signature-pyparsing)
+by adding actions to the individual parsers using the setParseAction() method.
+
+The package has undergone significant testing using the Hypothesis testing
+library (http://hypothesis.works/) and the external Hypothesis strategy
+implemented in the hs-dbus-signature package
+(https://github.com/stratis-storage/hs-dbus-signature).
+
+Downstream packagers, if incorporating testing into their packaging, are
+encouraged to use only the tests in the test_deterministic.py module, to
+avoid testing failures that may arise due to the non-deterministic behavior
+of Hypothesis tests.
```

### Comparing `into-dbus-python-0.8/tests/test_deterministic.py` & `into-dbus-python-0.8.2/tests/test_deterministic.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,24 +32,31 @@
     """
 
     def test_bad_array_value(self):
         """
         Verify that passing a dict for an array will raise an exception.
         """
         with self.assertRaises(IntoDPUnexpectedValueError):
-            xformer("a(qq)")([dict()])
+            xformer("a(qq)")([{}])
 
     def test_bad_base_case_value(self):
         """
         Verify that transforming a string to a numeric value will raise an
         exception.
         """
         with self.assertRaises(IntoDPUnexpectedValueError):
             xformer("x")(["string"])
 
+    def test_bad_struct_value(self):
+        """
+        Verify that transforming a dict when a struct is expected fails.
+        """
+        with self.assertRaises(IntoDPUnexpectedValueError):
+            xformer("(qq)")({})
+
     def test_variant_depth(self):
         """
         Verify that a nested variant has appropriate variant depth.
         """
         self.assertEqual(
             xformer("v")([("v", ("v", ("b", False)))])[0],
             dbus.Boolean(False, variant_level=3),
```

### Comparing `into-dbus-python-0.8/tests/test_hypothesis.py` & `into-dbus-python-0.8.2/tests/test_hypothesis.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 
         self.assertEqual(sig_orig, sig_synth)
 
         self.assertEqual(signature(value), sig_orig)
 
     @given(
         dbus_signatures(min_complete_types=1, blacklist="h")
-        .map(lambda s: "(%s)" % s)
+        .map(lambda s: f"({s})")
         .flatmap(
             lambda s: strategies.tuples(
                 strategies.just(s), STRATEGY_GENERATOR.parseString(s, parseAll=True)[0]
             )
         )
     )
     @settings(
```

