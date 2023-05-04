# Comparing `tmp/pyhid-usb-relay-0.1.0.tar.gz` & `tmp/pyhid_usb_relay-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pyhid-usb-relay/pyhid-usb-relay/dist/tmpo6ltbl45/pyhid-usb-relay-0.1.0.tar", last modified: Thu Sep  9 15:35:34 2021, max compression
+gzip compressed data, was "pyhid_usb_relay-0.1.1.tar", max compression
```

## Comparing `pyhid-usb-relay-0.1.0.tar` & `pyhid_usb_relay-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-09 15:35:34.000000 pyhid-usb-relay-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-09-09 15:35:26.000000 pyhid-usb-relay-0.1.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     2690 2021-09-09 15:35:34.000000 pyhid-usb-relay-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2021-09-09 15:35:26.000000 pyhid-usb-relay-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-09 15:35:34.000000 pyhid-usb-relay-0.1.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     5342 2021-09-09 15:35:26.000000 pyhid-usb-relay-0.1.0/bin/pyhid-usb-relay
--rw-r--r--   0 runner    (1001) docker     (121)      104 2021-09-09 15:35:26.000000 pyhid-usb-relay-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-09 15:35:34.000000 pyhid-usb-relay-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      961 2021-09-09 15:35:26.000000 pyhid-usb-relay-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-09 15:35:34.000000 pyhid-usb-relay-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-09 15:35:34.000000 pyhid-usb-relay-0.1.0/src/pyhid_usb_relay/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-09-09 15:35:26.000000 pyhid-usb-relay-0.1.0/src/pyhid_usb_relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4693 2021-09-09 15:35:26.000000 pyhid-usb-relay-0.1.0/src/pyhid_usb_relay/controller.py
--rw-r--r--   0 runner    (1001) docker     (121)      134 2021-09-09 15:35:26.000000 pyhid-usb-relay-0.1.0/src/pyhid_usb_relay/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-09-09 15:35:26.000000 pyhid-usb-relay-0.1.0/src/pyhid_usb_relay/find.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-09 15:35:34.000000 pyhid-usb-relay-0.1.0/src/pyhid_usb_relay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2690 2021-09-09 15:35:34.000000 pyhid-usb-relay-0.1.0/src/pyhid_usb_relay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      403 2021-09-09 15:35:34.000000 pyhid-usb-relay-0.1.0/src/pyhid_usb_relay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-09 15:35:34.000000 pyhid-usb-relay-0.1.0/src/pyhid_usb_relay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-09-09 15:35:34.000000 pyhid-usb-relay-0.1.0/src/pyhid_usb_relay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-09-09 15:35:34.000000 pyhid-usb-relay-0.1.0/src/pyhid_usb_relay.egg-info/top_level.txt
+-rw-r--r--   0        0        0     4051 2023-05-04 18:37:42.944763 pyhid_usb_relay-0.1.1/README.md
+-rw-r--r--   0        0        0      188 2023-05-04 18:37:42.944763 pyhid_usb_relay-0.1.1/pyhid_usb_relay/__init__.py
+-rw-r--r--   0        0        0     4708 2023-05-04 18:37:42.944763 pyhid_usb_relay-0.1.1/pyhid_usb_relay/controller.py
+-rw-r--r--   0        0        0      134 2023-05-04 18:37:42.944763 pyhid_usb_relay-0.1.1/pyhid_usb_relay/exceptions.py
+-rw-r--r--   0        0        0     1401 2023-05-04 18:37:42.944763 pyhid_usb_relay-0.1.1/pyhid_usb_relay/find.py
+-rw-r--r--   0        0        0     5339 2023-05-04 18:37:42.944763 pyhid_usb_relay-0.1.1/pyhid_usb_relay/main.py
+-rw-r--r--   0        0        0      656 2023-05-04 18:37:42.944763 pyhid_usb_relay-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4974 1970-01-01 00:00:00.000000 pyhid_usb_relay-0.1.1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyhid-usb-relay-0.1.0/bin/pyhid-usb-relay` & `pyhid_usb_relay-0.1.1/pyhid_usb_relay/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,23 +139,25 @@
     get_serial_parser.add_argument("address", type=int, help="Device USB address")
     get_serial_parser.set_defaults(func=relay_get_serial)
 
     set_serial_parser = subparser.add_parser(
         "set-serial", help="Set device serial number"
     )
     group = set_serial_parser.add_mutually_exclusive_group(required=True)
-    group.add_argument("--bus", nargs=2, metavar=("BUS", "ADDRESS"), type=int, help="Device USB bus number and address")
+    group.add_argument(
+        "--bus",
+        nargs=2,
+        metavar=("BUS", "ADDRESS"),
+        type=int,
+        help="Device USB bus number and address",
+    )
     group.add_argument("--serial", help="Control board with given serial ID")
     set_serial_parser.add_argument("new_serial", help="New serial number")
     set_serial_parser.set_defaults(func=relay_set_serial)
 
     args = parser.parse_args()
     try:
         return args.func(args)
     except (ValueError, IndexError, DeviceNotFoundError) as e:
         sys.stderr.write(str(e))
         sys.stderr.write("\n")
         return 1
-
-
-if __name__ == "__main__":
-    sys.exit(main())
```

### Comparing `pyhid-usb-relay-0.1.0/src/pyhid_usb_relay/controller.py` & `pyhid_usb_relay-0.1.1/pyhid_usb_relay/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,19 +65,18 @@
                 buf.append(0x00)
         buf.append(0x00)
         buf.append(0x00)
         self._set_hid_report(MAIN_REPORT, buf)
 
         self._update_status()
 
-
     def _update_status(self):
         data = self._get_hid_report(MAIN_REPORT, 8)
         try:
-            self.serial = data[0:5].tobytes().decode("utf-8")
+            self.serial = data[0:5].tobytes().rstrip(b"\x00").decode("utf-8")
         except UnicodeDecodeError:
             self.serial = "".join("%02x" % b for b in data[0:5])
         self.state = data[7]
 
     def _name_to_number(self, relay):
         def convert():
             invert = self.defaults.get("invert", False)
```

### Comparing `pyhid-usb-relay-0.1.0/src/pyhid_usb_relay/find.py` & `pyhid_usb_relay-0.1.1/pyhid_usb_relay/find.py`

 * *Files identical despite different names*

