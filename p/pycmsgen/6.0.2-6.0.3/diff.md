# Comparing `tmp/pycmsgen-6.0.2.tar.gz` & `tmp/pycmsgen-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycmsgen-6.0.2.tar", last modified: Wed May  3 19:44:57 2023, max compression
+gzip compressed data, was "pycmsgen-6.0.3.tar", last modified: Wed May  3 23:11:18 2023, max compression
```

## Comparing `pycmsgen-6.0.2.tar` & `pycmsgen-6.0.3.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:57.676194 pycmsgen-6.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-03 19:44:57.676194 pycmsgen-6.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:57.652193 pycmsgen-6.0.2/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/python/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:57.652193 pycmsgen-6.0.2/python/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/python/src/GitSHA1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26826 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/python/src/pycmsgen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-03 19:44:57.676194 pycmsgen-6.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:57.672193 pycmsgen-6.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/GitSHA1.h
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/MersenneTwister.h
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/Vec.h
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/XAlloc.h
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/alg.h
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/avgcalc.h
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/bitarray.h
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/boundedqueue.h
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clabstraction.h
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clause.h
--rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clauseallocator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clauseallocator.h
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clausecleaner.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clausecleaner.h
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clauseusagestats.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clauseusagestats.h
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/cloffset.h
--rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/cmsgen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/cmsgen.h
--rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/cnf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/cnf.h
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/completedetachreattacher.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/completedetachreattacher.h
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/constants.h
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/cset.h
--rw-r--r--   0 runner    (1001) docker     (123)    15765 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/dimacsparser.h
--rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/distillerlong.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/distillerlong.h
--rw-r--r--   0 runner    (1001) docker     (123)    16705 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/distillerlongwithimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/distillerlongwithimpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/drat.h
--rw-r--r--   0 runner    (1001) docker     (123)    32702 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/gaussian.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/gaussian.h
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/gausswatched.h
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/gqueuedata.h
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/hasher.h
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/heap.h
--rw-r--r--   0 runner    (1001) docker     (123)    31093 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/hyperengine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/hyperengine.h
--rw-r--r--   0 runner    (1001) docker     (123)    19182 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/implcache.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/implcache.h
--rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/intree.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/intree.h
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/main.h
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/main_common.h
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/matrixfinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/matrixfinder.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:57.672193 pycmsgen-6.0.2/src/msvc/
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/msvc/stdint.h
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/mystack.h
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/nomutex.h
--rw-r--r--   0 runner    (1001) docker     (123)    95034 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/occsimplifier.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16439 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/occsimplifier.h
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/packedmatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/packedrow.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/packedrow.h
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/popcnt.h
--rw-r--r--   0 runner    (1001) docker     (123)    28904 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/prober.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/prober.h
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/propby.h
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/propby_backup.h
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/propbyforgraph.h
--rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/propengine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/propengine.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:57.676194 pycmsgen-6.0.2/src/pycmsgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-03 19:44:57.000000 pycmsgen-6.0.2/src/pycmsgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-03 19:44:57.000000 pycmsgen-6.0.2/src/pycmsgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/reducedb.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/reducedb.h
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/sccfinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/sccfinder.h
--rw-r--r--   0 runner    (1001) docker     (123)    83433 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/searcher.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/searcher.h
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/searchhist.h
--rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/searchstats.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/searchstats.h
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/shareddata.h
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/signalcode.h
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/simplefile.h
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solutionextender.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solutionextender.h
--rw-r--r--   0 runner    (1001) docker     (123)    95790 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19985 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solver.h
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solverconf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solverconf.h
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solvertypes.h
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solvertypesmini.h
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/stamp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/stamp.h
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/str_impl_w_impl_stamp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/str_impl_w_impl_stamp.h
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/streambuffer.h
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/subsumeimplicit.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/subsumeimplicit.h
--rw-r--r--   0 runner    (1001) docker     (123)    27861 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/subsumestrengthen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/subsumestrengthen.h
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/time_mem.h
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/touchlist.h
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/trim.h
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/vardata.h
--rw-r--r--   0 runner    (1001) docker     (123)    32001 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/varreplacer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/varreplacer.h
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/varupdatehelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/watchalgos.h
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/watcharray.h
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/watched.h
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/watched_backup.h
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/xor.h
--rw-r--r--   0 runner    (1001) docker     (123)    25049 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/xorfinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/xorfinder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:11:18.030215 pycmsgen-6.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-03 23:11:18.030215 pycmsgen-6.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:11:18.018216 pycmsgen-6.0.3/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/python/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:11:18.018216 pycmsgen-6.0.3/python/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/python/src/GitSHA1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26826 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/python/src/pycmsgen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-03 23:11:18.034215 pycmsgen-6.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:11:18.030215 pycmsgen-6.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/GitSHA1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/MersenneTwister.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/Vec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/XAlloc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/alg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/avgcalc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/bitarray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/boundedqueue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/clabstraction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/clause.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/clauseallocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/clauseallocator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/clausecleaner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/clausecleaner.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/clauseusagestats.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/clauseusagestats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/cloffset.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/cmsgen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/cmsgen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/cnf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/cnf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/completedetachreattacher.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/completedetachreattacher.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/cset.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15765 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/dimacsparser.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/distillerlong.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/distillerlong.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16705 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/distillerlongwithimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/distillerlongwithimpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/drat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32702 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/gaussian.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/gaussian.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/gausswatched.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/gqueuedata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/hasher.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/heap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31093 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/hyperengine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/hyperengine.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19182 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/implcache.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/implcache.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/intree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/intree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/main.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/main_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/matrixfinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/matrixfinder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:11:18.030215 pycmsgen-6.0.3/src/msvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/msvc/stdint.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/mystack.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/nomutex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    95034 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/occsimplifier.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16439 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/occsimplifier.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/packedmatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/packedrow.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/packedrow.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/popcnt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28904 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/prober.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/prober.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/propby.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/propby_backup.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/propbyforgraph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/propengine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/propengine.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:11:18.030215 pycmsgen-6.0.3/src/pycmsgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-03 23:11:18.000000 pycmsgen-6.0.3/src/pycmsgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-03 23:11:18.000000 pycmsgen-6.0.3/src/pycmsgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/reducedb.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/reducedb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/sccfinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/sccfinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    83433 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/searcher.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/searcher.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/searchhist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/searchstats.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/searchstats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/shareddata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/signalcode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/simplefile.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/solutionextender.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/solutionextender.h
+-rw-r--r--   0 runner    (1001) docker     (123)    95124 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19852 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/solver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/solverconf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/solverconf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/solvertypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/solvertypesmini.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/stamp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/stamp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/str_impl_w_impl_stamp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/str_impl_w_impl_stamp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/streambuffer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/subsumeimplicit.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/subsumeimplicit.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27861 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/subsumestrengthen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/subsumestrengthen.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/time_mem.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/touchlist.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/trim.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/vardata.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32001 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/varreplacer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/varreplacer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/varupdatehelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/watchalgos.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/watcharray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/watched.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/watched_backup.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/xor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25049 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/xorfinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-05-03 23:11:00.000000 pycmsgen-6.0.3/src/xorfinder.h
```

### Comparing `pycmsgen-6.0.2/LICENSE.txt` & `pycmsgen-6.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/PKG-INFO` & `pycmsgen-6.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycmsgen
-Version: 6.0.2
+Version: 6.0.3
 Summary: Bindings to CMSGen, uniform-like sampler
 Home-page: https://github.com/meelgroup/cmsgen
 Author-email: Mate Soos <soos.mate@gmail.com>
 Maintainer-email: Mate Soos <soos.mate@gmail.com>
 License: CryptoMiniSat Copyright (c) Mate Soos 2009-2018
         All rights reserved.
```

### Comparing `pycmsgen-6.0.2/pyproject.toml` & `pycmsgen-6.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "toml", "pathlib"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pycmsgen"
-version = "6.0.2"
+version = "6.0.3"
 description = "Bindings to CMSGen, uniform-like sampler"
 keywords = ["sat", "sampling"]
 license = { file = "LICENSE.txt" }
 maintainers = [{name="Mate Soos", email="soos.mate@gmail.com"}]
 authors = [{name="Mate Soos", email="soos.mate@gmail.com"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `pycmsgen-6.0.2/python/README.md` & `pycmsgen-6.0.3/python/README.md`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/python/src/GitSHA1.cpp` & `pycmsgen-6.0.3/python/src/GitSHA1.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/python/src/pycmsgen.cpp` & `pycmsgen-6.0.3/python/src/pycmsgen.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/setup.py` & `pycmsgen-6.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/GitSHA1.h` & `pycmsgen-6.0.3/src/GitSHA1.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/MersenneTwister.h` & `pycmsgen-6.0.3/src/MersenneTwister.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/Vec.h` & `pycmsgen-6.0.3/src/Vec.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/XAlloc.h` & `pycmsgen-6.0.3/src/XAlloc.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/alg.h` & `pycmsgen-6.0.3/src/alg.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/avgcalc.h` & `pycmsgen-6.0.3/src/avgcalc.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/bitarray.h` & `pycmsgen-6.0.3/src/bitarray.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/boundedqueue.h` & `pycmsgen-6.0.3/src/boundedqueue.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/clabstraction.h` & `pycmsgen-6.0.3/src/clabstraction.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/clause.h` & `pycmsgen-6.0.3/src/clause.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/clauseallocator.cpp` & `pycmsgen-6.0.3/src/clauseallocator.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/clauseallocator.h` & `pycmsgen-6.0.3/src/clauseallocator.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/clausecleaner.cpp` & `pycmsgen-6.0.3/src/clausecleaner.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/clausecleaner.h` & `pycmsgen-6.0.3/src/clausecleaner.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/clauseusagestats.cpp` & `pycmsgen-6.0.3/src/clauseusagestats.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/clauseusagestats.h` & `pycmsgen-6.0.3/src/clauseusagestats.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/cloffset.h` & `pycmsgen-6.0.3/src/cloffset.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/cmsgen.cpp` & `pycmsgen-6.0.3/src/cmsgen.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/cmsgen.h` & `pycmsgen-6.0.3/src/cmsgen.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/cnf.cpp` & `pycmsgen-6.0.3/src/cnf.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/cnf.h` & `pycmsgen-6.0.3/src/cnf.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/completedetachreattacher.cpp` & `pycmsgen-6.0.3/src/completedetachreattacher.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/completedetachreattacher.h` & `pycmsgen-6.0.3/src/completedetachreattacher.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/constants.h` & `pycmsgen-6.0.3/src/constants.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/cset.h` & `pycmsgen-6.0.3/src/cset.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/dimacsparser.h` & `pycmsgen-6.0.3/src/dimacsparser.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/distillerlong.cpp` & `pycmsgen-6.0.3/src/distillerlong.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/distillerlong.h` & `pycmsgen-6.0.3/src/distillerlong.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/distillerlongwithimpl.cpp` & `pycmsgen-6.0.3/src/distillerlongwithimpl.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/distillerlongwithimpl.h` & `pycmsgen-6.0.3/src/distillerlongwithimpl.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/drat.h` & `pycmsgen-6.0.3/src/drat.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/gaussian.cpp` & `pycmsgen-6.0.3/src/gaussian.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/gaussian.h` & `pycmsgen-6.0.3/src/gaussian.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/gausswatched.h` & `pycmsgen-6.0.3/src/gausswatched.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/gqueuedata.h` & `pycmsgen-6.0.3/src/gqueuedata.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/hasher.h` & `pycmsgen-6.0.3/src/hasher.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/heap.h` & `pycmsgen-6.0.3/src/heap.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/hyperengine.cpp` & `pycmsgen-6.0.3/src/hyperengine.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/hyperengine.h` & `pycmsgen-6.0.3/src/hyperengine.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/implcache.cpp` & `pycmsgen-6.0.3/src/implcache.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/implcache.h` & `pycmsgen-6.0.3/src/implcache.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/intree.cpp` & `pycmsgen-6.0.3/src/intree.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/intree.h` & `pycmsgen-6.0.3/src/intree.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/main.h` & `pycmsgen-6.0.3/src/main.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/main_common.h` & `pycmsgen-6.0.3/src/main_common.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/matrixfinder.cpp` & `pycmsgen-6.0.3/src/matrixfinder.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/matrixfinder.h` & `pycmsgen-6.0.3/src/matrixfinder.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/msvc/stdint.h` & `pycmsgen-6.0.3/src/msvc/stdint.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/mystack.h` & `pycmsgen-6.0.3/src/mystack.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/nomutex.h` & `pycmsgen-6.0.3/src/nomutex.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/occsimplifier.cpp` & `pycmsgen-6.0.3/src/occsimplifier.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/occsimplifier.h` & `pycmsgen-6.0.3/src/occsimplifier.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/packedmatrix.h` & `pycmsgen-6.0.3/src/packedmatrix.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/packedrow.cpp` & `pycmsgen-6.0.3/src/packedrow.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/packedrow.h` & `pycmsgen-6.0.3/src/packedrow.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/popcnt.h` & `pycmsgen-6.0.3/src/popcnt.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/prober.cpp` & `pycmsgen-6.0.3/src/prober.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/prober.h` & `pycmsgen-6.0.3/src/prober.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/propby.h` & `pycmsgen-6.0.3/src/propby.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/propby_backup.h` & `pycmsgen-6.0.3/src/propby_backup.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/propbyforgraph.h` & `pycmsgen-6.0.3/src/propbyforgraph.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/propengine.cpp` & `pycmsgen-6.0.3/src/propengine.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/propengine.h` & `pycmsgen-6.0.3/src/propengine.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/pycmsgen.egg-info/PKG-INFO` & `pycmsgen-6.0.3/src/pycmsgen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycmsgen
-Version: 6.0.2
+Version: 6.0.3
 Summary: Bindings to CMSGen, uniform-like sampler
 Home-page: https://github.com/meelgroup/cmsgen
 Author-email: Mate Soos <soos.mate@gmail.com>
 Maintainer-email: Mate Soos <soos.mate@gmail.com>
 License: CryptoMiniSat Copyright (c) Mate Soos 2009-2018
         All rights reserved.
```

### Comparing `pycmsgen-6.0.2/src/pycmsgen.egg-info/SOURCES.txt` & `pycmsgen-6.0.3/src/pycmsgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/reducedb.cpp` & `pycmsgen-6.0.3/src/reducedb.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/reducedb.h` & `pycmsgen-6.0.3/src/reducedb.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/sccfinder.cpp` & `pycmsgen-6.0.3/src/sccfinder.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/sccfinder.h` & `pycmsgen-6.0.3/src/sccfinder.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/searcher.cpp` & `pycmsgen-6.0.3/src/searcher.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/searcher.h` & `pycmsgen-6.0.3/src/searcher.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/searchhist.h` & `pycmsgen-6.0.3/src/searchhist.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/searchstats.cpp` & `pycmsgen-6.0.3/src/searchstats.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/searchstats.h` & `pycmsgen-6.0.3/src/searchstats.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/shareddata.h` & `pycmsgen-6.0.3/src/shareddata.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/signalcode.h` & `pycmsgen-6.0.3/src/signalcode.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/simplefile.h` & `pycmsgen-6.0.3/src/simplefile.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/solutionextender.cpp` & `pycmsgen-6.0.3/src/solutionextender.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/solutionextender.h` & `pycmsgen-6.0.3/src/solutionextender.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/solver.cpp` & `pycmsgen-6.0.3/src/solver.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -3217,47 +3217,21 @@
     }
     return false;
 }
 
 void Solver::set_var_weight(
 const Lit lit, const double weight
 ) {
-    //cout << "set weight called lit: " << lit << " w: " << weight << endl;
-    assert(lit.var() < nVars());
-    if (weights_given.size() < nVars()) {
-        weights_given.resize(nVars(), GivenW());
-    }
-
-    if ((weights_given[lit.var()].pos && !lit.sign())
-        || (weights_given[lit.var()].neg && lit.sign())
-    ) {
-        cout << "ERROR: Giving weights twice for literal: " << lit << endl;
+    if (lit.sign()) {
+        cout << "ERROR: only positive literals can have weights."
+            << " You gave weight '" << weight << " to literal: '" << (lit) << "'"
+            << "NOTE: A weight of 0.7 for '-2' is the same as the weight of 0.3 for '2'" << endl;
         exit(-1);
-        return;
-    }
-
-    if (!weights_given[lit.var()].neg && !lit.sign()) {
-        weights_given[lit.var()].pos = true;
-        varData[lit.var()].weight = weight;
-        return;
     }
-
-    if (!weights_given[lit.var()].pos && lit.sign()) {
-        weights_given[lit.var()].neg = true;
-        varData[lit.var()].weight = weight;
-        return;
-    }
-
-    if (!lit.sign()) {
-        //this is the pos
-        weights_given[lit.var()].pos = true;
-        double neg = varData[lit.var()].weight;
-        double pos = weight;
-        varData[lit.var()].weight = pos/(pos + neg);
-    } else {
-        //this is the neg
-        weights_given[lit.var()].neg = true;
-        double neg = weight;
-        double pos = varData[lit.var()].weight;
-        varData[lit.var()].weight = pos/(pos + neg);
+    if (weight < 0.0 || weight > 1.0) {
+        cout << "ERROR: Weight must be between 0 and 1"
+            << " You gave weight '" << weight << " to literal: '" << (lit) << "'"
+            << endl;
+        exit(-1);
     }
+    varData[lit.var()].weight = weight;
 }
```

### Comparing `pycmsgen-6.0.2/src/solver.h` & `pycmsgen-6.0.3/src/solver.h`

 * *Files 2% similar despite different names*

```diff
@@ -362,19 +362,14 @@
         bool verify_model_implicit_clauses() const;
         bool verify_model_long_clauses(const vector<ClOffset>& cs) const;
 
 
         /////////////////////
         // Data
         size_t               zeroLevAssignsByCNF = 0;
-        struct GivenW {
-            bool pos = false;
-            bool neg = false;
-        };
-        vector<GivenW> weights_given;
 
         /////////////////////
         // Clauses
         bool addClauseHelper(vector<Lit>& ps);
         bool addClauseInt(vector<Lit>& ps, const bool red = false);
```

### Comparing `pycmsgen-6.0.2/src/solverconf.cpp` & `pycmsgen-6.0.3/src/solverconf.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/solverconf.h` & `pycmsgen-6.0.3/src/solverconf.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/solvertypes.h` & `pycmsgen-6.0.3/src/solvertypes.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/solvertypesmini.h` & `pycmsgen-6.0.3/src/solvertypesmini.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/stamp.cpp` & `pycmsgen-6.0.3/src/stamp.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/stamp.h` & `pycmsgen-6.0.3/src/stamp.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/str_impl_w_impl_stamp.cpp` & `pycmsgen-6.0.3/src/str_impl_w_impl_stamp.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/str_impl_w_impl_stamp.h` & `pycmsgen-6.0.3/src/str_impl_w_impl_stamp.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/streambuffer.h` & `pycmsgen-6.0.3/src/streambuffer.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/subsumeimplicit.cpp` & `pycmsgen-6.0.3/src/subsumeimplicit.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/subsumeimplicit.h` & `pycmsgen-6.0.3/src/subsumeimplicit.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/subsumestrengthen.cpp` & `pycmsgen-6.0.3/src/subsumestrengthen.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/subsumestrengthen.h` & `pycmsgen-6.0.3/src/subsumestrengthen.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/time_mem.h` & `pycmsgen-6.0.3/src/time_mem.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/touchlist.h` & `pycmsgen-6.0.3/src/touchlist.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/trim.h` & `pycmsgen-6.0.3/src/trim.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/vardata.h` & `pycmsgen-6.0.3/src/vardata.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/varreplacer.cpp` & `pycmsgen-6.0.3/src/varreplacer.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/varreplacer.h` & `pycmsgen-6.0.3/src/varreplacer.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/varupdatehelper.h` & `pycmsgen-6.0.3/src/varupdatehelper.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/watchalgos.h` & `pycmsgen-6.0.3/src/watchalgos.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/watcharray.h` & `pycmsgen-6.0.3/src/watcharray.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/watched.h` & `pycmsgen-6.0.3/src/watched.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/watched_backup.h` & `pycmsgen-6.0.3/src/watched_backup.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/xor.h` & `pycmsgen-6.0.3/src/xor.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/xorfinder.cpp` & `pycmsgen-6.0.3/src/xorfinder.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.2/src/xorfinder.h` & `pycmsgen-6.0.3/src/xorfinder.h`

 * *Files identical despite different names*

