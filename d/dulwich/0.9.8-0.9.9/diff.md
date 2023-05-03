# Comparing `tmp/dulwich-0.9.8.tar.gz` & `tmp/dulwich-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dulwich-0.9.8.tar", last modified: Sun Nov 30 17:27:45 2014, max compression
+gzip compressed data, was "dist/dulwich-0.9.9.tar", last modified: Sun Mar 22 00:16:16 2015, max compression
```

## Comparing `dulwich-0.9.8.tar` & `dulwich-0.9.9.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1152 2014-11-30 17:27:02.000000 dulwich-0.9.8/README.md
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/examples/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      273 2014-06-01 21:01:35.000000 dulwich-0.9.8/examples/config.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      867 2014-06-01 21:01:35.000000 dulwich-0.9.8/examples/clone.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      531 2014-06-08 21:51:22.000000 dulwich-0.9.8/examples/latest_change.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      490 2014-06-01 21:01:35.000000 dulwich-0.9.8/examples/diff.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1092 2014-06-01 21:01:35.000000 dulwich-0.9.8/HACKING
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      233 2014-06-01 21:01:35.000000 dulwich-0.9.8/MANIFEST.in
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1019 2014-11-30 17:27:45.000000 dulwich-0.9.8/PKG-INFO
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1132 2014-11-30 17:27:02.000000 dulwich-0.9.8/Makefile
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/docs/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     6949 2014-06-01 21:01:35.000000 dulwich-0.9.8/docs/conf.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      283 2014-06-01 21:01:35.000000 dulwich-0.9.8/docs/performance.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2274 2014-06-01 21:01:35.000000 dulwich-0.9.8/docs/protocol.txt
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/docs/tutorial/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      154 2014-06-01 21:01:35.000000 dulwich-0.9.8/docs/tutorial/Makefile
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      322 2014-11-30 17:27:02.000000 dulwich-0.9.8/docs/tutorial/conclusion.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2963 2014-06-08 21:51:22.000000 dulwich-0.9.8/docs/tutorial/repo.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     6005 2014-06-01 21:01:35.000000 dulwich-0.9.8/docs/tutorial/object-store.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2988 2014-06-01 21:01:35.000000 dulwich-0.9.8/docs/tutorial/remote.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1762 2014-06-01 21:01:35.000000 dulwich-0.9.8/docs/tutorial/tag.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      648 2014-06-01 21:01:35.000000 dulwich-0.9.8/docs/tutorial/introduction.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      160 2014-06-01 21:01:35.000000 dulwich-0.9.8/docs/tutorial/index.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3069 2014-06-01 21:01:35.000000 dulwich-0.9.8/docs/tutorial/file-format.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3302 2014-06-01 21:01:35.000000 dulwich-0.9.8/docs/Makefile
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3268 2014-06-01 21:01:35.000000 dulwich-0.9.8/docs/make.bat
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      420 2014-06-01 21:01:35.000000 dulwich-0.9.8/docs/index.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    30771 2014-11-30 17:27:16.000000 dulwich-0.9.8/NEWS
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    17987 2014-06-01 21:01:35.000000 dulwich-0.9.8/COPYING
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/bin/
--rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)     1043 2014-11-30 17:27:02.000000 dulwich-0.9.8/bin/dul-receive-pack
--rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)     1039 2014-11-30 17:27:02.000000 dulwich-0.9.8/bin/dul-upload-pack
--rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)    10298 2014-11-30 17:27:02.000000 dulwich-0.9.8/bin/dulwich
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       59 2014-11-30 17:27:45.000000 dulwich-0.9.8/setup.cfg
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     6311 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_file.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     9269 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_config.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2069 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_objectspec.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2419 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_blackbox.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    11453 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/utils.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    21819 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_client.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3765 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_hooks.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    39765 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_objects.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    10788 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_protocol.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    11996 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_index.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    38545 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_pack.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     4833 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_greenthreads.py
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/compat/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     9995 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/compat/server_utils.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     8163 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/compat/utils.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    17849 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/compat/test_client.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     6318 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/compat/test_pack.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     4291 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/compat/test_repository.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     4899 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/compat/test_web.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3270 2014-06-08 21:51:22.000000 dulwich-0.9.8/dulwich/tests/compat/test_server.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3422 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/compat/test_utils.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1271 2013-09-22 20:27:01.000000 dulwich-0.9.8/dulwich/tests/compat/__init__.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    40074 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_diff_tree.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    28927 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_repository.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    19091 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_refs.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    16109 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_lru_cache.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     8190 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_missing_obj_finder.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     7734 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_fastexport.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    26366 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_porcelain.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    16191 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_object_store.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    18398 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_web.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    17492 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_walk.py
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/tests/data/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/indexes/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      104 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/indexes/index
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/tests/data/trees/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/trees/70/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       71 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/trees/70/c190eb48fa8bbb50ddc692a17b44cb781af7f6
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/tests/data/commits/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/commits/0d/
--rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)      132 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/commits/0d/89f20333fbb1d2f3a94da77f4981373d8f4310
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/commits/5d/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      194 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/commits/5d/ac377bdded4c9aeb8dff595f0faeebcc8498cc
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/commits/60/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      163 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/commits/60/dacdc733de308bb77bb76ce0fb0f9b44c9769e
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/tests/data/tags/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/tags/71/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      289 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/tags/71/033db03a03c6a36721efcf1968dd8f8e0cf023
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/tests/data/blobs/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/blobs/11/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       62 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/blobs/11/11111111111111111111111111111111111111
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/blobs/6f/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       16 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/blobs/6f/670c0fb53f9463760b7295fbb814e965fb20c8
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/blobs/e6/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       15 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/blobs/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/blobs/95/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/blobs/95/4a536f7819d40e6f637f849ee187dd10066349
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/packs/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      214 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/packs/pack-bc63ddad95e7321ee734ea11a7a62d314e0d7481.pack
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1136 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/packs/pack-bc63ddad95e7321ee734ea11a7a62d314e0d7481.idx
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       23 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/HEAD
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/a2/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/a2/96d0bb611188cabb256919f36bc30117cca005
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/ff/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       96 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/ff/d47d45845a8f6576491e1edb97e3fe6a850e7f
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/4f/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/4f/2e6529203aa6d44b5af6e3292c837ceda003f9
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/4e/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/4e/f30bbfe26431a69c3820d3a683df54d688f2ec
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/2a/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      133 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/2a/72d929692c41d8554c07f6301757ba18a65d91
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/28/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      136 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/28/237f4dc30d0d462658d6b937b08a0f0b6ef55a
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/7d/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       71 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/7d/9a07d797595ef11344549b8d08198e48c15364
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/a9/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      161 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/a9/0fa2d900a17e99b433217e988c4eb4a2e9a097
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/b0/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      145 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/objects/b0/931cadc54336e78a1d980420e3268903b57a50
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      132 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/packed-refs
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/refs/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/refs/heads/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       41 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/refs/heads/master
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/refs/tags/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       41 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/a.git/refs/tags/mytag
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/empty.git/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       23 2013-10-23 23:39:14.000000 dulwich-0.9.8/dulwich/tests/data/repos/empty.git/HEAD
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/tests/data/repos/empty.git/objects/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/empty.git/objects/info/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       13 2013-10-23 23:39:14.000000 dulwich-0.9.8/dulwich/tests/data/repos/empty.git/objects/info/.gitignore
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/empty.git/objects/pack/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       13 2013-10-23 23:39:14.000000 dulwich-0.9.8/dulwich/tests/data/repos/empty.git/objects/pack/.gitignore
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      131 2013-10-23 23:39:14.000000 dulwich-0.9.8/dulwich/tests/data/repos/empty.git/config
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/tests/data/repos/empty.git/refs/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/empty.git/refs/heads/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       13 2013-10-23 23:39:14.000000 dulwich-0.9.8/dulwich/tests/data/repos/empty.git/refs/heads/.gitignore
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/empty.git/refs/tags/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       13 2013-10-23 23:39:14.000000 dulwich-0.9.8/dulwich/tests/data/repos/empty.git/refs/tags/.gitignore
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       23 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/HEAD
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/objects/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/objects/a1/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       29 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/objects/a1/8114c31713746a33a2e70d9914d1ef3e781425
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/objects/3b/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       48 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/objects/3b/9e5457140e738c2dcd39bf6d7acf88379b90d1
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/objects/cd/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      155 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/objects/cd/a609072918d7b70057b6bef9f4c2537843fcfe
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/objects/df/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      134 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/objects/df/6800012397fb85c56e7418dd4eb9405dee075c
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/objects/3e/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      150 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/objects/3e/c9c43c84ff242e3ef4a9fc5bc111fd780a76a8
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/objects/42/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      129 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/objects/42/d06bd4b77fed026b154d16493e5deab78f02ec
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      187 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/packed-refs
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/refs/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/refs/heads/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       41 2013-11-30 23:57:17.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/refs/heads/40-char-ref-aaaaaaaaaaaaaaaaaa
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       41 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/refs/heads/master
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       21 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/refs/heads/loop
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/refs/tags/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       41 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/refs.git/refs/tags/refs-0.2
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       23 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/HEAD
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/0d/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      132 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/0d/89f20333fbb1d2f3a94da77f4981373d8f4310
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/70/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       71 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/70/c190eb48fa8bbb50ddc692a17b44cb781af7f6
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/d8/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      102 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/d8/0c186a03f423a81b39df39dc87fd269736ca86
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/29/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       16 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/29/69be3e8ee1c0222396a5611407e4769f14e54b
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/ab/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      167 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/ab/64bbdcc51b170d21588e5c5d391ee5c0c96dfd
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/5d/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      194 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/5d/ac377bdded4c9aeb8dff595f0faeebcc8498cc
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/d4/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       96 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/d4/bdad6549dfedf25d3b89d21f506aff575b28a7
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/60/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      163 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/60/dacdc733de308bb77bb76ce0fb0f9b44c9769e
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/6f/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       16 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/6f/670c0fb53f9463760b7295fbb814e965fb20c8
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/90/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       95 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/90/182552c4a85a45ec2a835cadc3451bebdfe870
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/1b/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       96 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/1b/6318f651a534b38f9c7aedeebbd56c1e896853
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/e6/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       15 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/4c/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      167 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/4c/ffe90e0a41ad3f5190079d7c8f036bde29cbe6
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/95/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/objects/95/4a536f7819d40e6f637f849ee187dd10066349
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/refs/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/refs/heads/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       41 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/simple_merge.git/refs/heads/master
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      901 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/server_old.export
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       23 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/HEAD
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/76/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      195 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/76/01d7f6231db6a57f7bbb79ee52e4d462fd44d1
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/b2/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       46 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/b2/a2766a2879c209ab1176e7e778b81ae422eeaa
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/70/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       71 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/70/c190eb48fa8bbb50ddc692a17b44cb781af7f6
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/f9/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      131 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/f9/e39b120c68182a4ba35349f832d0e4e61f485c
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/29/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/29/69be3e8ee1c0222396a5611407e4769f14e54b
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/6f/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/6f/670c0fb53f9463760b7295fbb814e965fb20c8
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/fb/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      165 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/fb/5b0425c7ce46959bec94d54b9a157645e114f5
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/90/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       95 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/90/182552c4a85a45ec2a835cadc3451bebdfe870
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/38/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       70 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/38/74e9c60a6d149c44c928140f250d81e6381520
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/f5/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      166 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/f5/07291b64138b875c28e03469025b1ea20bc614
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/95/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/objects/95/4a536f7819d40e6f637f849ee187dd10066349
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/refs/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/refs/heads/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       41 2013-10-23 22:42:34.000000 dulwich-0.9.8/dulwich/tests/data/repos/ooo_merge.git/refs/heads/master
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1673 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/server_new.export
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:45.000000 dulwich-0.9.8/dulwich/tests/data/repos/submodule/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       16 2013-09-22 20:30:40.000000 dulwich-0.9.8/dulwich/tests/data/repos/submodule/dotgit
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       16 2014-06-08 21:51:22.000000 dulwich-0.9.8/dulwich/tests/data/repos/.gitattributes
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    17837 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_patch.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    30126 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_server.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3283 2014-05-24 14:16:07.000000 dulwich-0.9.8/dulwich/tests/test_utils.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     6440 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/test_grafts.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     5690 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/tests/__init__.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    27791 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/_compat.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     8104 2014-06-08 21:51:22.000000 dulwich-0.9.8/dulwich/fastexport.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     5108 2013-11-30 23:57:17.000000 dulwich-0.9.8/dulwich/errors.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    32652 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/repo.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     5863 2014-06-08 21:51:22.000000 dulwich-0.9.8/dulwich/file.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    64984 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/pack.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    12221 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/config.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    10657 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/_diff_tree.c
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich/contrib/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    34937 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/contrib/swift.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    24333 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/contrib/test_swift.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    12982 2014-06-08 21:51:22.000000 dulwich-0.9.8/dulwich/contrib/test_swift_smoke.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1056 2014-06-08 21:51:22.000000 dulwich-0.9.8/dulwich/contrib/__init__.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    36748 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/object_store.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    25087 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/refs.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2423 2013-09-22 20:27:01.000000 dulwich-0.9.8/dulwich/log_utils.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    42608 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/objects.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    17172 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/web.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    14319 2014-06-08 21:51:22.000000 dulwich-0.9.8/dulwich/lru_cache.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     7657 2014-06-08 21:51:22.000000 dulwich-0.9.8/dulwich/_objects.c
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     9370 2014-05-24 14:16:07.000000 dulwich-0.9.8/dulwich/patch.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     4748 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/hooks.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     4959 2014-06-08 21:51:22.000000 dulwich-0.9.8/dulwich/greenthreads.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      385 2013-11-30 16:20:54.000000 dulwich-0.9.8/dulwich/stdint.h
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    33114 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/server.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    15320 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/index.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     5667 2013-09-22 20:27:01.000000 dulwich-0.9.8/dulwich/_pack.c
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    15037 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/protocol.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    22133 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/porcelain.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    13974 2014-06-08 21:51:22.000000 dulwich-0.9.8/dulwich/walk.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    41727 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/client.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    22135 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/diff_tree.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      974 2014-11-30 17:27:02.000000 dulwich-0.9.8/dulwich/__init__.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1535 2014-02-26 00:21:51.000000 dulwich-0.9.8/dulwich/objectspec.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      387 2014-11-30 17:27:02.000000 dulwich-0.9.8/AUTHORS
--rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)     3559 2014-11-30 17:27:02.000000 dulwich-0.9.8/setup.py
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich.egg-info/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1019 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich.egg-info/PKG-INFO
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)        8 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich.egg-info/top_level.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     7917 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich.egg-info/SOURCES.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)        1 2014-11-30 17:27:44.000000 dulwich-0.9.8/dulwich.egg-info/dependency_links.txt
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1152 2015-03-22 00:13:56.000000 dulwich-0.9.9/README.md
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/examples/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      273 2015-03-18 01:06:13.000000 dulwich-0.9.9/examples/config.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      867 2015-03-18 01:06:13.000000 dulwich-0.9.9/examples/clone.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      531 2015-03-18 01:06:13.000000 dulwich-0.9.9/examples/latest_change.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      490 2015-03-18 01:06:13.000000 dulwich-0.9.9/examples/diff.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1092 2015-03-22 00:13:56.000000 dulwich-0.9.9/HACKING
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      233 2015-03-18 01:06:13.000000 dulwich-0.9.9/MANIFEST.in
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1019 2015-03-22 00:16:16.000000 dulwich-0.9.9/PKG-INFO
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1132 2015-03-18 01:06:13.000000 dulwich-0.9.9/Makefile
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/docs/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     6949 2015-03-18 01:06:13.000000 dulwich-0.9.9/docs/conf.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      283 2014-06-01 21:01:35.000000 dulwich-0.9.9/docs/performance.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2274 2014-06-01 21:01:35.000000 dulwich-0.9.9/docs/protocol.txt
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/docs/tutorial/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      154 2014-06-01 21:01:35.000000 dulwich-0.9.9/docs/tutorial/Makefile
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      322 2015-03-18 01:06:13.000000 dulwich-0.9.9/docs/tutorial/conclusion.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2963 2015-03-18 01:06:13.000000 dulwich-0.9.9/docs/tutorial/repo.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     6005 2014-06-01 21:01:35.000000 dulwich-0.9.9/docs/tutorial/object-store.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2988 2015-03-18 01:06:13.000000 dulwich-0.9.9/docs/tutorial/remote.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1762 2015-03-18 01:06:13.000000 dulwich-0.9.9/docs/tutorial/tag.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      648 2015-03-18 01:06:13.000000 dulwich-0.9.9/docs/tutorial/introduction.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      160 2015-03-18 01:06:13.000000 dulwich-0.9.9/docs/tutorial/index.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3069 2015-03-18 01:06:13.000000 dulwich-0.9.9/docs/tutorial/file-format.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3302 2014-06-01 21:01:35.000000 dulwich-0.9.9/docs/Makefile
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3268 2014-06-01 21:01:35.000000 dulwich-0.9.9/docs/make.bat
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      420 2014-06-01 21:01:35.000000 dulwich-0.9.9/docs/index.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    31006 2015-03-22 00:13:56.000000 dulwich-0.9.9/NEWS
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    17987 2014-06-01 21:01:35.000000 dulwich-0.9.9/COPYING
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/bin/
+-rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)     1043 2015-03-18 01:06:13.000000 dulwich-0.9.9/bin/dul-receive-pack
+-rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)     1039 2015-03-18 01:06:13.000000 dulwich-0.9.9/bin/dul-upload-pack
+-rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)    10298 2015-03-18 01:06:13.000000 dulwich-0.9.9/bin/dulwich
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       59 2015-03-22 00:16:16.000000 dulwich-0.9.9/setup.cfg
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     6311 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/test_file.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     9269 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/test_config.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2069 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/test_objectspec.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2419 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/test_blackbox.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    11453 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/utils.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    21819 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/test_client.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3765 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/test_hooks.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    39765 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/test_objects.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    10788 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/test_protocol.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    11996 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/test_index.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    38823 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/test_pack.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     4833 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/test_greenthreads.py
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/compat/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     9995 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/compat/server_utils.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     8163 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/compat/utils.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    17849 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/compat/test_client.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     6318 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/compat/test_pack.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     4291 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/compat/test_repository.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     4899 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/compat/test_web.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3270 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/compat/test_server.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3422 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/compat/test_utils.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1271 2013-09-22 20:27:01.000000 dulwich-0.9.9/dulwich/tests/compat/__init__.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    40074 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/test_diff_tree.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    28927 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/test_repository.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    19091 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/test_refs.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    16109 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/test_lru_cache.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     8190 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/test_missing_obj_finder.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     7734 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/test_fastexport.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    26366 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/test_porcelain.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    16191 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/test_object_store.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    18398 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/test_web.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    17492 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/test_walk.py
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/indexes/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      104 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/indexes/index
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/trees/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/trees/70/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       71 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/trees/70/c190eb48fa8bbb50ddc692a17b44cb781af7f6
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/commits/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/commits/0d/
+-rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)      132 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/commits/0d/89f20333fbb1d2f3a94da77f4981373d8f4310
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/commits/5d/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      194 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/commits/5d/ac377bdded4c9aeb8dff595f0faeebcc8498cc
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/commits/60/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      163 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/commits/60/dacdc733de308bb77bb76ce0fb0f9b44c9769e
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/tags/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/tags/71/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      289 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/tags/71/033db03a03c6a36721efcf1968dd8f8e0cf023
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/blobs/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/blobs/11/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       62 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/blobs/11/11111111111111111111111111111111111111
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/blobs/6f/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       16 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/blobs/6f/670c0fb53f9463760b7295fbb814e965fb20c8
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/blobs/e6/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       15 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/blobs/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/blobs/95/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/blobs/95/4a536f7819d40e6f637f849ee187dd10066349
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/packs/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      214 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/packs/pack-bc63ddad95e7321ee734ea11a7a62d314e0d7481.pack
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1136 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/packs/pack-bc63ddad95e7321ee734ea11a7a62d314e0d7481.idx
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       23 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/HEAD
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/a2/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/a2/96d0bb611188cabb256919f36bc30117cca005
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/ff/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       96 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/ff/d47d45845a8f6576491e1edb97e3fe6a850e7f
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/4f/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/4f/2e6529203aa6d44b5af6e3292c837ceda003f9
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/4e/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/4e/f30bbfe26431a69c3820d3a683df54d688f2ec
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/2a/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      133 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/2a/72d929692c41d8554c07f6301757ba18a65d91
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/28/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      136 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/28/237f4dc30d0d462658d6b937b08a0f0b6ef55a
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/7d/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       71 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/7d/9a07d797595ef11344549b8d08198e48c15364
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/a9/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      161 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/a9/0fa2d900a17e99b433217e988c4eb4a2e9a097
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/b0/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      145 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/objects/b0/931cadc54336e78a1d980420e3268903b57a50
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      132 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/packed-refs
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/refs/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/refs/heads/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       41 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/refs/heads/master
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/refs/tags/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       41 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/a.git/refs/tags/mytag
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/empty.git/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       23 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/data/repos/empty.git/HEAD
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/empty.git/objects/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/empty.git/objects/info/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       13 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/data/repos/empty.git/objects/info/.gitignore
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/empty.git/objects/pack/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       13 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/data/repos/empty.git/objects/pack/.gitignore
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      131 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/data/repos/empty.git/config
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/empty.git/refs/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/empty.git/refs/heads/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       13 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/data/repos/empty.git/refs/heads/.gitignore
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/empty.git/refs/tags/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       13 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/data/repos/empty.git/refs/tags/.gitignore
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       23 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/HEAD
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/objects/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/objects/a1/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       29 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/objects/a1/8114c31713746a33a2e70d9914d1ef3e781425
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/objects/3b/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       48 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/objects/3b/9e5457140e738c2dcd39bf6d7acf88379b90d1
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/objects/cd/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      155 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/objects/cd/a609072918d7b70057b6bef9f4c2537843fcfe
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/objects/df/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      134 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/objects/df/6800012397fb85c56e7418dd4eb9405dee075c
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/objects/3e/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      150 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/objects/3e/c9c43c84ff242e3ef4a9fc5bc111fd780a76a8
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/objects/42/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      129 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/objects/42/d06bd4b77fed026b154d16493e5deab78f02ec
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      187 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/packed-refs
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/refs/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/refs/heads/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       41 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/refs/heads/40-char-ref-aaaaaaaaaaaaaaaaaa
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       41 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/refs/heads/master
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       21 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/refs/heads/loop
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/refs/tags/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       41 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/refs.git/refs/tags/refs-0.2
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       23 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/HEAD
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/0d/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      132 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/0d/89f20333fbb1d2f3a94da77f4981373d8f4310
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/70/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       71 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/70/c190eb48fa8bbb50ddc692a17b44cb781af7f6
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/d8/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      102 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/d8/0c186a03f423a81b39df39dc87fd269736ca86
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/29/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       16 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/29/69be3e8ee1c0222396a5611407e4769f14e54b
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/ab/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      167 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/ab/64bbdcc51b170d21588e5c5d391ee5c0c96dfd
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/5d/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      194 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/5d/ac377bdded4c9aeb8dff595f0faeebcc8498cc
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/d4/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       96 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/d4/bdad6549dfedf25d3b89d21f506aff575b28a7
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/60/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      163 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/60/dacdc733de308bb77bb76ce0fb0f9b44c9769e
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/6f/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       16 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/6f/670c0fb53f9463760b7295fbb814e965fb20c8
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/90/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       95 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/90/182552c4a85a45ec2a835cadc3451bebdfe870
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/1b/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       96 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/1b/6318f651a534b38f9c7aedeebbd56c1e896853
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/e6/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       15 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/4c/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      167 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/4c/ffe90e0a41ad3f5190079d7c8f036bde29cbe6
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/95/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/objects/95/4a536f7819d40e6f637f849ee187dd10066349
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/refs/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/refs/heads/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       41 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/simple_merge.git/refs/heads/master
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      901 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/server_old.export
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       23 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/HEAD
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/76/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      195 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/76/01d7f6231db6a57f7bbb79ee52e4d462fd44d1
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/b2/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       46 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/b2/a2766a2879c209ab1176e7e778b81ae422eeaa
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/70/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       71 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/70/c190eb48fa8bbb50ddc692a17b44cb781af7f6
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/f9/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      131 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/f9/e39b120c68182a4ba35349f832d0e4e61f485c
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/29/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/29/69be3e8ee1c0222396a5611407e4769f14e54b
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/6f/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/6f/670c0fb53f9463760b7295fbb814e965fb20c8
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/fb/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      165 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/fb/5b0425c7ce46959bec94d54b9a157645e114f5
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/90/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       95 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/90/182552c4a85a45ec2a835cadc3451bebdfe870
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/38/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       70 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/38/74e9c60a6d149c44c928140f250d81e6381520
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/f5/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      166 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/f5/07291b64138b875c28e03469025b1ea20bc614
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/95/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       22 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/objects/95/4a536f7819d40e6f637f849ee187dd10066349
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/refs/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/refs/heads/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       41 2013-10-23 22:42:34.000000 dulwich-0.9.9/dulwich/tests/data/repos/ooo_merge.git/refs/heads/master
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1673 2013-09-22 20:30:40.000000 dulwich-0.9.9/dulwich/tests/data/repos/server_new.export
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/tests/data/repos/submodule/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       16 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/data/repos/submodule/dotgit
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       16 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/data/repos/.gitattributes
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    17837 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/test_patch.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    30126 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/test_server.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3283 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/test_utils.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     6440 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/tests/test_grafts.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     5690 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/tests/__init__.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    27791 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/_compat.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     8104 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/fastexport.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     5108 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/errors.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    32652 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/repo.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     5863 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/file.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    64984 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/pack.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    12221 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/config.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    10657 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/_diff_tree.c
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich/contrib/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    34937 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/contrib/swift.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    24333 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/contrib/test_swift.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    12982 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/contrib/test_swift_smoke.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1056 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/contrib/__init__.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    36748 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/object_store.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    25087 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/refs.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2423 2013-09-22 20:27:01.000000 dulwich-0.9.9/dulwich/log_utils.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    42608 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/objects.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    17172 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/web.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    14319 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/lru_cache.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     7657 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/_objects.c
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     9370 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/patch.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     4748 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/hooks.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     4959 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/greenthreads.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      385 2013-11-30 16:20:54.000000 dulwich-0.9.9/dulwich/stdint.h
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    33114 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/server.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    15320 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/index.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     5741 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/_pack.c
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    15037 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/protocol.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    22133 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/porcelain.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    13974 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/walk.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    41727 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/client.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    22135 2015-03-22 00:13:56.000000 dulwich-0.9.9/dulwich/diff_tree.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      974 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/__init__.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1535 2015-03-18 01:06:13.000000 dulwich-0.9.9/dulwich/objectspec.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      387 2015-03-18 01:06:13.000000 dulwich-0.9.9/AUTHORS
+-rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)     3559 2015-03-22 00:13:56.000000 dulwich-0.9.9/setup.py
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2015-03-22 00:16:16.000000 dulwich-0.9.9/dulwich.egg-info/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1019 2015-03-22 00:16:15.000000 dulwich-0.9.9/dulwich.egg-info/PKG-INFO
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)        8 2015-03-22 00:16:15.000000 dulwich-0.9.9/dulwich.egg-info/top_level.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     7917 2015-03-22 00:16:15.000000 dulwich-0.9.9/dulwich.egg-info/SOURCES.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)        1 2015-03-22 00:16:15.000000 dulwich-0.9.9/dulwich.egg-info/dependency_links.txt
```

### Comparing `dulwich-0.9.8/README.md` & `dulwich-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/examples/clone.py` & `dulwich-0.9.9/examples/clone.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/examples/latest_change.py` & `dulwich-0.9.9/examples/latest_change.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/HACKING` & `dulwich-0.9.9/HACKING`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/PKG-INFO` & `dulwich-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dulwich
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python Git Library
 Home-page: https://samba.org/~jelmer/dulwich
 Author: Jelmer Vernooij
 Author-email: jelmer@samba.org
 License: GPLv2 or later
 Description: 
               Python implementation of the Git file formats and protocols,
```

### Comparing `dulwich-0.9.8/Makefile` & `dulwich-0.9.9/Makefile`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/docs/conf.py` & `dulwich-0.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/docs/protocol.txt` & `dulwich-0.9.9/docs/protocol.txt`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/docs/tutorial/repo.txt` & `dulwich-0.9.9/docs/tutorial/repo.txt`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/docs/tutorial/object-store.txt` & `dulwich-0.9.9/docs/tutorial/object-store.txt`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/docs/tutorial/remote.txt` & `dulwich-0.9.9/docs/tutorial/remote.txt`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/docs/tutorial/tag.txt` & `dulwich-0.9.9/docs/tutorial/tag.txt`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/docs/tutorial/introduction.txt` & `dulwich-0.9.9/docs/tutorial/introduction.txt`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/docs/tutorial/file-format.txt` & `dulwich-0.9.9/docs/tutorial/file-format.txt`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/docs/Makefile` & `dulwich-0.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/docs/make.bat` & `dulwich-0.9.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/NEWS` & `dulwich-0.9.9/NEWS`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+0.9.9	2015-03-20
+
+ SECURITY BUG FIXES
+
+  * Fix buffer overflow in C implementation of pack apply_delta().
+    (CVE-2015-0838)
+
+    Thanks to Ivan Fratric of the Google Security Team for
+    reporting this issue.
+    (Jelmer Vernooij)
+
 0.9.8	2014-11-30
 
  BUG FIXES
 
   * Various fixes to improve test suite running on Windows.
     (Gary van der Merwe)
```

### Comparing `dulwich-0.9.8/COPYING` & `dulwich-0.9.9/COPYING`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/bin/dul-receive-pack` & `dulwich-0.9.9/bin/dul-receive-pack`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/bin/dul-upload-pack` & `dulwich-0.9.9/bin/dul-upload-pack`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/bin/dulwich` & `dulwich-0.9.9/bin/dulwich`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_file.py` & `dulwich-0.9.9/dulwich/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_config.py` & `dulwich-0.9.9/dulwich/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_objectspec.py` & `dulwich-0.9.9/dulwich/tests/test_objectspec.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_blackbox.py` & `dulwich-0.9.9/dulwich/tests/test_blackbox.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/utils.py` & `dulwich-0.9.9/dulwich/tests/utils.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_client.py` & `dulwich-0.9.9/dulwich/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_hooks.py` & `dulwich-0.9.9/dulwich/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_objects.py` & `dulwich-0.9.9/dulwich/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_protocol.py` & `dulwich-0.9.9/dulwich/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_index.py` & `dulwich-0.9.9/dulwich/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_pack.py` & `dulwich-0.9.9/dulwich/tests/test_pack.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,22 @@
     def test_empty_to_huge(self):
         self._test_roundtrip(self.test_string_empty, self.test_string_huge)
 
     def test_huge_copy(self):
         self._test_roundtrip(self.test_string_huge + self.test_string1,
                              self.test_string_huge + self.test_string2)
 
+    def test_dest_overflow(self):
+        self.assertRaises(
+            ValueError,
+            apply_delta, 'a'*0x10000, '\x80\x80\x04\x80\x80\x04\x80' + 'a'*0x10000)
+        self.assertRaises(
+            ValueError,
+            apply_delta, '', '\x00\x80\x02\xb0\x11\x11')
+
 
 @skipIfPY3
 class TestPackData(PackTests):
     """Tests getting the data from the packfile."""
 
     def test_create_pack(self):
         self.get_pack_data(pack1_sha).close()
```

### Comparing `dulwich-0.9.8/dulwich/tests/test_greenthreads.py` & `dulwich-0.9.9/dulwich/tests/test_greenthreads.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/compat/server_utils.py` & `dulwich-0.9.9/dulwich/tests/compat/server_utils.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/compat/utils.py` & `dulwich-0.9.9/dulwich/tests/compat/utils.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/compat/test_client.py` & `dulwich-0.9.9/dulwich/tests/compat/test_client.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/compat/test_pack.py` & `dulwich-0.9.9/dulwich/tests/compat/test_pack.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/compat/test_repository.py` & `dulwich-0.9.9/dulwich/tests/compat/test_repository.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/compat/test_web.py` & `dulwich-0.9.9/dulwich/tests/compat/test_web.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/compat/test_server.py` & `dulwich-0.9.9/dulwich/tests/compat/test_server.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/compat/test_utils.py` & `dulwich-0.9.9/dulwich/tests/compat/test_utils.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/compat/__init__.py` & `dulwich-0.9.9/dulwich/tests/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_diff_tree.py` & `dulwich-0.9.9/dulwich/tests/test_diff_tree.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_repository.py` & `dulwich-0.9.9/dulwich/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_refs.py` & `dulwich-0.9.9/dulwich/tests/test_refs.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_lru_cache.py` & `dulwich-0.9.9/dulwich/tests/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_missing_obj_finder.py` & `dulwich-0.9.9/dulwich/tests/test_missing_obj_finder.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_fastexport.py` & `dulwich-0.9.9/dulwich/tests/test_fastexport.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_porcelain.py` & `dulwich-0.9.9/dulwich/tests/test_porcelain.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_object_store.py` & `dulwich-0.9.9/dulwich/tests/test_object_store.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_web.py` & `dulwich-0.9.9/dulwich/tests/test_web.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_walk.py` & `dulwich-0.9.9/dulwich/tests/test_walk.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/data/packs/pack-bc63ddad95e7321ee734ea11a7a62d314e0d7481.idx` & `dulwich-0.9.9/dulwich/tests/data/packs/pack-bc63ddad95e7321ee734ea11a7a62d314e0d7481.idx`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/data/repos/server_old.export` & `dulwich-0.9.9/dulwich/tests/data/repos/server_old.export`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/data/repos/server_new.export` & `dulwich-0.9.9/dulwich/tests/data/repos/server_new.export`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_patch.py` & `dulwich-0.9.9/dulwich/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_server.py` & `dulwich-0.9.9/dulwich/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_utils.py` & `dulwich-0.9.9/dulwich/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/test_grafts.py` & `dulwich-0.9.9/dulwich/tests/test_grafts.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/tests/__init__.py` & `dulwich-0.9.9/dulwich/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/_compat.py` & `dulwich-0.9.9/dulwich/_compat.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/fastexport.py` & `dulwich-0.9.9/dulwich/fastexport.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/errors.py` & `dulwich-0.9.9/dulwich/errors.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/repo.py` & `dulwich-0.9.9/dulwich/repo.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/file.py` & `dulwich-0.9.9/dulwich/file.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/pack.py` & `dulwich-0.9.9/dulwich/pack.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/config.py` & `dulwich-0.9.9/dulwich/config.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/_diff_tree.c` & `dulwich-0.9.9/dulwich/_diff_tree.c`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/contrib/swift.py` & `dulwich-0.9.9/dulwich/contrib/swift.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/contrib/test_swift.py` & `dulwich-0.9.9/dulwich/contrib/test_swift.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/contrib/test_swift_smoke.py` & `dulwich-0.9.9/dulwich/contrib/test_swift_smoke.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/contrib/__init__.py` & `dulwich-0.9.9/dulwich/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/object_store.py` & `dulwich-0.9.9/dulwich/object_store.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/refs.py` & `dulwich-0.9.9/dulwich/refs.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/log_utils.py` & `dulwich-0.9.9/dulwich/log_utils.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/objects.py` & `dulwich-0.9.9/dulwich/objects.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/web.py` & `dulwich-0.9.9/dulwich/web.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/lru_cache.py` & `dulwich-0.9.9/dulwich/lru_cache.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/_objects.c` & `dulwich-0.9.9/dulwich/_objects.c`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/patch.py` & `dulwich-0.9.9/dulwich/patch.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/hooks.py` & `dulwich-0.9.9/dulwich/hooks.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/greenthreads.py` & `dulwich-0.9.9/dulwich/greenthreads.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/server.py` & `dulwich-0.9.9/dulwich/server.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/index.py` & `dulwich-0.9.9/dulwich/index.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/_pack.c` & `dulwich-0.9.9/dulwich/_pack.c`

 * *Files 2% similar despite different names*

```diff
@@ -142,18 +142,22 @@
 				cp_size = 0x10000;
 			if (cp_off + cp_size < cp_size ||
 				cp_off + cp_size > src_size ||
 				cp_size > dest_size)
 				break;
 			memcpy(out+outindex, src_buf+cp_off, cp_size);
 			outindex += cp_size;
+			dest_size -= cp_size;
 		} else if (cmd != 0) {
+			if (cmd > dest_size)
+				break;
 			memcpy(out+outindex, delta+index, cmd);
 			outindex += cmd;
 			index += cmd;
+			dest_size -= cmd;
 		} else {
 			PyErr_SetString(PyExc_ValueError, "Invalid opcode 0");
 			Py_DECREF(ret);
 			Py_DECREF(py_delta);
 			Py_DECREF(py_src_buf);
 			return NULL;
 		}
@@ -163,15 +167,15 @@
 
 	if (index != delta_len) {
 		PyErr_SetString(PyExc_ValueError, "delta not empty");
 		Py_DECREF(ret);
 		return NULL;
 	}
 
-	if (dest_size != outindex) {
+	if (dest_size != 0) {
 		PyErr_SetString(PyExc_ValueError, "dest size incorrect");
 		Py_DECREF(ret);
 		return NULL;
 	}
 
 	ret_list = Py_BuildValue("[N]", ret);
 	if (ret_list == NULL) {
```

### Comparing `dulwich-0.9.8/dulwich/protocol.py` & `dulwich-0.9.9/dulwich/protocol.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/porcelain.py` & `dulwich-0.9.9/dulwich/porcelain.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/walk.py` & `dulwich-0.9.9/dulwich/walk.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/client.py` & `dulwich-0.9.9/dulwich/client.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/diff_tree.py` & `dulwich-0.9.9/dulwich/diff_tree.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/dulwich/__init__.py` & `dulwich-0.9.9/dulwich/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 # MA  02110-1301, USA.
 
 
 """Python implementation of the Git file formats and protocols."""
 
-__version__ = (0, 9, 8)
+__version__ = (0, 9, 9)
```

### Comparing `dulwich-0.9.8/dulwich/objectspec.py` & `dulwich-0.9.9/dulwich/objectspec.py`

 * *Files identical despite different names*

### Comparing `dulwich-0.9.8/setup.py` & `dulwich-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 try:
     from setuptools import setup, Extension
 except ImportError:
     from distutils.core import setup, Extension
 from distutils.core import Distribution
 
-dulwich_version_string = '0.9.8'
+dulwich_version_string = '0.9.9'
 
 include_dirs = []
 # Windows MSVC support
 import os
 import sys
 if sys.platform == 'win32':
     include_dirs.append('dulwich')
```

### Comparing `dulwich-0.9.8/dulwich.egg-info/PKG-INFO` & `dulwich-0.9.9/dulwich.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dulwich
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python Git Library
 Home-page: https://samba.org/~jelmer/dulwich
 Author: Jelmer Vernooij
 Author-email: jelmer@samba.org
 License: GPLv2 or later
 Description: 
               Python implementation of the Git file formats and protocols,
```

### Comparing `dulwich-0.9.8/dulwich.egg-info/SOURCES.txt` & `dulwich-0.9.9/dulwich.egg-info/SOURCES.txt`

 * *Files identical despite different names*

