# Comparing `tmp/virt-firmware-23.4.tar.gz` & `tmp/virt-firmware-23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virt-firmware-23.4.tar", last modified: Fri Apr 14 07:50:34 2023, max compression
+gzip compressed data, was "virt-firmware-23.5.tar", last modified: Thu May  4 08:06:41 2023, max compression
```

## Comparing `virt-firmware-23.4.tar` & `virt-firmware-23.5.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.054046 virt-firmware-23.4/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    18012 2022-04-20 16:46:39.000000 virt-firmware-23.4/LICENSE
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      116 2023-01-26 11:26:15.000000 virt-firmware-23.4/MANIFEST.in
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2532 2023-04-14 07:50:34.054046 virt-firmware-23.4/PKG-INFO
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     2199 2022-07-18 11:50:43.000000 virt-firmware-23.4/README.md
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.048045 virt-firmware-23.4/experimental/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1820 2023-01-11 05:55:56.000000 virt-firmware-23.4/experimental/dbxupdate.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     8627 2023-03-03 09:52:27.000000 virt-firmware-23.4/experimental/measure.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.048045 virt-firmware-23.4/man/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      939 2023-04-14 07:21:17.000000 virt-firmware-23.4/man/virt-fw-dump.1
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      223 2022-10-05 11:46:37.000000 virt-firmware-23.4/man/virt-fw-dump.inc
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      734 2023-04-14 07:21:18.000000 virt-firmware-23.4/man/virt-fw-sigdb.1
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       45 2022-10-05 11:46:32.000000 virt-firmware-23.4/man/virt-fw-sigdb.inc
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4317 2023-04-14 07:21:18.000000 virt-firmware-23.4/man/virt-fw-vars.1
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      515 2022-10-05 11:55:41.000000 virt-firmware-23.4/man/virt-fw-vars.inc
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)       81 2022-03-30 09:41:51.000000 virt-firmware-23.4/pyproject.toml
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1027 2023-04-14 07:50:34.055045 virt-firmware-23.4/setup.cfg
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)       69 2022-03-30 09:41:51.000000 virt-firmware-23.4/setup.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.049045 virt-firmware-23.4/tests/
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.049045 virt-firmware-23.4/tests/data/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     3737 2022-11-24 12:28:42.000000 virt-firmware-23.4/tests/data/DBXUpdate-20100307.x64.bin
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1772 2022-05-11 20:36:49.000000 virt-firmware-23.4/tests/data/secboot.aws
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      345 2022-12-02 08:59:55.000000 virt-firmware-23.4/tests/test-dump.sh
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      271 2023-04-14 07:25:30.000000 virt-firmware-23.4/tests/test-pe.sh
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      185 2022-09-02 08:19:03.000000 virt-firmware-23.4/tests/test-sigdb.sh
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      689 2022-09-02 08:10:06.000000 virt-firmware-23.4/tests/test-vars.sh
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     3687 2022-12-07 13:29:04.000000 virt-firmware-23.4/tests/tests.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.046046 virt-firmware-23.4/virt/
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.050046 virt-firmware-23.4/virt/firmware/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      130 2022-11-10 08:06:38.000000 virt-firmware-23.4/virt/firmware/__init__.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.050046 virt-firmware-23.4/virt/firmware/aws/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    11381 2022-05-11 20:36:49.000000 virt-firmware-23.4/virt/firmware/aws/dict.v0
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.052045 virt-firmware-23.4/virt/firmware/certs/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4323 2022-07-07 16:26:41.000000 virt-firmware-23.4/virt/firmware/certs/CentOSSecureBootCA2.pem
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4339 2022-07-07 16:26:41.000000 virt-firmware-23.4/virt/firmware/certs/CentOSSecureBootCAkey1.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6739 2022-03-30 10:39:05.000000 virt-firmware-23.4/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6869 2022-03-30 10:39:05.000000 virt-firmware-23.4/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6698 2022-03-30 10:39:05.000000 virt-firmware-23.4/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4615 2022-07-07 08:32:28.000000 virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootCA3.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4431 2022-07-07 08:32:38.000000 virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootCA5.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4324 2022-07-07 08:32:47.000000 virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootCA6.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4500 2022-03-30 10:39:05.000000 virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5007 2022-07-16 16:13:52.000000 virt-firmware-23.4/virt/firmware/certs/fedoraca-20200709.pem
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)    21024 2023-01-11 05:55:56.000000 virt-firmware-23.4/virt/firmware/dump.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.053045 virt-firmware-23.4/virt/firmware/efi/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      110 2022-03-30 11:58:43.000000 virt-firmware-23.4/virt/firmware/efi/__init__.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     2774 2022-12-07 13:30:17.000000 virt-firmware-23.4/virt/firmware/efi/certs.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5109 2023-03-24 08:04:11.000000 virt-firmware-23.4/virt/firmware/efi/devpath.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1663 2022-12-14 07:11:30.000000 virt-firmware-23.4/virt/firmware/efi/efijson.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    17855 2023-03-27 15:52:53.000000 virt-firmware-23.4/virt/firmware/efi/efivar.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5173 2022-12-02 08:15:31.000000 virt-firmware-23.4/virt/firmware/efi/guids.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6167 2023-04-13 11:19:16.000000 virt-firmware-23.4/virt/firmware/efi/siglist.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1379 2022-03-30 10:39:05.000000 virt-firmware-23.4/virt/firmware/efi/ucs16.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1434 2023-01-11 05:55:56.000000 virt-firmware-23.4/virt/firmware/host.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1689 2023-01-11 05:55:56.000000 virt-firmware-23.4/virt/firmware/migrate.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      494 2022-05-11 20:36:49.000000 virt-firmware-23.4/virt/firmware/misc.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1588 2023-01-11 05:55:56.000000 virt-firmware-23.4/virt/firmware/sigdb.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)    13202 2023-04-13 10:13:39.000000 virt-firmware-23.4/virt/firmware/vars.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.053045 virt-firmware-23.4/virt/firmware/varstore/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       66 2023-03-03 10:32:41.000000 virt-firmware-23.4/virt/firmware/varstore/__init__.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5423 2022-11-24 13:01:24.000000 virt-firmware-23.4/virt/firmware/varstore/aws.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6271 2023-04-13 10:23:09.000000 virt-firmware-23.4/virt/firmware/varstore/edk2.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1400 2022-03-30 10:39:05.000000 virt-firmware-23.4/virt/firmware/varstore/linux.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.053045 virt-firmware-23.4/virt/peutils/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       60 2022-12-14 09:40:14.000000 virt-firmware-23.4/virt/peutils/__init__.py
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)     8733 2023-04-13 11:51:41.000000 virt-firmware-23.4/virt/peutils/peutils.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.054046 virt-firmware-23.4/virt_firmware.egg-info/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2532 2023-04-14 07:50:34.000000 virt-firmware-23.4/virt_firmware.egg-info/PKG-INFO
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1683 2023-04-14 07:50:34.000000 virt-firmware-23.4/virt_firmware.egg-info/SOURCES.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)        1 2023-04-14 07:50:34.000000 virt-firmware-23.4/virt_firmware.egg-info/dependency_links.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      358 2023-04-14 07:50:34.000000 virt-firmware-23.4/virt_firmware.egg-info/entry_points.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       31 2023-04-14 07:50:34.000000 virt-firmware-23.4/virt_firmware.egg-info/requires.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       68 2023-04-14 07:50:34.000000 virt-firmware-23.4/virt_firmware.egg-info/top_level.txt
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.145242 virt-firmware-23.5/
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    18012 2022-04-20 16:46:39.000000 virt-firmware-23.5/LICENSE
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      116 2023-01-26 11:26:15.000000 virt-firmware-23.5/MANIFEST.in
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2532 2023-05-04 08:06:41.145242 virt-firmware-23.5/PKG-INFO
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     2199 2022-07-18 11:50:43.000000 virt-firmware-23.5/README.md
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.135242 virt-firmware-23.5/experimental/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     5654 2023-05-04 07:26:42.000000 virt-firmware-23.5/experimental/bootcfg.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1820 2023-01-11 05:55:56.000000 virt-firmware-23.5/experimental/dbxupdate.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     8840 2023-05-03 10:09:28.000000 virt-firmware-23.5/experimental/measure.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.136242 virt-firmware-23.5/man/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      939 2023-05-04 07:54:14.000000 virt-firmware-23.5/man/virt-fw-dump.1
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      223 2022-10-05 11:46:37.000000 virt-firmware-23.5/man/virt-fw-dump.inc
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      734 2023-05-04 07:54:14.000000 virt-firmware-23.5/man/virt-fw-sigdb.1
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       45 2022-10-05 11:46:32.000000 virt-firmware-23.5/man/virt-fw-sigdb.inc
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4317 2023-05-04 07:54:14.000000 virt-firmware-23.5/man/virt-fw-vars.1
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      515 2022-10-05 11:55:41.000000 virt-firmware-23.5/man/virt-fw-vars.inc
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)       81 2022-03-30 09:41:51.000000 virt-firmware-23.5/pyproject.toml
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1027 2023-05-04 08:06:41.145242 virt-firmware-23.5/setup.cfg
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)       69 2022-03-30 09:41:51.000000 virt-firmware-23.5/setup.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.138242 virt-firmware-23.5/tests/
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.138242 virt-firmware-23.5/tests/data/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     3737 2022-11-24 12:28:42.000000 virt-firmware-23.5/tests/data/DBXUpdate-20100307.x64.bin
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1772 2022-05-11 20:36:49.000000 virt-firmware-23.5/tests/data/secboot.aws
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      345 2022-12-02 08:59:55.000000 virt-firmware-23.5/tests/test-dump.sh
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      271 2023-04-14 07:25:30.000000 virt-firmware-23.5/tests/test-pe.sh
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      185 2022-09-02 08:19:03.000000 virt-firmware-23.5/tests/test-sigdb.sh
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      689 2022-09-02 08:10:06.000000 virt-firmware-23.5/tests/test-vars.sh
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     3687 2022-12-07 13:29:04.000000 virt-firmware-23.5/tests/tests.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.134242 virt-firmware-23.5/virt/
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.139242 virt-firmware-23.5/virt/firmware/
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      130 2022-11-10 08:06:38.000000 virt-firmware-23.5/virt/firmware/__init__.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.139242 virt-firmware-23.5/virt/firmware/aws/
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    11381 2022-05-11 20:36:49.000000 virt-firmware-23.5/virt/firmware/aws/dict.v0
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.142242 virt-firmware-23.5/virt/firmware/certs/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4323 2022-07-07 16:26:41.000000 virt-firmware-23.5/virt/firmware/certs/CentOSSecureBootCA2.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4339 2022-07-07 16:26:41.000000 virt-firmware-23.5/virt/firmware/certs/CentOSSecureBootCAkey1.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6739 2022-03-30 10:39:05.000000 virt-firmware-23.5/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6869 2022-03-30 10:39:05.000000 virt-firmware-23.5/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6698 2022-03-30 10:39:05.000000 virt-firmware-23.5/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4615 2022-07-07 08:32:28.000000 virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootCA3.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4431 2022-07-07 08:32:38.000000 virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootCA5.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4324 2022-07-07 08:32:47.000000 virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootCA6.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4500 2022-03-30 10:39:05.000000 virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5007 2022-07-16 16:13:52.000000 virt-firmware-23.5/virt/firmware/certs/fedoraca-20200709.pem
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)    21517 2023-05-03 10:06:49.000000 virt-firmware-23.5/virt/firmware/dump.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.143242 virt-firmware-23.5/virt/firmware/efi/
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      123 2023-04-28 10:54:50.000000 virt-firmware-23.5/virt/firmware/efi/__init__.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1892 2023-04-28 11:18:07.000000 virt-firmware-23.5/virt/firmware/efi/bootentry.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     2774 2022-12-07 13:30:17.000000 virt-firmware-23.5/virt/firmware/efi/certs.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5109 2023-03-24 08:04:11.000000 virt-firmware-23.5/virt/firmware/efi/devpath.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1663 2022-12-14 07:11:30.000000 virt-firmware-23.5/virt/firmware/efi/efijson.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    17539 2023-04-28 11:17:30.000000 virt-firmware-23.5/virt/firmware/efi/efivar.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5173 2022-12-02 08:15:31.000000 virt-firmware-23.5/virt/firmware/efi/guids.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6167 2023-04-13 11:19:16.000000 virt-firmware-23.5/virt/firmware/efi/siglist.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1379 2022-03-30 10:39:05.000000 virt-firmware-23.5/virt/firmware/efi/ucs16.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1434 2023-01-11 05:55:56.000000 virt-firmware-23.5/virt/firmware/host.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1689 2023-01-11 05:55:56.000000 virt-firmware-23.5/virt/firmware/migrate.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      494 2022-05-11 20:36:49.000000 virt-firmware-23.5/virt/firmware/misc.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1588 2023-01-11 05:55:56.000000 virt-firmware-23.5/virt/firmware/sigdb.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)    13202 2023-04-13 10:13:39.000000 virt-firmware-23.5/virt/firmware/vars.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.144241 virt-firmware-23.5/virt/firmware/varstore/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       66 2023-03-03 10:32:41.000000 virt-firmware-23.5/virt/firmware/varstore/__init__.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5423 2022-11-24 13:01:24.000000 virt-firmware-23.5/virt/firmware/varstore/aws.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6271 2023-04-13 10:23:09.000000 virt-firmware-23.5/virt/firmware/varstore/edk2.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1707 2023-04-28 11:34:16.000000 virt-firmware-23.5/virt/firmware/varstore/linux.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.144241 virt-firmware-23.5/virt/peutils/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       60 2022-12-14 09:40:14.000000 virt-firmware-23.5/virt/peutils/__init__.py
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)     9437 2023-04-18 08:24:36.000000 virt-firmware-23.5/virt/peutils/peutils.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.145242 virt-firmware-23.5/virt_firmware.egg-info/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2532 2023-05-04 08:06:41.000000 virt-firmware-23.5/virt_firmware.egg-info/PKG-INFO
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1738 2023-05-04 08:06:41.000000 virt-firmware-23.5/virt_firmware.egg-info/SOURCES.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)        1 2023-05-04 08:06:41.000000 virt-firmware-23.5/virt_firmware.egg-info/dependency_links.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      358 2023-05-04 08:06:41.000000 virt-firmware-23.5/virt_firmware.egg-info/entry_points.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       31 2023-05-04 08:06:41.000000 virt-firmware-23.5/virt_firmware.egg-info/requires.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       68 2023-05-04 08:06:41.000000 virt-firmware-23.5/virt_firmware.egg-info/top_level.txt
```

### Comparing `virt-firmware-23.4/LICENSE` & `virt-firmware-23.5/LICENSE`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/PKG-INFO` & `virt-firmware-23.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virt-firmware
-Version: 23.4
+Version: 23.5
 Summary: tools for virtual machine firmware volumes
 Author: Gerd Hoffmann
 Author-email: kraxel@redhat.com
 License: GPLv2
 Project-URL: GitLab, https://gitlab.com/kraxel/virt-firmware
 Keywords: ovmf,armvirt,edk2,aws
 Description-Content-Type: text/markdown
```

### Comparing `virt-firmware-23.4/README.md` & `virt-firmware-23.5/README.md`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/experimental/dbxupdate.py` & `virt-firmware-23.5/experimental/dbxupdate.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/experimental/measure.py` & `virt-firmware-23.5/experimental/measure.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,21 +249,25 @@
 
     if not options.banks:
         options.banks = [ 'sha256', ]
 
     if options.image:
         with open(options.image, 'rb') as f:
             data = f.read()
+        data = dump.unqcow2(options.image, data)
         image = dump.Edk2Image(options.image, data)
         eventlog = measure_image(options.banks, image, options.version)
 
     elif options.vars:
         if edk2.Edk2VarStore.probe(options.vars):
             edk2store = edk2.Edk2VarStore(options.vars)
             varlist = edk2store.get_varlist()
+        elif edk2.Edk2VarStoreQcow2.probe(options.vars):
+            edk2store = edk2.Edk2VarStoreQcow2(options.vars)
+            varlist = edk2store.get_varlist()
         elif aws.AwsVarStore.probe(options.vars):
             awsstore = aws.AwsVarStore(options.vars)
             varlist = awsstore.get_varlist()
         else:
             logging.error("unknown input file format")
             return 1
         eventlog = measure_varlist(options.banks, varlist,
```

### Comparing `virt-firmware-23.4/man/virt-fw-dump.1` & `virt-firmware-23.5/man/virt-fw-dump.1`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/man/virt-fw-sigdb.1` & `virt-firmware-23.5/man/virt-fw-sigdb.1`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/man/virt-fw-vars.1` & `virt-firmware-23.5/man/virt-fw-vars.1`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/man/virt-fw-vars.inc` & `virt-firmware-23.5/man/virt-fw-vars.inc`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/setup.cfg` & `virt-firmware-23.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = virt-firmware
-version = 23.4
+version = 23.5
 description = tools for virtual machine firmware volumes
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = ovmf, armvirt, edk2, aws
 license = GPLv2
 license_files = LICENSE
 author = Gerd Hoffmann
```

### Comparing `virt-firmware-23.4/tests/data/DBXUpdate-20100307.x64.bin` & `virt-firmware-23.5/tests/data/DBXUpdate-20100307.x64.bin`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/tests/data/secboot.aws` & `virt-firmware-23.5/tests/data/secboot.aws`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/tests/test-vars.sh` & `virt-firmware-23.5/tests/test-vars.sh`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/tests/tests.py` & `virt-firmware-23.5/tests/tests.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/aws/dict.v0` & `virt-firmware-23.5/virt/firmware/aws/dict.v0`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/certs/CentOSSecureBootCA2.pem` & `virt-firmware-23.5/virt/firmware/certs/CentOSSecureBootCA2.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/certs/CentOSSecureBootCAkey1.pem` & `virt-firmware-23.5/virt/firmware/certs/CentOSSecureBootCAkey1.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem` & `virt-firmware-23.5/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem` & `virt-firmware-23.5/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem` & `virt-firmware-23.5/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootCA3.pem` & `virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootCA3.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootCA5.pem` & `virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootCA5.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootCA6.pem` & `virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootCA6.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem` & `virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/certs/fedoraca-20200709.pem` & `virt-firmware-23.5/virt/firmware/certs/fedoraca-20200709.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/dump.py` & `virt-firmware-23.5/virt/firmware/dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 """ dump content of ovmf firmware volumes """
 import sys
 import json
 import lzma
 import struct
 import hashlib
 import argparse
+import tempfile
+import subprocess
 import collections
 
 from virt.firmware.efi import guids
 from virt.firmware.efi import ucs16
 from virt.firmware.efi import efivar
 
 
@@ -612,14 +614,26 @@
 def print_image_data():
     print(json.dumps(jsonimgs, indent = 4, sort_keys = True))
 
 
 ########################################################################
 # main
 
+def unqcow2(filename, data):
+    (magic, version) = struct.unpack_from('>LL', data)
+    if magic != 0x514649fb:
+        return data
+    with tempfile.NamedTemporaryFile() as rawfile:
+        cmdline = [ 'qemu-img', 'convert',
+                    '-f', 'qcow2', '-O', 'raw',
+                    filename, rawfile.name ]
+        subprocess.run(cmdline, check = True)
+        filedata = rawfile.read()
+    return filedata
+
 def walk_tree(item, pfunc, indent = 0):
     inc = pfunc(item, indent)
     if isinstance(item, collections.UserList):
         for i in list(item):
             walk_tree(i, pfunc, indent + inc)
 
 def main():
@@ -647,14 +661,15 @@
     if not options.input:
         print('ERROR: no input file specified (try -h for help)')
         sys.exit(1)
 
     for filename in options.input:
         with open(filename, 'rb') as f:
             data = f.read()
+        data = unqcow2(filename, data)
         image = Edk2Image(filename, data)
 
         if options.fmt == 'all' or options.fmt is None:
             walk_tree(image, print_all)
         elif options.fmt == 'volumes':
             walk_tree(image, print_volumes)
         elif options.fmt == 'modules':
```

### Comparing `virt-firmware-23.4/virt/firmware/efi/certs.py` & `virt-firmware-23.5/virt/firmware/efi/certs.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/efi/devpath.py` & `virt-firmware-23.5/virt/firmware/efi/devpath.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/efi/efijson.py` & `virt-firmware-23.5/virt/firmware/efi/efijson.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/efi/efivar.py` & `virt-firmware-23.5/virt/firmware/efi/efivar.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 import datetime
 import collections
 
 from cryptography import x509
 
 from virt.firmware.efi import guids
 from virt.firmware.efi import ucs16
+from virt.firmware.efi import certs
 from virt.firmware.efi import devpath
 from virt.firmware.efi import siglist
-from virt.firmware.efi import certs
+from virt.firmware.efi import bootentry
 
 ##################################################################################################
 # constants
 
 # variable attributes
 EFI_VARIABLE_NON_VOLATILE                          = 0x00000001
 EFI_VARIABLE_BOOTSERVICE_ACCESS                    = 0x00000002
@@ -249,20 +250,17 @@
         self.update_time()
 
     def set_uint32(self, value):
         self.data = value.to_bytes(4, byteorder = 'little')
         self.update_time()
 
     def set_boot_entry(self, attr, title, path, optdata = None):
-        pathdata = bytes(path)
-        self.data = struct.pack('=LH', attr, len(pathdata))
-        self.data += bytes(title)
-        self.data += pathdata
-        if optdata:
-            self.data += optdata
+        entry = bootentry.BootEntry(attr = attr, title = title,
+                                    devicepath = path, optdata = optdata)
+        self.data = bytes(entry)
         self.update_time()
 
     def set_boot_next(self, index):
         self.data = struct.pack('=H', index)
         self.update_time()
 
     def append_boot_order(self, index):
@@ -276,24 +274,16 @@
 
     def fmt_ascii(self):
         string = self.data.decode().rstrip('\0')
         string = re.sub(r'\n', r'\\n', string)
         return f'ascii: "{string}"'
 
     def fmt_boot_entry(self):
-        (attr, pathsize) = struct.unpack_from('=LH', self.data)
-        name = ucs16.from_ucs16(self.data, 6)
-        path = self.data[ name.size() + 6 :
-                          name.size() + 6 + pathsize ]
-        optdata = self.data[ name.size() + 6 + pathsize : ]
-        obj = devpath.DevicePath(path)
-        string = f'boot entry: name="{name}" devpath={obj}'
-        if len(optdata):
-            string += f' optdata={optdata.hex()}'
-        return string
+        entry = bootentry.BootEntry(data = self.data)
+        return f'boot entry: {entry}'
 
     def fmt_boot_list(self):
         bootlist = []
         for pos in range(len(self.data) >> 1):
             nr = struct.unpack_from('=H', self.data, pos * 2)
             bootlist.append(f'{nr[0]:04x}')
             desc= ", ".join(bootlist)
@@ -366,15 +356,16 @@
     def set_boot_entry(self, index, title, path, optdata = None):
         name = f'Boot{index:04X}'
         var = self.get(name)
         if not var:
             var = self.create(name)
         t = ucs16.from_string(title)
         logging.info('set variable %s: %s = %s', name, t, path)
-        var.set_boot_entry(1, t, path, optdata)
+        var.set_boot_entry(bootentry.LOAD_OPTION_ACTIVE,
+                           t, path, optdata)
 
     def add_boot_entry(self, title, path, optdata = None):
         for index in range(0xffff):
             name = f'Boot{index:04X}'
             var = self.get(name)
             if not var:
                 self.set_boot_entry(index, title, path, optdata)
```

### Comparing `virt-firmware-23.4/virt/firmware/efi/guids.py` & `virt-firmware-23.5/virt/firmware/efi/guids.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/efi/siglist.py` & `virt-firmware-23.5/virt/firmware/efi/siglist.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/efi/ucs16.py` & `virt-firmware-23.5/virt/firmware/efi/ucs16.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/host.py` & `virt-firmware-23.5/virt/firmware/host.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/migrate.py` & `virt-firmware-23.5/virt/firmware/migrate.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/sigdb.py` & `virt-firmware-23.5/virt/firmware/sigdb.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/vars.py` & `virt-firmware-23.5/virt/firmware/vars.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/varstore/aws.py` & `virt-firmware-23.5/virt/firmware/varstore/aws.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/varstore/edk2.py` & `virt-firmware-23.5/virt/firmware/varstore/edk2.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.4/virt/firmware/varstore/linux.py` & `virt-firmware-23.5/virt/firmware/varstore/linux.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,29 @@
 from virt.firmware.efi import efivar
 
 # pylint: disable=too-few-public-methods
 class LinuxVarStore:
     """  class for linux efivarfs varstore """
 
     @staticmethod
+    def get_variable(name, guid,
+                     path = '/sys/firmware/efi/efivars'):
+        filename = os.path.join(path, f'{name}-{guid}')
+        try:
+            with open(filename, "rb") as f:
+                attr = int.from_bytes(f.read(4), byteorder='little', signed=False)
+                data = f.read()
+                var = efivar.EfiVar(ucs16.from_string(name),
+                                    guid = guids.parse_str(guid),
+                                    attr = attr, data = data)
+            return var
+        except OSError:
+            return None
+
+    @staticmethod
     def get_varlist(path = '/sys/firmware/efi/efivars',
                     volatile = False):
 
         varlist = efivar.EfiVarList()
         if not os.path.isdir(path):
             return varlist
 
@@ -23,16 +38,11 @@
         with os.scandir(path) as it:
             for entry in it:
                 if not entry.is_file():
                     continue
                 name = entry.name[ : len(entry.name) - 37 ]
                 guid = entry.name[ len(entry.name) - 36 : ]
                 filename = os.path.join(path, entry.name)
-                with open(filename, "rb") as f:
-                    attr = int.from_bytes(f.read(4), byteorder='little', signed=False)
-                    data = f.read()
-                if attr & efivar.EFI_VARIABLE_NON_VOLATILE or volatile:
-                    var = efivar.EfiVar(ucs16.from_string(name),
-                                        guid = guids.parse_str(guid),
-                                        attr = attr, data = data)
+                var = LinuxVarStore.get_variable(name, guid, path)
+                if var and (var.attr & efivar.EFI_VARIABLE_NON_VOLATILE or volatile):
                     varlist[name] = var
         return varlist
```

### Comparing `virt-firmware-23.4/virt/peutils/peutils.py` & `virt-firmware-23.5/virt/peutils/peutils.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,14 +59,20 @@
             print_cert(sl.x509, verbose)
         elif str(sl.guid) == guids.EfiCertSha256:
             print('#          sha256')
             print(f'#             {len(sl)} entries')
         else:
             print(f'#          {sl.guid}')
 
+def print_sbat_entries(name, data):
+    print(f'#       {name}')
+    entries = data.decode().rstrip('\n').split('\n')
+    for entry in entries:
+        print(f'#           {entry}')
+
 def sig_type2(data, extract = False, verbose = False):
     certs = pkcs7.load_der_pkcs7_certificates(data)
     for cert in certs:
         print_cert(cert, verbose)
 
         if extract:
             scn = common_name(cert.subject)
@@ -87,41 +93,58 @@
 def pe_string(pe, index):
     """ lookup string in string table (right after symbol table) """
     strtab  = pe.FILE_HEADER.PointerToSymbolTable
     strtab += pe.FILE_HEADER.NumberOfSymbols * 18
     strtab += index
     return getcstr(pe.__data__[strtab:])
 
+def pe_section_flags(sec):
+    r = '-'
+    w = '-'
+    x = '-'
+    if sec.Characteristics & pefile.SECTION_CHARACTERISTICS['IMAGE_SCN_MEM_READ']:
+        r = 'r'
+    if sec.Characteristics & pefile.SECTION_CHARACTERISTICS['IMAGE_SCN_MEM_WRITE']:
+        w = 'w'
+    if sec.Characteristics & pefile.SECTION_CHARACTERISTICS['IMAGE_SCN_MEM_EXECUTE']:
+        x = 'x'
+    return r + w + x
+
 def efi_binary(filename, extract = False, verbose = False):
     print(f'# file: {filename}')
     pe = pefile.PE(filename)
     for sec in pe.sections:
         if sec.Name.startswith(b'/'):
             idx = getcstr(sec.Name[1:])
             sec.Name = pe_string(pe, int(idx))
         print(f'#    section: 0x{sec.PointerToRawData:06x} +0x{sec.SizeOfRawData:06x}'
+              f' {pe_section_flags(sec)}'
               f' ({sec.Name.decode()})')
         if sec.Name == b'.sbat\0\0\0':
-            sbat = pe.__data__[ sec.PointerToRawData :
-                                sec.PointerToRawData + sec.SizeOfRawData ]
+            sbat = sec.get_data()
             entries = sbat.decode().rstrip('\n\0').split('\n')
             for entry in entries:
                 print(f'#       {entry}')
         if sec.Name == b'.vendor_cert':
-            vcert = pe.__data__[ sec.PointerToRawData :
-                                 sec.PointerToRawData + sec.SizeOfRawData ]
+            vcert = sec.get_data()
             (dbs, dbxs, dbo, dbxo) = struct.unpack_from('<IIII', vcert)
             if dbs:
                 print(f'#       db: {dbo} +{dbs}')
                 db = vcert [ dbo : dbo + dbs ]
                 print_vendor_cert(db, verbose)
             if dbxs:
                 print(f'#       dbx: {dbxo} +{dbxs}')
                 dbx = vcert [ dbxo : dbxo + dbxs ]
                 print_vendor_cert(dbx, verbose)
+        if sec.Name == b'.sbatlevel':
+            levels = sec.get_data()
+            (version, poff, loff) = struct.unpack_from('<III', levels)
+            print_sbat_entries('previous', getcstr(levels[poff + 4:]))
+            print_sbat_entries('latest', getcstr(levels[loff + 4:]))
+
     sighdr = pe.OPTIONAL_HEADER.DATA_DIRECTORY[4]
     if sighdr.VirtualAddress and sighdr.Size:
         print(f'#    sigdata: 0x{sighdr.VirtualAddress:06x} +0x{sighdr.Size:06x}')
         sigs = pe.__data__[ sighdr.VirtualAddress :
                             sighdr.VirtualAddress + sighdr.Size ]
         pos = 0
         index = 0
```

### Comparing `virt-firmware-23.4/virt_firmware.egg-info/PKG-INFO` & `virt-firmware-23.5/virt_firmware.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virt-firmware
-Version: 23.4
+Version: 23.5
 Summary: tools for virtual machine firmware volumes
 Author: Gerd Hoffmann
 Author-email: kraxel@redhat.com
 License: GPLv2
 Project-URL: GitLab, https://gitlab.com/kraxel/virt-firmware
 Keywords: ovmf,armvirt,edk2,aws
 Description-Content-Type: text/markdown
```

### Comparing `virt-firmware-23.4/virt_firmware.egg-info/SOURCES.txt` & `virt-firmware-23.5/virt_firmware.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+experimental/bootcfg.py
 experimental/dbxupdate.py
 experimental/measure.py
 man/virt-fw-dump.1
 man/virt-fw-dump.inc
 man/virt-fw-sigdb.1
 man/virt-fw-sigdb.inc
 man/virt-fw-vars.1
@@ -34,14 +35,15 @@
 virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem
 virt/firmware/certs/RedHatSecureBootCA3.pem
 virt/firmware/certs/RedHatSecureBootCA5.pem
 virt/firmware/certs/RedHatSecureBootCA6.pem
 virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem
 virt/firmware/certs/fedoraca-20200709.pem
 virt/firmware/efi/__init__.py
+virt/firmware/efi/bootentry.py
 virt/firmware/efi/certs.py
 virt/firmware/efi/devpath.py
 virt/firmware/efi/efijson.py
 virt/firmware/efi/efivar.py
 virt/firmware/efi/guids.py
 virt/firmware/efi/siglist.py
 virt/firmware/efi/ucs16.py
```

