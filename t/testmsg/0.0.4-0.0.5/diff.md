# Comparing `tmp/testmsg-0.0.4.tar.gz` & `tmp/testmsg-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testmsg-0.0.4.tar", last modified: Wed May  3 14:14:32 2023, max compression
+gzip compressed data, was "testmsg-0.0.5.tar", last modified: Thu May  4 15:42:50 2023, max compression
```

## Comparing `testmsg-0.0.4.tar` & `testmsg-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-05-03 14:14:32.227098 testmsg-0.0.4/
--rw-r--r--   0 xenon     (1000) xenon     (1000)     2782 2023-05-03 14:14:32.227098 testmsg-0.0.4/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)     1933 2023-05-02 22:33:15.000000 testmsg-0.0.4/README.md
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-05-03 14:14:32.227098 testmsg-0.0.4/bin/
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2997 2023-05-03 14:14:16.000000 testmsg-0.0.4/bin/testmsg
--rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-05-03 14:14:32.227098 testmsg-0.0.4/setup.cfg
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1242 2023-05-02 21:41:24.000000 testmsg-0.0.4/setup.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-05-03 14:14:32.227098 testmsg-0.0.4/testmsg.egg-info/
--rw-r--r--   0 xenon     (1000) xenon     (1000)     2782 2023-05-03 14:14:32.000000 testmsg-0.0.4/testmsg.egg-info/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)      154 2023-05-03 14:14:32.000000 testmsg-0.0.4/testmsg.egg-info/SOURCES.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-05-03 14:14:32.000000 testmsg-0.0.4/testmsg.egg-info/dependency_links.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-05-03 14:14:32.000000 testmsg-0.0.4/testmsg.egg-info/top_level.txt
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-05-04 15:42:50.725884 testmsg-0.0.5/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     2782 2023-05-04 15:42:50.725884 testmsg-0.0.5/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     1933 2023-05-02 22:33:15.000000 testmsg-0.0.5/README.md
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-05-04 15:42:50.725884 testmsg-0.0.5/bin/
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     3086 2023-05-04 15:37:17.000000 testmsg-0.0.5/bin/testmsg
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-05-04 15:42:50.725884 testmsg-0.0.5/setup.cfg
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1242 2023-05-02 21:41:24.000000 testmsg-0.0.5/setup.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-05-04 15:42:50.725884 testmsg-0.0.5/testmsg.egg-info/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     2782 2023-05-04 15:42:50.000000 testmsg-0.0.5/testmsg.egg-info/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      154 2023-05-04 15:42:50.000000 testmsg-0.0.5/testmsg.egg-info/SOURCES.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-05-04 15:42:50.000000 testmsg-0.0.5/testmsg.egg-info/dependency_links.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-05-04 15:42:50.000000 testmsg-0.0.5/testmsg.egg-info/top_level.txt
```

### Comparing `testmsg-0.0.4/PKG-INFO` & `testmsg-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testmsg
-Version: 0.0.4
+Version: 0.0.5
 Summary: UNKNOWN
 Home-page: https://github.com/yaroslaff/testmsg
 Author: Yaroslav Polyakov
 Author-email: yaroslaff@gmail.com
 License: MIT
 Description: # testmsg
         Generate RFC822 compliant e-mail messages for tests and send it over SMTP.
```

### Comparing `testmsg-0.0.4/README.md` & `testmsg-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `testmsg-0.0.4/bin/testmsg` & `testmsg-0.0.5/bin/testmsg`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.\n" \
     "Ut enim ad minim veniam," \
     "quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.\n" \
     "Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.\n" \
     "Excepteur sint occaecat cupidatat non proident, " \
     "sunt in culpa qui officia deserunt mollit anim id est laborum.\n"
 
-version='0.0.4'
+version='0.0.5'
 
 def get_args():
     parser = argparse.ArgumentParser(description=f'Generate/Send valid RFC822 email messages for testing {version}')
     parser.add_argument('-f', '--from', dest='_from', default='from@example.com', metavar='EMAIL')
     parser.add_argument('-t', '--to', default='to@example.net', metavar='EMAIL')
     parser.add_argument('-s', '--subject', metavar='Subject', default='Sent with github.com/yaroslaff/testmsg')
     parser.add_argument('-a', '--add', nargs=2, action='append', dest='headers', metavar=('HEADER', 'VALUE'), help='add header')
@@ -74,15 +74,17 @@
     # Send the message via our own SMTP server.
     if args.send:
         smtp = smtplib.SMTP(args.send)
         if args.verbose:
             smtp.set_debuglevel(True)
         try:
             r = smtp.send_message(msg)
-        except smtplib.SMTPException as e:
+        except smtplib.SMTPResponseException as e:
             print(e.smtp_code, e.smtp_error.decode(), file=sys.stderr)
+        except smtplib.SMTPException as e:
+            print(e, file=sys.stderr)
         smtp.quit()
     else:
         print(msg)
 
 if __name__ == '__main__':
     main()
```

### Comparing `testmsg-0.0.4/setup.py` & `testmsg-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `testmsg-0.0.4/testmsg.egg-info/PKG-INFO` & `testmsg-0.0.5/testmsg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testmsg
-Version: 0.0.4
+Version: 0.0.5
 Summary: UNKNOWN
 Home-page: https://github.com/yaroslaff/testmsg
 Author: Yaroslav Polyakov
 Author-email: yaroslaff@gmail.com
 License: MIT
 Description: # testmsg
         Generate RFC822 compliant e-mail messages for tests and send it over SMTP.
```

