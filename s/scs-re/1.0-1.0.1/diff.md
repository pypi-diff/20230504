# Comparing `tmp/scs_re-1.0-py3.11-linux-x86_64.egg` & `tmp/scs_re-1.0.1-py3.11-linux-x86_64.egg`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 312824 bytes, number of entries: 19
--rwxr-xr-x  2.0 unx   797952 b- defN 23-May-03 22:40 scs_sre.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      433 b- defN 23-May-03 22:40 scs_sre.py
--rw-r--r--  2.0 unx      182 b- defN 23-May-03 22:40 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      246 b- defN 23-May-03 22:40 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-03 22:40 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx       40 b- defN 23-May-03 22:40 EGG-INFO/native_libs.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-03 22:40 EGG-INFO/not-zip-safe
--rw-r--r--  2.0 unx       15 b- defN 23-May-03 22:40 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx      937 b- defN 23-May-03 22:40 __pycache__/scs_sre.cpython-311.pyc
+Zip file size: 313470 bytes, number of entries: 19
+-rwxr-xr-x  2.0 unx   797952 b- defN 23-May-03 22:48 scs_sre.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      433 b- defN 23-May-03 22:48 scs_sre.py
+-rw-r--r--  2.0 unx     1553 b- defN 23-May-03 22:48 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      246 b- defN 23-May-03 22:48 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-03 22:48 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       40 b- defN 23-May-03 22:48 EGG-INFO/native_libs.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-03 22:48 EGG-INFO/not-zip-safe
+-rw-r--r--  2.0 unx       15 b- defN 23-May-03 22:48 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx      937 b- defN 23-May-03 22:48 __pycache__/scs_sre.cpython-311.pyc
 -rw-r--r--  2.0 unx    15877 b- defN 23-Apr-29 13:22 scs_re/__init__.py
 -rw-r--r--  2.0 unx     5445 b- defN 23-Apr-29 13:25 scs_re/_casefix.py
 -rw-r--r--  2.0 unx    26110 b- defN 23-May-03 22:23 scs_re/_compiler.py
 -rw-r--r--  2.0 unx     5930 b- defN 23-Apr-30 11:08 scs_re/_constants.py
 -rw-r--r--  2.0 unx    42112 b- defN 23-Apr-29 13:23 scs_re/_parser.py
--rw-r--r--  2.0 unx    19316 b- defN 23-May-03 22:40 scs_re/__pycache__/__init__.cpython-311.pyc
--rw-r--r--  2.0 unx     1859 b- defN 23-May-03 22:40 scs_re/__pycache__/_casefix.cpython-311.pyc
--rw-r--r--  2.0 unx    31938 b- defN 23-May-03 22:40 scs_re/__pycache__/_compiler.cpython-311.pyc
--rw-r--r--  2.0 unx     5963 b- defN 23-May-03 22:40 scs_re/__pycache__/_constants.cpython-311.pyc
--rw-r--r--  2.0 unx    49885 b- defN 23-May-03 22:40 scs_re/__pycache__/_parser.cpython-311.pyc
-19 files, 1004242 bytes uncompressed, 310306 bytes compressed:  69.1%
+-rw-r--r--  2.0 unx    19316 b- defN 23-May-03 22:48 scs_re/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--  2.0 unx     1859 b- defN 23-May-03 22:48 scs_re/__pycache__/_casefix.cpython-311.pyc
+-rw-r--r--  2.0 unx    31938 b- defN 23-May-03 22:48 scs_re/__pycache__/_compiler.cpython-311.pyc
+-rw-r--r--  2.0 unx     5963 b- defN 23-May-03 22:48 scs_re/__pycache__/_constants.cpython-311.pyc
+-rw-r--r--  2.0 unx    49885 b- defN 23-May-03 22:48 scs_re/__pycache__/_parser.cpython-311.pyc
+19 files, 1005613 bytes uncompressed, 310952 bytes compressed:  69.1%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,4 +1,28 @@
 Metadata-Version: 2.1
 Name: scs-re
-Version: 1.0
+Version: 1.0.1
 Summary: Modification of cpython `re` module in which patterns match any string that is a prefix of a matching string under its regex
+Description-Content-Type: text/markdown
+
+# Modified Regex for Syntactically Constrained LLM Sampling
+
+The `scs_re` package is a modified version of the python `re` module that returns a match for any prefix of a string matching the original regex pattern. For example, the pattern `^abcd` matches the string `abc`. This behavior is used to consider the validity of beams under a particular regex pattern during a language model's output generation.
+
+**Note**: This behavior is only expected for patterns that begin with `^` and end with `$` and therefore define a match contstraint over all characters in a sequence.
+
+### Building from source
+
+We use the _sre module from the python 3.11 branch of Python/cpython/Modules/_sre. You can clone the original source by running
+    ```bash
+    svn export https://github.com/python/cpython/branches/3.11/Modules/_sre _sre
+    ```
+The module requires python 3.11 headers to compile. To install run
+    ```bash
+    wget https://www.python.org/ftp/python/3.11.3/Python-3.11.3.tar.xz
+    tar xf Python-3.11.3.tar.xz
+    cd Python-3.11.3
+    ./configure --enable-optimizations --enable-shared
+    make -j$(nproc)
+    sudo make altinstall
+    ```
+Then you can install the package with `sudo python3.11 setup.py install` to install. **The python version you install to must be the same version whose headers were compiled against**.
```

## __pycache__/scs_sre.cpython-311.pyc

### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e295364 (Thu May  4 03:40:14 2023 UTC)
+moddate:  0x1f2b5364 (Thu May  4 03:48:47 2023 UTC)
 files sz: 433
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

