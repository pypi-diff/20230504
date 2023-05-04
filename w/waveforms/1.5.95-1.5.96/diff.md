# Comparing `tmp/waveforms-1.5.95.tar.gz` & `tmp/waveforms-1.5.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waveforms-1.5.95.tar", last modified: Wed May  3 16:09:11 2023, max compression
+gzip compressed data, was "waveforms-1.5.96.tar", last modified: Thu May  4 17:10:59 2023, max compression
```

## Comparing `waveforms-1.5.95.tar` & `waveforms-1.5.96.tar`

### file list

```diff
@@ -1,307 +1,207 @@
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.541471 waveforms-1.5.95/
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.481532 waveforms-1.5.95/.github/
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.482090 waveforms-1.5.95/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 feihoo87   (501) staff       (20)      620 2021-08-10 05:39:31.000000 waveforms-1.5.95/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 feihoo87   (501) staff       (20)      595 2021-08-10 05:39:31.000000 waveforms-1.5.95/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 feihoo87   (501) staff       (20)      114 2021-08-10 05:39:31.000000 waveforms-1.5.95/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.482475 waveforms-1.5.95/.github/workflows/
--rw-r--r--   0 feihoo87   (501) staff       (20)     1767 2023-02-17 12:03:33.000000 waveforms-1.5.95/.github/workflows/workflow.yml
--rw-r--r--   0 feihoo87   (501) staff       (20)     1864 2023-02-24 07:44:45.000000 waveforms-1.5.95/.gitignore
--rw-r--r--   0 feihoo87   (501) staff       (20)     1065 2020-06-25 03:04:31.000000 waveforms-1.5.95/LICENSE
--rw-r--r--   0 feihoo87   (501) staff       (20)       75 2023-02-02 18:17:10.000000 waveforms-1.5.95/MANIFEST.in
--rw-r--r--   0 feihoo87   (501) staff       (20)     2728 2023-05-03 16:09:11.541319 waveforms-1.5.95/PKG-INFO
--rw-r--r--   0 feihoo87   (501) staff       (20)     1561 2022-07-05 10:17:01.000000 waveforms-1.5.95/README.md
--rw-r--r--   0 feihoo87   (501) staff       (20)     2009 2023-04-22 10:28:00.000000 waveforms-1.5.95/pyproject.toml
--rw-r--r--   0 feihoo87   (501) staff       (20)       38 2023-05-03 16:09:11.541523 waveforms-1.5.95/setup.cfg
--rw-r--r--   0 feihoo87   (501) staff       (20)     1037 2023-02-02 17:40:18.000000 waveforms-1.5.95/setup.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.485101 waveforms-1.5.95/src/
--rw-r--r--   0 feihoo87   (501) staff       (20)     4567 2023-01-30 03:16:44.000000 waveforms-1.5.95/src/complex.h
--rw-r--r--   0 feihoo87   (501) staff       (20)     1124 2023-01-30 03:20:18.000000 waveforms-1.5.95/src/fraction.h
--rw-r--r--   0 feihoo87   (501) staff       (20)    32248 2023-01-24 15:21:09.000000 waveforms-1.5.95/src/ikcp.c
--rw-r--r--   0 feihoo87   (501) staff       (20)    12165 2023-01-24 09:12:23.000000 waveforms-1.5.95/src/ikcp.h
--rw-r--r--   0 feihoo87   (501) staff       (20)     5239 2023-03-17 14:01:01.000000 waveforms-1.5.95/src/kcp.c
--rw-r--r--   0 feihoo87   (501) staff       (20)     4703 2022-07-03 09:33:18.000000 waveforms-1.5.95/src/multi_type_logit.c
--rw-r--r--   0 feihoo87   (501) staff       (20)     5134 2023-01-24 03:12:57.000000 waveforms-1.5.95/src/prime.c
--rw-r--r--   0 feihoo87   (501) staff       (20)     6036 2023-02-02 16:59:39.000000 waveforms-1.5.95/src/waveform.c
--rw-r--r--   0 feihoo87   (501) staff       (20)     3432 2023-02-02 17:37:01.000000 waveforms-1.5.95/src/waveform.h
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.488510 waveforms-1.5.95/tests/
--rw-r--r--   0 feihoo87   (501) staff       (20)     9188 2021-08-28 07:10:31.000000 waveforms-1.5.95/tests/config.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      225 2021-06-06 08:24:55.000000 waveforms-1.5.95/tests/test_clifford.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     4255 2022-08-10 09:11:02.000000 waveforms-1.5.95/tests/test_compile.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      398 2022-04-15 14:27:20.000000 waveforms-1.5.95/tests/test_config.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3261 2022-09-28 10:42:06.000000 waveforms-1.5.95/tests/test_dicttree.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3229 2022-08-10 09:37:15.000000 waveforms-1.5.95/tests/test_lisp.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    32676 2021-11-12 17:26:30.000000 waveforms-1.5.95/tests/test_msgpack.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     4181 2022-04-15 14:28:44.000000 waveforms-1.5.95/tests/test_namespace.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2732 2022-10-01 17:17:16.000000 waveforms-1.5.95/tests/test_registry.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    10699 2023-04-27 16:43:42.000000 waveforms-1.5.95/tests/test_scan_iter.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1895 2021-08-24 13:43:49.000000 waveforms-1.5.95/tests/test_tomo.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      473 2021-07-15 10:07:10.000000 waveforms-1.5.95/tests/test_verify.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     4902 2022-10-16 08:07:02.000000 waveforms-1.5.95/tests/test_vm.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     4788 2022-06-28 09:26:19.000000 waveforms-1.5.95/tests/test_waveform.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.492277 waveforms-1.5.95/waveforms/
--rw-r--r--   0 feihoo87   (501) staff       (20)      683 2023-04-28 02:45:10.000000 waveforms-1.5.95/waveforms/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      599 2022-07-03 09:33:18.000000 waveforms-1.5.95/waveforms/autoreload.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     7804 2021-09-09 06:48:10.000000 waveforms-1.5.95/waveforms/baseconfig.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     4926 2023-01-30 06:19:13.000000 waveforms-1.5.95/waveforms/cache.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1945 2023-04-28 05:30:41.000000 waveforms-1.5.95/waveforms/dataset.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     8963 2023-04-29 12:22:47.000000 waveforms-1.5.95/waveforms/dicttree.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2719 2023-01-20 10:59:36.000000 waveforms-1.5.95/waveforms/loader.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.494491 waveforms-1.5.95/waveforms/math/
--rw-r--r--   0 feihoo87   (501) staff       (20)      209 2023-04-17 15:03:03.000000 waveforms-1.5.95/waveforms/math/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     7117 2023-02-16 06:19:33.000000 waveforms-1.5.95/waveforms/math/bayes.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     6460 2023-02-16 05:39:47.000000 waveforms-1.5.95/waveforms/math/fibheap.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.496846 waveforms-1.5.95/waveforms/math/fit/
--rw-r--r--   0 feihoo87   (501) staff       (20)      890 2023-04-14 15:49:05.000000 waveforms-1.5.95/waveforms/math/fit/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2108 2023-04-14 03:03:47.000000 waveforms-1.5.95/waveforms/math/fit/_fit.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     4074 2023-04-04 05:15:25.000000 waveforms-1.5.95/waveforms/math/fit/delay.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2468 2023-02-20 03:23:23.000000 waveforms-1.5.95/waveforms/math/fit/geo.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2806 2023-04-20 10:27:23.000000 waveforms-1.5.95/waveforms/math/fit/qubit_dynamics.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    12988 2023-04-20 10:21:42.000000 waveforms-1.5.95/waveforms/math/fit/readout.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     7928 2023-03-29 08:06:28.000000 waveforms-1.5.95/waveforms/math/fit/resonator.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     8948 2023-05-02 08:01:05.000000 waveforms-1.5.95/waveforms/math/fit/simple.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3678 2023-04-14 15:49:59.000000 waveforms-1.5.95/waveforms/math/fit/spectrum.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2577 2023-04-04 06:01:49.000000 waveforms-1.5.95/waveforms/math/graph.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.497703 waveforms-1.5.95/waveforms/math/group/
--rw-r--r--   0 feihoo87   (501) staff       (20)      988 2023-04-29 02:07:14.000000 waveforms-1.5.95/waveforms/math/group/_SU_n_.py
--rw-r--r--   0 feihoo87   (501) staff       (20)       22 2023-04-27 15:44:54.000000 waveforms-1.5.95/waveforms/math/group/__init__.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.497932 waveforms-1.5.95/waveforms/math/group/clifford/
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-05-02 03:24:55.000000 waveforms-1.5.95/waveforms/math/group/clifford/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      486 2023-05-02 03:26:07.000000 waveforms-1.5.95/waveforms/math/group/clifford/funtions.py
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-05-02 03:32:14.000000 waveforms-1.5.95/waveforms/math/group/symplectic.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     7131 2023-01-20 07:52:04.000000 waveforms-1.5.95/waveforms/math/prime.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.498991 waveforms-1.5.95/waveforms/math/signal/
--rw-r--r--   0 feihoo87   (501) staff       (20)      272 2022-03-08 16:35:57.000000 waveforms-1.5.95/waveforms/math/signal/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2100 2023-02-24 12:17:40.000000 waveforms-1.5.95/waveforms/math/signal/demodulate.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     7751 2023-04-12 07:27:09.000000 waveforms-1.5.95/waveforms/math/signal/distortion.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     7634 2023-03-29 02:17:59.000000 waveforms-1.5.95/waveforms/math/signal/func.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     9582 2023-05-02 03:03:17.000000 waveforms-1.5.95/waveforms/math/transmon.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     6860 2022-01-30 08:42:13.000000 waveforms-1.5.95/waveforms/namespace.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.503275 waveforms-1.5.95/waveforms/qlisp/
--rw-r--r--   0 feihoo87   (501) staff       (20)      608 2023-02-18 15:49:44.000000 waveforms-1.5.95/waveforms/qlisp/__init__.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.503368 waveforms-1.5.95/waveforms/qlisp/arch/
--rw-r--r--   0 feihoo87   (501) staff       (20)     1079 2023-03-17 05:52:56.000000 waveforms-1.5.95/waveforms/qlisp/arch/__init__.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.503965 waveforms-1.5.95/waveforms/qlisp/arch/basic/
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2022-08-10 10:22:51.000000 waveforms-1.5.95/waveforms/qlisp/arch/basic/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     8085 2022-08-10 10:25:05.000000 waveforms-1.5.95/waveforms/qlisp/arch/basic/arch.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     5962 2022-08-10 10:25:30.000000 waveforms-1.5.95/waveforms/qlisp/arch/basic/config.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     8624 2023-01-16 07:17:36.000000 waveforms-1.5.95/waveforms/qlisp/assembly.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     6255 2023-03-16 13:04:22.000000 waveforms-1.5.95/waveforms/qlisp/base.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1325 2022-08-10 08:40:07.000000 waveforms-1.5.95/waveforms/qlisp/commands.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2519 2023-03-17 05:54:01.000000 waveforms-1.5.95/waveforms/qlisp/compiler.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    16920 2022-08-10 08:56:56.000000 waveforms-1.5.95/waveforms/qlisp/config.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    17969 2023-02-12 14:18:56.000000 waveforms-1.5.95/waveforms/qlisp/interpreter.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     4466 2023-02-18 03:35:10.000000 waveforms-1.5.95/waveforms/qlisp/library.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.504214 waveforms-1.5.95/waveforms/qlisp/libs/
--rw-r--r--   0 feihoo87   (501) staff       (20)    11269 2023-04-21 06:17:03.000000 waveforms-1.5.95/waveforms/qlisp/libs/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3499 2022-10-26 03:14:59.000000 waveforms-1.5.95/waveforms/qlisp/macro.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    16227 2022-08-10 09:36:02.000000 waveforms-1.5.95/waveforms/qlisp/parse.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1193 2023-02-18 15:28:51.000000 waveforms-1.5.95/waveforms/qlisp/prog.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.505632 waveforms-1.5.95/waveforms/qlisp/qasm/
--rw-r--r--   0 feihoo87   (501) staff       (20)     1187 2022-08-10 07:42:39.000000 waveforms-1.5.95/waveforms/qlisp/qasm/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     4400 2022-08-10 09:06:47.000000 waveforms-1.5.95/waveforms/qlisp/qasm/eval.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      850 2021-08-13 08:32:17.000000 waveforms-1.5.95/waveforms/qlisp/qasm/exceptions.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.506026 waveforms-1.5.95/waveforms/qlisp/qasm/libs/
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-02-02 15:49:07.000000 waveforms-1.5.95/waveforms/qlisp/qasm/libs/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     4802 2021-05-15 16:08:50.000000 waveforms-1.5.95/waveforms/qlisp/qasm/libs/qelib1.inc
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.510473 waveforms-1.5.95/waveforms/qlisp/qasm/node/
--rw-r--r--   0 feihoo87   (501) staff       (20)     1244 2021-05-11 14:56:30.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1144 2021-08-24 13:29:05.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/barrier.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3016 2021-08-24 13:28:56.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/binaryop.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1677 2021-08-24 13:28:44.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/binaryoperator.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1663 2021-08-24 13:28:39.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/creg.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1842 2021-08-24 13:28:32.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/customunitary.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1289 2021-08-24 13:28:24.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/expressionlist.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3474 2021-08-24 13:28:17.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/external.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1434 2021-08-24 13:28:10.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/format.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2306 2021-08-24 13:28:04.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/gate.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1543 2021-08-24 13:27:59.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/gatebody.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3257 2021-08-24 13:27:52.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/id.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1261 2021-08-24 13:27:45.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/idlist.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1354 2021-08-24 13:27:40.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/if_.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1512 2021-08-24 13:27:34.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/indexedid.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2159 2021-08-24 13:27:28.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/intnode.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1260 2021-08-24 13:27:22.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/measure.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1969 2020-08-19 05:59:10.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/node.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      856 2020-08-19 06:02:21.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/nodeexception.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2145 2021-08-24 13:27:14.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/opaque.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2551 2021-08-24 13:29:20.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/prefix.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1329 2021-08-24 13:26:51.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/primarylist.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1198 2020-08-19 06:21:51.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/program.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1663 2020-08-19 06:22:21.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/qreg.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2623 2021-04-25 10:09:37.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/real.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1142 2020-08-19 06:23:52.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/reset.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1601 2020-08-19 06:24:34.000000 waveforms-1.5.95/waveforms/qlisp/qasm/node/unaryoperator.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1805 2021-05-30 11:08:56.000000 waveforms-1.5.95/waveforms/qlisp/qasm/qasm.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     5276 2021-06-09 15:23:31.000000 waveforms-1.5.95/waveforms/qlisp/qasm/qasmlexer.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    36242 2021-05-30 11:09:23.000000 waveforms-1.5.95/waveforms/qlisp/qasm/qasmparser.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.511986 waveforms-1.5.95/waveforms/qlisp/qc/
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2022-10-18 12:30:46.000000 waveforms-1.5.95/waveforms/qlisp/qc/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     6785 2022-10-20 03:15:39.000000 waveforms-1.5.95/waveforms/qlisp/qc/assembler.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     8848 2022-10-18 14:28:02.000000 waveforms-1.5.95/waveforms/qlisp/qc/compiler.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      962 2022-10-20 02:32:05.000000 waveforms-1.5.95/waveforms/qlisp/qc/embedded.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     4120 2023-02-10 16:45:08.000000 waveforms-1.5.95/waveforms/qlisp/qc/instruction.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2060 2022-10-18 14:28:01.000000 waveforms-1.5.95/waveforms/qlisp/qc/linker.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1522 2023-02-19 14:14:36.000000 waveforms-1.5.95/waveforms/qlisp/qc/opcode.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.512867 waveforms-1.5.95/waveforms/qlisp/simulator/
--rw-r--r--   0 feihoo87   (501) staff       (20)     9407 2022-08-10 08:02:32.000000 waveforms-1.5.95/waveforms/qlisp/simulator/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3824 2023-02-18 03:54:36.000000 waveforms-1.5.95/waveforms/qlisp/simulator/mat.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    10003 2023-04-26 09:10:26.000000 waveforms-1.5.95/waveforms/qlisp/simulator/simple.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2268 2022-08-09 07:08:07.000000 waveforms-1.5.95/waveforms/qlisp/tokenize.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      278 2023-01-30 08:26:54.000000 waveforms-1.5.95/waveforms/qlisp/typing.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2200 2022-08-10 08:50:27.000000 waveforms-1.5.95/waveforms/qlisp/utils.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.514312 waveforms-1.5.95/waveforms/qlisp/vm/
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2022-10-18 12:26:24.000000 waveforms-1.5.95/waveforms/qlisp/vm/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     5825 2022-10-27 06:10:35.000000 waveforms-1.5.95/waveforms/qlisp/vm/cmds.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2605 2022-10-18 14:27:58.000000 waveforms-1.5.95/waveforms/qlisp/vm/dispatch.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      407 2022-10-18 12:39:51.000000 waveforms-1.5.95/waveforms/qlisp/vm/mem.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2915 2022-10-28 09:20:02.000000 waveforms-1.5.95/waveforms/qlisp/vm/operators.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3133 2022-10-18 14:27:52.000000 waveforms-1.5.95/waveforms/qlisp/vm/vm.py
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2022-10-08 13:21:12.000000 waveforms-1.5.95/waveforms/qlisp/vm.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.516841 waveforms-1.5.95/waveforms/qlisp2/
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-02-19 09:01:51.000000 waveforms-1.5.95/waveforms/qlisp2/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3763 2023-03-04 10:56:47.000000 waveforms-1.5.95/waveforms/qlisp2/assembler.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1830 2023-02-19 13:59:47.000000 waveforms-1.5.95/waveforms/qlisp2/compiler.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2661 2023-02-19 09:11:47.000000 waveforms-1.5.95/waveforms/qlisp2/config.py
--rw-r--r--   0 feihoo87   (501) staff       (20)       26 2023-02-19 09:06:51.000000 waveforms-1.5.95/waveforms/qlisp2/context.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      954 2023-02-20 04:57:04.000000 waveforms-1.5.95/waveforms/qlisp2/instruction.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     4283 2023-02-19 09:07:46.000000 waveforms-1.5.95/waveforms/qlisp2/library.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.517426 waveforms-1.5.95/waveforms/qlisp2/libs/
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-02-19 09:13:02.000000 waveforms-1.5.95/waveforms/qlisp2/libs/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      268 2023-02-19 13:52:27.000000 waveforms-1.5.95/waveforms/qlisp2/libs/cz.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2020 2023-02-19 11:55:06.000000 waveforms-1.5.95/waveforms/qlisp2/libs/stdlib.py
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-02-19 14:00:28.000000 waveforms-1.5.95/waveforms/qlisp2/linker.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    10447 2023-02-19 14:14:52.000000 waveforms-1.5.95/waveforms/qlisp2/opcode.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     8455 2023-02-26 11:45:15.000000 waveforms-1.5.95/waveforms/qlisp2/parser.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      885 2023-02-19 14:01:23.000000 waveforms-1.5.95/waveforms/qlisp2/vm.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.518962 waveforms-1.5.95/waveforms/quantum/
--rw-r--r--   0 feihoo87   (501) staff       (20)      468 2022-08-10 09:47:21.000000 waveforms-1.5.95/waveforms/quantum/__init__.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.519204 waveforms-1.5.95/waveforms/quantum/circuit/
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2021-06-02 10:26:02.000000 waveforms-1.5.95/waveforms/quantum/circuit/__init__.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.521629 waveforms-1.5.95/waveforms/quantum/circuit/qlisp/
--rw-r--r--   0 feihoo87   (501) staff       (20)      319 2021-09-03 07:21:49.000000 waveforms-1.5.95/waveforms/quantum/circuit/qlisp/__init__.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.522174 waveforms-1.5.95/waveforms/quantum/circuit/qlisp/arch/
--rw-r--r--   0 feihoo87   (501) staff       (20)      214 2022-08-10 09:31:10.000000 waveforms-1.5.95/waveforms/quantum/circuit/qlisp/arch/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      405 2022-08-10 09:30:29.000000 waveforms-1.5.95/waveforms/quantum/circuit/qlisp/arch/base.py
--rw-r--r--   0 feihoo87   (501) staff       (20)       70 2022-08-10 09:13:01.000000 waveforms-1.5.95/waveforms/quantum/circuit/qlisp/assembly_left.py
--rw-r--r--   0 feihoo87   (501) staff       (20)       58 2022-08-10 09:12:28.000000 waveforms-1.5.95/waveforms/quantum/circuit/qlisp/assembly_right.py
--rw-r--r--   0 feihoo87   (501) staff       (20)       55 2022-08-10 09:13:43.000000 waveforms-1.5.95/waveforms/quantum/circuit/qlisp/compiler.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      322 2022-08-10 09:15:58.000000 waveforms-1.5.95/waveforms/quantum/circuit/qlisp/config.py
--rw-r--r--   0 feihoo87   (501) staff       (20)       69 2022-08-10 09:16:40.000000 waveforms-1.5.95/waveforms/quantum/circuit/qlisp/library.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      279 2022-08-10 09:18:46.000000 waveforms-1.5.95/waveforms/quantum/circuit/qlisp/macro.py
--rw-r--r--   0 feihoo87   (501) staff       (20)       48 2022-08-10 09:19:30.000000 waveforms-1.5.95/waveforms/quantum/circuit/qlisp/qasm.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      428 2022-08-10 09:21:51.000000 waveforms-1.5.95/waveforms/quantum/circuit/qlisp/qlisp.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      158 2022-10-09 15:47:03.000000 waveforms-1.5.95/waveforms/quantum/circuit/qlisp/stdlib.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      141 2022-08-10 09:25:50.000000 waveforms-1.5.95/waveforms/quantum/circuit/qlisp/utils.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.522357 waveforms-1.5.95/waveforms/quantum/circuit/simulator/
--rw-r--r--   0 feihoo87   (501) staff       (20)      376 2022-08-10 09:46:31.000000 waveforms-1.5.95/waveforms/quantum/circuit/simulator/__init__.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.523517 waveforms-1.5.95/waveforms/quantum/clifford/
--rw-r--r--   0 feihoo87   (501) staff       (20)      439 2021-06-06 09:01:59.000000 waveforms-1.5.95/waveforms/quantum/clifford/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    10579 2023-02-18 16:22:40.000000 waveforms-1.5.95/waveforms/quantum/clifford/clifford.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     5099 2021-07-26 16:11:04.000000 waveforms-1.5.95/waveforms/quantum/clifford/db.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2413 2022-02-19 11:45:12.000000 waveforms-1.5.95/waveforms/quantum/clifford/mat.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1345 2022-08-10 09:56:08.000000 waveforms-1.5.95/waveforms/quantum/clifford/seq2mat.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     8295 2022-08-10 10:06:20.000000 waveforms-1.5.95/waveforms/quantum/math.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2029 2023-02-18 15:52:44.000000 waveforms-1.5.95/waveforms/quantum/rb.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    12740 2023-04-07 09:31:12.000000 waveforms-1.5.95/waveforms/quantum/tomo.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3825 2023-04-14 15:50:33.000000 waveforms-1.5.95/waveforms/quantum/transmon.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3961 2023-02-18 15:51:43.000000 waveforms-1.5.95/waveforms/quantum/xeb.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    21432 2023-01-29 09:38:11.000000 waveforms-1.5.95/waveforms/registry.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.524343 waveforms-1.5.95/waveforms/scan/
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-05-02 03:17:05.000000 waveforms-1.5.95/waveforms/scan/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-05-02 03:17:32.000000 waveforms-1.5.95/waveforms/scan/dataset.py
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-05-02 03:22:21.000000 waveforms-1.5.95/waveforms/scan/optimize.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     7998 2023-05-02 03:18:38.000000 waveforms-1.5.95/waveforms/scan/scanner.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      252 2023-04-27 07:38:41.000000 waveforms-1.5.95/waveforms/scan/transforms.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    26353 2023-04-27 16:43:06.000000 waveforms-1.5.95/waveforms/scan_iter.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.524850 waveforms-1.5.95/waveforms/security/
--rw-r--r--   0 feihoo87   (501) staff       (20)       64 2021-07-14 14:15:41.000000 waveforms-1.5.95/waveforms/security/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1296 2021-07-14 14:39:40.000000 waveforms-1.5.95/waveforms/security/verify.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.525812 waveforms-1.5.95/waveforms/server/
--rw-r--r--   0 feihoo87   (501) staff       (20)      600 2021-08-24 15:36:28.000000 waveforms-1.5.95/waveforms/server/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1722 2021-10-08 05:02:59.000000 waveforms-1.5.95/waveforms/server/__main__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    32530 2022-02-15 02:51:51.000000 waveforms-1.5.95/waveforms/server/umsgpack.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2674 2022-08-13 09:32:16.000000 waveforms-1.5.95/waveforms/server/websocket.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.526830 waveforms-1.5.95/waveforms/sys/
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2021-11-19 12:14:58.000000 waveforms-1.5.95/waveforms/sys/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      985 2022-08-10 10:47:52.000000 waveforms-1.5.95/waveforms/sys/bootstrap.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    23875 2023-05-03 15:41:55.000000 waveforms-1.5.95/waveforms/sys/chat.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.528197 waveforms-1.5.95/waveforms/sys/device/
--rw-r--r--   0 feihoo87   (501) staff       (20)      149 2023-03-17 15:12:36.000000 waveforms-1.5.95/waveforms/sys/device/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      906 2023-03-15 16:23:55.000000 waveforms-1.5.95/waveforms/sys/device/__main__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     6423 2023-03-17 15:12:21.000000 waveforms-1.5.95/waveforms/sys/device/basedevice.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2501 2023-03-15 16:29:22.000000 waveforms-1.5.95/waveforms/sys/device/loader.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1564 2021-10-08 05:25:36.000000 waveforms-1.5.95/waveforms/sys/device/utils.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.528837 waveforms-1.5.95/waveforms/sys/drivers/
--rw-r--r--   0 feihoo87   (501) staff       (20)     1867 2023-03-15 16:14:55.000000 waveforms-1.5.95/waveforms/sys/drivers/FakeInstrument.py
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-02-22 16:47:33.000000 waveforms-1.5.95/waveforms/sys/drivers/__init__.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.528945 waveforms-1.5.95/waveforms/sys/executor/
--rw-r--r--   0 feihoo87   (501) staff       (20)     5867 2023-03-08 03:19:32.000000 waveforms-1.5.95/waveforms/sys/executor/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2889 2022-08-10 10:16:42.000000 waveforms-1.5.95/waveforms/sys/ipy_events.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.530886 waveforms-1.5.95/waveforms/sys/net/
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2022-11-04 02:05:49.000000 waveforms-1.5.95/waveforms/sys/net/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    23509 2023-03-13 13:43:32.000000 waveforms-1.5.95/waveforms/sys/net/dhcp.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     5322 2023-03-13 13:45:13.000000 waveforms-1.5.95/waveforms/sys/net/dhcpd.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    38172 2023-02-20 16:16:19.000000 waveforms-1.5.95/waveforms/sys/net/kad.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     5761 2023-04-03 16:07:47.000000 waveforms-1.5.95/waveforms/sys/net/kcp.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     4964 2022-12-23 08:24:12.000000 waveforms-1.5.95/waveforms/sys/net/nginx.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     5350 2023-03-02 14:43:50.000000 waveforms-1.5.95/waveforms/sys/progress.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.532948 waveforms-1.5.95/waveforms/sys/rpc/
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-04-03 12:14:49.000000 waveforms-1.5.95/waveforms/sys/rpc/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-04-03 12:15:12.000000 waveforms-1.5.95/waveforms/sys/rpc/client.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2567 2023-04-03 12:23:32.000000 waveforms-1.5.95/waveforms/sys/rpc/exceptions.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    11979 2023-04-03 12:27:38.000000 waveforms-1.5.95/waveforms/sys/rpc/rpc.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3355 2023-04-03 12:21:16.000000 waveforms-1.5.95/waveforms/sys/rpc/serialize.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      713 2023-04-03 16:29:33.000000 waveforms-1.5.95/waveforms/sys/rpc/server.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      713 2023-04-03 16:30:44.000000 waveforms-1.5.95/waveforms/sys/rpc/socket.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      594 2023-04-03 12:30:03.000000 waveforms-1.5.95/waveforms/sys/rpc/utils.py
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-04-03 12:14:58.000000 waveforms-1.5.95/waveforms/sys/rpc/worker.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.535114 waveforms-1.5.95/waveforms/sys/sched/
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2022-08-10 10:30:18.000000 waveforms-1.5.95/waveforms/sys/sched/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3874 2022-08-10 10:32:24.000000 waveforms-1.5.95/waveforms/sys/sched/_bigbrother.py
--rw-r--r--   0 feihoo87   (501) staff       (20)      663 2022-12-06 16:38:00.000000 waveforms-1.5.95/waveforms/sys/sched/lock.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    18704 2022-08-10 10:31:27.000000 waveforms-1.5.95/waveforms/sys/sched/main_loop.py
--rw-r--r--   0 feihoo87   (501) staff       (20)       26 2022-08-13 18:05:52.000000 waveforms-1.5.95/waveforms/sys/sched/settings.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    27213 2022-08-16 08:40:57.000000 waveforms-1.5.95/waveforms/sys/sched/task.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3425 2022-08-11 14:08:54.000000 waveforms-1.5.95/waveforms/sys/sched/task_tree.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2512 2022-08-11 14:01:09.000000 waveforms-1.5.95/waveforms/sys/sched/tree2.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.537514 waveforms-1.5.95/waveforms/sys/storage/
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2021-11-19 12:19:43.000000 waveforms-1.5.95/waveforms/sys/storage/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     9952 2022-04-23 04:09:45.000000 waveforms-1.5.95/waveforms/sys/storage/asynsqlite.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1946 2023-04-03 02:56:46.000000 waveforms-1.5.95/waveforms/sys/storage/chunk.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     8001 2022-04-15 14:34:45.000000 waveforms-1.5.95/waveforms/sys/storage/config.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     6070 2022-04-16 03:02:22.000000 waveforms-1.5.95/waveforms/sys/storage/config2.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     6043 2022-08-10 10:13:51.000000 waveforms-1.5.95/waveforms/sys/storage/crud.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2424 2023-03-31 02:32:59.000000 waveforms-1.5.95/waveforms/sys/storage/file.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.538580 waveforms-1.5.95/waveforms/sys/storage/fs/
--rw-r--r--   0 feihoo87   (501) staff       (20)       48 2023-04-03 03:03:11.000000 waveforms-1.5.95/waveforms/sys/storage/fs/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1985 2023-04-03 03:09:00.000000 waveforms-1.5.95/waveforms/sys/storage/fs/chunk.py
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-04-03 03:01:41.000000 waveforms-1.5.95/waveforms/sys/storage/fs/file.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3576 2023-04-03 03:10:55.000000 waveforms-1.5.95/waveforms/sys/storage/fs/index.py
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-04-03 03:02:09.000000 waveforms-1.5.95/waveforms/sys/storage/fs/pack.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.539744 waveforms-1.5.95/waveforms/sys/storage/models/
--rw-r--r--   0 feihoo87   (501) staff       (20)        0 2023-01-29 05:18:37.000000 waveforms-1.5.95/waveforms/sys/storage/models/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2678 2023-01-29 05:25:47.000000 waveforms-1.5.95/waveforms/sys/storage/models/association.py
--rw-r--r--   0 feihoo87   (501) staff       (20)       71 2023-01-29 05:19:35.000000 waveforms-1.5.95/waveforms/sys/storage/models/base.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2771 2023-03-31 02:30:19.000000 waveforms-1.5.95/waveforms/sys/storage/models/record.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2132 2023-03-31 02:30:13.000000 waveforms-1.5.95/waveforms/sys/storage/models/report.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     1214 2023-01-29 06:43:41.000000 waveforms-1.5.95/waveforms/sys/storage/models/tag.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    20092 2023-02-23 05:12:38.000000 waveforms-1.5.95/waveforms/sys/storage/models.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    12401 2022-04-23 06:37:32.000000 waveforms-1.5.95/waveforms/sys/storage/sqlite.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.540220 waveforms-1.5.95/waveforms/units/
--rw-r--r--   0 feihoo87   (501) staff       (20)     1376 2023-02-23 12:50:39.000000 waveforms-1.5.95/waveforms/units/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     3836 2023-02-23 12:51:17.000000 waveforms-1.5.95/waveforms/units/units.py
--rw-r--r--   0 feihoo87   (501) staff       (20)       96 2023-05-03 15:42:44.000000 waveforms-1.5.95/waveforms/version.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.540982 waveforms-1.5.95/waveforms/visualization/
--rw-r--r--   0 feihoo87   (501) staff       (20)    12975 2023-04-07 03:48:01.000000 waveforms-1.5.95/waveforms/visualization/__init__.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     9999 2023-04-01 02:52:50.000000 waveforms-1.5.95/waveforms/visualization/plot_layout.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     2693 2023-04-07 02:14:11.000000 waveforms-1.5.95/waveforms/visualization/plot_seq.py
--rw-r--r--   0 feihoo87   (501) staff       (20)    39644 2023-04-28 14:27:01.000000 waveforms-1.5.95/waveforms/waveform.py
--rw-r--r--   0 feihoo87   (501) staff       (20)     7065 2023-04-27 16:09:50.000000 waveforms-1.5.95/waveforms/waveform_parser.py
-drwxr-xr-x   0 feihoo87   (501) staff       (20)        0 2023-05-03 16:09:11.493026 waveforms-1.5.95/waveforms.egg-info/
--rw-r--r--   0 feihoo87   (501) staff       (20)     2728 2023-05-03 16:09:11.000000 waveforms-1.5.95/waveforms.egg-info/PKG-INFO
--rw-r--r--   0 feihoo87   (501) staff       (20)     7855 2023-05-03 16:09:11.000000 waveforms-1.5.95/waveforms.egg-info/SOURCES.txt
--rw-r--r--   0 feihoo87   (501) staff       (20)        1 2023-05-03 16:09:11.000000 waveforms-1.5.95/waveforms.egg-info/dependency_links.txt
--rw-r--r--   0 feihoo87   (501) staff       (20)       63 2023-05-03 16:09:11.000000 waveforms-1.5.95/waveforms.egg-info/entry_points.txt
--rw-r--r--   0 feihoo87   (501) staff       (20)      350 2023-05-03 16:09:11.000000 waveforms-1.5.95/waveforms.egg-info/requires.txt
--rw-r--r--   0 feihoo87   (501) staff       (20)       10 2023-05-03 16:09:11.000000 waveforms-1.5.95/waveforms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.598239 waveforms-1.5.96/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-04 17:09:54.000000 waveforms-1.5.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 17:09:54.000000 waveforms-1.5.96/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-04 17:10:59.598239 waveforms-1.5.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-04 17:09:54.000000 waveforms-1.5.96/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-04 17:09:54.000000 waveforms-1.5.96/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:10:59.598239 waveforms-1.5.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-04 17:09:54.000000 waveforms-1.5.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.586239 waveforms-1.5.96/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    32248 2023-05-04 17:09:54.000000 waveforms-1.5.96/src/ikcp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-04 17:09:54.000000 waveforms-1.5.96/src/ikcp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-05-04 17:09:54.000000 waveforms-1.5.96/src/kcp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-04 17:09:54.000000 waveforms-1.5.96/src/prime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-04 17:09:54.000000 waveforms-1.5.96/src/waveform.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-04 17:09:54.000000 waveforms-1.5.96/src/waveform.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.586239 waveforms-1.5.96/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-04 17:09:54.000000 waveforms-1.5.96/tests/test_clifford.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-04 17:09:54.000000 waveforms-1.5.96/tests/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-04 17:09:54.000000 waveforms-1.5.96/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-04 17:09:54.000000 waveforms-1.5.96/tests/test_dicttree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-04 17:09:54.000000 waveforms-1.5.96/tests/test_lisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32676 2023-05-04 17:09:54.000000 waveforms-1.5.96/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-04 17:09:54.000000 waveforms-1.5.96/tests/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-04 17:09:54.000000 waveforms-1.5.96/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-05-04 17:09:54.000000 waveforms-1.5.96/tests/test_scan_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-04 17:09:54.000000 waveforms-1.5.96/tests/test_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-04 17:09:54.000000 waveforms-1.5.96/tests/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-04 17:09:54.000000 waveforms-1.5.96/tests/test_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-04 17:09:54.000000 waveforms-1.5.96/tests/test_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.590239 waveforms-1.5.96/waveforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/baseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/dicttree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.590239 waveforms-1.5.96/waveforms/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/bayes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/fibheap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.590239 waveforms-1.5.96/waveforms/math/fit/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/fit/_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/fit/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/fit/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/fit/qubit_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/fit/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/fit/resonator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/fit/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/fit/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.590239 waveforms-1.5.96/waveforms/math/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/group/_SU_n_.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/group/permutation_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/prime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.590239 waveforms-1.5.96/waveforms/math/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/signal/demodulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/signal/distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/signal/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/math/transmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.590239 waveforms-1.5.96/waveforms/qlisp/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.590239 waveforms-1.5.96/waveforms/qlisp/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.590239 waveforms-1.5.96/waveforms/qlisp/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/prog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.594239 waveforms-1.5.96/waveforms/qlisp/qasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.594239 waveforms-1.5.96/waveforms/qlisp/qasm/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/libs/qelib1.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.594239 waveforms-1.5.96/waveforms/qlisp/qasm/node/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/binaryop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/binaryoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/creg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/customunitary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/expressionlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/gatebody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/idlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/if_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/indexedid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/intnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/nodeexception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/opaque.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/primarylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/qreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/node/unaryoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/qasmlexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/qasm/qasmparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.594239 waveforms-1.5.96/waveforms/qlisp/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/simulator/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/simulator/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/qlisp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.594239 waveforms-1.5.96/waveforms/quantum/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.594239 waveforms-1.5.96/waveforms/quantum/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/circuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.598239 waveforms-1.5.96/waveforms/quantum/circuit/qlisp/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/circuit/qlisp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.598239 waveforms-1.5.96/waveforms/quantum/circuit/qlisp/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/circuit/qlisp/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/circuit/qlisp/arch/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/circuit/qlisp/assembly_left.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/circuit/qlisp/assembly_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/circuit/qlisp/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/circuit/qlisp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/circuit/qlisp/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/circuit/qlisp/macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/circuit/qlisp/qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/circuit/qlisp/qlisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/circuit/qlisp/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/circuit/qlisp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.598239 waveforms-1.5.96/waveforms/quantum/circuit/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/circuit/simulator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.598239 waveforms-1.5.96/waveforms/quantum/clifford/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/clifford/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/clifford/clifford.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/clifford/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/clifford/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/clifford/seq2mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/rb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/transmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/quantum/xeb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.598239 waveforms-1.5.96/waveforms/scan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/scan/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/scan/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26353 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/scan_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.598239 waveforms-1.5.96/waveforms/security/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/security/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.598239 waveforms-1.5.96/waveforms/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32530 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/server/umsgpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.598239 waveforms-1.5.96/waveforms/sys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22126 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.598239 waveforms-1.5.96/waveforms/sys/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/device/basedevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/device/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/device/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.598239 waveforms-1.5.96/waveforms/sys/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/drivers/FakeInstrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/ipy_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.598239 waveforms-1.5.96/waveforms/sys/net/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23509 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/net/dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/net/dhcpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38172 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/net/kad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/net/kcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.598239 waveforms-1.5.96/waveforms/sys/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/storage/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/sys/storage/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.598239 waveforms-1.5.96/waveforms/units/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.598239 waveforms-1.5.96/waveforms/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/visualization/plot_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/visualization/plot_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39644 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-05-04 17:09:54.000000 waveforms-1.5.96/waveforms/waveform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:59.590239 waveforms-1.5.96/waveforms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-04 17:10:59.000000 waveforms-1.5.96/waveforms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-05-04 17:10:59.000000 waveforms-1.5.96/waveforms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:10:59.000000 waveforms-1.5.96/waveforms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 17:10:59.000000 waveforms-1.5.96/waveforms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-04 17:10:59.000000 waveforms-1.5.96/waveforms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 17:10:59.000000 waveforms-1.5.96/waveforms.egg-info/top_level.txt
```

### Comparing `waveforms-1.5.95/LICENSE` & `waveforms-1.5.96/LICENSE`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/PKG-INFO` & `waveforms-1.5.96/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveforms
-Version: 1.5.95
+Version: 1.5.96
 Summary: Edit waveforms used in experiment
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/feihoo87/waveforms
 Project-URL: Bug Reports, https://github.com/feihoo87/waveforms/issues
 Project-URL: Source, https://github.com/feihoo87/waveforms/
```

### Comparing `waveforms-1.5.95/README.md` & `waveforms-1.5.96/README.md`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/pyproject.toml` & `waveforms-1.5.96/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -40,19 +40,21 @@
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 full = [
     "blinker>=1.4",
     "matplotlib>=3.4.1",
+    "openai>=0.27.0",
     "portalocker>=1.4.0",
     "SQLAlchemy>=1.4.11",
     "scikit-learn>=0.24.1",
     "scikit-optimize>=0.8.1",
-    "tenacity>=8.2.2"
+    "tenacity>=8.2.2",
+    "tiktoken>=0.3.3"
 ]
 test = [
     "pytest>=4.4.0"
 ]
 docs = [
     "Sphinx",
     "sphinxcontrib-napoleon",
```

### Comparing `waveforms-1.5.95/setup.py` & `waveforms-1.5.96/setup.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/src/ikcp.c` & `waveforms-1.5.96/src/ikcp.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/src/ikcp.h` & `waveforms-1.5.96/src/ikcp.h`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/src/kcp.c` & `waveforms-1.5.96/src/kcp.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/src/prime.c` & `waveforms-1.5.96/src/prime.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/src/waveform.c` & `waveforms-1.5.96/src/waveform.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/src/waveform.h` & `waveforms-1.5.96/src/waveform.h`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/tests/test_compile.py` & `waveforms-1.5.96/tests/test_compile.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/tests/test_dicttree.py` & `waveforms-1.5.96/tests/test_dicttree.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/tests/test_lisp.py` & `waveforms-1.5.96/tests/test_lisp.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/tests/test_msgpack.py` & `waveforms-1.5.96/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/tests/test_namespace.py` & `waveforms-1.5.96/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/tests/test_registry.py` & `waveforms-1.5.96/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/tests/test_scan_iter.py` & `waveforms-1.5.96/tests/test_scan_iter.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/tests/test_tomo.py` & `waveforms-1.5.96/tests/test_tomo.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/tests/test_vm.py` & `waveforms-1.5.96/tests/test_vm.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/tests/test_waveform.py` & `waveforms-1.5.96/tests/test_waveform.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/__init__.py` & `waveforms-1.5.96/waveforms/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/autoreload.py` & `waveforms-1.5.96/waveforms/autoreload.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/baseconfig.py` & `waveforms-1.5.96/waveforms/baseconfig.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/cache.py` & `waveforms-1.5.96/waveforms/cache.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/dicttree.py` & `waveforms-1.5.96/waveforms/dicttree.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/loader.py` & `waveforms-1.5.96/waveforms/loader.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/bayes.py` & `waveforms-1.5.96/waveforms/math/bayes.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/fibheap.py` & `waveforms-1.5.96/waveforms/math/fibheap.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/fit/__init__.py` & `waveforms-1.5.96/waveforms/math/fit/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/fit/_fit.py` & `waveforms-1.5.96/waveforms/math/fit/_fit.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/fit/delay.py` & `waveforms-1.5.96/waveforms/math/fit/delay.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/fit/geo.py` & `waveforms-1.5.96/waveforms/math/fit/geo.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/fit/qubit_dynamics.py` & `waveforms-1.5.96/waveforms/math/fit/qubit_dynamics.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/fit/readout.py` & `waveforms-1.5.96/waveforms/math/fit/readout.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/fit/resonator.py` & `waveforms-1.5.96/waveforms/math/fit/resonator.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/fit/simple.py` & `waveforms-1.5.96/waveforms/math/fit/simple.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/fit/spectrum.py` & `waveforms-1.5.96/waveforms/math/fit/spectrum.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/graph.py` & `waveforms-1.5.96/waveforms/math/graph.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/group/_SU_n_.py` & `waveforms-1.5.96/waveforms/math/group/_SU_n_.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/prime.py` & `waveforms-1.5.96/waveforms/math/prime.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/signal/demodulate.py` & `waveforms-1.5.96/waveforms/math/signal/demodulate.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/signal/distortion.py` & `waveforms-1.5.96/waveforms/math/signal/distortion.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/signal/func.py` & `waveforms-1.5.96/waveforms/math/signal/func.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/math/transmon.py` & `waveforms-1.5.96/waveforms/math/transmon.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/namespace.py` & `waveforms-1.5.96/waveforms/namespace.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/__init__.py` & `waveforms-1.5.96/waveforms/qlisp/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/arch/__init__.py` & `waveforms-1.5.96/waveforms/qlisp/arch/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/arch/basic/config.py` & `waveforms-1.5.96/waveforms/qlisp/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,174 +1,251 @@
-import copy
+from __future__ import annotations
+
 import warnings
-from itertools import permutations
-from typing import Union
+from abc import ABC, abstractmethod
+from collections import defaultdict
+from dataclasses import dataclass, field
+from enum import Flag, auto
+from typing import Any, Literal, NamedTuple, Optional, Union
+
+from ..waveform import Waveform, zero
+
+
+class Signal(Flag):
+    trace = auto()
+    iq = auto()
+    state = auto()
+
+    _avg_trace = auto()
+    _avg_iq = auto()
+    _avg_state = auto()
+    _count = auto()
+    _remote = auto()
+
+    trace_avg = trace | _avg_trace
+
+    iq_avg = iq | _avg_iq
+
+    population = state | _avg_state
+    count = state | _count
+    diag = state | _count | _avg_state
+
+    remote_trace_avg = trace_avg | _remote
+    remote_iq_avg = iq_avg | _remote
+    remote_state = state | _remote
+    remote_population = population | _remote
+    remote_count = count | _remote
+
 
-from waveforms.baseconfig import _flattenDictIter, _foldDict, _query, _update
-from waveforms.namespace import DictDriver
-from waveforms.qlisp import (ABCCompileConfigMixin, ADChannel, AWGChannel,
-                             ConfigProxy, GateConfig, MultADChannel,
-                             MultAWGChannel)
-
-
-def _getSharedCoupler(qubitsDict: dict) -> set[str]:
-    s = set(qubitsDict[0]['couplers'])
-    for qubit in qubitsDict[1:]:
-        s = s & set(qubit['couplers'])
-    return s
-
-
-def _makeAWGChannelInfo(section: str, cfgDict: dict,
-                        name: str) -> Union[str, dict]:
-    ret = {}
-    if name == 'RF':
-        if cfgDict['channel']['DDS'] is not None:
-            assert cfgDict['waveform'][
-                'DDS_LO'] is not None, 'error in config `DDS_LO.'
-            return {
-                'I': f"{section}.waveform.DDS",
-                'lofreq': cfgDict['waveform']['DDS_LO']
-            }
-        if cfgDict['channel']['I'] is not None:
-            ret['I'] = f"{section}.waveform.RF.I"
-        if cfgDict['channel']['Q'] is not None:
-            ret['Q'] = f"{section}.waveform.RF.Q"
-        ret['lofreq'] = cfgDict['setting']['LO']
-        return ret
-    elif name == 'AD.trigger':
-        return f"{section}.waveform.TRIG"
+def gateName(st):
+    if isinstance(st[0], str):
+        return st[0]
     else:
-        return f"{section}.waveform.{name}"
+        return st[0][0]
 
 
-class CompileConfigMixin(ABCCompileConfigMixin):
+class QLispError(SyntaxError):
+    pass
 
-    def _getAWGChannel(self, name,
-                       *qubits) -> Union[AWGChannel, MultAWGChannel]:
 
-        qubitsDict = [self.getQubit(q) for q in qubits]
+class MeasurementTask(NamedTuple):
+    qubit: str
+    cbit: int
+    time: float
+    signal: Signal
+    params: dict
+    hardware: Union[ADChannel, MultADChannel] = None
+    shift: float = 0
+
+
+class AWGChannel(NamedTuple):
+    name: str
+    sampleRate: float
+    size: int = -1
+    amplitude: Optional[float] = None
+    offset: Optional[float] = None
+    commandAddresses: tuple = ()
+
+
+class MultAWGChannel(NamedTuple):
+    I: Optional[AWGChannel] = None
+    Q: Optional[AWGChannel] = None
+    LO: Optional[str] = None
+    lo_freq: float = -1
+    lo_power: Optional[float] = None
+
+
+class ADChannel(NamedTuple):
+    name: str
+    sampleRate: float = 1e9
+    trigger: str = ''
+    triggerDelay: float = 0
+    triggerClockCycle: float = 8e-9
+    commandAddresses: tuple = ()
+
 
-        if name.startswith('readoutLine.'):
-            name = name.removeprefix('readoutLine.')
-            section = qubitsDict[0]['probe']
-            cfgDict = self.getReadout(section)
-        elif name.startswith('coupler.'):
-            name = name.removeprefix('coupler.')
-            section = _getSharedCoupler(qubitsDict).pop()
-            cfgDict = self.getCoupler(section)
-        else:
-            section = qubits[0]
-            cfgDict = qubitsDict[0]
-
-        chInfo = _makeAWGChannelInfo(section, cfgDict, name)
-
-        if isinstance(chInfo, str):
-            return AWGChannel(chInfo, -1)
-        else:
-            info = {'lo_freq': chInfo['lofreq']}
-            if 'I' in chInfo:
-                info['I'] = AWGChannel(chInfo['I'], -1)
-            if 'Q' in chInfo:
-                info['Q'] = AWGChannel(chInfo['Q'], -1)
-            return MultAWGChannel(**info)
+class MultADChannel(NamedTuple):
+    I: Optional[ADChannel] = None
+    Q: Optional[ADChannel] = None
+    IQ: Optional[ADChannel] = None
+    Ref: Optional[ADChannel] = None
+    LO: Optional[str] = None
+    lo_freq: float = -1
+    lo_power: Optional[float] = None
 
+
+class GateConfig(NamedTuple):
+    name: str
+    qubits: tuple
+    type: str = 'default'
+    params: dict = {}
+
+
+class ABCCompileConfigMixin(ABC):
+    """
+    Mixin for configs that can be used by compiler.
+    """
+
+    @abstractmethod
+    def _getAWGChannel(self, name,
+                       *qubits) -> Union[AWGChannel, MultAWGChannel]:
+        """
+        Get AWG channel by name and qubits.
+        """
+        pass
+
+    @abstractmethod
     def _getADChannel(self, qubit) -> Union[ADChannel, MultADChannel]:
-        rl = self.getQubit(qubit)['probe']
-        rlDict = self.getReadout(rl)
-        chInfo = {
-            'IQ': rlDict['channel']['ADC'],
-            'LO': rlDict['channel']['LO'],
-            'TRIG': rlDict['channel']['TRIG'],
-            'lofreq': rlDict['setting']['LO'],
-            'trigger':
-            f'{rl}.waveform.TRIG' if rlDict['channel']['TRIG'] else '',
-            'sampleRate': rlDict['adcsr'],
-            'triggerDelay': rlDict['setting']['TRIGD'],
-            'triggerClockCycle': rlDict['setting'].get('triggerClockCycle',
-                                                       8e-9),
-            'triggerDelayAddress': rlDict['channel'].get('DATRIGD', '')
-        }
-
-        return MultADChannel(
-            IQ=ADChannel(
-                chInfo['IQ'], chInfo['sampleRate'], chInfo['trigger'],
-                chInfo['triggerDelay'], chInfo['triggerClockCycle'],
-                (('triggerDelayAddress', chInfo['triggerDelayAddress']), )),
-            LO=chInfo['LO'],
-            lo_freq=chInfo['lofreq'],
-        )
-
-    def _getGateConfig(self, name, *qubits, type=None) -> GateConfig:
-        try:
-            gate = self.getGate(name, *qubits)
-            if not isinstance(gate, dict):
-                return None
-            qubits = gate['qubits']
-            if type is None:
-                type = gate.get('default_type', 'default')
-            if type not in gate:
-                params = gate['params']
-            else:
-                params = gate[type]
-        except:
-            type = 'default'
-            params = {}
-        return GateConfig(name, qubits, type, params)
+        """
+        Get AD channel by qubit.
+        """
+        pass
 
+    @abstractmethod
+    def _getGateConfig(self, name, *qubits) -> GateConfig:
+        """
+        Return the gate config for the given qubits.
+
+        Args:
+            name: Name of the gate.
+            qubits: Qubits to which the gate is applied.
+        
+        Returns:
+            GateConfig for the given qubits.
+            if the gate is not found, return None.
+        """
+        pass
+
+    @abstractmethod
     def _getAllQubitLabels(self) -> list[str]:
-        return self.keys('Q*')
+        """
+        Return all qubit labels.
+        """
+        pass
 
 
-class LocalConfig(ConfigProxy, CompileConfigMixin):
+__config_factory = None
 
-    def __init__(self, data) -> None:
-        self._history = None
-        self.__driver = DictDriver(copy.deepcopy(data))
-
-    def query(self, q):
-        return self.__driver.query(q)
-
-    def keys(self, pattern='*'):
-        return self.__driver.keys(pattern)
-
-    def update(self, q, v, cache=False):
-        self.__driver.update_many({q: v})
-
-    def getQubit(self, name):
-        return self.query(name)
-
-    def getCoupler(self, name):
-        return self.query(name)
-
-    def getReadout(self, name):
-        return self.query(name)
-
-    def getReadoutLine(self, name):
-        return self.query(name)
-
-    def getGate(self, name, *qubits):
-        order_senstive = self.query(f"gate.{name}.__order_senstive__")
-        if order_senstive is None:
-            order_senstive = True
-        if len(qubits) == 1 or order_senstive:
-            ret = self.query(f"gate.{name}.{'_'.join(qubits)}")
-            if isinstance(ret, dict):
-                ret['qubits'] = tuple(qubits)
-                return ret
-            else:
-                raise Exception(f"gate {name} of {qubits} not calibrated.")
-        else:
-            for qlist in permutations(qubits):
-                try:
-                    ret = self.query(f"gate.{name}.{'_'.join(qlist)}")
-                    if isinstance(ret, dict):
-                        ret['qubits'] = tuple(qlist)
-                        return ret
-                except:
-                    break
-            raise Exception(f"gate {name} of {qubits} not calibrated.")
 
-    def clear_buffer(self):
-        pass
+def set_config_factory(factory):
+    global __config_factory
+    __config_factory = factory
+
+
+def getConfig() -> ABCCompileConfigMixin:
+    if __config_factory is None:
+        raise FileNotFoundError(
+            'set_config_factory(factory) must be run first.')
+    else:
+        return __config_factory()
+
+
+@dataclass
+class Context():
+    cfg: ABCCompileConfigMixin = field(default_factory=getConfig)
+    scopes: list[dict[str, Any]] = field(default_factory=lambda: [dict()])
+    qlisp: list = field(default_factory=list)
+    time: dict[str,
+               float] = field(default_factory=lambda: defaultdict(lambda: 0))
+    addressTable: dict = field(default_factory=dict)
+    waveforms: dict[str, Waveform] = field(
+        default_factory=lambda: defaultdict(zero))
+    raw_waveforms: dict[tuple[str, ...], Waveform] = field(
+        default_factory=lambda: defaultdict(zero))
+    measures: dict[int, MeasurementTask] = field(default_factory=dict)
+    phases_ext: dict[str, dict[Union[int, str], float]] = field(
+        default_factory=lambda: defaultdict(lambda: defaultdict(lambda: 0)))
+    biases: dict[str,
+                 float] = field(default_factory=lambda: defaultdict(lambda: 0))
+    end: float = 0
+
+    @property
+    def channel(self):
+        return self.raw_waveforms
+
+    @property
+    def phases(self):
+
+        class D():
+            __slots__ = ('ctx', )
+
+            def __init__(self, ctx):
+                self.ctx = ctx
+
+            def __getitem__(self, qubit):
+                return self.ctx.phases_ext[qubit][1] - self.ctx.phases_ext[
+                    qubit][0]
+
+            def __setitem__(self, qubit, phase):
+                self.ctx.phases_ext[qubit][
+                    1] = phase + self.ctx.phases_ext[qubit][0]
+
+        return D(self)
+
+    @property
+    def params(self):
+        return self.scopes[-1]
+
+    @property
+    def vars(self):
+        return self.scopes[-2]
+
+    @property
+    def globals(self):
+        return self.scopes[0]
+
+    def qubit(self, q):
+        return self.addressTable[q]
+
+
+@dataclass
+class QLispCode():
+    cfg: ABCCompileConfigMixin = field(repr=False)
+    qlisp: list = field(repr=True)
+    waveforms: dict[str, Waveform] = field(repr=True)
+    measures: dict[int, list[MeasurementTask]] = field(repr=True)
+    end: float = field(default=0, repr=True)
+    signal: Signal = Signal.state
+    shots: int = 1024
+    arch: str = 'general'
+    cbit_alias: dict[int, tuple[int, int]] = field(default_factory=dict)
+    sub_code_count: int = 0
+
+
+def set_context_factory(factory):
+    warnings.warn('set_context_factory is deprecated', DeprecationWarning, 2)
+
+
+def create_context(ctx: Optional[Context] = None, **kw) -> Context:
+    if ctx is None:
+        return Context(**kw)
+    else:
+        if 'cfg' not in kw:
+            kw['cfg'] = ctx.cfg
+        sub_ctx = Context(**kw)
+        sub_ctx.time.update(ctx.time)
+        #sub_ctx.phases.update(ctx.phases)
+        sub_ctx.biases.update(ctx.biases)
+        for k, v in ctx.phases_ext.items():
+            sub_ctx.phases_ext[k].update(v)
 
-    def export(self):
-        return copy.deepcopy(self.__driver.dct)
+        return sub_ctx
```

### Comparing `waveforms-1.5.95/waveforms/qlisp/assembly.py` & `waveforms-1.5.96/waveforms/qlisp/assembly.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/commands.py` & `waveforms-1.5.96/waveforms/qlisp/commands.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/compiler.py` & `waveforms-1.5.96/waveforms/qlisp/compiler.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/config.py` & `waveforms-1.5.96/waveforms/qlisp/config.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/interpreter.py` & `waveforms-1.5.96/waveforms/qlisp/interpreter.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/library.py` & `waveforms-1.5.96/waveforms/qlisp/library.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/libs/__init__.py` & `waveforms-1.5.96/waveforms/qlisp/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/macro.py` & `waveforms-1.5.96/waveforms/qlisp/macro.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/parse.py` & `waveforms-1.5.96/waveforms/qlisp/parse.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/prog.py` & `waveforms-1.5.96/waveforms/qlisp/prog.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/__init__.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/eval.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/eval.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/exceptions.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/exceptions.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/libs/qelib1.inc` & `waveforms-1.5.96/waveforms/qlisp/qasm/libs/qelib1.inc`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/__init__.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/barrier.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/barrier.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/binaryop.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/binaryop.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/binaryoperator.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/binaryoperator.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/creg.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/creg.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/customunitary.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/customunitary.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/expressionlist.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/expressionlist.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/external.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/external.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/format.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/format.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/gate.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/gate.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/gatebody.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/gatebody.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/id.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/id.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/idlist.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/idlist.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/if_.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/if_.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/indexedid.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/indexedid.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/intnode.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/intnode.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/measure.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/measure.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/node.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/node.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/nodeexception.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/nodeexception.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/opaque.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/opaque.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/prefix.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/prefix.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/primarylist.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/primarylist.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/program.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/program.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/qreg.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/qreg.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/real.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/real.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/reset.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/reset.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/node/unaryoperator.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/node/unaryoperator.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/qasm.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/qasm.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/qasmlexer.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/qasmlexer.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qasm/qasmparser.py` & `waveforms-1.5.96/waveforms/qlisp/qasm/qasmparser.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/qc/assembler.py` & `waveforms-1.5.96/waveforms/waveform_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,60 @@
 import tempfile
 from ast import literal_eval
 from functools import lru_cache
 
 import ply.lex as lex
 import ply.yacc as yacc
 
+from . import waveform
+
+
+class _WaveLexer:
+    """Waveform Lexer.
+    """
 
-class _Lexer:
     def __init__(self):
         """Create a PLY lexer."""
         self.lexer = lex.lex(module=self, debug=False)
 
     def input(self, data):
         self.lexer.input(data)
 
     def token(self):
         """Return the next token."""
         ret = self.lexer.token()
         return ret
 
     literals = r'=()[]<>,.+-/*^'
     functions = [
-        'D', 'chirp', 'const', 'cos', 'cosPulse', 'cut', 'exp', 'gaussian',
-        'general_cosine', 'hanning', 'interp', 'mixing', 'one', 'poly',
-        'samplingPoints', 'sign', 'sin', 'sinc', 'square', 'step', 'zero'
+        'D', 'chirp', 'const', 'cos', 'cosh', 'coshPulse', 'cosPulse', 'cut',
+        'exp', 'gaussian', 'general_cosine', 'hanning', 'interp', 'mixing',
+        'one', 'poly', 'samplingPoints', 'sign', 'sin', 'sinc', 'sinh',
+        'square', 'step', 'zero'
     ]
     tokens = [
-        'PUSH', 'POP', 'DUP', 'INT', 'STRING', 'ID', 'LSHIFT', 'RSHIFT', 'POW',
+        'REAL', 'IMAG', 'INT', 'STRING', 'ID', 'LSHIFT', 'RSHIFT', 'POW',
+        'CONST', 'FUNCTION'
     ]
 
     def t_ID(self, t):
         r'[a-zA-Z_][a-zA-Z_0-9]*'
         if t.value in ['pi', 'e', 'inf']:
             t.type = 'CONST'
             return t
         if t.value in self.functions:
             t.type = 'FUNCTION'
             return t
         else:
             return t
 
+    def t_IMAG(self, t):
+        r'((([0-9]+|([0-9]+)?\.[0-9]+|[0-9]+\.)[eE][+-]?[0-9]+)|(([0-9]+)?\.[0-9]+|[0-9]+\.)|[1-9][0-9]*|0)j'
+        return t
+
     def t_REAL(self, t):
         r'(([0-9]+|([0-9]+)?\.[0-9]+|[0-9]+\.)[eE][+-]?[0-9]+)|(([0-9]+)?\.[0-9]+|[0-9]+\.)'
         return t
 
     def t_INT(self, t):
         r'[1-9][0-9]*|0'
         return t
@@ -70,18 +81,18 @@
     t_ignore = ' \t\r\n'
 
     def t_error(self, t):
         raise SyntaxError("Unable to match any token rule, got -->%s<-- " %
                           t.value)
 
 
-class _Parser:
+class _WaveParser:
 
     def __init__(self):
-        self.lexer = _Lexer()
+        self.lexer = _WaveLexer()
         self.tokens = self.lexer.tokens
         self.parse_dir = tempfile.mkdtemp(prefix='waveforms')
         self.precedence = (('left', 'RSHIFT', 'LSHIFT'), ('left', '+', '-'),
                            ('left', '*', '/'), ('left', 'POW',
                                                 '^'), ('right', 'UMINUS'))
         self.parser = yacc.yacc(module=self,
                                 debug=False,
@@ -112,17 +123,18 @@
 
     def p_const(self, p):
         """
         expression : CONST
         """
         p[0] = {'pi': waveform.pi, 'e': waveform.e, 'inf': waveform.inf}[p[1]]
 
-    def p_real_int_string(self, p):
+    def p_real_imag_int_string(self, p):
         """
         expression : REAL
+                   | IMAG
                    | INT
                    | STRING
         """
         p[0] = literal_eval(p[1])
 
     def p_tuple_list(self, p):
         """
@@ -253,26 +265,16 @@
             p[0] = kwds
             # p[0] = p[1] | {p[3]: p[5]}   # only works on Python>=3.9
 
     def p_error(self, p):
         raise SyntaxError("Syntax error in input!")
 
 
-__parser = _Parser()
+_wave_parser = _WaveParser()
 
 
 @lru_cache(maxsize=1024)
 def wave_eval(expr: str) -> waveform.Waveform:
     try:
-        return __parser.parse(expr)
+        return _wave_parser.parse(expr)
     except:
         raise SyntaxError(f"Illegal expression '{expr}'")
-
-
-
-"""
-PUSH 1
-PUSH 2
-ADD
-PUSH 3
-PUSH 4
-"""
```

### Comparing `waveforms-1.5.95/waveforms/qlisp/simulator/__init__.py` & `waveforms-1.5.96/waveforms/qlisp/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/simulator/mat.py` & `waveforms-1.5.96/waveforms/qlisp/simulator/mat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/simulator/simple.py` & `waveforms-1.5.96/waveforms/qlisp/simulator/simple.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/tokenize.py` & `waveforms-1.5.96/waveforms/qlisp/tokenize.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/qlisp/utils.py` & `waveforms-1.5.96/waveforms/qlisp/utils.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/quantum/clifford/clifford.py` & `waveforms-1.5.96/waveforms/quantum/clifford/clifford.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/quantum/clifford/db.py` & `waveforms-1.5.96/waveforms/quantum/clifford/db.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/quantum/clifford/mat.py` & `waveforms-1.5.96/waveforms/quantum/clifford/mat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/quantum/clifford/seq2mat.py` & `waveforms-1.5.96/waveforms/quantum/clifford/seq2mat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/quantum/math.py` & `waveforms-1.5.96/waveforms/quantum/math.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/quantum/rb.py` & `waveforms-1.5.96/waveforms/quantum/rb.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/quantum/tomo.py` & `waveforms-1.5.96/waveforms/quantum/tomo.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/quantum/transmon.py` & `waveforms-1.5.96/waveforms/quantum/transmon.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/quantum/xeb.py` & `waveforms-1.5.96/waveforms/quantum/xeb.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/registry.py` & `waveforms-1.5.96/waveforms/registry.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/scan_iter.py` & `waveforms-1.5.96/waveforms/scan_iter.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/security/verify.py` & `waveforms-1.5.96/waveforms/security/verify.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/server/__init__.py` & `waveforms-1.5.96/waveforms/server/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/server/__main__.py` & `waveforms-1.5.96/waveforms/server/__main__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/server/umsgpack.py` & `waveforms-1.5.96/waveforms/server/umsgpack.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/sys/chat.py` & `waveforms-1.5.96/waveforms/sys/chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import dataclasses
 import logging
 import pickle
+import re
 import time
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 from pathlib import Path
 from random import shuffle
 from typing import Any, List, Optional, TypedDict
 
 import numpy as np
 import openai
+import tenacity
 import tiktoken
 from IPython import get_ipython
 from IPython.display import Markdown, display
-from openai.error import APIError, RateLimitError, Timeout
+from openai.error import APIError, RateLimitError, Timeout, ServiceUnavailableError, APIConnectionError
 from scipy import spatial
 
 logger = logging.getLogger(__name__)
 
 
 class Message(TypedDict):
     """OpenAI Message object containing a role and the message content"""
@@ -151,14 +153,19 @@
         next_message_to_add_index,
         current_tokens_used,
         insertion_index,
         current_context,
     )
 
 
+@tenacity.retry(wait=tenacity.wait_exponential(multiplier=1, min=4, max=10),
+                stop=tenacity.stop_after_attempt(5),
+                retry=tenacity.retry_if_exception_type(
+                    (RateLimitError, APIError, Timeout,
+                     ServiceUnavailableError, APIConnectionError)))
 def create_chat_completion(
     messages: List[Message],  # type: ignore
     model: Optional[str] = None,
     temperature: float = 0.9,
     max_tokens: Optional[int] = None,
 ) -> str:
     """Create a chat completion using the OpenAI API
@@ -168,47 +175,29 @@
         model (str, optional): The model to use. Defaults to None.
         temperature (float, optional): The temperature to use. Defaults to 0.9.
         max_tokens (int, optional): The max tokens to use. Defaults to None.
 
     Returns:
         str: The response from the chat completion
     """
-
-    num_retries = 10
-    warned_user = False
-    response = None
-    for attempt in range(num_retries):
-        backoff = 2**(attempt + 2)
-        try:
-            response = openai.ChatCompletion.create(
-                model=model,
-                messages=messages,
-                temperature=temperature,
-                max_tokens=max_tokens,
-            )
-            break
-        except RateLimitError:
-            if not warned_user:
-                logger.warn(
-                    f"Please double check that you have setup a PAID OpenAI API Account. "
-                )
-                warned_user = True
-        except (APIError, Timeout) as e:
-            if e.http_status != 502:
-                raise
-            if attempt == num_retries - 1:
-                raise
-        time.sleep(backoff)
-    if response is None:
-        logger.error("FAILED TO GET RESPONSE FROM OPENAI")
-        quit(1)
+    response = openai.ChatCompletion.create(
+        model=model,
+        messages=messages,
+        temperature=temperature,
+        max_tokens=max_tokens,
+    )
     resp = response.choices[0].message["content"]
     return resp
 
 
+@tenacity.retry(wait=tenacity.wait_exponential(multiplier=1, min=4, max=10),
+                stop=tenacity.stop_after_attempt(5),
+                retry=tenacity.retry_if_exception_type(
+                    (RateLimitError, APIError, Timeout,
+                     ServiceUnavailableError, APIConnectionError)))
 def get_embedding(
     text: str,
     *_,
     model: str = EMBEDDING_MODEL,
     **kwargs,
 ) -> List[float]:
     """Create an embedding using the OpenAI API
@@ -247,106 +236,98 @@
         summary (str): The summary of the conversation so far.
         model (str): The name of the model to use for tokenization.
         token_limit (int): The maximum number of tokens allowed in the API call.
 
     Returns:
         str: The AI's response.
     """
-    while True:
-        try:
-            # Reserve 1000 tokens for the response
 
-            if token_limit is None:
-                token_limit = token_limits(model)
+    # Reserve 1000 tokens for the response
 
-            logger.debug(f"Token limit: {token_limit}")
-            send_token_limit = token_limit - 1000
-            if len(full_message_history) == 0:
-                relevant_memory = ""
-            else:
-                recent_history = full_message_history[-5:]
-                shuffle(recent_history)
-                relevant_memories = permanent_memory.get_relevant(
-                    str(recent_history), 5)
-                if relevant_memories:
-                    shuffle(relevant_memories)
-                relevant_memory = str(relevant_memories)
-
-            logger.debug(f"Memory Stats: {permanent_memory.get_stats()}")
-
-            (
-                next_message_to_add_index,
-                current_tokens_used,
-                insertion_index,
-                current_context,
-            ) = generate_context(prompt, relevant_memory, full_message_history,
-                                 model, summary)
-
-            while current_tokens_used > 2500:
-                # remove memories until we are under 2500 tokens
-                relevant_memory = relevant_memory[:-1]
-                (
-                    next_message_to_add_index,
-                    current_tokens_used,
-                    insertion_index,
-                    current_context,
-                ) = generate_context(prompt, relevant_memory,
-                                     full_message_history, model, summary)
-
-            current_tokens_used += count_message_tokens(
-                [create_chat_message("user", user_input)],
-                model)  # Account for user input (appended later)
-
-            while next_message_to_add_index >= 0:
-                # print (f"CURRENT TOKENS USED: {current_tokens_used}")
-                message_to_add = full_message_history[
-                    next_message_to_add_index]
-
-                tokens_to_add = count_message_tokens([message_to_add], model)
-                if current_tokens_used + tokens_to_add > send_token_limit:
-                    break
-
-                # Add the most recent message to the start of the current context,
-                #  after the two system prompts.
-                current_context.insert(
-                    insertion_index,
-                    full_message_history[next_message_to_add_index])
-
-                # Count the currently used tokens
-                current_tokens_used += tokens_to_add
-
-                # Move to the next most recent message in the full message history
-                next_message_to_add_index -= 1
-
-            # Append user input, the length of this is accounted for above
-            current_context.extend([create_chat_message("user", user_input)])
-
-            # Calculate remaining tokens
-            tokens_remaining = token_limit - current_tokens_used
-            # assert tokens_remaining >= 0, "Tokens remaining is negative.
-
-            # TODO: use a model defined elsewhere, so that model can contain
-            # temperature and other settings we care about
-            assistant_reply = create_chat_completion(
-                model=model,
-                messages=current_context,
-                max_tokens=tokens_remaining,
-            )
-
-            # Update full message history
-            full_message_history.append(create_chat_message(
-                "user", user_input))
-            full_message_history.append(
-                create_chat_message("assistant", assistant_reply))
-
-            return assistant_reply
-        except RateLimitError:
-            # TODO: When we switch to langchain, this is built in
-            print("Error: ", "API Rate Limit Reached. Waiting 10 seconds...")
-            time.sleep(10)
+    if token_limit is None:
+        token_limit = token_limits(model)
+
+    logger.debug(f"Token limit: {token_limit}")
+    send_token_limit = token_limit - 1000
+    if len(full_message_history) == 0:
+        relevant_memory = ""
+    else:
+        recent_history = full_message_history[-5:]
+        shuffle(recent_history)
+        relevant_memories = permanent_memory.get_relevant(
+            str(recent_history), 5)
+        if relevant_memories:
+            shuffle(relevant_memories)
+        relevant_memory = str(relevant_memories)
+
+    logger.debug(f"Memory Stats: {permanent_memory.get_stats()}")
+
+    (
+        next_message_to_add_index,
+        current_tokens_used,
+        insertion_index,
+        current_context,
+    ) = generate_context(prompt, relevant_memory, full_message_history, model,
+                         summary)
+
+    while current_tokens_used > 2500:
+        # remove memories until we are under 2500 tokens
+        relevant_memory = relevant_memory[:-1]
+        (
+            next_message_to_add_index,
+            current_tokens_used,
+            insertion_index,
+            current_context,
+        ) = generate_context(prompt, relevant_memory, full_message_history,
+                             model, summary)
+
+    current_tokens_used += count_message_tokens(
+        [create_chat_message("user", user_input)],
+        model)  # Account for user input (appended later)
+
+    while next_message_to_add_index >= 0:
+        # print (f"CURRENT TOKENS USED: {current_tokens_used}")
+        message_to_add = full_message_history[next_message_to_add_index]
+
+        tokens_to_add = count_message_tokens([message_to_add], model)
+        if current_tokens_used + tokens_to_add > send_token_limit:
+            break
+
+        # Add the most recent message to the start of the current context,
+        #  after the two system prompts.
+        current_context.insert(insertion_index,
+                               full_message_history[next_message_to_add_index])
+
+        # Count the currently used tokens
+        current_tokens_used += tokens_to_add
+
+        # Move to the next most recent message in the full message history
+        next_message_to_add_index -= 1
+
+    # Append user input, the length of this is accounted for above
+    current_context.extend([create_chat_message("user", user_input)])
+
+    # Calculate remaining tokens
+    tokens_remaining = token_limit - current_tokens_used
+    # assert tokens_remaining >= 0, "Tokens remaining is negative.
+
+    # TODO: use a model defined elsewhere, so that model can contain
+    # temperature and other settings we care about
+    assistant_reply = create_chat_completion(
+        model=model,
+        messages=current_context,
+        max_tokens=tokens_remaining,
+    )
+
+    # Update full message history
+    full_message_history.append(create_chat_message("user", user_input))
+    full_message_history.append(
+        create_chat_message("assistant", assistant_reply))
+
+    return assistant_reply
 
 
 def create_default_embeddings():
     return np.zeros((0, EMBED_DIM)).astype(np.float32)
 
 
 @dataclasses.dataclass
@@ -533,67 +514,50 @@
         self._save_future = None
 
     def __del__(self):
         if self._save_future is not None:
             self._save_future.result()
         self._pool.shutdown()
 
-    def _completion(self,
-                    messages,
-                    model=None,
-                    temperature=1.0,
-                    top_p=1.0,
-                    n=1):
-        if model is None:
-            model = self.model
-        completion = openai.ChatCompletion.create(model=model,
-                                                  messages=messages,
-                                                  temperature=temperature,
-                                                  top_p=top_p,
-                                                  n=n)
-        self.last_time = datetime.now()
-        return completion.choices[0].message
-
-    def _completion_stream(self, messages, temperature=1.0, top_p=1.0, n=1):
-        completion = openai.ChatCompletion.create(model=self.model,
-                                                  messages=messages,
-                                                  temperature=temperature,
-                                                  top_p=top_p,
-                                                  n=n,
-                                                  stream=True)
-        for choice in completion.choices:
-            yield choice.message
+    def _validate_title(self, title: str) -> str:
+        rstr = f"[\\/:*?\"<>|\n\r\t]+"
+        title = re.sub(rstr, " ", title)
+        title = title.strip()
+        if len(title) > 100:
+            title = title[:100]
+        while title[-1] in ' .。,，-_':
+            title = title[:-1]
+        return title
 
     def make_title(self):
         messages = [{
             "role": "system",
             "content": 'You are a helpful assistant.'
         }]
 
         tokens = count_string_tokens(messages[0]['content'], self.model)
 
         query = ("请根据以下对话内容，总结出中文标题，长度不超过100个字符。"
-                 "请注意，标题中不得包含任何不能用于文件路径的字符，并且不包含额外内容和结尾的句号。\n"
+                 "请注意，标题必须是合法的文件名，省略结尾的句号。返回结果不得包含额外的解释和格式。\n"
                  "对话内容：\n")
 
         text = []
         for msg in self.history:
             text.append(f'{msg["role"]} :\n<quote>{msg["content"]}</quote>')
             tokens += count_string_tokens(query + '\n'.join(text), self.model)
             if tokens > token_limits(self.model) - 500:
                 text.pop()
                 break
         messages.append({"role": "user", "content": query + '\n'.join(text)})
 
         try:
-            message = self._completion(messages)
-            content = message['content']
-            if len(content) > 100:
-                content = content[:100]
-            return f"{time.strftime('%Y%m%d%H%M%S')} {content}"
+            self.last_time = datetime.now()
+            content = create_chat_completion(messages, self.model)
+            title = self._validate_title(content)
+            return f"{time.strftime('%Y%m%d%H%M%S')} {title}"
         except:
             return f"{time.strftime('%Y%m%d%H%M%S')} untitled"
 
     def ask(self, query):
         self.last_time = datetime.now()
 
         reply = chat_with_ai(self.system_prompt, query, self.history,
```

### Comparing `waveforms-1.5.95/waveforms/sys/device/basedevice.py` & `waveforms-1.5.96/waveforms/sys/device/basedevice.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/sys/device/loader.py` & `waveforms-1.5.96/waveforms/sys/device/loader.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/sys/device/utils.py` & `waveforms-1.5.96/waveforms/sys/device/utils.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/sys/drivers/FakeInstrument.py` & `waveforms-1.5.96/waveforms/sys/drivers/FakeInstrument.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/sys/ipy_events.py` & `waveforms-1.5.96/waveforms/sys/ipy_events.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/sys/net/dhcp.py` & `waveforms-1.5.96/waveforms/sys/net/dhcp.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/sys/net/dhcpd.py` & `waveforms-1.5.96/waveforms/sys/net/dhcpd.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/sys/net/kad.py` & `waveforms-1.5.96/waveforms/sys/net/kad.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/sys/net/kcp.py` & `waveforms-1.5.96/waveforms/sys/net/kcp.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/sys/progress.py` & `waveforms-1.5.96/waveforms/sys/progress.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/sys/storage/crud.py` & `waveforms-1.5.96/waveforms/sys/storage/crud.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/sys/storage/models.py` & `waveforms-1.5.96/waveforms/sys/storage/models.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/units/__init__.py` & `waveforms-1.5.96/waveforms/units/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/visualization/__init__.py` & `waveforms-1.5.96/waveforms/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/visualization/plot_layout.py` & `waveforms-1.5.96/waveforms/visualization/plot_layout.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/visualization/plot_seq.py` & `waveforms-1.5.96/waveforms/visualization/plot_seq.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms/waveform.py` & `waveforms-1.5.96/waveforms/waveform.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.95/waveforms.egg-info/PKG-INFO` & `waveforms-1.5.96/waveforms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveforms
-Version: 1.5.95
+Version: 1.5.96
 Summary: Edit waveforms used in experiment
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/feihoo87/waveforms
 Project-URL: Bug Reports, https://github.com/feihoo87/waveforms/issues
 Project-URL: Source, https://github.com/feihoo87/waveforms/
```

