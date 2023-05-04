# Comparing `tmp/openxes_cli_py-0.1.7.tar.gz` & `tmp/openxes_cli_py-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openxes_cli_py-0.1.7.tar", max compression
+gzip compressed data, was "openxes_cli_py-0.1.8.tar", max compression
```

## Comparing `openxes_cli_py-0.1.7.tar` & `openxes_cli_py-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      744 2023-05-04 15:18:32.209949 openxes_cli_py-0.1.7/README.md
--rw-r--r--   0        0        0  3717515 2023-05-04 15:18:32.233950 openxes_cli_py-0.1.7/lib/openxes-cli.jar
--rw-r--r--   0        0        0      481 2023-05-04 15:18:32.233950 openxes_cli_py-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-04 15:18:32.233950 openxes_cli_py-0.1.7/src/openxes_cli/__init__.py
--rw-r--r--   0        0        0     1216 2023-05-04 15:18:32.233950 openxes_cli_py-0.1.7/src/openxes_cli/lib.py
--rw-r--r--   0        0        0     1140 1970-01-01 00:00:00.000000 openxes_cli_py-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      744 2023-05-04 15:36:43.323321 openxes_cli_py-0.1.8/README.md
+-rw-r--r--   0        0        0  3717531 2023-05-04 15:36:43.339321 openxes_cli_py-0.1.8/lib/openxes-cli.jar
+-rw-r--r--   0        0        0      481 2023-05-04 15:36:43.339321 openxes_cli_py-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-04 15:36:43.339321 openxes_cli_py-0.1.8/src/openxes_cli/__init__.py
+-rw-r--r--   0        0        0     1216 2023-05-04 15:36:43.339321 openxes_cli_py-0.1.8/src/openxes_cli/lib.py
+-rw-r--r--   0        0        0     1140 1970-01-01 00:00:00.000000 openxes_cli_py-0.1.8/PKG-INFO
```

### Comparing `openxes_cli_py-0.1.7/README.md` & `openxes_cli_py-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `openxes_cli_py-0.1.7/lib/openxes-cli.jar` & `openxes_cli_py-0.1.8/lib/openxes-cli.jar`

 * *Files 0% similar despite different names*

#### zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 3717515 bytes, number of entries: 3013
-drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 14:52 META-INF/
+Zip file size: 3717531 bytes, number of entries: 3013
+drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 18:33 META-INF/
 -rw-r--r--  2.0 unx       67 b- defN 23-May-04 13:51 META-INF/MANIFEST.MF
 drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 14:19 ee/
 drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 14:19 ee/ut/
 drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 14:19 ee/ut/cs/
 drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 14:19 ee/ut/cs/sep/
-drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 14:41 ee/ut/cs/sep/openxescli/
+drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 18:33 ee/ut/cs/sep/openxescli/
 -rw-r--r--  2.0 unx     7140 b- defN 23-May-04 14:19 ee/ut/cs/sep/openxescli/Event.class
--rw-r--r--  2.0 unx     5172 b- defN 23-May-04 14:23 ee/ut/cs/sep/openxescli/CsvSerializer.class
+-rw-r--r--  2.0 unx     5199 b- defN 23-May-04 18:33 ee/ut/cs/sep/openxescli/CsvSerializer.class
 -rw-r--r--  2.0 unx     3164 b- defN 23-May-04 14:41 ee/ut/cs/sep/openxescli/Main.class
 -rw-r--r--  2.0 unx     6693 b- defN 23-May-04 14:19 ee/ut/cs/sep/openxescli/EventLog.class
--rw-r--r--  2.0 unx     4911 b- defN 23-May-04 14:25 ee/ut/cs/sep/openxescli/Converter.class
+-rw-r--r--  2.0 unx     4911 b- defN 23-May-04 18:33 ee/ut/cs/sep/openxescli/Converter.class
 -rw-r--r--  2.0 unx     2220 b- defN 23-May-04 14:19 ee/ut/cs/sep/openxescli/Trace.class
 drwxr-xr-x  2.0 unx        0 b- defN 15-May-27 16:27 org/
 drwxr-xr-x  2.0 unx        0 b- defN 15-May-27 16:27 org/deckfour/
 drwxr-xr-x  2.0 unx        0 b- defN 15-May-27 16:27 org/deckfour/xes/
 drwxr-xr-x  2.0 unx        0 b- defN 15-May-27 16:27 org/deckfour/xes/classification/
 -rw-r--r--  2.0 unx     1667 b- defN 17-Dec-08 11:48 org/deckfour/xes/classification/XEventAndClassifier.class
 -rw-r--r--  2.0 unx     4206 b- defN 17-Dec-12 15:41 org/deckfour/xes/classification/XEventAttributeClassifier.class
@@ -3008,8 +3008,8 @@
 -rw-r--r--  2.0 unx      907 b- defN 17-Sep-06 14:23 javax/activation/SecuritySupport$2.class
 -rw-r--r--  2.0 unx     1510 b- defN 17-Sep-06 14:23 javax/activation/SecuritySupport$3.class
 -rw-r--r--  2.0 unx     1408 b- defN 17-Sep-06 14:23 javax/activation/SecuritySupport$4.class
 -rw-r--r--  2.0 unx      775 b- defN 17-Sep-06 14:23 javax/activation/SecuritySupport$5.class
 -rw-r--r--  2.0 unx     2116 b- defN 17-Sep-06 14:23 javax/activation/SecuritySupport.class
 -rw-r--r--  2.0 unx     1420 b- defN 17-Sep-06 14:23 javax/activation/URLDataSource.class
 -rw-r--r--  2.0 unx      485 b- defN 17-Sep-06 14:23 javax/activation/UnsupportedDataTypeException.class
-3013 files, 7969613 bytes uncompressed, 3164197 bytes compressed:  60.3%
+3013 files, 7969640 bytes uncompressed, 3164213 bytes compressed:  60.3%
```

#### ee/ut/cs/sep/openxescli/CsvSerializer.class

##### procyon -ec {}

```diff
@@ -42,15 +42,15 @@
                 for (int i = 0; i < xTrace.size(); ++i) {
                     csvEvent.setCaseId(((XAttribute)xTrace.getAttributes().get((Object)"concept:name")).toString());
                     final XEvent event = (XEvent)xTrace.get(i);
                     final XAttributeMap attributes = event.getAttributes();
                     final String timestamp = ((XAttribute)attributes.getOrDefault((Object)"time:timestamp", (Object)new XAttributeLiteralImpl("time:timestamp", ""))).toString();
                     final String activity = ((XAttribute)attributes.getOrDefault((Object)"concept:name", (Object)new XAttributeLiteralImpl("concept:name", ""))).toString();
                     final String resource = ((XAttribute)attributes.getOrDefault((Object)"org:resource", (Object)new XAttributeLiteralImpl("org:resource", ""))).toString();
-                    final String transition = ((XAttribute)attributes.getOrDefault((Object)"lifecycle:transition", (Object)new XAttributeLiteralImpl("lifecycle:transition", "complete"))).toString();
+                    final String transition = ((XAttribute)attributes.getOrDefault((Object)"lifecycle:transition", (Object)new XAttributeLiteralImpl("lifecycle:transition", "complete"))).toString().toLowerCase();
                     if (transition.equals("start")) {
                         csvEvent.setStartTimestamp(timestamp);
                         csvEvent.setActivity(activity);
                         csvEvent.setResource(resource);
                     }
                     else if (transition.equals("complete")) {
                         if (!CsvSerializer.$assertionsDisabled && csvEvent.getActivity() != null && !csvEvent.getActivity().equals(activity)) {
```

### Comparing `openxes_cli_py-0.1.7/src/openxes_cli/lib.py` & `openxes_cli_py-0.1.8/src/openxes_cli/lib.py`

 * *Files identical despite different names*

### Comparing `openxes_cli_py-0.1.7/PKG-INFO` & `openxes_cli_py-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxes-cli-py
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Ihar Suvorau
 Author-email: ihar.suvorau@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

