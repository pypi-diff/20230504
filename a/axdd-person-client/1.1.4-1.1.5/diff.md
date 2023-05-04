# Comparing `tmp/axdd-person-client-1.1.4.tar.gz` & `tmp/axdd-person-client-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axdd-person-client-1.1.4.tar", last modified: Thu May  4 16:43:48 2023, max compression
+gzip compressed data, was "axdd-person-client-1.1.5.tar", last modified: Thu May  4 19:27:47 2023, max compression
```

## Comparing `axdd-person-client-1.1.4.tar` & `axdd-person-client-1.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:48.846678 axdd-person-client-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-04 16:43:48.846678 axdd-person-client-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:48.842678 axdd-person-client-1.1.4/axdd_person_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-04 16:43:48.000000 axdd-person-client-1.1.4/axdd_person_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-05-04 16:43:48.000000 axdd-person-client-1.1.4/axdd_person_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 16:43:48.000000 axdd-person-client-1.1.4/axdd_person_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-04 16:43:48.000000 axdd-person-client-1.1.4/axdd_person_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-04 16:43:48.000000 axdd-person-client-1.1.4/axdd_person_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:48.842678 axdd-person-client-1.1.4/conf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/conf/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 16:43:48.846678 axdd-person-client-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:48.842678 axdd-person-client-1.1.4/uw_person_client/
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:48.842678 axdd-person-client-1.1.4/uw_person_client/clients/
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25860 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/clients/core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/clients/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3549 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/components.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:48.846678 axdd-person-client-1.1.4/uw_person_client/databases/
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/databases/postgres.py
--rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/databases/uwpds.py
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:48.846678 axdd-person-client-1.1.4/uw_person_client/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (122)    34221 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/tests/test_core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/tests/test_mock_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:47.087322 axdd-person-client-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-04 19:27:47.087322 axdd-person-client-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:47.083322 axdd-person-client-1.1.5/axdd_person_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-04 19:27:46.000000 axdd-person-client-1.1.5/axdd_person_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-05-04 19:27:47.000000 axdd-person-client-1.1.5/axdd_person_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 19:27:46.000000 axdd-person-client-1.1.5/axdd_person_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-04 19:27:46.000000 axdd-person-client-1.1.5/axdd_person_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-04 19:27:46.000000 axdd-person-client-1.1.5/axdd_person_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:47.083322 axdd-person-client-1.1.5/conf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/conf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 19:27:47.087322 axdd-person-client-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:47.087322 axdd-person-client-1.1.5/uw_person_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:47.087322 axdd-person-client-1.1.5/uw_person_client/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25868 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/clients/core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/clients/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3549 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/components.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:47.087322 axdd-person-client-1.1.5/uw_person_client/databases/
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/databases/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5858 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/databases/uwpds.py
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:47.087322 axdd-person-client-1.1.5/uw_person_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34221 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/tests/test_core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/tests/test_mock_client.py
```

### Comparing `axdd-person-client-1.1.4/LICENSE` & `axdd-person-client-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.4/PKG-INFO` & `axdd-person-client-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.4
+Version: 1.1.5
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.4/README.md` & `axdd-person-client-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.4/axdd_person_client.egg-info/PKG-INFO` & `axdd-person-client-1.1.5/axdd_person_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.4
+Version: 1.1.5
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.4/axdd_person_client.egg-info/SOURCES.txt` & `axdd-person-client-1.1.5/axdd_person_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.4/conf/settings.py` & `axdd-person-client-1.1.5/conf/settings.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.4/setup.py` & `axdd-person-client-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.4/uw_person_client/clients/__init__.py` & `axdd-person-client-1.1.5/uw_person_client/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.4/uw_person_client/clients/core_client.py` & `axdd-person-client-1.1.5/uw_person_client/clients/core_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
             for transfer in sqla_student.transfer:
                 transfer = self._map_transfer(transfer)
                 student.transfers.append(transfer)
 
         if include_student_holds:
             # map holds
             student.holds = []
-            for hold in sqla_student.hold:
+            for hold in sqla_student.student_hold:
                 hold = self._map_hold(hold)
                 student.holds.append(hold)
 
         return student
 
     def _map_employee(self, sqla_employee):
         employee = Employee()
```

### Comparing `axdd-person-client-1.1.4/uw_person_client/clients/mock_client.py` & `axdd-person-client-1.1.5/uw_person_client/clients/mock_client.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.4/uw_person_client/components.py` & `axdd-person-client-1.1.5/uw_person_client/components.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.4/uw_person_client/databases/__init__.py` & `axdd-person-client-1.1.5/uw_person_client/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.4/uw_person_client/databases/postgres.py` & `axdd-person-client-1.1.5/uw_person_client/databases/postgres.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.4/uw_person_client/databases/uwpds.py` & `axdd-person-client-1.1.5/uw_person_client/databases/uwpds.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.Student = UWPDS.Base.classes.student
         self.Major = UWPDS.Base.classes.major
         self.Sport = UWPDS.Base.classes.sport
         self.StudentToSport = UWPDS.Base.classes.student_to_sport
         self.StudentToAdviser = UWPDS.Base.classes.student_to_adviser
         self.Transcript = UWPDS.Base.classes.transcript
         self.Transfer = UWPDS.Base.classes.transfer
-        self.Hold = UWPDS.Base.classes.hold
+        self.Hold = UWPDS.Base.classes.student_hold
         self.Term = UWPDS.Base.classes.term
 
     def initialize_relationships(self):
         student_to_sport = Table(
             'student_to_sport',
             UWPDS.Base.metadata,
             autoload=True,
@@ -86,20 +86,20 @@
             pending_major_3_id = Column(
                 'pending_major_3_id',
                 ForeignKey('major.id', ondelete="CASCADE"))
             pending_major_3 = \
                 relationship("major", foreign_keys=[pending_major_3_id],
                              viewonly=True)
             transcript = relationship(
-                "transcript", back_populates="student", uselist=True,
+                "Transcript", back_populates="student", uselist=True,
                 viewonly=True)
             transfer = relationship(
                 "transfer", back_populates="student", uselist=True,
                 viewonly=True)
-            hold = relationship(
+            student_hold = relationship(
                 "student_hold", back_populates="student", uselist=True,
                 order_by="student_hold.seq", viewonly=True)
             academic_term_id = Column(
                 'academic_term_id', ForeignKey('term.id', ondelete="CASCADE"))
             academic_term = \
                 relationship("term", foreign_keys=[academic_term_id],
                              viewonly=True)
```

### Comparing `axdd-person-client-1.1.4/uw_person_client/tests/test_core_client.py` & `axdd-person-client-1.1.5/uw_person_client/tests/test_core_client.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.4/uw_person_client/tests/test_mock_client.py` & `axdd-person-client-1.1.5/uw_person_client/tests/test_mock_client.py`

 * *Files identical despite different names*

