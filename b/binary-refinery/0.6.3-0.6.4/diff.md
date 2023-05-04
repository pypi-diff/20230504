# Comparing `tmp/binary-refinery-0.6.3.tar.gz` & `tmp/binary-refinery-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/refinery/refinery/dist/.tmp-wywh22z2/binary-refinery-0.6.3.tar", last modified: Sat Apr 22 08:00:13 2023, max compression
+gzip compressed data, was "/home/runner/work/refinery/refinery/dist/.tmp-bndbqtg7/binary-refinery-0.6.4.tar", last modified: Thu May  4 17:30:57 2023, max compression
```

## Comparing `binary-refinery-0.6.3.tar` & `binary-refinery-0.6.4.tar`

### file list

```diff
@@ -1,379 +1,381 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/binary_refinery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/binary_refinery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11744 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/binary_refinery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/binary_refinery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/binary_refinery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/binary_refinery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/binary_refinery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/
--rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/__init__.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49846 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/data/rich.json
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/explore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59012 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/argformats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/decompression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/deobfuscation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/dex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/lib/dotnet/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/dotnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/dotnet/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    30549 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/dotnet/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/dotnet/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/dotnet/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)    23050 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)    23540 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)    34226 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/mime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/mscrypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/murmur.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/lib/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    16925 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/patterns/tlds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/powershell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/ripemd128.py
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/serpent.py
--rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/suffixtree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/lib/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/thirdparty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   163388 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/thirdparty/acefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/thirdparty/batch_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/thirdparty/pcode2code.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/thirdparty/xxhash.py
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/vfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/lib/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/
--rw-r--r--   0 runner    (1001) docker     (123)    69083 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/blockwise/
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/alu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/bitrev.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/byteswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/neg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/rev.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/rotl.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/rotr.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/shl.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/shr.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/terminate.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/blockwise/xor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/compression/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/ap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/blz.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/bz2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/jcalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lz4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lzf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lzg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lzjb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lznt1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/lzo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/mscf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/qlz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/szdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/compression/zl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/blowfish.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/camellia.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/chacha.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/des.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/des3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/gost.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/hc128.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/isaac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rabbit.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rc2.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rc4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rc4mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rc5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rc6.py
--rw-r--r--   0 runner    (1001) docker     (123)    48363 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rijndael.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rncrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/rsakey.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/salsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/seal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/secstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/serpent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/tea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/vigenere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/xtea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/cipher/xxtea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/checksums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/cryptographic.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/imphash.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/murmur.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/password_hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/hash/xxhash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/CryptDeriveKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/DESDerive.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/PasswordDeriveBytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/kblob.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/pbkdf1.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/pbkdf2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/crypto/keyderive/unixcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/atbash.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/b32.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/b58.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/b64.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/b85.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/cp1252.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/esc.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/htmlesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/netbios.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/ps1str.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/recode.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/u16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/uuenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/encoding/wshenc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/a3x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/formats/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xt7z.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtasar.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtcab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtcpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtiso.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtnode.py
--rw-r--r--   0 runner    (1001) docker     (123)    46900 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtnsis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtpyi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xttar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/archive/xtzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/bat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/deserialize_php.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/dexstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/evtx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/formats/exe/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/exe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/exe/vaddr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/exe/vmemref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/exe/vsect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/exe/vsnip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/exe/vstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/hexload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/httpresponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/ifps.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/ifpsstr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/formats/java/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/java/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/java/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/java/jvdasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/java/jvstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/msgpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/formats/office/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/doctxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/officecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/vbapc.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/vbastr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/xlmdeobf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/xlxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/xtdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/xtone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/xtrtf.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/office/xtvba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pcap_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/formats/pe/
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnblob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dncfx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnfields.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnhdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnmr.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnstr.py
--rw-r--r--   0 runner    (1001) docker     (123)    30943 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/pemeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/peoverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/perc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/pesig.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pe/pestrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/pkcs7sig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/stego.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/formats/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/malware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/malware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/malware/n40.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/chop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/cm.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/cull.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/dedup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/eat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/ef.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/iff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/iffp.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/iffs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/iffx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/max.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/min.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/mvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/mvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/pick.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/pop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/put.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/sep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/sorted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/meta/xfcc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/autoxor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/couple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/datefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/drp.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/nop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/urlfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/misc/xkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/obfuscation/
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/obfuscation/js/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/js/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/js/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/js/getattr.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/js/tuples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/brackets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/securestring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/stringreplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/typecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/ps1/uncurly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/brackets.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/char.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/dummies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/stringreplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/stringreverse.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/obfuscation/vba/vba.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve_7z.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve_pe.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve_rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/carve_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/defang.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/dnsdomain.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/mimewords.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/resplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/resub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/rex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/struct_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/subfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/urlguards.py
--rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/xtp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/pattern/xtw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/sinks/
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/asm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/iemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/peek.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/ppjscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/ppjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/sinks/ppxml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/refinery/units/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/cca.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/ccp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/cfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/clower.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/cswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/cupper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/rep.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/repl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/snip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/stretch.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/termfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/refinery/units/strings/trim.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-22 08:00:13.000000 binary-refinery-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-22 07:59:59.000000 binary-refinery-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/binary_refinery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/binary_refinery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/binary_refinery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/binary_refinery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/binary_refinery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/binary_refinery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/binary_refinery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/__init__.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49846 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/data/rich.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/explore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59048 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/argformats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/decompression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/deobfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/dex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/lib/dotnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/dotnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/dotnet/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30549 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/dotnet/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/dotnet/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/dotnet/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23050 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23540 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34515 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/mscrypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/murmur.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/lib/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    16925 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/patterns/tlds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/powershell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/ripemd128.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/serpent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/suffixtree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/lib/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/thirdparty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   163388 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/thirdparty/acefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/thirdparty/batch_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/thirdparty/pcode2code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/thirdparty/xxhash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/vfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/lib/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    70098 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/blockwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/alu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/bitrev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/byteswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/neg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/rev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/rotl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/rotr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/shl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/shr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/terminate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/blockwise/xor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/blz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/bz2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/jcalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/lz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/lz4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/lzf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/lzg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/lzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/lzjb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/lznt1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/lzo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/mscf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/qlz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/szdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/compression/zl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/camellia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/chacha.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/des.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/des3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/gost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/hc128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/isaac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/rc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/rc4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/rc4mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/rc5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/rc6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48363 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/rijndael.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/rncrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/rot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/rsakey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/salsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/seal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/secstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/serpent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/tea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/vigenere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/xtea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/cipher/xxtea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/crypto/hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/hash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/hash/checksums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/hash/cryptographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/hash/imphash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/hash/murmur.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/hash/password_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/hash/xxhash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/crypto/keyderive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/keyderive/CryptDeriveKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/keyderive/DESDerive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/keyderive/PasswordDeriveBytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/keyderive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/keyderive/hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/keyderive/hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/keyderive/kblob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/keyderive/pbkdf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/keyderive/pbkdf2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/crypto/keyderive/unixcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/atbash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/b32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/b58.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/b64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/b85.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/cp1252.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/esc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/htmlesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/netbios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/ps1str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/recode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/u16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/uuenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/encoding/wshenc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/a3x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/formats/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/archive/xt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/archive/xt7z.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/archive/xtace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/archive/xtasar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/archive/xtcab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/archive/xtcpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/archive/xtiso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/archive/xtiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/archive/xtnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46989 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/archive/xtnsis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/archive/xtpyi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/archive/xttar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/archive/xtzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/bat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/deserialize_php.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/dexstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/evtx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/formats/exe/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/exe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/exe/vaddr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/exe/vmemref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/exe/vsect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/exe/vsnip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/exe/vstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/hexload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/httpresponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/ifps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/ifpsstr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/formats/java/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/java/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/java/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/java/jvdasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/java/jvstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11032 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/msi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/formats/office/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/office/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/office/doctxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/office/officecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/office/vbapc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/office/vbastr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/office/xlmdeobf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/office/xlxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/office/xtdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/office/xtone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/office/xtrtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/office/xtvba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pcap_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/formats/pe/
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/dnblob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/dncfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/dnds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/dnfields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/dnhdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/dnmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/dnrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/dnstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30943 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pe/pemeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pe/peoverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pe/perc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pe/pesig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pe/pestrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/pkcs7sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/stego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/tnetmtm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/formats/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/malware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/malware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/malware/n40.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/chop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/cm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/cull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/dedup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/eat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/ef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/iff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/iffp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/iffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/iffx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/min.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/mvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/mvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/pick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/pop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/sep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/sorted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/meta/xfcc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/misc/autoxor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/misc/couple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/misc/datefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/misc/drp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/misc/nop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/misc/urlfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/misc/xkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/obfuscation/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/js/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/js/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/js/getattr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/js/tuples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/obfuscation/ps1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/ps1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/ps1/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/ps1/brackets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/ps1/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/ps1/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/ps1/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/ps1/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/ps1/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/ps1/securestring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/ps1/stringreplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/ps1/typecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/ps1/uncurly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/obfuscation/vba/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/vba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/vba/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/vba/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/vba/brackets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/vba/char.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/vba/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/vba/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/vba/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/vba/dummies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/vba/stringreplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/vba/stringreverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/obfuscation/vba/vba.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/carve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/carve_7z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/carve_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/carve_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/carve_pe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/carve_rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/carve_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/carve_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/defang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/dnsdomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/mimewords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/resplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/resub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/rex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/struct_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/subfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/urlguards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/xtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/pattern/xtw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/sinks/asm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/sinks/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/sinks/iemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/sinks/peek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/sinks/ppjscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/sinks/ppjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/sinks/ppxml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/refinery/units/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/strings/cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/strings/ccp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/strings/cfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/strings/clower.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/strings/cswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/strings/cupper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/strings/rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/strings/repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/strings/snip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/strings/stretch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/strings/termfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/refinery/units/strings/trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-04 17:30:57.000000 binary-refinery-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-04 17:30:37.000000 binary-refinery-0.6.4/setup.py
```

### Comparing `binary-refinery-0.6.3/LICENSE` & `binary-refinery-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/PKG-INFO` & `binary-refinery-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-refinery
-Version: 0.6.3
+Version: 0.6.4
 Summary: A toolkit to transform and refine (mostly) binary data.
 Home-page: https://github.com/binref/refinery/
 Author: Jesko Huettenhain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -38,14 +38,15 @@
 Provides-Extra: vmemref
 Provides-Extra: vstack
 Provides-Extra: vbapc
 Provides-Extra: vbastr
 Provides-Extra: xtrtf
 Provides-Extra: xtvba
 Provides-Extra: pcap
+Provides-Extra: tnetmtm
 Provides-Extra: transpose
 Provides-Extra: asm
 Provides-Extra: iemap
 Provides-Extra: peek
 Provides-Extra: ppjscript
 License-File: LICENSE
```

### Comparing `binary-refinery-0.6.3/README.md` & `binary-refinery-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/binary_refinery.egg-info/PKG-INFO` & `binary-refinery-0.6.4/binary_refinery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-refinery
-Version: 0.6.3
+Version: 0.6.4
 Summary: A toolkit to transform and refine (mostly) binary data.
 Home-page: https://github.com/binref/refinery/
 Author: Jesko Huettenhain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -38,14 +38,15 @@
 Provides-Extra: vmemref
 Provides-Extra: vstack
 Provides-Extra: vbapc
 Provides-Extra: vbastr
 Provides-Extra: xtrtf
 Provides-Extra: xtvba
 Provides-Extra: pcap
+Provides-Extra: tnetmtm
 Provides-Extra: transpose
 Provides-Extra: asm
 Provides-Extra: iemap
 Provides-Extra: peek
 Provides-Extra: ppjscript
 License-File: LICENSE
```

### Comparing `binary-refinery-0.6.3/binary_refinery.egg-info/SOURCES.txt` & `binary-refinery-0.6.4/binary_refinery.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -170,20 +170,22 @@
 refinery/units/formats/html.py
 refinery/units/formats/httpresponse.py
 refinery/units/formats/ifps.py
 refinery/units/formats/ifpsstr.py
 refinery/units/formats/json.py
 refinery/units/formats/lnk.py
 refinery/units/formats/msgpack.py
+refinery/units/formats/msi.py
 refinery/units/formats/pcap.py
 refinery/units/formats/pcap_http.py
 refinery/units/formats/pdf.py
 refinery/units/formats/pkcs7.py
 refinery/units/formats/pkcs7sig.py
 refinery/units/formats/stego.py
+refinery/units/formats/tnetmtm.py
 refinery/units/formats/winreg.py
 refinery/units/formats/xml.py
 refinery/units/formats/archive/__init__.py
 refinery/units/formats/archive/xt.py
 refinery/units/formats/archive/xt7z.py
 refinery/units/formats/archive/xtace.py
 refinery/units/formats/archive/xtasar.py
```

### Comparing `binary-refinery-0.6.3/binary_refinery.egg-info/entry_points.txt` & `binary-refinery-0.6.4/binary_refinery.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -224,14 +224,15 @@
 sub = refinery.units.blockwise.sub:sub.run
 subfiles = refinery.units.pattern.subfiles:subfiles.run
 swap = refinery.units.meta.swap:swap.run
 szdd = refinery.units.compression.szdd:szdd.run
 tea = refinery.units.crypto.cipher.tea:tea.run
 termfit = refinery.units.strings.termfit:termfit.run
 terminate = refinery.units.blockwise.terminate:terminate.run
+tnetmtm = refinery.units.formats.tnetmtm:tnetmtm.run
 transpose = refinery.units.meta.transpose:transpose.run
 trim = refinery.units.strings.trim:trim.run
 u16 = refinery.units.encoding.u16:u16.run
 ucrypt = refinery.units.crypto.keyderive.unixcrypt:ucrypt.run
 url = refinery.units.encoding.url:url.run
 urlfix = refinery.units.misc.urlfix:urlfix.run
 urlguards = refinery.units.pattern.urlguards:urlguards.run
@@ -262,14 +263,15 @@
 xtdoc = refinery.units.formats.office.xtdoc:xtdoc.run
 xtea = refinery.units.crypto.cipher.xtea:xtea.run
 xthtml = refinery.units.formats.html:xthtml.run
 xtiso = refinery.units.formats.archive.xtiso:xtiso.run
 xtiss = refinery.units.formats.archive.xtiss:xtiss.run
 xtjson = refinery.units.formats.json:xtjson.run
 xtmail = refinery.units.formats.email:xtmail.run
+xtmsi = refinery.units.formats.msi:xtmsi.run
 xtnode = refinery.units.formats.archive.xtnode:xtnode.run
 xtnsis = refinery.units.formats.archive.xtnsis:xtnsis.run
 xtone = refinery.units.formats.office.xtone:xtone.run
 xtp = refinery.units.pattern.xtp:xtp.run
 xtpdf = refinery.units.formats.pdf:xtpdf.run
 xtpyi = refinery.units.formats.archive.xtpyi:xtpyi.run
 xtrtf = refinery.units.formats.office.xtrtf:xtrtf.run
```

### Comparing `binary-refinery-0.6.3/binary_refinery.egg-info/requires.txt` & `binary-refinery-0.6.4/binary_refinery.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,55 +5,56 @@
 pefile
 pycryptodomex
 pyelftools
 setuptools
 toml
 wheel
 python-magic
-XLMMacroDeobfuscator
-phpserialize
-pycdlib
-xdis
-pyonenote
-decompyle3
-cabarchive
+python-registry
 pyperclip
-LnkParse3
 capstone
+pyonenote
+pyxlsb2
 xlrd2
-PyPDF2>=3.0.0
 openpyxl
-extract-msg
+Pillow
+cabarchive
+LnkParse3
+phpserialize
+xdis
+olefile
 asn1crypto
+javaobj-py3>=0.4.0.1
+decompyle3
 chardet
+uncompyle6
+extract-msg
 py7zr
+pycdlib
+XLMMacroDeobfuscator
 msoffcrypto-tool
-uncompyle6
-pyxlsb2
-olefile
-Pillow
-python-registry
-javaobj-py3>=0.4.0.1
+PyPDF2>=3.0.0
 
 [add]
 numpy
 
 [all]
-angr
 colorama
-python-evtx
-oletools
 jsbeautifier
+angr
+unicorn
+chardet
+python-evtx
 capstone
-numpy
-pypcapkit[scapy]<0.16.0
+oletools
 intervaltree
+pypcapkit[scapy]<0.16.0
 pyzipper
-unicorn
-chardet
+mitmproxy
+numpy
 
 [alu]
 numpy
 
 [asm]
 angr
 
@@ -110,30 +111,33 @@
 
 [shr]
 numpy
 
 [sub]
 numpy
 
+[tnetmtm]
+mitmproxy
+
 [transpose]
 numpy
 
 [vbapc]
 oletools
 
 [vbastr]
 oletools
 
 [vmemref]
 angr
 
 [vstack]
+unicorn
 intervaltree
 capstone
-unicorn
 
 [xor]
 numpy
 
 [xtrtf]
 oletools
```

### Comparing `binary-refinery-0.6.3/refinery/__init__.pkl` & `binary-refinery-0.6.4/refinery/__init__.pkl`

 * *Files 6% similar despite different names*

```diff
@@ -432,486 +432,493 @@
 00001af0: 0100 006a 1001 0000 5803 0000 006c 6e6b  ...j....X....lnk
 00001b00: 7213 0100 0058 1a00 0000 7265 6669 6e65  r....X....refine
 00001b10: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
 00001b20: 2e6c 6e6b 7214 0100 0058 0700 0000 6d73  .lnkr....X....ms
 00001b30: 6770 6163 6b72 1501 0000 581e 0000 0072  gpackr....X....r
 00001b40: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
 00001b50: 726d 6174 732e 6d73 6770 6163 6b72 1601  rmats.msgpackr..
-00001b60: 0000 5806 0000 0064 6f63 7478 7472 1701  ..X....doctxtr..
-00001b70: 0000 5824 0000 0072 6566 696e 6572 792e  ..X$...refinery.
-00001b80: 756e 6974 732e 666f 726d 6174 732e 6f66  units.formats.of
-00001b90: 6669 6365 2e64 6f63 7478 7472 1801 0000  fice.doctxtr....
-00001ba0: 580b 0000 006f 6666 6963 6563 7279 7074  X....officecrypt
-00001bb0: 7219 0100 0058 2900 0000 7265 6669 6e65  r....X)...refine
-00001bc0: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
-00001bd0: 2e6f 6666 6963 652e 6f66 6669 6365 6372  .office.officecr
-00001be0: 7970 7472 1a01 0000 5805 0000 0076 6261  yptr....X....vba
-00001bf0: 7063 721b 0100 0058 2300 0000 7265 6669  pcr....X#...refi
-00001c00: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
-00001c10: 7473 2e6f 6666 6963 652e 7662 6170 6372  ts.office.vbapcr
-00001c20: 1c01 0000 5806 0000 0076 6261 7374 7272  ....X....vbastrr
-00001c30: 1d01 0000 5824 0000 0072 6566 696e 6572  ....X$...refiner
-00001c40: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-00001c50: 6f66 6669 6365 2e76 6261 7374 7272 1e01  office.vbastrr..
-00001c60: 0000 5808 0000 0078 6c6d 6465 6f62 6672  ..X....xlmdeobfr
-00001c70: 1f01 0000 5826 0000 0072 6566 696e 6572  ....X&...refiner
-00001c80: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-00001c90: 6f66 6669 6365 2e78 6c6d 6465 6f62 6672  office.xlmdeobfr
-00001ca0: 2001 0000 5805 0000 0078 6c78 7472 7221   ...X....xlxtrr!
-00001cb0: 0100 0058 2300 0000 7265 6669 6e65 7279  ...X#...refinery
-00001cc0: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e6f  .units.formats.o
-00001cd0: 6666 6963 652e 786c 7874 7272 2201 0000  ffice.xlxtrr"...
-00001ce0: 5805 0000 0078 7464 6f63 7223 0100 0058  X....xtdocr#...X
-00001cf0: 2300 0000 7265 6669 6e65 7279 2e75 6e69  #...refinery.uni
-00001d00: 7473 2e66 6f72 6d61 7473 2e6f 6666 6963  ts.formats.offic
-00001d10: 652e 7874 646f 6372 2401 0000 5805 0000  e.xtdocr$...X...
-00001d20: 0078 746f 6e65 7225 0100 0058 2300 0000  .xtoner%...X#...
-00001d30: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
-00001d40: 6f72 6d61 7473 2e6f 6666 6963 652e 7874  ormats.office.xt
-00001d50: 6f6e 6572 2601 0000 5805 0000 0078 7472  oner&...X....xtr
-00001d60: 7466 7227 0100 0058 2300 0000 7265 6669  tfr'...X#...refi
-00001d70: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
-00001d80: 7473 2e6f 6666 6963 652e 7874 7274 6672  ts.office.xtrtfr
-00001d90: 2801 0000 5805 0000 0078 7476 6261 7229  (...X....xtvbar)
-00001da0: 0100 0058 2300 0000 7265 6669 6e65 7279  ...X#...refinery
-00001db0: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e6f  .units.formats.o
-00001dc0: 6666 6963 652e 7874 7662 6172 2a01 0000  ffice.xtvbar*...
-00001dd0: 5804 0000 0070 6361 7072 2b01 0000 581b  X....pcapr+...X.
-00001de0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00001df0: 732e 666f 726d 6174 732e 7063 6170 722c  s.formats.pcapr,
-00001e00: 0100 0058 0900 0000 7063 6170 5f68 7474  ...X....pcap_htt
-00001e10: 7072 2d01 0000 5820 0000 0072 6566 696e  pr-...X ...refin
-00001e20: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
-00001e30: 732e 7063 6170 5f68 7474 7072 2e01 0000  s.pcap_httpr....
-00001e40: 5805 0000 0078 7470 6466 722f 0100 0058  X....xtpdfr/...X
-00001e50: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-00001e60: 7473 2e66 6f72 6d61 7473 2e70 6466 7230  ts.formats.pdfr0
-00001e70: 0100 0058 0600 0000 646e 626c 6f62 7231  ...X....dnblobr1
-00001e80: 0100 0058 2700 0000 7265 6669 6e65 7279  ...X'...refinery
-00001e90: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e70  .units.formats.p
-00001ea0: 652e 646f 746e 6574 2e64 6e62 6c6f 6272  e.dotnet.dnblobr
-00001eb0: 3201 0000 5805 0000 0064 6e63 6678 7233  2...X....dncfxr3
-00001ec0: 0100 0058 2600 0000 7265 6669 6e65 7279  ...X&...refinery
-00001ed0: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e70  .units.formats.p
-00001ee0: 652e 646f 746e 6574 2e64 6e63 6678 7234  e.dotnet.dncfxr4
-00001ef0: 0100 0058 0400 0000 646e 6473 7235 0100  ...X....dndsr5..
-00001f00: 0058 2500 0000 7265 6669 6e65 7279 2e75  .X%...refinery.u
-00001f10: 6e69 7473 2e66 6f72 6d61 7473 2e70 652e  nits.formats.pe.
-00001f20: 646f 746e 6574 2e64 6e64 7372 3601 0000  dotnet.dndsr6...
-00001f30: 5808 0000 0064 6e66 6965 6c64 7372 3701  X....dnfieldsr7.
-00001f40: 0000 5829 0000 0072 6566 696e 6572 792e  ..X)...refinery.
-00001f50: 756e 6974 732e 666f 726d 6174 732e 7065  units.formats.pe
-00001f60: 2e64 6f74 6e65 742e 646e 6669 656c 6473  .dotnet.dnfields
-00001f70: 7238 0100 0058 0500 0000 646e 6864 7272  r8...X....dnhdrr
-00001f80: 3901 0000 5826 0000 0072 6566 696e 6572  9...X&...refiner
-00001f90: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-00001fa0: 7065 2e64 6f74 6e65 742e 646e 6864 7272  pe.dotnet.dnhdrr
-00001fb0: 3a01 0000 5804 0000 0064 6e6d 7272 3b01  :...X....dnmrr;.
-00001fc0: 0000 5825 0000 0072 6566 696e 6572 792e  ..X%...refinery.
-00001fd0: 756e 6974 732e 666f 726d 6174 732e 7065  units.formats.pe
-00001fe0: 2e64 6f74 6e65 742e 646e 6d72 723c 0100  .dotnet.dnmrr<..
-00001ff0: 0058 0400 0000 646e 7263 723d 0100 0058  .X....dnrcr=...X
-00002000: 2500 0000 7265 6669 6e65 7279 2e75 6e69  %...refinery.uni
-00002010: 7473 2e66 6f72 6d61 7473 2e70 652e 646f  ts.formats.pe.do
-00002020: 746e 6574 2e64 6e72 6372 3e01 0000 5805  tnet.dnrcr>...X.
-00002030: 0000 0064 6e73 7472 723f 0100 0058 2600  ...dnstrr?...X&.
-00002040: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00002050: 2e66 6f72 6d61 7473 2e70 652e 646f 746e  .formats.pe.dotn
-00002060: 6574 2e64 6e73 7472 7240 0100 0058 0600  et.dnstrr@...X..
-00002070: 0000 7065 6d65 7461 7241 0100 0058 2000  ..pemetarA...X .
-00002080: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00002090: 2e66 6f72 6d61 7473 2e70 652e 7065 6d65  .formats.pe.peme
-000020a0: 7461 7242 0100 0058 0900 0000 7065 6f76  tarB...X....peov
-000020b0: 6572 6c61 7972 4301 0000 5823 0000 0072  erlayrC...X#...r
-000020c0: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
-000020d0: 726d 6174 732e 7065 2e70 656f 7665 726c  rmats.pe.peoverl
-000020e0: 6179 7244 0100 0058 0400 0000 7065 7263  ayrD...X....perc
-000020f0: 7245 0100 0058 1e00 0000 7265 6669 6e65  rE...X....refine
-00002100: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
-00002110: 2e70 652e 7065 7263 7246 0100 0058 0500  .pe.percrF...X..
-00002120: 0000 7065 7369 6772 4701 0000 581f 0000  ..pesigrG...X...
-00002130: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00002140: 666f 726d 6174 732e 7065 2e70 6573 6967  formats.pe.pesig
-00002150: 7248 0100 0058 0700 0000 7065 7374 7269  rH...X....pestri
-00002160: 7072 4901 0000 5821 0000 0072 6566 696e  prI...X!...refin
-00002170: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
-00002180: 732e 7065 2e70 6573 7472 6970 724a 0100  s.pe.pestriprJ..
-00002190: 0058 0500 0000 706b 6373 3772 4b01 0000  .X....pkcs7rK...
-000021a0: 581c 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-000021b0: 6974 732e 666f 726d 6174 732e 706b 6373  its.formats.pkcs
-000021c0: 3772 4c01 0000 5808 0000 0070 6b63 7337  7rL...X....pkcs7
-000021d0: 7369 6772 4d01 0000 581f 0000 0072 6566  sigrM...X....ref
-000021e0: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
-000021f0: 6174 732e 706b 6373 3773 6967 724e 0100  ats.pkcs7sigrN..
-00002200: 0058 0500 0000 7374 6567 6f72 4f01 0000  .X....stegorO...
-00002210: 581c 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-00002220: 6974 732e 666f 726d 6174 732e 7374 6567  its.formats.steg
-00002230: 6f72 5001 0000 5806 0000 0077 696e 7265  orP...X....winre
-00002240: 6772 5101 0000 581d 0000 0072 6566 696e  grQ...X....refin
-00002250: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
-00002260: 732e 7769 6e72 6567 7252 0100 0058 0500  s.winregrR...X..
-00002270: 0000 7874 786d 6c72 5301 0000 581a 0000  ..xtxmlrS...X...
-00002280: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00002290: 666f 726d 6174 732e 786d 6c72 5401 0000  formats.xmlrT...
-000022a0: 5803 0000 006e 3430 7255 0100 0058 1a00  X....n40rU...X..
-000022b0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-000022c0: 2e6d 616c 7761 7265 2e6e 3430 7256 0100  .malware.n40rV..
-000022d0: 0058 0400 0000 6368 6f70 7257 0100 0058  .X....choprW...X
-000022e0: 1800 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-000022f0: 7473 2e6d 6574 612e 6368 6f70 7258 0100  ts.meta.choprX..
-00002300: 0058 0200 0000 636d 7259 0100 0058 1600  .X....cmrY...X..
-00002310: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00002320: 2e6d 6574 612e 636d 725a 0100 0058 0400  .meta.cmrZ...X..
-00002330: 0000 6375 6c6c 725b 0100 0058 1800 0000  ..cullr[...X....
-00002340: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
-00002350: 6574 612e 6375 6c6c 725c 0100 0058 0500  eta.cullr\...X..
-00002360: 0000 6465 6475 7072 5d01 0000 5819 0000  ..dedupr]...X...
-00002370: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00002380: 6d65 7461 2e64 6564 7570 725e 0100 0058  meta.dedupr^...X
-00002390: 0300 0000 6561 7472 5f01 0000 5817 0000  ....eatr_...X...
-000023a0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000023b0: 6d65 7461 2e65 6174 7260 0100 0058 0200  meta.eatr`...X..
-000023c0: 0000 6566 7261 0100 0058 1600 0000 7265  ..efra...X....re
-000023d0: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
-000023e0: 612e 6566 7262 0100 0058 0400 0000 656d  a.efrb...X....em
-000023f0: 6974 7263 0100 0058 1800 0000 7265 6669  itrc...X....refi
-00002400: 6e65 7279 2e75 6e69 7473 2e6d 6574 612e  nery.units.meta.
-00002410: 656d 6974 7264 0100 0058 0500 0000 6772  emitrd...X....gr
-00002420: 6f75 7072 6501 0000 5819 0000 0072 6566  oupre...X....ref
-00002430: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
-00002440: 2e67 726f 7570 7266 0100 0058 0700 0000  .grouprf...X....
-00002450: 6772 6f75 7062 7972 6701 0000 581b 0000  groupbyrg...X...
-00002460: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00002470: 6d65 7461 2e67 726f 7570 6279 7268 0100  meta.groupbyrh..
-00002480: 0058 0300 0000 6966 6672 6901 0000 5817  .X....iffri...X.
-00002490: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-000024a0: 732e 6d65 7461 2e69 6666 726a 0100 0058  s.meta.iffrj...X
-000024b0: 0400 0000 6966 6670 726b 0100 0058 1800  ....iffprk...X..
-000024c0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-000024d0: 2e6d 6574 612e 6966 6670 726c 0100 0058  .meta.iffprl...X
-000024e0: 0400 0000 6966 6673 726d 0100 0058 1800  ....iffsrm...X..
-000024f0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00002500: 2e6d 6574 612e 6966 6673 726e 0100 0058  .meta.iffsrn...X
-00002510: 0400 0000 6966 6678 726f 0100 0058 1800  ....iffxro...X..
-00002520: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00002530: 2e6d 6574 612e 6966 6678 7270 0100 0058  .meta.iffxrp...X
-00002540: 0400 0000 6d61 785f 7271 0100 0058 1700  ....max_rq...X..
-00002550: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00002560: 2e6d 6574 612e 6d61 7872 7201 0000 5804  .meta.maxrr...X.
-00002570: 0000 006d 696e 5f72 7301 0000 5817 0000  ...min_rs...X...
-00002580: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00002590: 6d65 7461 2e6d 696e 7274 0100 0058 0300  meta.minrt...X..
-000025a0: 0000 6d76 6372 7501 0000 5817 0000 0072  ..mvcru...X....r
-000025b0: 6566 696e 6572 792e 756e 6974 732e 6d65  efinery.units.me
-000025c0: 7461 2e6d 7663 7276 0100 0058 0300 0000  ta.mvcrv...X....
-000025d0: 6d76 6772 7701 0000 5817 0000 0072 6566  mvgrw...X....ref
-000025e0: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
-000025f0: 2e6d 7667 7278 0100 0058 0300 0000 7061  .mvgrx...X....pa
-00002600: 6472 7901 0000 5817 0000 0072 6566 696e  dry...X....refin
-00002610: 6572 792e 756e 6974 732e 6d65 7461 2e70  ery.units.meta.p
-00002620: 6164 727a 0100 0058 0400 0000 7069 636b  adrz...X....pick
-00002630: 727b 0100 0058 1800 0000 7265 6669 6e65  r{...X....refine
-00002640: 7279 2e75 6e69 7473 2e6d 6574 612e 7069  ry.units.meta.pi
-00002650: 636b 727c 0100 0058 0300 0000 706f 7072  ckr|...X....popr
-00002660: 7d01 0000 5817 0000 0072 6566 696e 6572  }...X....refiner
-00002670: 792e 756e 6974 732e 6d65 7461 2e70 6f70  y.units.meta.pop
-00002680: 727e 0100 0058 0400 0000 7075 7368 727f  r~...X....pushr.
-00002690: 0100 0058 1800 0000 7265 6669 6e65 7279  ...X....refinery
-000026a0: 2e75 6e69 7473 2e6d 6574 612e 7075 7368  .units.meta.push
-000026b0: 7280 0100 0058 0300 0000 7075 7472 8101  r....X....putr..
-000026c0: 0000 5817 0000 0072 6566 696e 6572 792e  ..X....refinery.
-000026d0: 756e 6974 732e 6d65 7461 2e70 7574 7282  units.meta.putr.
-000026e0: 0100 0058 0500 0000 7175 6575 6572 8301  ...X....queuer..
-000026f0: 0000 5819 0000 0072 6566 696e 6572 792e  ..X....refinery.
-00002700: 756e 6974 732e 6d65 7461 2e71 7565 7565  units.meta.queue
-00002710: 7284 0100 0058 0600 0000 7265 6475 6365  r....X....reduce
-00002720: 7285 0100 0058 1a00 0000 7265 6669 6e65  r....X....refine
-00002730: 7279 2e75 6e69 7473 2e6d 6574 612e 7265  ry.units.meta.re
-00002740: 6475 6365 7286 0100 0058 0500 0000 7363  ducer....X....sc
-00002750: 6f70 6572 8701 0000 5819 0000 0072 6566  oper....X....ref
-00002760: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
-00002770: 2e73 636f 7065 7288 0100 0058 0300 0000  .scoper....X....
-00002780: 7365 7072 8901 0000 5817 0000 0072 6566  sepr....X....ref
-00002790: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
-000027a0: 2e73 6570 728a 0100 0058 0600 0000 736f  .sepr....X....so
-000027b0: 7274 6564 728b 0100 0058 1a00 0000 7265  rtedr....X....re
-000027c0: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
-000027d0: 612e 736f 7274 6564 728c 0100 0058 0400  a.sortedr....X..
-000027e0: 0000 7377 6170 728d 0100 0058 1800 0000  ..swapr....X....
-000027f0: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
-00002800: 6574 612e 7377 6170 728e 0100 0058 0900  eta.swapr....X..
-00002810: 0000 7472 616e 7370 6f73 6572 8f01 0000  ..transposer....
-00002820: 581d 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-00002830: 6974 732e 6d65 7461 2e74 7261 6e73 706f  its.meta.transpo
-00002840: 7365 7290 0100 0058 0400 0000 7866 6363  ser....X....xfcc
-00002850: 7291 0100 0058 1800 0000 7265 6669 6e65  r....X....refine
-00002860: 7279 2e75 6e69 7473 2e6d 6574 612e 7866  ry.units.meta.xf
-00002870: 6363 7292 0100 0058 0700 0000 6175 746f  ccr....X....auto
-00002880: 786f 7272 9301 0000 581b 0000 0072 6566  xorr....X....ref
-00002890: 696e 6572 792e 756e 6974 732e 6d69 7363  inery.units.misc
-000028a0: 2e61 7574 6f78 6f72 7294 0100 0058 0600  .autoxorr....X..
-000028b0: 0000 636f 7570 6c65 7295 0100 0058 1a00  ..coupler....X..
-000028c0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-000028d0: 2e6d 6973 632e 636f 7570 6c65 7296 0100  .misc.coupler...
-000028e0: 0058 0700 0000 6461 7465 6669 7872 9701  .X....datefixr..
-000028f0: 0000 581b 0000 0072 6566 696e 6572 792e  ..X....refinery.
-00002900: 756e 6974 732e 6d69 7363 2e64 6174 6566  units.misc.datef
-00002910: 6978 7298 0100 0058 0300 0000 6472 7072  ixr....X....drpr
-00002920: 9901 0000 5817 0000 0072 6566 696e 6572  ....X....refiner
-00002930: 792e 756e 6974 732e 6d69 7363 2e64 7270  y.units.misc.drp
-00002940: 729a 0100 0058 0300 0000 6e6f 7072 9b01  r....X....nopr..
-00002950: 0000 5817 0000 0072 6566 696e 6572 792e  ..X....refinery.
-00002960: 756e 6974 732e 6d69 7363 2e6e 6f70 729c  units.misc.nopr.
-00002970: 0100 0058 0600 0000 7572 6c66 6978 729d  ...X....urlfixr.
-00002980: 0100 0058 1a00 0000 7265 6669 6e65 7279  ...X....refinery
-00002990: 2e75 6e69 7473 2e6d 6973 632e 7572 6c66  .units.misc.urlf
-000029a0: 6978 729e 0100 0058 0400 0000 786b 6579  ixr....X....xkey
-000029b0: 729f 0100 0058 1800 0000 7265 6669 6e65  r....X....refine
-000029c0: 7279 2e75 6e69 7473 2e6d 6973 632e 786b  ry.units.misc.xk
-000029d0: 6579 72a0 0100 0058 0e00 0000 6465 6f62  eyr....X....deob
-000029e0: 5f6a 735f 6172 7261 7973 72a1 0100 0058  _js_arraysr....X
-000029f0: 2400 0000 7265 6669 6e65 7279 2e75 6e69  $...refinery.uni
-00002a00: 7473 2e6f 6266 7573 6361 7469 6f6e 2e6a  ts.obfuscation.j
-00002a10: 732e 6172 7261 7973 72a2 0100 0058 0f00  s.arraysr....X..
-00002a20: 0000 6465 6f62 5f6a 735f 6765 7461 7474  ..deob_js_getatt
-00002a30: 7272 a301 0000 5825 0000 0072 6566 696e  rr....X%...refin
-00002a40: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
-00002a50: 6174 696f 6e2e 6a73 2e67 6574 6174 7472  ation.js.getattr
-00002a60: 72a4 0100 0058 0e00 0000 6465 6f62 5f6a  r....X....deob_j
-00002a70: 735f 7475 706c 6573 72a5 0100 0058 2400  s_tuplesr....X$.
-00002a80: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00002a90: 2e6f 6266 7573 6361 7469 6f6e 2e6a 732e  .obfuscation.js.
-00002aa0: 7475 706c 6573 72a6 0100 0058 0800 0000  tuplesr....X....
-00002ab0: 6465 6f62 5f70 7331 72a7 0100 0058 2200  deob_ps1r....X".
-00002ac0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00002ad0: 2e6f 6266 7573 6361 7469 6f6e 2e70 7331  .obfuscation.ps1
-00002ae0: 2e61 6c6c 72a8 0100 0058 1100 0000 6465  .allr....X....de
-00002af0: 6f62 5f70 7331 5f62 7261 636b 6574 7372  ob_ps1_bracketsr
-00002b00: a901 0000 5827 0000 0072 6566 696e 6572  ....X'...refiner
-00002b10: 792e 756e 6974 732e 6f62 6675 7363 6174  y.units.obfuscat
-00002b20: 696f 6e2e 7073 312e 6272 6163 6b65 7473  ion.ps1.brackets
-00002b30: 72aa 0100 0058 0e00 0000 6465 6f62 5f70  r....X....deob_p
-00002b40: 7331 5f63 6173 6573 72ab 0100 0058 2400  s1_casesr....X$.
-00002b50: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00002b60: 2e6f 6266 7573 6361 7469 6f6e 2e70 7331  .obfuscation.ps1
-00002b70: 2e63 6173 6573 72ac 0100 0058 0f00 0000  .casesr....X....
-00002b80: 6465 6f62 5f70 7331 5f63 6f6e 6361 7472  deob_ps1_concatr
-00002b90: ad01 0000 5825 0000 0072 6566 696e 6572  ....X%...refiner
-00002ba0: 792e 756e 6974 732e 6f62 6675 7363 6174  y.units.obfuscat
-00002bb0: 696f 6e2e 7073 312e 636f 6e63 6174 72ae  ion.ps1.concatr.
-00002bc0: 0100 0058 0f00 0000 6465 6f62 5f70 7331  ...X....deob_ps1
-00002bd0: 5f65 7363 6170 6572 af01 0000 5825 0000  _escaper....X%..
-00002be0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00002bf0: 6f62 6675 7363 6174 696f 6e2e 7073 312e  obfuscation.ps1.
-00002c00: 6573 6361 7065 72b0 0100 0058 0f00 0000  escaper....X....
-00002c10: 6465 6f62 5f70 7331 5f66 6f72 6d61 7472  deob_ps1_formatr
-00002c20: b101 0000 5825 0000 0072 6566 696e 6572  ....X%...refiner
-00002c30: 792e 756e 6974 732e 6f62 6675 7363 6174  y.units.obfuscat
-00002c40: 696f 6e2e 7073 312e 666f 726d 6174 72b2  ion.ps1.formatr.
-00002c50: 0100 0058 0f00 0000 6465 6f62 5f70 7331  ...X....deob_ps1
-00002c60: 5f69 6e76 6f6b 6572 b301 0000 5825 0000  _invoker....X%..
-00002c70: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00002c80: 6f62 6675 7363 6174 696f 6e2e 7073 312e  obfuscation.ps1.
-00002c90: 696e 766f 6b65 72b4 0100 0058 0f00 0000  invoker....X....
-00002ca0: 6465 6f62 5f70 7331 5f73 6563 7374 7272  deob_ps1_secstrr
-00002cb0: b501 0000 582b 0000 0072 6566 696e 6572  ....X+...refiner
-00002cc0: 792e 756e 6974 732e 6f62 6675 7363 6174  y.units.obfuscat
-00002cd0: 696f 6e2e 7073 312e 7365 6375 7265 7374  ion.ps1.securest
-00002ce0: 7269 6e67 72b6 0100 0058 1600 0000 6465  ringr....X....de
-00002cf0: 6f62 5f70 7331 5f73 7472 696e 6772 6570  ob_ps1_stringrep
-00002d00: 6c61 6365 72b7 0100 0058 2c00 0000 7265  lacer....X,...re
-00002d10: 6669 6e65 7279 2e75 6e69 7473 2e6f 6266  finery.units.obf
-00002d20: 7573 6361 7469 6f6e 2e70 7331 2e73 7472  uscation.ps1.str
-00002d30: 696e 6772 6570 6c61 6365 72b8 0100 0058  ingreplacer....X
-00002d40: 1100 0000 6465 6f62 5f70 7331 5f74 7970  ....deob_ps1_typ
-00002d50: 6563 6173 7472 b901 0000 5827 0000 0072  ecastr....X'...r
-00002d60: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
-00002d70: 6675 7363 6174 696f 6e2e 7073 312e 7479  fuscation.ps1.ty
-00002d80: 7065 6361 7374 72ba 0100 0058 1000 0000  pecastr....X....
-00002d90: 6465 6f62 5f70 7331 5f75 6e63 7572 6c79  deob_ps1_uncurly
-00002da0: 72bb 0100 0058 2600 0000 7265 6669 6e65  r....X&...refine
-00002db0: 7279 2e75 6e69 7473 2e6f 6266 7573 6361  ry.units.obfusca
-00002dc0: 7469 6f6e 2e70 7331 2e75 6e63 7572 6c79  tion.ps1.uncurly
-00002dd0: 72bc 0100 0058 0800 0000 6465 6f62 5f76  r....X....deob_v
-00002de0: 6261 72bd 0100 0058 2200 0000 7265 6669  bar....X"...refi
-00002df0: 6e65 7279 2e75 6e69 7473 2e6f 6266 7573  nery.units.obfus
-00002e00: 6361 7469 6f6e 2e76 6261 2e61 6c6c 72be  cation.vba.allr.
-00002e10: 0100 0058 1300 0000 6465 6f62 5f76 6261  ...X....deob_vba
-00002e20: 5f61 7269 7468 6d65 7469 6372 bf01 0000  _arithmeticr....
-00002e30: 5829 0000 0072 6566 696e 6572 792e 756e  X)...refinery.un
-00002e40: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
-00002e50: 7662 612e 6172 6974 686d 6574 6963 72c0  vba.arithmeticr.
-00002e60: 0100 0058 1100 0000 6465 6f62 5f76 6261  ...X....deob_vba
-00002e70: 5f62 7261 636b 6574 7372 c101 0000 5827  _bracketsr....X'
-00002e80: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00002e90: 732e 6f62 6675 7363 6174 696f 6e2e 7662  s.obfuscation.vb
-00002ea0: 612e 6272 6163 6b65 7473 72c2 0100 0058  a.bracketsr....X
-00002eb0: 1600 0000 6465 6f62 5f76 6261 5f63 6861  ....deob_vba_cha
-00002ec0: 725f 6675 6e63 7469 6f6e 72c3 0100 0058  r_functionr....X
-00002ed0: 2300 0000 7265 6669 6e65 7279 2e75 6e69  #...refinery.uni
-00002ee0: 7473 2e6f 6266 7573 6361 7469 6f6e 2e76  ts.obfuscation.v
-00002ef0: 6261 2e63 6861 7272 c401 0000 5811 0000  ba.charr....X...
-00002f00: 0064 656f 625f 7662 615f 636f 6d6d 656e  .deob_vba_commen
-00002f10: 7473 72c5 0100 0058 2700 0000 7265 6669  tsr....X'...refi
-00002f20: 6e65 7279 2e75 6e69 7473 2e6f 6266 7573  nery.units.obfus
-00002f30: 6361 7469 6f6e 2e76 6261 2e63 6f6d 6d65  cation.vba.comme
-00002f40: 6e74 7372 c601 0000 580f 0000 0064 656f  ntsr....X....deo
-00002f50: 625f 7662 615f 636f 6e63 6174 72c7 0100  b_vba_concatr...
-00002f60: 0058 2500 0000 7265 6669 6e65 7279 2e75  .X%...refinery.u
-00002f70: 6e69 7473 2e6f 6266 7573 6361 7469 6f6e  nits.obfuscation
-00002f80: 2e76 6261 2e63 6f6e 6361 7472 c801 0000  .vba.concatr....
-00002f90: 5812 0000 0064 656f 625f 7662 615f 636f  X....deob_vba_co
-00002fa0: 6e73 7461 6e74 7372 c901 0000 5828 0000  nstantsr....X(..
-00002fb0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00002fc0: 6f62 6675 7363 6174 696f 6e2e 7662 612e  obfuscation.vba.
-00002fd0: 636f 6e73 7461 6e74 7372 ca01 0000 5818  constantsr....X.
-00002fe0: 0000 0064 656f 625f 7662 615f 6475 6d6d  ...deob_vba_dumm
-00002ff0: 795f 7661 7269 6162 6c65 7372 cb01 0000  y_variablesr....
-00003000: 5826 0000 0072 6566 696e 6572 792e 756e  X&...refinery.un
-00003010: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
-00003020: 7662 612e 6475 6d6d 6965 7372 cc01 0000  vba.dummiesr....
-00003030: 5816 0000 0064 656f 625f 7662 615f 7374  X....deob_vba_st
-00003040: 7269 6e67 7265 706c 6163 6572 cd01 0000  ringreplacer....
-00003050: 582c 0000 0072 6566 696e 6572 792e 756e  X,...refinery.un
-00003060: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
-00003070: 7662 612e 7374 7269 6e67 7265 706c 6163  vba.stringreplac
-00003080: 6572 ce01 0000 5816 0000 0064 656f 625f  er....X....deob_
-00003090: 7662 615f 7374 7269 6e67 7265 7665 7273  vba_stringrevers
-000030a0: 6572 cf01 0000 582c 0000 0072 6566 696e  er....X,...refin
-000030b0: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
-000030c0: 6174 696f 6e2e 7662 612e 7374 7269 6e67  ation.vba.string
-000030d0: 7265 7665 7273 6572 d001 0000 5815 0000  reverser....X...
-000030e0: 0064 656f 625f 7662 615f 6368 725f 6c69  .deob_vba_chr_li
-000030f0: 7465 7261 6c73 72d1 0100 0058 2200 0000  teralsr....X"...
-00003100: 7265 6669 6e65 7279 2e75 6e69 7473 2e6f  refinery.units.o
-00003110: 6266 7573 6361 7469 6f6e 2e76 6261 2e76  bfuscation.vba.v
-00003120: 6261 72d2 0100 0058 0500 0000 6361 7276  bar....X....carv
-00003130: 6572 d301 0000 581c 0000 0072 6566 696e  er....X....refin
-00003140: 6572 792e 756e 6974 732e 7061 7474 6572  ery.units.patter
-00003150: 6e2e 6361 7276 6572 d401 0000 5808 0000  n.carver....X...
-00003160: 0063 6172 7665 5f37 7a72 d501 0000 581f  .carve_7zr....X.
-00003170: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00003180: 732e 7061 7474 6572 6e2e 6361 7276 655f  s.pattern.carve_
-00003190: 377a 72d6 0100 0058 0a00 0000 6361 7276  7zr....X....carv
-000031a0: 655f 6a73 6f6e 72d7 0100 0058 2100 0000  e_jsonr....X!...
-000031b0: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
-000031c0: 6174 7465 726e 2e63 6172 7665 5f6a 736f  attern.carve_jso
-000031d0: 6e72 d801 0000 5809 0000 0063 6172 7665  nr....X....carve
-000031e0: 5f6c 6e6b 72d9 0100 0058 2000 0000 7265  _lnkr....X ...re
-000031f0: 6669 6e65 7279 2e75 6e69 7473 2e70 6174  finery.units.pat
-00003200: 7465 726e 2e63 6172 7665 5f6c 6e6b 72da  tern.carve_lnkr.
-00003210: 0100 0058 0800 0000 6361 7276 655f 7065  ...X....carve_pe
-00003220: 72db 0100 0058 1f00 0000 7265 6669 6e65  r....X....refine
-00003230: 7279 2e75 6e69 7473 2e70 6174 7465 726e  ry.units.pattern
-00003240: 2e63 6172 7665 5f70 6572 dc01 0000 5809  .carve_per....X.
-00003250: 0000 0063 6172 7665 5f72 7466 72dd 0100  ...carve_rtfr...
-00003260: 0058 2000 0000 7265 6669 6e65 7279 2e75  .X ...refinery.u
-00003270: 6e69 7473 2e70 6174 7465 726e 2e63 6172  nits.pattern.car
-00003280: 7665 5f72 7466 72de 0100 0058 0900 0000  ve_rtfr....X....
-00003290: 6361 7276 655f 786d 6c72 df01 0000 5820  carve_xmlr....X 
-000032a0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-000032b0: 732e 7061 7474 6572 6e2e 6361 7276 655f  s.pattern.carve_
-000032c0: 786d 6c72 e001 0000 5809 0000 0063 6172  xmlr....X....car
-000032d0: 7665 5f7a 6970 72e1 0100 0058 2000 0000  ve_zipr....X ...
-000032e0: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
-000032f0: 6174 7465 726e 2e63 6172 7665 5f7a 6970  attern.carve_zip
-00003300: 72e2 0100 0058 0600 0000 6465 6661 6e67  r....X....defang
-00003310: 72e3 0100 0058 1d00 0000 7265 6669 6e65  r....X....refine
-00003320: 7279 2e75 6e69 7473 2e70 6174 7465 726e  ry.units.pattern
-00003330: 2e64 6566 616e 6772 e401 0000 5809 0000  .defangr....X...
-00003340: 0064 6e73 646f 6d61 696e 72e5 0100 0058  .dnsdomainr....X
-00003350: 2000 0000 7265 6669 6e65 7279 2e75 6e69   ...refinery.uni
-00003360: 7473 2e70 6174 7465 726e 2e64 6e73 646f  ts.pattern.dnsdo
-00003370: 6d61 696e 72e6 0100 0058 0900 0000 6d69  mainr....X....mi
-00003380: 6d65 776f 7264 7372 e701 0000 5820 0000  mewordsr....X ..
-00003390: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000033a0: 7061 7474 6572 6e2e 6d69 6d65 776f 7264  pattern.mimeword
-000033b0: 7372 e801 0000 5807 0000 0072 6573 706c  sr....X....respl
-000033c0: 6974 72e9 0100 0058 1e00 0000 7265 6669  itr....X....refi
-000033d0: 6e65 7279 2e75 6e69 7473 2e70 6174 7465  nery.units.patte
-000033e0: 726e 2e72 6573 706c 6974 72ea 0100 0058  rn.resplitr....X
-000033f0: 0500 0000 7265 7375 6272 eb01 0000 581c  ....resubr....X.
-00003400: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00003410: 732e 7061 7474 6572 6e2e 7265 7375 6272  s.pattern.resubr
-00003420: ec01 0000 5803 0000 0072 6578 72ed 0100  ....X....rexr...
-00003430: 0058 1a00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-00003440: 6e69 7473 2e70 6174 7465 726e 2e72 6578  nits.pattern.rex
-00003450: 72ee 0100 0058 0600 0000 7374 7275 6374  r....X....struct
-00003460: 72ef 0100 0058 2400 0000 7265 6669 6e65  r....X$...refine
-00003470: 7279 2e75 6e69 7473 2e70 6174 7465 726e  ry.units.pattern
-00003480: 2e73 7472 7563 745f 7061 7273 6572 72f0  .struct_parserr.
-00003490: 0100 0058 0800 0000 7375 6266 696c 6573  ...X....subfiles
-000034a0: 72f1 0100 0058 1f00 0000 7265 6669 6e65  r....X....refine
-000034b0: 7279 2e75 6e69 7473 2e70 6174 7465 726e  ry.units.pattern
-000034c0: 2e73 7562 6669 6c65 7372 f201 0000 5809  .subfilesr....X.
-000034d0: 0000 0075 726c 6775 6172 6473 72f3 0100  ...urlguardsr...
-000034e0: 0058 2000 0000 7265 6669 6e65 7279 2e75  .X ...refinery.u
-000034f0: 6e69 7473 2e70 6174 7465 726e 2e75 726c  nits.pattern.url
-00003500: 6775 6172 6473 72f4 0100 0058 0300 0000  guardsr....X....
-00003510: 7874 7072 f501 0000 581a 0000 0072 6566  xtpr....X....ref
-00003520: 696e 6572 792e 756e 6974 732e 7061 7474  inery.units.patt
-00003530: 6572 6e2e 7874 7072 f601 0000 5803 0000  ern.xtpr....X...
-00003540: 0078 7477 72f7 0100 0058 1a00 0000 7265  .xtwr....X....re
-00003550: 6669 6e65 7279 2e75 6e69 7473 2e70 6174  finery.units.pat
-00003560: 7465 726e 2e78 7477 72f8 0100 0058 0300  tern.xtwr....X..
-00003570: 0000 6173 6d72 f901 0000 5818 0000 0072  ..asmr....X....r
-00003580: 6566 696e 6572 792e 756e 6974 732e 7369  efinery.units.si
-00003590: 6e6b 732e 6173 6d72 fa01 0000 5804 0000  nks.asmr....X...
-000035a0: 0064 756d 7072 fb01 0000 5819 0000 0072  .dumpr....X....r
-000035b0: 6566 696e 6572 792e 756e 6974 732e 7369  efinery.units.si
-000035c0: 6e6b 732e 6475 6d70 72fc 0100 0058 0500  nks.dumpr....X..
-000035d0: 0000 6965 6d61 7072 fd01 0000 581a 0000  ..iemapr....X...
-000035e0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000035f0: 7369 6e6b 732e 6965 6d61 7072 fe01 0000  sinks.iemapr....
-00003600: 5804 0000 0070 6565 6b72 ff01 0000 5819  X....peekr....X.
-00003610: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00003620: 732e 7369 6e6b 732e 7065 656b 7200 0200  s.sinks.peekr...
-00003630: 0058 0900 0000 7070 6a73 6372 6970 7472  .X....ppjscriptr
-00003640: 0102 0000 581e 0000 0072 6566 696e 6572  ....X....refiner
-00003650: 792e 756e 6974 732e 7369 6e6b 732e 7070  y.units.sinks.pp
-00003660: 6a73 6372 6970 7472 0202 0000 5806 0000  jscriptr....X...
-00003670: 0070 706a 736f 6e72 0302 0000 581b 0000  .ppjsonr....X...
-00003680: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00003690: 7369 6e6b 732e 7070 6a73 6f6e 7204 0200  sinks.ppjsonr...
-000036a0: 0058 0500 0000 7070 786d 6c72 0502 0000  .X....ppxmlr....
-000036b0: 581a 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-000036c0: 6974 732e 7369 6e6b 732e 7070 786d 6c72  its.sinks.ppxmlr
-000036d0: 0602 0000 5803 0000 0063 6361 7207 0200  ....X....ccar...
-000036e0: 0058 1a00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-000036f0: 6e69 7473 2e73 7472 696e 6773 2e63 6361  nits.strings.cca
-00003700: 7208 0200 0058 0300 0000 6363 7072 0902  r....X....ccpr..
-00003710: 0000 581a 0000 0072 6566 696e 6572 792e  ..X....refinery.
-00003720: 756e 6974 732e 7374 7269 6e67 732e 6363  units.strings.cc
-00003730: 7072 0a02 0000 5804 0000 0063 666d 7472  pr....X....cfmtr
-00003740: 0b02 0000 581b 0000 0072 6566 696e 6572  ....X....refiner
-00003750: 792e 756e 6974 732e 7374 7269 6e67 732e  y.units.strings.
-00003760: 6366 6d74 720c 0200 0058 0600 0000 636c  cfmtr....X....cl
-00003770: 6f77 6572 720d 0200 0058 1d00 0000 7265  owerr....X....re
-00003780: 6669 6e65 7279 2e75 6e69 7473 2e73 7472  finery.units.str
-00003790: 696e 6773 2e63 6c6f 7765 7272 0e02 0000  ings.clowerr....
-000037a0: 5805 0000 0063 7377 6170 720f 0200 0058  X....cswapr....X
-000037b0: 1c00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-000037c0: 7473 2e73 7472 696e 6773 2e63 7377 6170  ts.strings.cswap
-000037d0: 7210 0200 0058 0600 0000 6375 7070 6572  r....X....cupper
+00001b60: 0000 5805 0000 0078 746d 7369 7217 0100  ..X....xtmsir...
+00001b70: 0058 1a00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+00001b80: 6e69 7473 2e66 6f72 6d61 7473 2e6d 7369  nits.formats.msi
+00001b90: 7218 0100 0058 0600 0000 646f 6374 7874  r....X....doctxt
+00001ba0: 7219 0100 0058 2400 0000 7265 6669 6e65  r....X$...refine
+00001bb0: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
+00001bc0: 2e6f 6666 6963 652e 646f 6374 7874 721a  .office.doctxtr.
+00001bd0: 0100 0058 0b00 0000 6f66 6669 6365 6372  ...X....officecr
+00001be0: 7970 7472 1b01 0000 5829 0000 0072 6566  yptr....X)...ref
+00001bf0: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
+00001c00: 6174 732e 6f66 6669 6365 2e6f 6666 6963  ats.office.offic
+00001c10: 6563 7279 7074 721c 0100 0058 0500 0000  ecryptr....X....
+00001c20: 7662 6170 6372 1d01 0000 5823 0000 0072  vbapcr....X#...r
+00001c30: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
+00001c40: 726d 6174 732e 6f66 6669 6365 2e76 6261  rmats.office.vba
+00001c50: 7063 721e 0100 0058 0600 0000 7662 6173  pcr....X....vbas
+00001c60: 7472 721f 0100 0058 2400 0000 7265 6669  trr....X$...refi
+00001c70: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
+00001c80: 7473 2e6f 6666 6963 652e 7662 6173 7472  ts.office.vbastr
+00001c90: 7220 0100 0058 0800 0000 786c 6d64 656f  r ...X....xlmdeo
+00001ca0: 6266 7221 0100 0058 2600 0000 7265 6669  bfr!...X&...refi
+00001cb0: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
+00001cc0: 7473 2e6f 6666 6963 652e 786c 6d64 656f  ts.office.xlmdeo
+00001cd0: 6266 7222 0100 0058 0500 0000 786c 7874  bfr"...X....xlxt
+00001ce0: 7272 2301 0000 5823 0000 0072 6566 696e  rr#...X#...refin
+00001cf0: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
+00001d00: 732e 6f66 6669 6365 2e78 6c78 7472 7224  s.office.xlxtrr$
+00001d10: 0100 0058 0500 0000 7874 646f 6372 2501  ...X....xtdocr%.
+00001d20: 0000 5823 0000 0072 6566 696e 6572 792e  ..X#...refinery.
+00001d30: 756e 6974 732e 666f 726d 6174 732e 6f66  units.formats.of
+00001d40: 6669 6365 2e78 7464 6f63 7226 0100 0058  fice.xtdocr&...X
+00001d50: 0500 0000 7874 6f6e 6572 2701 0000 5823  ....xtoner'...X#
+00001d60: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00001d70: 732e 666f 726d 6174 732e 6f66 6669 6365  s.formats.office
+00001d80: 2e78 746f 6e65 7228 0100 0058 0500 0000  .xtoner(...X....
+00001d90: 7874 7274 6672 2901 0000 5823 0000 0072  xtrtfr)...X#...r
+00001da0: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
+00001db0: 726d 6174 732e 6f66 6669 6365 2e78 7472  rmats.office.xtr
+00001dc0: 7466 722a 0100 0058 0500 0000 7874 7662  tfr*...X....xtvb
+00001dd0: 6172 2b01 0000 5823 0000 0072 6566 696e  ar+...X#...refin
+00001de0: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
+00001df0: 732e 6f66 6669 6365 2e78 7476 6261 722c  s.office.xtvbar,
+00001e00: 0100 0058 0400 0000 7063 6170 722d 0100  ...X....pcapr-..
+00001e10: 0058 1b00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+00001e20: 6e69 7473 2e66 6f72 6d61 7473 2e70 6361  nits.formats.pca
+00001e30: 7072 2e01 0000 5809 0000 0070 6361 705f  pr....X....pcap_
+00001e40: 6874 7470 722f 0100 0058 2000 0000 7265  httpr/...X ...re
+00001e50: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
+00001e60: 6d61 7473 2e70 6361 705f 6874 7470 7230  mats.pcap_httpr0
+00001e70: 0100 0058 0500 0000 7874 7064 6672 3101  ...X....xtpdfr1.
+00001e80: 0000 581a 0000 0072 6566 696e 6572 792e  ..X....refinery.
+00001e90: 756e 6974 732e 666f 726d 6174 732e 7064  units.formats.pd
+00001ea0: 6672 3201 0000 5806 0000 0064 6e62 6c6f  fr2...X....dnblo
+00001eb0: 6272 3301 0000 5827 0000 0072 6566 696e  br3...X'...refin
+00001ec0: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
+00001ed0: 732e 7065 2e64 6f74 6e65 742e 646e 626c  s.pe.dotnet.dnbl
+00001ee0: 6f62 7234 0100 0058 0500 0000 646e 6366  obr4...X....dncf
+00001ef0: 7872 3501 0000 5826 0000 0072 6566 696e  xr5...X&...refin
+00001f00: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
+00001f10: 732e 7065 2e64 6f74 6e65 742e 646e 6366  s.pe.dotnet.dncf
+00001f20: 7872 3601 0000 5804 0000 0064 6e64 7372  xr6...X....dndsr
+00001f30: 3701 0000 5825 0000 0072 6566 696e 6572  7...X%...refiner
+00001f40: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
+00001f50: 7065 2e64 6f74 6e65 742e 646e 6473 7238  pe.dotnet.dndsr8
+00001f60: 0100 0058 0800 0000 646e 6669 656c 6473  ...X....dnfields
+00001f70: 7239 0100 0058 2900 0000 7265 6669 6e65  r9...X)...refine
+00001f80: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
+00001f90: 2e70 652e 646f 746e 6574 2e64 6e66 6965  .pe.dotnet.dnfie
+00001fa0: 6c64 7372 3a01 0000 5805 0000 0064 6e68  ldsr:...X....dnh
+00001fb0: 6472 723b 0100 0058 2600 0000 7265 6669  drr;...X&...refi
+00001fc0: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
+00001fd0: 7473 2e70 652e 646f 746e 6574 2e64 6e68  ts.pe.dotnet.dnh
+00001fe0: 6472 723c 0100 0058 0400 0000 646e 6d72  drr<...X....dnmr
+00001ff0: 723d 0100 0058 2500 0000 7265 6669 6e65  r=...X%...refine
+00002000: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
+00002010: 2e70 652e 646f 746e 6574 2e64 6e6d 7272  .pe.dotnet.dnmrr
+00002020: 3e01 0000 5804 0000 0064 6e72 6372 3f01  >...X....dnrcr?.
+00002030: 0000 5825 0000 0072 6566 696e 6572 792e  ..X%...refinery.
+00002040: 756e 6974 732e 666f 726d 6174 732e 7065  units.formats.pe
+00002050: 2e64 6f74 6e65 742e 646e 7263 7240 0100  .dotnet.dnrcr@..
+00002060: 0058 0500 0000 646e 7374 7272 4101 0000  .X....dnstrrA...
+00002070: 5826 0000 0072 6566 696e 6572 792e 756e  X&...refinery.un
+00002080: 6974 732e 666f 726d 6174 732e 7065 2e64  its.formats.pe.d
+00002090: 6f74 6e65 742e 646e 7374 7272 4201 0000  otnet.dnstrrB...
+000020a0: 5806 0000 0070 656d 6574 6172 4301 0000  X....pemetarC...
+000020b0: 5820 0000 0072 6566 696e 6572 792e 756e  X ...refinery.un
+000020c0: 6974 732e 666f 726d 6174 732e 7065 2e70  its.formats.pe.p
+000020d0: 656d 6574 6172 4401 0000 5809 0000 0070  emetarD...X....p
+000020e0: 656f 7665 726c 6179 7245 0100 0058 2300  eoverlayrE...X#.
+000020f0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00002100: 2e66 6f72 6d61 7473 2e70 652e 7065 6f76  .formats.pe.peov
+00002110: 6572 6c61 7972 4601 0000 5804 0000 0070  erlayrF...X....p
+00002120: 6572 6372 4701 0000 581e 0000 0072 6566  ercrG...X....ref
+00002130: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
+00002140: 6174 732e 7065 2e70 6572 6372 4801 0000  ats.pe.percrH...
+00002150: 5805 0000 0070 6573 6967 7249 0100 0058  X....pesigrI...X
+00002160: 1f00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+00002170: 7473 2e66 6f72 6d61 7473 2e70 652e 7065  ts.formats.pe.pe
+00002180: 7369 6772 4a01 0000 5807 0000 0070 6573  sigrJ...X....pes
+00002190: 7472 6970 724b 0100 0058 2100 0000 7265  triprK...X!...re
+000021a0: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
+000021b0: 6d61 7473 2e70 652e 7065 7374 7269 7072  mats.pe.pestripr
+000021c0: 4c01 0000 5805 0000 0070 6b63 7337 724d  L...X....pkcs7rM
+000021d0: 0100 0058 1c00 0000 7265 6669 6e65 7279  ...X....refinery
+000021e0: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e70  .units.formats.p
+000021f0: 6b63 7337 724e 0100 0058 0800 0000 706b  kcs7rN...X....pk
+00002200: 6373 3773 6967 724f 0100 0058 1f00 0000  cs7sigrO...X....
+00002210: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
+00002220: 6f72 6d61 7473 2e70 6b63 7337 7369 6772  ormats.pkcs7sigr
+00002230: 5001 0000 5805 0000 0073 7465 676f 7251  P...X....stegorQ
+00002240: 0100 0058 1c00 0000 7265 6669 6e65 7279  ...X....refinery
+00002250: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e73  .units.formats.s
+00002260: 7465 676f 7252 0100 0058 0700 0000 746e  tegorR...X....tn
+00002270: 6574 6d74 6d72 5301 0000 581e 0000 0072  etmtmrS...X....r
+00002280: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
+00002290: 726d 6174 732e 746e 6574 6d74 6d72 5401  rmats.tnetmtmrT.
+000022a0: 0000 5806 0000 0077 696e 7265 6772 5501  ..X....winregrU.
+000022b0: 0000 581d 0000 0072 6566 696e 6572 792e  ..X....refinery.
+000022c0: 756e 6974 732e 666f 726d 6174 732e 7769  units.formats.wi
+000022d0: 6e72 6567 7256 0100 0058 0500 0000 7874  nregrV...X....xt
+000022e0: 786d 6c72 5701 0000 581a 0000 0072 6566  xmlrW...X....ref
+000022f0: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
+00002300: 6174 732e 786d 6c72 5801 0000 5803 0000  ats.xmlrX...X...
+00002310: 006e 3430 7259 0100 0058 1a00 0000 7265  .n40rY...X....re
+00002320: 6669 6e65 7279 2e75 6e69 7473 2e6d 616c  finery.units.mal
+00002330: 7761 7265 2e6e 3430 725a 0100 0058 0400  ware.n40rZ...X..
+00002340: 0000 6368 6f70 725b 0100 0058 1800 0000  ..chopr[...X....
+00002350: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
+00002360: 6574 612e 6368 6f70 725c 0100 0058 0200  eta.chopr\...X..
+00002370: 0000 636d 725d 0100 0058 1600 0000 7265  ..cmr]...X....re
+00002380: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
+00002390: 612e 636d 725e 0100 0058 0400 0000 6375  a.cmr^...X....cu
+000023a0: 6c6c 725f 0100 0058 1800 0000 7265 6669  llr_...X....refi
+000023b0: 6e65 7279 2e75 6e69 7473 2e6d 6574 612e  nery.units.meta.
+000023c0: 6375 6c6c 7260 0100 0058 0500 0000 6465  cullr`...X....de
+000023d0: 6475 7072 6101 0000 5819 0000 0072 6566  dupra...X....ref
+000023e0: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
+000023f0: 2e64 6564 7570 7262 0100 0058 0300 0000  .deduprb...X....
+00002400: 6561 7472 6301 0000 5817 0000 0072 6566  eatrc...X....ref
+00002410: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
+00002420: 2e65 6174 7264 0100 0058 0200 0000 6566  .eatrd...X....ef
+00002430: 7265 0100 0058 1600 0000 7265 6669 6e65  re...X....refine
+00002440: 7279 2e75 6e69 7473 2e6d 6574 612e 6566  ry.units.meta.ef
+00002450: 7266 0100 0058 0400 0000 656d 6974 7267  rf...X....emitrg
+00002460: 0100 0058 1800 0000 7265 6669 6e65 7279  ...X....refinery
+00002470: 2e75 6e69 7473 2e6d 6574 612e 656d 6974  .units.meta.emit
+00002480: 7268 0100 0058 0500 0000 6772 6f75 7072  rh...X....groupr
+00002490: 6901 0000 5819 0000 0072 6566 696e 6572  i...X....refiner
+000024a0: 792e 756e 6974 732e 6d65 7461 2e67 726f  y.units.meta.gro
+000024b0: 7570 726a 0100 0058 0700 0000 6772 6f75  uprj...X....grou
+000024c0: 7062 7972 6b01 0000 581b 0000 0072 6566  pbyrk...X....ref
+000024d0: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
+000024e0: 2e67 726f 7570 6279 726c 0100 0058 0300  .groupbyrl...X..
+000024f0: 0000 6966 6672 6d01 0000 5817 0000 0072  ..iffrm...X....r
+00002500: 6566 696e 6572 792e 756e 6974 732e 6d65  efinery.units.me
+00002510: 7461 2e69 6666 726e 0100 0058 0400 0000  ta.iffrn...X....
+00002520: 6966 6670 726f 0100 0058 1800 0000 7265  iffpro...X....re
+00002530: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
+00002540: 612e 6966 6670 7270 0100 0058 0400 0000  a.iffprp...X....
+00002550: 6966 6673 7271 0100 0058 1800 0000 7265  iffsrq...X....re
+00002560: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
+00002570: 612e 6966 6673 7272 0100 0058 0400 0000  a.iffsrr...X....
+00002580: 6966 6678 7273 0100 0058 1800 0000 7265  iffxrs...X....re
+00002590: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
+000025a0: 612e 6966 6678 7274 0100 0058 0400 0000  a.iffxrt...X....
+000025b0: 6d61 785f 7275 0100 0058 1700 0000 7265  max_ru...X....re
+000025c0: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
+000025d0: 612e 6d61 7872 7601 0000 5804 0000 006d  a.maxrv...X....m
+000025e0: 696e 5f72 7701 0000 5817 0000 0072 6566  in_rw...X....ref
+000025f0: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
+00002600: 2e6d 696e 7278 0100 0058 0300 0000 6d76  .minrx...X....mv
+00002610: 6372 7901 0000 5817 0000 0072 6566 696e  cry...X....refin
+00002620: 6572 792e 756e 6974 732e 6d65 7461 2e6d  ery.units.meta.m
+00002630: 7663 727a 0100 0058 0300 0000 6d76 6772  vcrz...X....mvgr
+00002640: 7b01 0000 5817 0000 0072 6566 696e 6572  {...X....refiner
+00002650: 792e 756e 6974 732e 6d65 7461 2e6d 7667  y.units.meta.mvg
+00002660: 727c 0100 0058 0300 0000 7061 6472 7d01  r|...X....padr}.
+00002670: 0000 5817 0000 0072 6566 696e 6572 792e  ..X....refinery.
+00002680: 756e 6974 732e 6d65 7461 2e70 6164 727e  units.meta.padr~
+00002690: 0100 0058 0400 0000 7069 636b 727f 0100  ...X....pickr...
+000026a0: 0058 1800 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+000026b0: 6e69 7473 2e6d 6574 612e 7069 636b 7280  nits.meta.pickr.
+000026c0: 0100 0058 0300 0000 706f 7072 8101 0000  ...X....popr....
+000026d0: 5817 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+000026e0: 6974 732e 6d65 7461 2e70 6f70 7282 0100  its.meta.popr...
+000026f0: 0058 0400 0000 7075 7368 7283 0100 0058  .X....pushr....X
+00002700: 1800 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+00002710: 7473 2e6d 6574 612e 7075 7368 7284 0100  ts.meta.pushr...
+00002720: 0058 0300 0000 7075 7472 8501 0000 5817  .X....putr....X.
+00002730: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002740: 732e 6d65 7461 2e70 7574 7286 0100 0058  s.meta.putr....X
+00002750: 0500 0000 7175 6575 6572 8701 0000 5819  ....queuer....X.
+00002760: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002770: 732e 6d65 7461 2e71 7565 7565 7288 0100  s.meta.queuer...
+00002780: 0058 0600 0000 7265 6475 6365 7289 0100  .X....reducer...
+00002790: 0058 1a00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+000027a0: 6e69 7473 2e6d 6574 612e 7265 6475 6365  nits.meta.reduce
+000027b0: 728a 0100 0058 0500 0000 7363 6f70 6572  r....X....scoper
+000027c0: 8b01 0000 5819 0000 0072 6566 696e 6572  ....X....refiner
+000027d0: 792e 756e 6974 732e 6d65 7461 2e73 636f  y.units.meta.sco
+000027e0: 7065 728c 0100 0058 0300 0000 7365 7072  per....X....sepr
+000027f0: 8d01 0000 5817 0000 0072 6566 696e 6572  ....X....refiner
+00002800: 792e 756e 6974 732e 6d65 7461 2e73 6570  y.units.meta.sep
+00002810: 728e 0100 0058 0600 0000 736f 7274 6564  r....X....sorted
+00002820: 728f 0100 0058 1a00 0000 7265 6669 6e65  r....X....refine
+00002830: 7279 2e75 6e69 7473 2e6d 6574 612e 736f  ry.units.meta.so
+00002840: 7274 6564 7290 0100 0058 0400 0000 7377  rtedr....X....sw
+00002850: 6170 7291 0100 0058 1800 0000 7265 6669  apr....X....refi
+00002860: 6e65 7279 2e75 6e69 7473 2e6d 6574 612e  nery.units.meta.
+00002870: 7377 6170 7292 0100 0058 0900 0000 7472  swapr....X....tr
+00002880: 616e 7370 6f73 6572 9301 0000 581d 0000  ansposer....X...
+00002890: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+000028a0: 6d65 7461 2e74 7261 6e73 706f 7365 7294  meta.transposer.
+000028b0: 0100 0058 0400 0000 7866 6363 7295 0100  ...X....xfccr...
+000028c0: 0058 1800 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+000028d0: 6e69 7473 2e6d 6574 612e 7866 6363 7296  nits.meta.xfccr.
+000028e0: 0100 0058 0700 0000 6175 746f 786f 7272  ...X....autoxorr
+000028f0: 9701 0000 581b 0000 0072 6566 696e 6572  ....X....refiner
+00002900: 792e 756e 6974 732e 6d69 7363 2e61 7574  y.units.misc.aut
+00002910: 6f78 6f72 7298 0100 0058 0600 0000 636f  oxorr....X....co
+00002920: 7570 6c65 7299 0100 0058 1a00 0000 7265  upler....X....re
+00002930: 6669 6e65 7279 2e75 6e69 7473 2e6d 6973  finery.units.mis
+00002940: 632e 636f 7570 6c65 729a 0100 0058 0700  c.coupler....X..
+00002950: 0000 6461 7465 6669 7872 9b01 0000 581b  ..datefixr....X.
+00002960: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002970: 732e 6d69 7363 2e64 6174 6566 6978 729c  s.misc.datefixr.
+00002980: 0100 0058 0300 0000 6472 7072 9d01 0000  ...X....drpr....
+00002990: 5817 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+000029a0: 6974 732e 6d69 7363 2e64 7270 729e 0100  its.misc.drpr...
+000029b0: 0058 0300 0000 6e6f 7072 9f01 0000 5817  .X....nopr....X.
+000029c0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+000029d0: 732e 6d69 7363 2e6e 6f70 72a0 0100 0058  s.misc.nopr....X
+000029e0: 0600 0000 7572 6c66 6978 72a1 0100 0058  ....urlfixr....X
+000029f0: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+00002a00: 7473 2e6d 6973 632e 7572 6c66 6978 72a2  ts.misc.urlfixr.
+00002a10: 0100 0058 0400 0000 786b 6579 72a3 0100  ...X....xkeyr...
+00002a20: 0058 1800 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+00002a30: 6e69 7473 2e6d 6973 632e 786b 6579 72a4  nits.misc.xkeyr.
+00002a40: 0100 0058 0e00 0000 6465 6f62 5f6a 735f  ...X....deob_js_
+00002a50: 6172 7261 7973 72a5 0100 0058 2400 0000  arraysr....X$...
+00002a60: 7265 6669 6e65 7279 2e75 6e69 7473 2e6f  refinery.units.o
+00002a70: 6266 7573 6361 7469 6f6e 2e6a 732e 6172  bfuscation.js.ar
+00002a80: 7261 7973 72a6 0100 0058 0f00 0000 6465  raysr....X....de
+00002a90: 6f62 5f6a 735f 6765 7461 7474 7272 a701  ob_js_getattrr..
+00002aa0: 0000 5825 0000 0072 6566 696e 6572 792e  ..X%...refinery.
+00002ab0: 756e 6974 732e 6f62 6675 7363 6174 696f  units.obfuscatio
+00002ac0: 6e2e 6a73 2e67 6574 6174 7472 72a8 0100  n.js.getattrr...
+00002ad0: 0058 0e00 0000 6465 6f62 5f6a 735f 7475  .X....deob_js_tu
+00002ae0: 706c 6573 72a9 0100 0058 2400 0000 7265  plesr....X$...re
+00002af0: 6669 6e65 7279 2e75 6e69 7473 2e6f 6266  finery.units.obf
+00002b00: 7573 6361 7469 6f6e 2e6a 732e 7475 706c  uscation.js.tupl
+00002b10: 6573 72aa 0100 0058 0800 0000 6465 6f62  esr....X....deob
+00002b20: 5f70 7331 72ab 0100 0058 2200 0000 7265  _ps1r....X"...re
+00002b30: 6669 6e65 7279 2e75 6e69 7473 2e6f 6266  finery.units.obf
+00002b40: 7573 6361 7469 6f6e 2e70 7331 2e61 6c6c  uscation.ps1.all
+00002b50: 72ac 0100 0058 1100 0000 6465 6f62 5f70  r....X....deob_p
+00002b60: 7331 5f62 7261 636b 6574 7372 ad01 0000  s1_bracketsr....
+00002b70: 5827 0000 0072 6566 696e 6572 792e 756e  X'...refinery.un
+00002b80: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
+00002b90: 7073 312e 6272 6163 6b65 7473 72ae 0100  ps1.bracketsr...
+00002ba0: 0058 0e00 0000 6465 6f62 5f70 7331 5f63  .X....deob_ps1_c
+00002bb0: 6173 6573 72af 0100 0058 2400 0000 7265  asesr....X$...re
+00002bc0: 6669 6e65 7279 2e75 6e69 7473 2e6f 6266  finery.units.obf
+00002bd0: 7573 6361 7469 6f6e 2e70 7331 2e63 6173  uscation.ps1.cas
+00002be0: 6573 72b0 0100 0058 0f00 0000 6465 6f62  esr....X....deob
+00002bf0: 5f70 7331 5f63 6f6e 6361 7472 b101 0000  _ps1_concatr....
+00002c00: 5825 0000 0072 6566 696e 6572 792e 756e  X%...refinery.un
+00002c10: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
+00002c20: 7073 312e 636f 6e63 6174 72b2 0100 0058  ps1.concatr....X
+00002c30: 0f00 0000 6465 6f62 5f70 7331 5f65 7363  ....deob_ps1_esc
+00002c40: 6170 6572 b301 0000 5825 0000 0072 6566  aper....X%...ref
+00002c50: 696e 6572 792e 756e 6974 732e 6f62 6675  inery.units.obfu
+00002c60: 7363 6174 696f 6e2e 7073 312e 6573 6361  scation.ps1.esca
+00002c70: 7065 72b4 0100 0058 0f00 0000 6465 6f62  per....X....deob
+00002c80: 5f70 7331 5f66 6f72 6d61 7472 b501 0000  _ps1_formatr....
+00002c90: 5825 0000 0072 6566 696e 6572 792e 756e  X%...refinery.un
+00002ca0: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
+00002cb0: 7073 312e 666f 726d 6174 72b6 0100 0058  ps1.formatr....X
+00002cc0: 0f00 0000 6465 6f62 5f70 7331 5f69 6e76  ....deob_ps1_inv
+00002cd0: 6f6b 6572 b701 0000 5825 0000 0072 6566  oker....X%...ref
+00002ce0: 696e 6572 792e 756e 6974 732e 6f62 6675  inery.units.obfu
+00002cf0: 7363 6174 696f 6e2e 7073 312e 696e 766f  scation.ps1.invo
+00002d00: 6b65 72b8 0100 0058 0f00 0000 6465 6f62  ker....X....deob
+00002d10: 5f70 7331 5f73 6563 7374 7272 b901 0000  _ps1_secstrr....
+00002d20: 582b 0000 0072 6566 696e 6572 792e 756e  X+...refinery.un
+00002d30: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
+00002d40: 7073 312e 7365 6375 7265 7374 7269 6e67  ps1.securestring
+00002d50: 72ba 0100 0058 1600 0000 6465 6f62 5f70  r....X....deob_p
+00002d60: 7331 5f73 7472 696e 6772 6570 6c61 6365  s1_stringreplace
+00002d70: 72bb 0100 0058 2c00 0000 7265 6669 6e65  r....X,...refine
+00002d80: 7279 2e75 6e69 7473 2e6f 6266 7573 6361  ry.units.obfusca
+00002d90: 7469 6f6e 2e70 7331 2e73 7472 696e 6772  tion.ps1.stringr
+00002da0: 6570 6c61 6365 72bc 0100 0058 1100 0000  eplacer....X....
+00002db0: 6465 6f62 5f70 7331 5f74 7970 6563 6173  deob_ps1_typecas
+00002dc0: 7472 bd01 0000 5827 0000 0072 6566 696e  tr....X'...refin
+00002dd0: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
+00002de0: 6174 696f 6e2e 7073 312e 7479 7065 6361  ation.ps1.typeca
+00002df0: 7374 72be 0100 0058 1000 0000 6465 6f62  str....X....deob
+00002e00: 5f70 7331 5f75 6e63 7572 6c79 72bf 0100  _ps1_uncurlyr...
+00002e10: 0058 2600 0000 7265 6669 6e65 7279 2e75  .X&...refinery.u
+00002e20: 6e69 7473 2e6f 6266 7573 6361 7469 6f6e  nits.obfuscation
+00002e30: 2e70 7331 2e75 6e63 7572 6c79 72c0 0100  .ps1.uncurlyr...
+00002e40: 0058 0800 0000 6465 6f62 5f76 6261 72c1  .X....deob_vbar.
+00002e50: 0100 0058 2200 0000 7265 6669 6e65 7279  ...X"...refinery
+00002e60: 2e75 6e69 7473 2e6f 6266 7573 6361 7469  .units.obfuscati
+00002e70: 6f6e 2e76 6261 2e61 6c6c 72c2 0100 0058  on.vba.allr....X
+00002e80: 1300 0000 6465 6f62 5f76 6261 5f61 7269  ....deob_vba_ari
+00002e90: 7468 6d65 7469 6372 c301 0000 5829 0000  thmeticr....X)..
+00002ea0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00002eb0: 6f62 6675 7363 6174 696f 6e2e 7662 612e  obfuscation.vba.
+00002ec0: 6172 6974 686d 6574 6963 72c4 0100 0058  arithmeticr....X
+00002ed0: 1100 0000 6465 6f62 5f76 6261 5f62 7261  ....deob_vba_bra
+00002ee0: 636b 6574 7372 c501 0000 5827 0000 0072  cketsr....X'...r
+00002ef0: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
+00002f00: 6675 7363 6174 696f 6e2e 7662 612e 6272  fuscation.vba.br
+00002f10: 6163 6b65 7473 72c6 0100 0058 1600 0000  acketsr....X....
+00002f20: 6465 6f62 5f76 6261 5f63 6861 725f 6675  deob_vba_char_fu
+00002f30: 6e63 7469 6f6e 72c7 0100 0058 2300 0000  nctionr....X#...
+00002f40: 7265 6669 6e65 7279 2e75 6e69 7473 2e6f  refinery.units.o
+00002f50: 6266 7573 6361 7469 6f6e 2e76 6261 2e63  bfuscation.vba.c
+00002f60: 6861 7272 c801 0000 5811 0000 0064 656f  harr....X....deo
+00002f70: 625f 7662 615f 636f 6d6d 656e 7473 72c9  b_vba_commentsr.
+00002f80: 0100 0058 2700 0000 7265 6669 6e65 7279  ...X'...refinery
+00002f90: 2e75 6e69 7473 2e6f 6266 7573 6361 7469  .units.obfuscati
+00002fa0: 6f6e 2e76 6261 2e63 6f6d 6d65 6e74 7372  on.vba.commentsr
+00002fb0: ca01 0000 580f 0000 0064 656f 625f 7662  ....X....deob_vb
+00002fc0: 615f 636f 6e63 6174 72cb 0100 0058 2500  a_concatr....X%.
+00002fd0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00002fe0: 2e6f 6266 7573 6361 7469 6f6e 2e76 6261  .obfuscation.vba
+00002ff0: 2e63 6f6e 6361 7472 cc01 0000 5812 0000  .concatr....X...
+00003000: 0064 656f 625f 7662 615f 636f 6e73 7461  .deob_vba_consta
+00003010: 6e74 7372 cd01 0000 5828 0000 0072 6566  ntsr....X(...ref
+00003020: 696e 6572 792e 756e 6974 732e 6f62 6675  inery.units.obfu
+00003030: 7363 6174 696f 6e2e 7662 612e 636f 6e73  scation.vba.cons
+00003040: 7461 6e74 7372 ce01 0000 5818 0000 0064  tantsr....X....d
+00003050: 656f 625f 7662 615f 6475 6d6d 795f 7661  eob_vba_dummy_va
+00003060: 7269 6162 6c65 7372 cf01 0000 5826 0000  riablesr....X&..
+00003070: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00003080: 6f62 6675 7363 6174 696f 6e2e 7662 612e  obfuscation.vba.
+00003090: 6475 6d6d 6965 7372 d001 0000 5816 0000  dummiesr....X...
+000030a0: 0064 656f 625f 7662 615f 7374 7269 6e67  .deob_vba_string
+000030b0: 7265 706c 6163 6572 d101 0000 582c 0000  replacer....X,..
+000030c0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+000030d0: 6f62 6675 7363 6174 696f 6e2e 7662 612e  obfuscation.vba.
+000030e0: 7374 7269 6e67 7265 706c 6163 6572 d201  stringreplacer..
+000030f0: 0000 5816 0000 0064 656f 625f 7662 615f  ..X....deob_vba_
+00003100: 7374 7269 6e67 7265 7665 7273 6572 d301  stringreverser..
+00003110: 0000 582c 0000 0072 6566 696e 6572 792e  ..X,...refinery.
+00003120: 756e 6974 732e 6f62 6675 7363 6174 696f  units.obfuscatio
+00003130: 6e2e 7662 612e 7374 7269 6e67 7265 7665  n.vba.stringreve
+00003140: 7273 6572 d401 0000 5815 0000 0064 656f  rser....X....deo
+00003150: 625f 7662 615f 6368 725f 6c69 7465 7261  b_vba_chr_litera
+00003160: 6c73 72d5 0100 0058 2200 0000 7265 6669  lsr....X"...refi
+00003170: 6e65 7279 2e75 6e69 7473 2e6f 6266 7573  nery.units.obfus
+00003180: 6361 7469 6f6e 2e76 6261 2e76 6261 72d6  cation.vba.vbar.
+00003190: 0100 0058 0500 0000 6361 7276 6572 d701  ...X....carver..
+000031a0: 0000 581c 0000 0072 6566 696e 6572 792e  ..X....refinery.
+000031b0: 756e 6974 732e 7061 7474 6572 6e2e 6361  units.pattern.ca
+000031c0: 7276 6572 d801 0000 5808 0000 0063 6172  rver....X....car
+000031d0: 7665 5f37 7a72 d901 0000 581f 0000 0072  ve_7zr....X....r
+000031e0: 6566 696e 6572 792e 756e 6974 732e 7061  efinery.units.pa
+000031f0: 7474 6572 6e2e 6361 7276 655f 377a 72da  ttern.carve_7zr.
+00003200: 0100 0058 0a00 0000 6361 7276 655f 6a73  ...X....carve_js
+00003210: 6f6e 72db 0100 0058 2100 0000 7265 6669  onr....X!...refi
+00003220: 6e65 7279 2e75 6e69 7473 2e70 6174 7465  nery.units.patte
+00003230: 726e 2e63 6172 7665 5f6a 736f 6e72 dc01  rn.carve_jsonr..
+00003240: 0000 5809 0000 0063 6172 7665 5f6c 6e6b  ..X....carve_lnk
+00003250: 72dd 0100 0058 2000 0000 7265 6669 6e65  r....X ...refine
+00003260: 7279 2e75 6e69 7473 2e70 6174 7465 726e  ry.units.pattern
+00003270: 2e63 6172 7665 5f6c 6e6b 72de 0100 0058  .carve_lnkr....X
+00003280: 0800 0000 6361 7276 655f 7065 72df 0100  ....carve_per...
+00003290: 0058 1f00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+000032a0: 6e69 7473 2e70 6174 7465 726e 2e63 6172  nits.pattern.car
+000032b0: 7665 5f70 6572 e001 0000 5809 0000 0063  ve_per....X....c
+000032c0: 6172 7665 5f72 7466 72e1 0100 0058 2000  arve_rtfr....X .
+000032d0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+000032e0: 2e70 6174 7465 726e 2e63 6172 7665 5f72  .pattern.carve_r
+000032f0: 7466 72e2 0100 0058 0900 0000 6361 7276  tfr....X....carv
+00003300: 655f 786d 6c72 e301 0000 5820 0000 0072  e_xmlr....X ...r
+00003310: 6566 696e 6572 792e 756e 6974 732e 7061  efinery.units.pa
+00003320: 7474 6572 6e2e 6361 7276 655f 786d 6c72  ttern.carve_xmlr
+00003330: e401 0000 5809 0000 0063 6172 7665 5f7a  ....X....carve_z
+00003340: 6970 72e5 0100 0058 2000 0000 7265 6669  ipr....X ...refi
+00003350: 6e65 7279 2e75 6e69 7473 2e70 6174 7465  nery.units.patte
+00003360: 726e 2e63 6172 7665 5f7a 6970 72e6 0100  rn.carve_zipr...
+00003370: 0058 0600 0000 6465 6661 6e67 72e7 0100  .X....defangr...
+00003380: 0058 1d00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+00003390: 6e69 7473 2e70 6174 7465 726e 2e64 6566  nits.pattern.def
+000033a0: 616e 6772 e801 0000 5809 0000 0064 6e73  angr....X....dns
+000033b0: 646f 6d61 696e 72e9 0100 0058 2000 0000  domainr....X ...
+000033c0: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
+000033d0: 6174 7465 726e 2e64 6e73 646f 6d61 696e  attern.dnsdomain
+000033e0: 72ea 0100 0058 0900 0000 6d69 6d65 776f  r....X....mimewo
+000033f0: 7264 7372 eb01 0000 5820 0000 0072 6566  rdsr....X ...ref
+00003400: 696e 6572 792e 756e 6974 732e 7061 7474  inery.units.patt
+00003410: 6572 6e2e 6d69 6d65 776f 7264 7372 ec01  ern.mimewordsr..
+00003420: 0000 5807 0000 0072 6573 706c 6974 72ed  ..X....resplitr.
+00003430: 0100 0058 1e00 0000 7265 6669 6e65 7279  ...X....refinery
+00003440: 2e75 6e69 7473 2e70 6174 7465 726e 2e72  .units.pattern.r
+00003450: 6573 706c 6974 72ee 0100 0058 0500 0000  esplitr....X....
+00003460: 7265 7375 6272 ef01 0000 581c 0000 0072  resubr....X....r
+00003470: 6566 696e 6572 792e 756e 6974 732e 7061  efinery.units.pa
+00003480: 7474 6572 6e2e 7265 7375 6272 f001 0000  ttern.resubr....
+00003490: 5803 0000 0072 6578 72f1 0100 0058 1a00  X....rexr....X..
+000034a0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+000034b0: 2e70 6174 7465 726e 2e72 6578 72f2 0100  .pattern.rexr...
+000034c0: 0058 0600 0000 7374 7275 6374 72f3 0100  .X....structr...
+000034d0: 0058 2400 0000 7265 6669 6e65 7279 2e75  .X$...refinery.u
+000034e0: 6e69 7473 2e70 6174 7465 726e 2e73 7472  nits.pattern.str
+000034f0: 7563 745f 7061 7273 6572 72f4 0100 0058  uct_parserr....X
+00003500: 0800 0000 7375 6266 696c 6573 72f5 0100  ....subfilesr...
+00003510: 0058 1f00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+00003520: 6e69 7473 2e70 6174 7465 726e 2e73 7562  nits.pattern.sub
+00003530: 6669 6c65 7372 f601 0000 5809 0000 0075  filesr....X....u
+00003540: 726c 6775 6172 6473 72f7 0100 0058 2000  rlguardsr....X .
+00003550: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00003560: 2e70 6174 7465 726e 2e75 726c 6775 6172  .pattern.urlguar
+00003570: 6473 72f8 0100 0058 0300 0000 7874 7072  dsr....X....xtpr
+00003580: f901 0000 581a 0000 0072 6566 696e 6572  ....X....refiner
+00003590: 792e 756e 6974 732e 7061 7474 6572 6e2e  y.units.pattern.
+000035a0: 7874 7072 fa01 0000 5803 0000 0078 7477  xtpr....X....xtw
+000035b0: 72fb 0100 0058 1a00 0000 7265 6669 6e65  r....X....refine
+000035c0: 7279 2e75 6e69 7473 2e70 6174 7465 726e  ry.units.pattern
+000035d0: 2e78 7477 72fc 0100 0058 0300 0000 6173  .xtwr....X....as
+000035e0: 6d72 fd01 0000 5818 0000 0072 6566 696e  mr....X....refin
+000035f0: 6572 792e 756e 6974 732e 7369 6e6b 732e  ery.units.sinks.
+00003600: 6173 6d72 fe01 0000 5804 0000 0064 756d  asmr....X....dum
+00003610: 7072 ff01 0000 5819 0000 0072 6566 696e  pr....X....refin
+00003620: 6572 792e 756e 6974 732e 7369 6e6b 732e  ery.units.sinks.
+00003630: 6475 6d70 7200 0200 0058 0500 0000 6965  dumpr....X....ie
+00003640: 6d61 7072 0102 0000 581a 0000 0072 6566  mapr....X....ref
+00003650: 696e 6572 792e 756e 6974 732e 7369 6e6b  inery.units.sink
+00003660: 732e 6965 6d61 7072 0202 0000 5804 0000  s.iemapr....X...
+00003670: 0070 6565 6b72 0302 0000 5819 0000 0072  .peekr....X....r
+00003680: 6566 696e 6572 792e 756e 6974 732e 7369  efinery.units.si
+00003690: 6e6b 732e 7065 656b 7204 0200 0058 0900  nks.peekr....X..
+000036a0: 0000 7070 6a73 6372 6970 7472 0502 0000  ..ppjscriptr....
+000036b0: 581e 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+000036c0: 6974 732e 7369 6e6b 732e 7070 6a73 6372  its.sinks.ppjscr
+000036d0: 6970 7472 0602 0000 5806 0000 0070 706a  iptr....X....ppj
+000036e0: 736f 6e72 0702 0000 581b 0000 0072 6566  sonr....X....ref
+000036f0: 696e 6572 792e 756e 6974 732e 7369 6e6b  inery.units.sink
+00003700: 732e 7070 6a73 6f6e 7208 0200 0058 0500  s.ppjsonr....X..
+00003710: 0000 7070 786d 6c72 0902 0000 581a 0000  ..ppxmlr....X...
+00003720: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00003730: 7369 6e6b 732e 7070 786d 6c72 0a02 0000  sinks.ppxmlr....
+00003740: 5803 0000 0063 6361 720b 0200 0058 1a00  X....ccar....X..
+00003750: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00003760: 2e73 7472 696e 6773 2e63 6361 720c 0200  .strings.ccar...
+00003770: 0058 0300 0000 6363 7072 0d02 0000 581a  .X....ccpr....X.
+00003780: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00003790: 732e 7374 7269 6e67 732e 6363 7072 0e02  s.strings.ccpr..
+000037a0: 0000 5804 0000 0063 666d 7472 0f02 0000  ..X....cfmtr....
+000037b0: 581b 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+000037c0: 6974 732e 7374 7269 6e67 732e 6366 6d74  its.strings.cfmt
+000037d0: 7210 0200 0058 0600 0000 636c 6f77 6572  r....X....clower
 000037e0: 7211 0200 0058 1d00 0000 7265 6669 6e65  r....X....refine
 000037f0: 7279 2e75 6e69 7473 2e73 7472 696e 6773  ry.units.strings
-00003800: 2e63 7570 7065 7272 1202 0000 5803 0000  .cupperr....X...
-00003810: 0072 6570 7213 0200 0058 1a00 0000 7265  .repr....X....re
-00003820: 6669 6e65 7279 2e75 6e69 7473 2e73 7472  finery.units.str
-00003830: 696e 6773 2e72 6570 7214 0200 0058 0400  ings.repr....X..
-00003840: 0000 7265 706c 7215 0200 0058 1b00 0000  ..replr....X....
-00003850: 7265 6669 6e65 7279 2e75 6e69 7473 2e73  refinery.units.s
-00003860: 7472 696e 6773 2e72 6570 6c72 1602 0000  trings.replr....
-00003870: 5804 0000 0073 6e69 7072 1702 0000 581b  X....snipr....X.
-00003880: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00003890: 732e 7374 7269 6e67 732e 736e 6970 7218  s.strings.snipr.
-000038a0: 0200 0058 0700 0000 7374 7265 7463 6872  ...X....stretchr
-000038b0: 1902 0000 581e 0000 0072 6566 696e 6572  ....X....refiner
-000038c0: 792e 756e 6974 732e 7374 7269 6e67 732e  y.units.strings.
-000038d0: 7374 7265 7463 6872 1a02 0000 5807 0000  stretchr....X...
-000038e0: 0074 6572 6d66 6974 721b 0200 0058 1e00  .termfitr....X..
-000038f0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00003900: 2e73 7472 696e 6773 2e74 6572 6d66 6974  .strings.termfit
-00003910: 721c 0200 0058 0400 0000 7472 696d 721d  r....X....trimr.
-00003920: 0200 0058 1b00 0000 7265 6669 6e65 7279  ...X....refinery
-00003930: 2e75 6e69 7473 2e73 7472 696e 6773 2e74  .units.strings.t
-00003940: 7269 6d72 1e02 0000 752e                 rimr....u.
+00003800: 2e63 6c6f 7765 7272 1202 0000 5805 0000  .clowerr....X...
+00003810: 0063 7377 6170 7213 0200 0058 1c00 0000  .cswapr....X....
+00003820: 7265 6669 6e65 7279 2e75 6e69 7473 2e73  refinery.units.s
+00003830: 7472 696e 6773 2e63 7377 6170 7214 0200  trings.cswapr...
+00003840: 0058 0600 0000 6375 7070 6572 7215 0200  .X....cupperr...
+00003850: 0058 1d00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+00003860: 6e69 7473 2e73 7472 696e 6773 2e63 7570  nits.strings.cup
+00003870: 7065 7272 1602 0000 5803 0000 0072 6570  perr....X....rep
+00003880: 7217 0200 0058 1a00 0000 7265 6669 6e65  r....X....refine
+00003890: 7279 2e75 6e69 7473 2e73 7472 696e 6773  ry.units.strings
+000038a0: 2e72 6570 7218 0200 0058 0400 0000 7265  .repr....X....re
+000038b0: 706c 7219 0200 0058 1b00 0000 7265 6669  plr....X....refi
+000038c0: 6e65 7279 2e75 6e69 7473 2e73 7472 696e  nery.units.strin
+000038d0: 6773 2e72 6570 6c72 1a02 0000 5804 0000  gs.replr....X...
+000038e0: 0073 6e69 7072 1b02 0000 581b 0000 0072  .snipr....X....r
+000038f0: 6566 696e 6572 792e 756e 6974 732e 7374  efinery.units.st
+00003900: 7269 6e67 732e 736e 6970 721c 0200 0058  rings.snipr....X
+00003910: 0700 0000 7374 7265 7463 6872 1d02 0000  ....stretchr....
+00003920: 581e 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+00003930: 6974 732e 7374 7269 6e67 732e 7374 7265  its.strings.stre
+00003940: 7463 6872 1e02 0000 5807 0000 0074 6572  tchr....X....ter
+00003950: 6d66 6974 721f 0200 0058 1e00 0000 7265  mfitr....X....re
+00003960: 6669 6e65 7279 2e75 6e69 7473 2e73 7472  finery.units.str
+00003970: 696e 6773 2e74 6572 6d66 6974 7220 0200  ings.termfitr ..
+00003980: 0058 0400 0000 7472 696d 7221 0200 0058  .X....trimr!...X
+00003990: 1b00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+000039a0: 7473 2e73 7472 696e 6773 2e74 7269 6d72  ts.strings.trimr
+000039b0: 2202 0000 752e                           "...u.
```

### Comparing `binary-refinery-0.6.3/refinery/__init__.py` & `binary-refinery-0.6.4/refinery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 1. `refinery.lib.frame`: framing syntax for working on lists of binary chunks
 2. `refinery.lib.argformats`: the multibin syntax for refinery arguments
 3. `refinery.lib.meta`: defining and using metadata variables within frames
 4. `refinery.units`: writing custom units, add command-line arguments, and how to use refinery
    units within Python code.
 """
-__version__ = '0.6.3'
+__version__ = '0.6.4'
 __distribution__ = 'binary-refinery'
 
 from typing import Dict, List, Optional, Type
 from importlib import resources
 from datetime import datetime
 
 import pickle
```

### Comparing `binary-refinery-0.6.3/refinery/data/rich.json` & `binary-refinery-0.6.4/refinery/data/rich.json`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/explore.py` & `binary-refinery-0.6.4/refinery/explore.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/argformats.py` & `binary-refinery-0.6.4/refinery/lib/argformats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1083,26 +1083,28 @@
         """
         Convert a binary input into the integer that it encodes in big endian format, and vice versa.
         """
         if isinstance(arg, int):
             size, remainder = divmod(arg.bit_length(), 8)
             if remainder: size += 1
             return arg.to_bytes(size, 'big')
-        return int.from_bytes(arg, 'big')
+        else:
+            return int.from_bytes(arg, 'big')
 
     @handler.register('le')
     def le(self, arg: Union[int, ByteString]) -> int:
         """
         Convert a binary input into the integer that it encodes in little endian format, and vice versa.
         """
         if isinstance(arg, int):
             size, remainder = divmod(arg.bit_length(), 8)
             if remainder: size += 1
             return arg.to_bytes(size, 'little')
-        return int.from_bytes(arg, 'little')
+        else:
+            return int.from_bytes(arg, 'little')
 
     @handler.register('reduce')
     def reduce(self, it: Iterable[int], reduction: str, seed: Optional[str] = None) -> int:
         """
         The handler `reduce[reduction, seed=0]` has two parameters. The string `reduction` is a
         Python expression that involves the two special variables `S` (the state) and `B`
         (the current block value). This expression is evaluated for every `B` in the incoming
```

### Comparing `binary-refinery-0.6.3/refinery/lib/argparser.py` & `binary-refinery-0.6.4/refinery/lib/argparser.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/chunks.py` & `binary-refinery-0.6.4/refinery/lib/chunks.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/crypto.py` & `binary-refinery-0.6.4/refinery/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/decompression.py` & `binary-refinery-0.6.4/refinery/lib/decompression.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/decorators.py` & `binary-refinery-0.6.4/refinery/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/deobfuscation.py` & `binary-refinery-0.6.4/refinery/lib/deobfuscation.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/dex.py` & `binary-refinery-0.6.4/refinery/lib/dex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/dotnet/deserialize.py` & `binary-refinery-0.6.4/refinery/lib/dotnet/deserialize.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/dotnet/header.py` & `binary-refinery-0.6.4/refinery/lib/dotnet/header.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/dotnet/resources.py` & `binary-refinery-0.6.4/refinery/lib/dotnet/resources.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/dotnet/types.py` & `binary-refinery-0.6.4/refinery/lib/dotnet/types.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/environment.py` & `binary-refinery-0.6.4/refinery/lib/environment.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/executable.py` & `binary-refinery-0.6.4/refinery/lib/executable.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/frame.py` & `binary-refinery-0.6.4/refinery/lib/frame.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/inline.py` & `binary-refinery-0.6.4/refinery/lib/inline.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/java.py` & `binary-refinery-0.6.4/refinery/lib/java.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/json.py` & `binary-refinery-0.6.4/refinery/lib/json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/loader.py` & `binary-refinery-0.6.4/refinery/lib/loader.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/magic.py` & `binary-refinery-0.6.4/refinery/lib/magic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/meta.py` & `binary-refinery-0.6.4/refinery/lib/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 from __future__ import annotations
 
 import abc
 import contextlib
 import string
 import codecs
 import itertools
+import os
 
 from io import StringIO
 from urllib.parse import quote_from_bytes, unquote_to_bytes
 from typing import Callable, Dict, Iterable, Optional, ByteString, Union, TYPE_CHECKING
 
 from refinery.lib.structures import MemoryFile
 from refinery.lib.tools import isbuffer, entropy, index_of_coincidence
@@ -149,24 +150,33 @@
     @abc.abstractmethod
     def __str__(self): ...
 
     @abc.abstractmethod
     def __repr__(self): ...
 
 
-_PRINTABLE = (
-    B'0123456789'
-    B'!#$%&()*,-./:;=?@[\\]{}~'
-    B'abcdefghijklmnopqrstuvwxyz'
-    B'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
-)
-
-_IS_PRINTABLE = bytearray(256)
-for p in _PRINTABLE:
-    _IS_PRINTABLE[p] = 1
+_PRINT_SAFE = set(string.printable.encode('latin1')) - set(b'|<>&\t\n\r\x0B\x0B')
+if os.name == 'nt':
+    _PRINT_SAFE -= set(b'^"')
+else:
+    _PRINT_SAFE -= set(b'*?\'"')
+_PRINT_SAFE = bytes(_PRINT_SAFE)
+_IS_PRINT_SAFE = bytearray(256)
+for p in _PRINT_SAFE:
+    _IS_PRINT_SAFE[p] = 1
+
+
+def is_print_safe(string: str):
+    if not string.isprintable():
+        return False
+    for letter in string:
+        code = ord(letter)
+        if code < len(_IS_PRINT_SAFE) and not _IS_PRINT_SAFE[code]:
+            return False
+    return True
 
 
 class ByteStringWrapper(bytearray, CustomStringRepresentation):
     """
     Represents a binary string and a preferred codec in case it is printable. Casting this wrapper class
     will decode the string using the given codec, using backslash escape sequences to handle decoding
     errors. The `repr` case returns a hexadecimal representation of the binary data. Finally, the object
@@ -252,22 +262,22 @@
                     prefix = None
             if prefix is None:
                 representation = self.string
                 prefix = self._CODECS[self.codec]
         except AttributeError:
             representation = None
         else:
-            if not representation.isprintable() or any(c in representation for c in '&<|>'):
+            if not is_print_safe(representation):
                 representation = None
             elif prefix != 's' or self.requires_prefix(representation):
                 representation = F'{prefix}:{representation}'
         if representation is None:
-            if sum(_IS_PRINTABLE[c] for c in self) >= len(self) * 0.8:
+            if sum(_IS_PRINT_SAFE[c] for c in self) > len(self) * 0.6:
                 from urllib.parse import quote_from_bytes
-                quoted = quote_from_bytes(self, _PRINTABLE)
+                quoted = quote_from_bytes(self, _PRINT_SAFE)
                 representation = F'q:{quoted}'
             else:
                 representation = F'h:{self.hex()}'
         self._representation = representation
         return representation
 
     def __str__(self):
```

### Comparing `binary-refinery-0.6.3/refinery/lib/mime.py` & `binary-refinery-0.6.4/refinery/lib/mime.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     'application/vnd.lotus-1-2-3': '123',
     'application/vnd.microsoft.portable-executable': 'exe',
     'application/vnd.mozilla.xul+xml': 'xul',
     'application/vnd.ms-cab-compressed': 'cab',
     'application/vnd.ms-excel': 'xls',
     'application/vnd.ms-fontobject': 'eot',
     'application/vnd.ms-powerpoint': 'ppt',
+    'application/vnd.ms-outlook': 'eml',
     'application/vnd.oasis.opendocument.presentation': 'odp',
     'application/vnd.oasis.opendocument.spreadsheet': 'ods',
     'application/vnd.oasis.opendocument.text': 'odt',
     'application/vnd.openxmlformats-officedocument.presentationml.presentation': 'pptx',
     'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet': 'xlsx',
     'application/vnd.openxmlformats-officedocument.wordprocessingml.document': 'docx',
     'application/vnd.rar': 'rar',
@@ -247,15 +248,15 @@
     description: str
     mime: str
 
     _GZIP_PEEK_MAXIMUM = 1024
     _GZIP_PEEK_MINIMUM = 64
     _GZIP_DC_CHUNK_LEN = 16
 
-    def __init__(self, data, default='bin'):
+    def __init__(self, data, default='bin', decompress=True):
         if not magic:
             raise NoMagicAvailable
         if not isinstance(data, bytes):
             data = bytes(data)
         mime = magicparse(data, mime=True)
         self.mime = mime.split(';')[0].lower()
         self.description = magicparse(data)
@@ -263,15 +264,15 @@
             extension = FileTypeMap[self.mime]
         except KeyError:
             extension = default
         if self.description == 'Microsoft OOXML':
             extension = 'docx'
         if extension == 'exe':
             extension = 'dll' if '(DLL)' in self.description else 'exe'
-        elif extension in ('gz', 'gzip', 'bz2'):
+        elif extension in ('gz', 'gzip', 'bz2') and decompress:
             if extension == 'bz2':
                 import bz2
                 dc = bz2.BZ2Decompressor()
             else:
                 import zlib
                 dc = zlib.decompressobj(0x10)
             mv = memoryview(data)
```

### Comparing `binary-refinery-0.6.3/refinery/lib/mscrypto.py` & `binary-refinery-0.6.4/refinery/lib/mscrypto.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/murmur.py` & `binary-refinery-0.6.4/refinery/lib/murmur.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/patterns/__init__.py` & `binary-refinery-0.6.4/refinery/lib/patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/patterns/tlds.py` & `binary-refinery-0.6.4/refinery/lib/patterns/tlds.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/powershell.py` & `binary-refinery-0.6.4/refinery/lib/powershell.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/ripemd128.py` & `binary-refinery-0.6.4/refinery/lib/ripemd128.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/serpent.py` & `binary-refinery-0.6.4/refinery/lib/serpent.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/structures.py` & `binary-refinery-0.6.4/refinery/lib/structures.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/suffixtree.py` & `binary-refinery-0.6.4/refinery/lib/suffixtree.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/thirdparty/acefile.py` & `binary-refinery-0.6.4/refinery/lib/thirdparty/acefile.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/thirdparty/batch_interpreter.py` & `binary-refinery-0.6.4/refinery/lib/thirdparty/batch_interpreter.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/thirdparty/pcode2code.py` & `binary-refinery-0.6.4/refinery/lib/thirdparty/pcode2code.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/thirdparty/xxhash.py` & `binary-refinery-0.6.4/refinery/lib/thirdparty/xxhash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/tools.py` & `binary-refinery-0.6.4/refinery/lib/tools.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/types.py` & `binary-refinery-0.6.4/refinery/lib/types.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/vfs.py` & `binary-refinery-0.6.4/refinery/lib/vfs.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/lib/xml.py` & `binary-refinery-0.6.4/refinery/lib/xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/__init__.py` & `binary-refinery-0.6.4/refinery/units/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,14 +234,21 @@
     If this exception is thrown, processing of the entire input stream
     is aborted instead of just aborting the processing of the current
     chunk.
     """
     pass
 
 
+class RefineryException(RuntimeError):
+    """
+    This is an exception that was not generated by an external library.
+    """
+    pass
+
+
 class Entry:
     """
     An empty class marker. Any entry point unit (i.e. any unit that can be executed
     via the command line) is an instance of this class.
     """
     pass
 
@@ -336,17 +343,17 @@
 
             def __missing__(self, key):
                 if key == 'choices':
                     return ', '.join(self.arg.kwargs['choices'])
                 if key == 'default':
                     default: Union[bytes, int, str] = self.arg.kwargs['default']
                     if isinstance(default, int):
-                        return repr(default)
+                        return default
                     if not isbuffer(default):
-                        return str(default)
+                        return default
                     if default.isalnum():
                         return default.decode('latin-1')
                     return F'H:{default.hex()}'
                 if key == 'varname':
                     return self.arg.kwargs.get('metavar', self.arg.destination)
 
         try:
@@ -1237,22 +1244,27 @@
         elif isinstance(exception, VariableMissing):
             self.log_warn('critical error:', exception.args[0])
             abort_execution = True
         elif isinstance(exception, GeneratorExit):
             raise exception
         elif isinstance(exception, RefineryImportMissing):
             self.log_fail(F'dependency {exception.missing} is missing; run pip install {exception.install}')
+        elif isinstance(exception, RefineryException):
+            self.log_fail(exception.args[0])
         else:
             try:
                 explanation = exception.args[0]
             except (AttributeError, IndexError):
                 explanation = exception
             if not isinstance(explanation, str):
                 explanation = exception
-            message = F'exception of type {exception.__class__.__name__}; {explanation!s}'
+            explanation = str(explanation).strip()
+            message = F'exception of type {exception.__class__.__name__}'
+            if explanation:
+                message = F'{message}; {explanation!s}'
             if self.log_level <= LogLevel.INFO and data is not None:
                 from refinery.units.sinks.peek import peek
                 peeked = str(data | peek(lines=2, decode=True, stdout=True))
                 message = F'{message}\n{peeked}'
             self.log_fail(message)
 
         if self.log_debug():
@@ -1480,24 +1492,34 @@
             converter = get_converter(stream)
             if converter is None:
                 stream.update(self)
                 return stream
             return {converter(chunk) for chunk in self}
         elif isinstance(stream, dict):
             key, convert = one(stream.items())
-            output: Dict[Any, List[Any]] = {}
+            output: Dict[Any, Union[List[Chunk], Set[Chunk]]] = {}
+            deconflict = None
+            if isinstance(convert, (list, set)):
+                deconflict = type(convert)
+                convert = one(convert)
             for item in self:
                 try:
                     value = item.meta[key]
                 except KeyError:
                     value = None
-                bag = output.setdefault(value, [])
                 if convert is not ...:
                     item = convert(item)
-                bag.append(item)
+                if deconflict:
+                    bag = output.setdefault(value, deconflict())
+                    if isinstance(bag, list):
+                        bag.append(item)
+                    else:
+                        bag.add(item)
+                else:
+                    output[value] = item
             return output
         elif isinstance(stream, (bytearray, memoryview)):
             with MemoryFile(stream) as stdout:
                 return (self | stdout).getvalue()
         elif callable(stream):
             with MemoryFile(bytearray()) as stdout:
                 self | stdout
@@ -1667,14 +1689,20 @@
             return False
 
     @classmethod
     def _output(cls, *messages, clip=False) -> str:
         def transform(message):
             if callable(message):
                 message = message()
+            if isinstance(message, Exception):
+                args = [arg for arg in message.args if isinstance(arg, str)]
+                if len(args) == 1:
+                    message = args[0]
+                else:
+                    message = str(message)
             if isinstance(message, str):
                 return message
             if isbuffer(message):
                 import codecs
                 message: Union[bytes, bytearray, memoryview]
                 pmsg: str = codecs.decode(message, cls.codec, 'surrogateescape')
                 if not pmsg.isprintable():
```

### Comparing `binary-refinery-0.6.3/refinery/units/blockwise/__init__.py` & `binary-refinery-0.6.4/refinery/units/blockwise/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/blockwise/alu.py` & `binary-refinery-0.6.4/refinery/units/blockwise/alu.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/blockwise/bitrev.py` & `binary-refinery-0.6.4/refinery/units/blockwise/bitrev.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/blockwise/byteswap.py` & `binary-refinery-0.6.4/refinery/units/blockwise/byteswap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/blockwise/map.py` & `binary-refinery-0.6.4/refinery/units/blockwise/map.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/blockwise/pack.py` & `binary-refinery-0.6.4/refinery/units/blockwise/pack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/blockwise/rev.py` & `binary-refinery-0.6.4/refinery/units/blockwise/rev.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/blockwise/terminate.py` & `binary-refinery-0.6.4/refinery/units/blockwise/terminate.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/blockwise/xor.py` & `binary-refinery-0.6.4/refinery/units/blockwise/xor.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/ap.py` & `binary-refinery-0.6.4/refinery/units/compression/ap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/blz.py` & `binary-refinery-0.6.4/refinery/units/compression/blz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/bz2.py` & `binary-refinery-0.6.4/refinery/units/compression/bz2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/decompress.py` & `binary-refinery-0.6.4/refinery/units/compression/decompress.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/jcalg.py` & `binary-refinery-0.6.4/refinery/units/compression/jcalg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/lz.py` & `binary-refinery-0.6.4/refinery/units/compression/lz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/lz4.py` & `binary-refinery-0.6.4/refinery/units/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/lzf.py` & `binary-refinery-0.6.4/refinery/units/compression/lzf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/lzg.py` & `binary-refinery-0.6.4/refinery/units/compression/lzg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/lzip.py` & `binary-refinery-0.6.4/refinery/units/compression/lzip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/lzjb.py` & `binary-refinery-0.6.4/refinery/units/compression/lzjb.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/lznt1.py` & `binary-refinery-0.6.4/refinery/units/compression/lznt1.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/lzo.py` & `binary-refinery-0.6.4/refinery/units/compression/lzo.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/mscf.py` & `binary-refinery-0.6.4/refinery/units/compression/mscf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/qlz.py` & `binary-refinery-0.6.4/refinery/units/compression/qlz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/szdd.py` & `binary-refinery-0.6.4/refinery/units/compression/szdd.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/compression/zl.py` & `binary-refinery-0.6.4/refinery/units/compression/zl.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/__init__.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/camellia.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/camellia.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/chacha.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/chacha.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/gost.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/gost.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/hc128.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/hc128.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/isaac.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/isaac.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/rabbit.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/rabbit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/rc2.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/rc2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/rc4mod.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/rc4mod.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/rc5.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/rc5.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/rc6.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/rc6.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/rijndael.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/rijndael.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/rncrypt.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/rncrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/rot.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/rot.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/rsa.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/rsa.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/rsakey.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/rsakey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/salsa.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/salsa.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/seal.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/seal.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/secstr.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/secstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/serpent.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/serpent.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/tea.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/tea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/vigenere.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/vigenere.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/xtea.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/xtea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/cipher/xxtea.py` & `binary-refinery-0.6.4/refinery/units/crypto/cipher/xxtea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/hash/__init__.py` & `binary-refinery-0.6.4/refinery/units/crypto/hash/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/hash/checksums.py` & `binary-refinery-0.6.4/refinery/units/crypto/hash/checksums.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/hash/cryptographic.py` & `binary-refinery-0.6.4/refinery/units/crypto/hash/cryptographic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/hash/imphash.py` & `binary-refinery-0.6.4/refinery/units/crypto/hash/imphash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/hash/murmur.py` & `binary-refinery-0.6.4/refinery/units/crypto/hash/murmur.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/hash/xxhash.py` & `binary-refinery-0.6.4/refinery/units/crypto/hash/xxhash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/keyderive/CryptDeriveKey.py` & `binary-refinery-0.6.4/refinery/units/crypto/keyderive/CryptDeriveKey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/keyderive/DESDerive.py` & `binary-refinery-0.6.4/refinery/units/crypto/keyderive/DESDerive.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/keyderive/PasswordDeriveBytes.py` & `binary-refinery-0.6.4/refinery/units/crypto/keyderive/PasswordDeriveBytes.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/keyderive/__init__.py` & `binary-refinery-0.6.4/refinery/units/crypto/keyderive/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/keyderive/kblob.py` & `binary-refinery-0.6.4/refinery/units/crypto/keyderive/kblob.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/keyderive/pbkdf1.py` & `binary-refinery-0.6.4/refinery/units/crypto/keyderive/pbkdf1.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/keyderive/pbkdf2.py` & `binary-refinery-0.6.4/refinery/units/crypto/keyderive/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/crypto/keyderive/unixcrypt.py` & `binary-refinery-0.6.4/refinery/units/crypto/keyderive/unixcrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/encoding/atbash.py` & `binary-refinery-0.6.4/refinery/units/encoding/atbash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/encoding/b32.py` & `binary-refinery-0.6.4/refinery/units/encoding/b32.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/encoding/b64.py` & `binary-refinery-0.6.4/refinery/units/encoding/b64.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/encoding/base.py` & `binary-refinery-0.6.4/refinery/units/encoding/base.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/encoding/esc.py` & `binary-refinery-0.6.4/refinery/units/encoding/esc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/encoding/hex.py` & `binary-refinery-0.6.4/refinery/units/encoding/hex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/encoding/netbios.py` & `binary-refinery-0.6.4/refinery/units/encoding/netbios.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/encoding/ps1str.py` & `binary-refinery-0.6.4/refinery/units/encoding/ps1str.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/encoding/recode.py` & `binary-refinery-0.6.4/refinery/units/encoding/recode.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/encoding/url.py` & `binary-refinery-0.6.4/refinery/units/encoding/url.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/encoding/uuenc.py` & `binary-refinery-0.6.4/refinery/units/encoding/uuenc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/encoding/wshenc.py` & `binary-refinery-0.6.4/refinery/units/encoding/wshenc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/__init__.py` & `binary-refinery-0.6.4/refinery/units/formats/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,16 @@
             self.data = self.data()
         return self.data
 
     def __init__(self, _br__path: str, _br__data: Union[ByteString, Callable[[], ByteString]], **_br__meta):
         self.path = _br__path
         self.data = _br__data
         self.meta = _br__meta
+        for key in [key for key, value in _br__meta.items() if value is None]:
+            del _br__meta[key]
 
 
 class EndOfStringNotFound(ValueError):
     def __init__(self):
         super().__init__('end of string could not be determined')
```

### Comparing `binary-refinery-0.6.3/refinery/units/formats/a3x.py` & `binary-refinery-0.6.4/refinery/units/formats/a3x.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/archive/__init__.py` & `binary-refinery-0.6.4/refinery/units/formats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/archive/xt.py` & `binary-refinery-0.6.4/refinery/units/formats/archive/xt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 from typing import List, Type
 
 from refinery.units.formats.archive import ArchiveUnit
+from refinery.units import RefineryException
 
 
 class xt(ArchiveUnit):
     """
     Extract files from archives. The unit tries to identify the archive format and use the
     correct extractor.
     """
@@ -40,14 +41,16 @@
         yield xttar
         from refinery.units.formats.archive.xtiss import xtiss
         yield xtiss
         from refinery.units.formats.archive.xtzip import xtzip
         yield xtzip
         from refinery.units.formats.archive.xt7z import xt7z
         yield xt7z
+        from refinery.units.formats.msi import xtmsi
+        yield xtmsi
         from refinery.units.formats.office.xtdoc import xtdoc
         yield xtdoc
         from refinery.units.formats.json import xtjson
         yield xtjson
         from refinery.units.formats.exe.vsect import vsect
         yield vsect
 
@@ -78,29 +81,31 @@
             def __iter__(self):
                 handler = self.handler
                 if self.fallback:
                     verdict = True
                 else:
                     verdict = handler.handles(data)
                 if verdict is False:
-                    self.unit.log_info(F'handler {handler.name} cannot handle this data')
+                    self.unit.log_info(F'rejected: {handler.name}')
                 elif verdict is True:
+                    if not self.fallback:
+                        self.unit.log_info(F'accepted: {handler.name}')
                     try:
                         unit = handler(*pos_args, **key_args)
                     except TypeError as error:
-                        self.unit.log_debug(F'handler {handler.name} failed: {error!s}')
+                        self.unit.log_debug('handler construction failed:', error)
                         return
-                    if not self.fallback:
-                        self.unit.log_info(F'handler {handler.name} can handle this input data')
                     try:
-                        yield from unit.unpack(data)
-                    except Exception as E:
+                        for item in unit.unpack(data):
+                            item.get_data()
+                            yield item
+                    except Exception as error:
                         if not self.fallback:
-                            errors[handler.name] = E
-                        self.unit.log_info(F'unpacking with {handler.name} failed: {E!s}')
+                            errors[handler.name] = error
+                        self.unit.log_debug('handler unpacking failed:', error)
                         return
                     else:
                         self.success = True
                         return
                 elif verdict is None:
                     fallback.append(handler)
 
@@ -118,9 +123,9 @@
             yield from it
             if it.success:
                 return
 
         if not errors:
             raise ValueError('input data did not match any known archive format')
         for name, error in errors.items():
-            self.log_info(F'error when trying to unpack with {name}', error)
-        raise ValueError('failed to unpack with all known methods')
+            self.log_info(F'error when trying to unpack with {name}:', error)
+        raise RefineryException('none of the available unpackers could handle this data')
```

### Comparing `binary-refinery-0.6.3/refinery/units/formats/archive/xt7z.py` & `binary-refinery-0.6.4/refinery/units/formats/archive/xt7z.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/archive/xtace.py` & `binary-refinery-0.6.4/refinery/units/formats/archive/xtace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/archive/xtasar.py` & `binary-refinery-0.6.4/refinery/units/formats/archive/xtasar.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/archive/xtcab.py` & `binary-refinery-0.6.4/refinery/units/formats/archive/xtcab.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/archive/xtcpio.py` & `binary-refinery-0.6.4/refinery/units/formats/archive/xtcpio.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/archive/xtiso.py` & `binary-refinery-0.6.4/refinery/units/formats/archive/xtiso.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/archive/xtiss.py` & `binary-refinery-0.6.4/refinery/units/formats/archive/xtiss.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/archive/xtnode.py` & `binary-refinery-0.6.4/refinery/units/formats/archive/xtnode.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/archive/xtnsis.py` & `binary-refinery-0.6.4/refinery/units/formats/archive/xtnsis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1053,14 +1053,17 @@
             if self.solid:
                 self._solid_iter = it
             self.entry_offset_delta = header_entry.compressed_size
             header_data = header_entry.data
         else:
             self.entry_offset_delta = len(header_data)
 
+        if not header_data:
+            raise ValueError('header data had length zero')
+
         xtnsis.log_debug(F'read header of length {len(header_data)}')
 
         self.header = NSHeader(header_data, size=self.size_of_header)
         self.reader = reader
 
     @property
     def script(self):
```

### Comparing `binary-refinery-0.6.3/refinery/units/formats/archive/xtpyi.py` & `binary-refinery-0.6.4/refinery/units/formats/archive/xtpyi.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/archive/xttar.py` & `binary-refinery-0.6.4/refinery/units/formats/archive/xttar.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/archive/xtzip.py` & `binary-refinery-0.6.4/refinery/units/formats/archive/xtzip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/bat.py` & `binary-refinery-0.6.4/refinery/units/formats/bat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/deserialize_php.py` & `binary-refinery-0.6.4/refinery/units/formats/deserialize_php.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/email.py` & `binary-refinery-0.6.4/refinery/units/formats/email.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,16 @@
             lambda h=head: '\n'.join(F'{k}: {v}' for k, v in h).encode(self.codec))
         yield UnpackResult('headers.json',
             lambda jsn=jh: json.dumps(jsn, indent=4).encode(self.codec))
 
     @PathExtractorUnit.Requires('extract-msg', optional=False)
     def _extract_msg():
         import extract_msg.message
-        return extract_msg.message
+        import extract_msg.enums
+        return extract_msg
 
     def _get_parts_outlook(self, data):
         def ensure_bytes(data):
             return data if isinstance(data, bytes) else data.encode(self.codec)
 
         def make_message(name, msg):
             with NoLogging():
@@ -52,15 +53,15 @@
                 yield UnpackResult(F'{name}.txt', ensure_bytes(txt))
             if htm:
                 yield UnpackResult(F'{name}.htm', ensure_bytes(htm))
 
         msgcount = 0
 
         with NoLogging():
-            class ForgivingMessage(self._extract_msg.Message):
+            class ForgivingMessage(self._extract_msg.message.Message):
                 """
                 If parsing the input bytes fails early, the "__open" private attribute may not
                 yet exist. This hack prevents an exception to occur in the destructor.
                 """
                 def __getattr__(self, key: str):
                     if key.endswith('_open'):
                         return False
@@ -74,21 +75,21 @@
             for attachment in getattr(msg, 'attachments', ()):
                 yield attachment
                 if attachment.type == 'data':
                     continue
                 yield from attachments(attachment.data)
 
         for attachment in attachments(msg):
-            self.log_debug(attachment)
-            if attachment.type == 'msg':
+            at = attachment.type
+            if at is self._extract_msg.enums.AttachmentType.MSG:
                 msgcount += 1
                 yield from make_message(F'attachments/msg_{msgcount:d}', attachment.data)
                 continue
             if not isbuffer(attachment.data):
-                self.log_warn(F'unknown attachment of type {attachment.type}, please report this!')
+                self.log_warn(F'unknown attachment of type {at}, please report this!')
                 continue
             path = attachment.longFilename or attachment.shortFilename
             yield UnpackResult(F'attachments/{path}', attachment.data)
 
     @PathExtractorUnit.Requires('chardet', optional=False)
     def _chardet():
         import chardet
@@ -143,10 +144,19 @@
             yield from self._get_parts_outlook(data)
         except Exception:
             self.log_debug('failed parsing input as Outlook message')
             yield from self._get_parts_regular(data)
 
     @classmethod
     def handles(cls, data: bytearray) -> bool:
+        markers = [
+            b'\nReceived:\x20from'
+            b'\nSubject:\x20',
+            b'\nTo:\x20',
+            b'\nBcc:\x20',
+            b'\nContent-Transfer-Encoding:\x20',
+            b'\nContent-Type:\x20',
+            b'\nReturn-Path:\x20',
+        ]
         if data.startswith(B'\xD0\xCF\x11\xE0\xA1\xB1\x1A\xE1'):
-            return True
-        return b'\nReceived: from' in data
+            markers = [marker.decode('latin1').encode('utf-16le') for marker in markers]
+        return sum(1 for marker in markers if marker in data) >= 3
```

### Comparing `binary-refinery-0.6.3/refinery/units/formats/evtx.py` & `binary-refinery-0.6.4/refinery/units/formats/evtx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/exe/vaddr.py` & `binary-refinery-0.6.4/refinery/units/formats/exe/vaddr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/exe/vmemref.py` & `binary-refinery-0.6.4/refinery/units/formats/exe/vmemref.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/exe/vsect.py` & `binary-refinery-0.6.4/refinery/units/formats/exe/vsect.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/exe/vsnip.py` & `binary-refinery-0.6.4/refinery/units/formats/exe/vsnip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/exe/vstack.py` & `binary-refinery-0.6.4/refinery/units/formats/exe/vstack.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,22 @@
     executable: Executable
     address: int
     writes: IntervalTree
     disassembler: Optional[Cs] = None
     waiting: int = 0
     calling: bool = False
 
+    def disassemble(self, address: int, size: int):
+        if self.disassembler is None:
+            return None
+        pos = self.executable.location_from_address(address).physical.position
+        end = pos + size
+        return next(self.disassembler.disasm(
+            bytes(self.executable.data[pos:end]), address, 1))
+
 
 class vstack(Unit):
     """
     The unit emulates instructions at a given address in the input executable (PE/ELF/MachO) and
     extracts data patches that are written to the stack during emulation. Emulation is halted as
     soon as a certain number of instructions has not performed any memory writes, or when an error
     occurs.
@@ -151,14 +159,16 @@
 
         for segment in exe.segments():
             pmem = segment.physical
             vmem = segment.virtual
             try:
                 emulator.mem_map(vmem.lower, align(block_size, len(vmem)))
                 emulator.mem_write(vmem.lower, bytes(image[pmem.slice()]))
+            except KeyboardInterrupt:
+                raise
             except Exception as error:
                 if address in vmem:
                     raise
                 width = exe.pointer_size // 4
                 self.log_info(F'error mapping segment [{vmem.lower:0{width}X}-{vmem.upper:0{width}X}]: {error!s}')
 
         end_of_code = exe.location_from_address(address).virtual.box.upper
@@ -200,37 +210,42 @@
             R'aborting emulation; access error '
             F'at 0x{address:0{state.executable.pointer_size//4}X}; '
             F'value={value:0{size*2}X}; code={access}')
         emu.emu_stop()
         return False
 
     def _hook_code(self, emu: Uc, address: int, size: int, state: EmuState):
-        waiting = state.waiting
-
-        if address == state.address:
-            if waiting > self.args.halt_after:
-                emu.emu_stop()
-                return False
-            state.waiting += 1
-            state.address += size
-            state.calling = False
-        else:
-            state.calling = True
-
-        def debug_message():
-            pos = state.executable.location_from_address(address).physical.position
-            end = pos + size
-            instruction = next(state.disassembler.disasm(bytes(state.executable.data[pos:end]), address, 1))
-            flags = 'C' if state.calling else ' '
-            return (
-                F'emulating [wait={waiting}] [{flags}] 0x{address:0{state.executable.pointer_size//4}X}: '
-                F'{instruction.mnemonic} {instruction.op_str}'
-            )
+        try:
+            waiting = state.waiting
 
-        self.log_debug(debug_message)
+            if address == state.address:
+                if waiting > self.args.halt_after:
+                    emu.emu_stop()
+                    return False
+                state.waiting += 1
+                state.address += size
+                state.calling = False
+            else:
+                instruction = state.disassemble(address, size)
+                if instruction and instruction.mnemonic == 'call':
+                    state.calling = True
+
+            def debug_message():
+                instruction = state.disassemble(address, size)
+                flags = 'C' if state.calling else ' '
+                return (
+                    F'emulating [wait={waiting}] [{flags}] 0x{address:0{state.executable.pointer_size//4}X}: '
+                    F'{instruction.mnemonic} {instruction.op_str}'
+                )
+
+            self.log_debug(debug_message)
+
+        except KeyboardInterrupt:
+            emu.emu_stop()
+            return False
 
     def _uc_arch(self, arch: Arch) -> Tuple[int, int]:
         uc = self._unicorn
         return {
             Arch.X8632   : (uc.UC_ARCH_X86,   uc.UC_MODE_32),     # noqa
             Arch.X8664   : (uc.UC_ARCH_X86,   uc.UC_MODE_64),     # noqa
             Arch.ARM32   : (uc.UC_ARCH_ARM,   uc.UC_MODE_ARM),    # noqa
```

### Comparing `binary-refinery-0.6.3/refinery/units/formats/hexload.py` & `binary-refinery-0.6.4/refinery/units/formats/hexload.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/html.py` & `binary-refinery-0.6.4/refinery/units/formats/html.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/httpresponse.py` & `binary-refinery-0.6.4/refinery/units/formats/httpresponse.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/ifps.py` & `binary-refinery-0.6.4/refinery/units/formats/ifps.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/ifpsstr.py` & `binary-refinery-0.6.4/refinery/units/formats/ifpsstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/java/deserialize.py` & `binary-refinery-0.6.4/refinery/units/formats/java/deserialize.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/java/jvdasm.py` & `binary-refinery-0.6.4/refinery/units/formats/java/jvdasm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/json.py` & `binary-refinery-0.6.4/refinery/units/formats/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,8 +103,8 @@
             from refinery.units.pattern.carve_json import carve_json
             doc = data | carve_json | json.loads
         try:
             it = doc.values()
         except AttributeError:
             it = doc
         for item in it:
-            yield json.dumps(item).encode(self.codec)
+            yield json.dumps(item, indent=4).encode(self.codec)
```

### Comparing `binary-refinery-0.6.3/refinery/units/formats/lnk.py` & `binary-refinery-0.6.4/refinery/units/formats/lnk.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/msgpack.py` & `binary-refinery-0.6.4/refinery/units/formats/msgpack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/office/doctxt.py` & `binary-refinery-0.6.4/refinery/units/formats/office/doctxt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/office/officecrypt.py` & `binary-refinery-0.6.4/refinery/units/formats/office/officecrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/office/vbapc.py` & `binary-refinery-0.6.4/refinery/units/formats/office/vbapc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/office/vbastr.py` & `binary-refinery-0.6.4/refinery/units/formats/office/vbastr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/office/xlmdeobf.py` & `binary-refinery-0.6.4/refinery/units/formats/office/xlmdeobf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/office/xlxtr.py` & `binary-refinery-0.6.4/refinery/units/formats/office/xlxtr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/office/xtdoc.py` & `binary-refinery-0.6.4/refinery/units/formats/office/xtdoc.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,27 @@
 from typing import Optional
 
 from refinery.units.formats import PathExtractorUnit, UnpackResult
 from refinery.units.formats.archive.xtzip import xtzip
 from refinery.lib.structures import MemoryFile
 
 
+def convert_msi_name(name: str):
+    def _decode(alphabet='0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz._!'):
+        for character in name:
+            code = ord(character)
+            if 0x3800 <= code < 0x4800:
+                yield alphabet[(code - 0x3800) & 0x3F] + alphabet[((code - 0x3800) >> 6) & 0x3F]
+            elif 0x4800 <= code <= 0x4840:
+                yield alphabet[code - 0x4800]
+            else:
+                yield character
+    return ''.join(_decode())
+
+
 class xtdoc(PathExtractorUnit):
     """
     Extract files from an OLE document such as a Microsoft Word DOCX file.
     """
 
     @PathExtractorUnit.Requires('olefile', optional=False)
     def _olefile():
@@ -30,14 +43,15 @@
                     continue
                 path = '/'.join(item)
                 olestream = oledoc.openstream(path)
                 c0 = ord(item[-1][:1])
                 if c0 < 20:
                     item[-1] = F'[{c0:d}]{item[-1][1:]}'
                     path = '/'.join(item)
+                path = convert_msi_name(path)
                 self.log_debug('exploring:', path)
                 yield UnpackResult(path, olestream.read())
 
     @classmethod
     def handles(self, data: bytearray) -> Optional[bool]:
         if data.startswith(B'\xD0\xCF\x11\xE0'):
             return True
```

### Comparing `binary-refinery-0.6.3/refinery/units/formats/office/xtone.py` & `binary-refinery-0.6.4/refinery/units/formats/office/xtone.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/office/xtrtf.py` & `binary-refinery-0.6.4/refinery/units/formats/office/xtrtf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/office/xtvba.py` & `binary-refinery-0.6.4/refinery/units/formats/office/xtvba.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pcap.py` & `binary-refinery-0.6.4/refinery/units/formats/pcap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pcap_http.py` & `binary-refinery-0.6.4/refinery/units/formats/pcap_http.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pdf.py` & `binary-refinery-0.6.4/refinery/units/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pe/__init__.py` & `binary-refinery-0.6.4/refinery/units/formats/pe/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/__init__.py` & `binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dncfx.py` & `binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/dncfx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnds.py` & `binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/dnds.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnfields.py` & `binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/dnfields.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnhdr.py` & `binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/dnhdr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnmr.py` & `binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/dnmr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnrc.py` & `binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/dnrc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pe/dotnet/dnstr.py` & `binary-refinery-0.6.4/refinery/units/formats/pe/dotnet/dnstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pe/pemeta.py` & `binary-refinery-0.6.4/refinery/units/formats/pe/pemeta.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pe/peoverlay.py` & `binary-refinery-0.6.4/refinery/units/formats/pe/peoverlay.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pe/perc.py` & `binary-refinery-0.6.4/refinery/units/formats/pe/perc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pe/pesig.py` & `binary-refinery-0.6.4/refinery/units/formats/pe/pesig.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pe/pestrip.py` & `binary-refinery-0.6.4/refinery/units/formats/pe/pestrip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pkcs7.py` & `binary-refinery-0.6.4/refinery/units/formats/pkcs7.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/pkcs7sig.py` & `binary-refinery-0.6.4/refinery/units/formats/pkcs7sig.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/stego.py` & `binary-refinery-0.6.4/refinery/units/formats/stego.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/winreg.py` & `binary-refinery-0.6.4/refinery/units/formats/winreg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/formats/xml.py` & `binary-refinery-0.6.4/refinery/units/formats/xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/malware/n40.py` & `binary-refinery-0.6.4/refinery/units/malware/n40.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/__init__.py` & `binary-refinery-0.6.4/refinery/units/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/chop.py` & `binary-refinery-0.6.4/refinery/units/meta/chop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/cm.py` & `binary-refinery-0.6.4/refinery/units/meta/cm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/cull.py` & `binary-refinery-0.6.4/refinery/units/meta/cull.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/dedup.py` & `binary-refinery-0.6.4/refinery/units/meta/dedup.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/eat.py` & `binary-refinery-0.6.4/refinery/units/meta/eat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/ef.py` & `binary-refinery-0.6.4/refinery/units/meta/ef.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/emit.py` & `binary-refinery-0.6.4/refinery/units/meta/emit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/group.py` & `binary-refinery-0.6.4/refinery/units/meta/group.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/groupby.py` & `binary-refinery-0.6.4/refinery/units/meta/groupby.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/iff.py` & `binary-refinery-0.6.4/refinery/units/meta/iff.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/iffp.py` & `binary-refinery-0.6.4/refinery/units/meta/iffp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/iffs.py` & `binary-refinery-0.6.4/refinery/units/meta/iffs.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/iffx.py` & `binary-refinery-0.6.4/refinery/units/meta/iffx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/max.py` & `binary-refinery-0.6.4/refinery/units/meta/max.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/min.py` & `binary-refinery-0.6.4/refinery/units/meta/min.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/mvc.py` & `binary-refinery-0.6.4/refinery/units/meta/mvc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/mvg.py` & `binary-refinery-0.6.4/refinery/units/meta/mvg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/pad.py` & `binary-refinery-0.6.4/refinery/units/meta/pad.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/pick.py` & `binary-refinery-0.6.4/refinery/units/meta/pick.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/pop.py` & `binary-refinery-0.6.4/refinery/units/meta/pop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/push.py` & `binary-refinery-0.6.4/refinery/units/meta/push.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/put.py` & `binary-refinery-0.6.4/refinery/units/meta/put.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,33 @@
 import functools
 
 from refinery.units import Arg, Unit, Chunk
 from refinery.lib.argformats import numseq
 from refinery.lib.tools import isbuffer
 from refinery.lib.meta import check_variable_name
 
+_EMPTY = object()
+
 
 class put(Unit):
     """
     Can be used to add a meta variable to the processed chunk. Note that meta variables
     cease to exist outside a frame.
     """
     def __init__(
         self,
         name : Arg(help='The name of the variable to be used.', type=str),
         value: Arg(help='The value for the variable. If no value is given, the entire current chunk is stored.',
-            type=functools.partial(numseq, typecheck=False)) = None
+            type=functools.partial(numseq, typecheck=False)) = _EMPTY
     ):
         super().__init__(name=check_variable_name(name), value=value)
 
     def process(self, data: Chunk):
         value = self.args.value
-        if value is None:
+        if value is _EMPTY:
             value = data
         if not isinstance(value, (int, float)) and not isbuffer(value):
             try:
                 len(value)
             except TypeError:
                 if isinstance(value, itertools.repeat):
                     value = next(value)
```

### Comparing `binary-refinery-0.6.3/refinery/units/meta/queue.py` & `binary-refinery-0.6.4/refinery/units/meta/queue.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/reduce.py` & `binary-refinery-0.6.4/refinery/units/meta/reduce.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/scope.py` & `binary-refinery-0.6.4/refinery/units/meta/scope.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/sep.py` & `binary-refinery-0.6.4/refinery/units/meta/sep.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/sorted.py` & `binary-refinery-0.6.4/refinery/units/meta/sorted.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/swap.py` & `binary-refinery-0.6.4/refinery/units/meta/swap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/transpose.py` & `binary-refinery-0.6.4/refinery/units/meta/transpose.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/meta/xfcc.py` & `binary-refinery-0.6.4/refinery/units/meta/xfcc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/misc/autoxor.py` & `binary-refinery-0.6.4/refinery/units/misc/autoxor.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/misc/couple.py` & `binary-refinery-0.6.4/refinery/units/misc/couple.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/misc/datefix.py` & `binary-refinery-0.6.4/refinery/units/misc/datefix.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/misc/drp.py` & `binary-refinery-0.6.4/refinery/units/misc/drp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/misc/nop.py` & `binary-refinery-0.6.4/refinery/units/misc/nop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/misc/urlfix.py` & `binary-refinery-0.6.4/refinery/units/misc/urlfix.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/misc/xkey.py` & `binary-refinery-0.6.4/refinery/units/misc/xkey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/__init__.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/js/arrays.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/js/arrays.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/js/getattr.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/js/getattr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/js/tuples.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/js/tuples.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/__init__.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/ps1/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/all.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/ps1/all.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/brackets.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/ps1/brackets.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/cases.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/ps1/cases.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/concat.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/ps1/concat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/format.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/ps1/format.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/invoke.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/ps1/invoke.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/securestring.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/ps1/securestring.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/stringreplace.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/ps1/stringreplace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/typecast.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/ps1/typecast.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/ps1/uncurly.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/ps1/uncurly.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/vba/all.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/vba/all.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/vba/arithmetic.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/vba/arithmetic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/vba/brackets.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/vba/brackets.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/vba/char.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/vba/char.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/vba/concat.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/vba/concat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/vba/constants.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/vba/constants.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/vba/dummies.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/vba/dummies.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/vba/stringreplace.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/vba/stringreplace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/obfuscation/vba/stringreverse.py` & `binary-refinery-0.6.4/refinery/units/obfuscation/vba/stringreverse.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/__init__.py` & `binary-refinery-0.6.4/refinery/units/pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/carve.py` & `binary-refinery-0.6.4/refinery/units/pattern/carve.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,17 @@
         if not decode:
             decoder = NotImplemented
         elif self.args.format in (formats.multiline_string, formats.string):
             def decoder(chunk):
                 return decoder.unesc(chunk[1:-1])
             from ..encoding.esc import esc
             decoder.unesc = esc()
+        elif self.args.format is formats.integer:
+            from ..encoding.base import base
+            decoder = base()
         elif self.args.format in (formats.uppercase_hex, formats.hex):
             from ..encoding.hex import hex
             decoder = hex()
         elif self.args.format is formats.hexdump:
             from ..formats.hexload import hexload
             decoder = hexload()
         elif self.args.format is formats.intarray:
```

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/carve_7z.py` & `binary-refinery-0.6.4/refinery/units/pattern/carve_7z.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/carve_json.py` & `binary-refinery-0.6.4/refinery/units/pattern/carve_json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/carve_lnk.py` & `binary-refinery-0.6.4/refinery/units/pattern/carve_lnk.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/carve_pe.py` & `binary-refinery-0.6.4/refinery/units/pattern/carve_pe.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/carve_rtf.py` & `binary-refinery-0.6.4/refinery/units/pattern/carve_rtf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/carve_xml.py` & `binary-refinery-0.6.4/refinery/units/pattern/carve_xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/carve_zip.py` & `binary-refinery-0.6.4/refinery/units/pattern/carve_zip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/defang.py` & `binary-refinery-0.6.4/refinery/units/pattern/defang.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/dnsdomain.py` & `binary-refinery-0.6.4/refinery/units/pattern/dnsdomain.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/mimewords.py` & `binary-refinery-0.6.4/refinery/units/pattern/mimewords.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/resplit.py` & `binary-refinery-0.6.4/refinery/units/pattern/resplit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/resub.py` & `binary-refinery-0.6.4/refinery/units/pattern/resub.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/rex.py` & `binary-refinery-0.6.4/refinery/units/pattern/rex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/struct_parser.py` & `binary-refinery-0.6.4/refinery/units/pattern/struct_parser.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/subfiles.py` & `binary-refinery-0.6.4/refinery/units/pattern/subfiles.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/urlguards.py` & `binary-refinery-0.6.4/refinery/units/pattern/urlguards.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/xtp.py` & `binary-refinery-0.6.4/refinery/units/pattern/xtp.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,15 @@
         'cdnjs.cloudflare.com'    : 4,
         'comodo.net'              : 1,
         'comodoca.com'            : 1,
         'curl.haxx.se'            : 1,
         'digicert.com'            : 1,
         'dublincore.org'          : 1,
         'fontawesome.com'         : 1,
+        'facebook.com'            : 4,
         'github.com'              : 3,
         'globalsign.com'          : 1,
         'globalsign.net'          : 1,
         'godaddy.com'             : 1,
         'google.com'              : 4,
         'googleapis.com'          : 5,
         'googleusercontent.com'   : 5,
```

### Comparing `binary-refinery-0.6.3/refinery/units/pattern/xtw.py` & `binary-refinery-0.6.4/refinery/units/pattern/xtw.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/sinks/__init__.py` & `binary-refinery-0.6.4/refinery/units/sinks/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/sinks/asm.py` & `binary-refinery-0.6.4/refinery/units/sinks/asm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/sinks/dump.py` & `binary-refinery-0.6.4/refinery/units/sinks/dump.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/sinks/iemap.py` & `binary-refinery-0.6.4/refinery/units/sinks/iemap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/sinks/peek.py` & `binary-refinery-0.6.4/refinery/units/sinks/peek.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             if value is None:
                 continue
             if isinstance(value, CustomStringRepresentation):
                 value = repr(value).strip()
             elif isbuffer(value):
                 value = repr(ByteStringWrapper(value))
             elif isinstance(value, int):
-                if value in range(-99, 100):
+                if value in range(-999, 1000):
                     value = str(value)
                 elif value > 0:
                     value = F'0x{value:X}'
                 else:
                     value = F'-0x{-value:X}'
             elif isinstance(value, float):
                 value = F'{value:.4f}'
```

### Comparing `binary-refinery-0.6.3/refinery/units/sinks/ppjscript.py` & `binary-refinery-0.6.4/refinery/units/sinks/ppjscript.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/sinks/ppjson.py` & `binary-refinery-0.6.4/refinery/units/sinks/ppjson.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/sinks/ppxml.py` & `binary-refinery-0.6.4/refinery/units/sinks/ppxml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/strings/cfmt.py` & `binary-refinery-0.6.4/refinery/units/strings/cfmt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/strings/cswap.py` & `binary-refinery-0.6.4/refinery/units/strings/cswap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/strings/rep.py` & `binary-refinery-0.6.4/refinery/units/strings/rep.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/strings/repl.py` & `binary-refinery-0.6.4/refinery/units/strings/repl.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/strings/snip.py` & `binary-refinery-0.6.4/refinery/units/strings/snip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/strings/stretch.py` & `binary-refinery-0.6.4/refinery/units/strings/stretch.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/strings/termfit.py` & `binary-refinery-0.6.4/refinery/units/strings/termfit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/refinery/units/strings/trim.py` & `binary-refinery-0.6.4/refinery/units/strings/trim.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.3/setup.py` & `binary-refinery-0.6.4/setup.py`

 * *Files identical despite different names*

