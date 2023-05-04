# Comparing `tmp/axdd-person-client-1.1.3.tar.gz` & `tmp/axdd-person-client-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axdd-person-client-1.1.3.tar", last modified: Mon Apr 24 19:23:22 2023, max compression
+gzip compressed data, was "axdd-person-client-1.1.4.tar", last modified: Thu May  4 16:43:48 2023, max compression
```

## Comparing `axdd-person-client-1.1.3.tar` & `axdd-person-client-1.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:22.856109 axdd-person-client-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-04-24 19:23:22.856109 axdd-person-client-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:22.852108 axdd-person-client-1.1.3/axdd_person_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-04-24 19:23:22.000000 axdd-person-client-1.1.3/axdd_person_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-04-24 19:23:22.000000 axdd-person-client-1.1.3/axdd_person_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 19:23:22.000000 axdd-person-client-1.1.3/axdd_person_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-04-24 19:23:22.000000 axdd-person-client-1.1.3/axdd_person_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-24 19:23:22.000000 axdd-person-client-1.1.3/axdd_person_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:22.852108 axdd-person-client-1.1.3/conf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/conf/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-24 19:23:22.856109 axdd-person-client-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:22.856109 axdd-person-client-1.1.3/uw_person_client/
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:22.856109 axdd-person-client-1.1.3/uw_person_client/clients/
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25233 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/clients/core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/clients/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/components.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:22.856109 axdd-person-client-1.1.3/uw_person_client/databases/
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/databases/postgres.py
--rw-r--r--   0 runner    (1001) docker     (122)     5633 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/databases/uwpds.py
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:22.856109 axdd-person-client-1.1.3/uw_person_client/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (122)    33750 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/tests/test_core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/tests/test_mock_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:48.846678 axdd-person-client-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-04 16:43:48.846678 axdd-person-client-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:48.842678 axdd-person-client-1.1.4/axdd_person_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-04 16:43:48.000000 axdd-person-client-1.1.4/axdd_person_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-05-04 16:43:48.000000 axdd-person-client-1.1.4/axdd_person_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 16:43:48.000000 axdd-person-client-1.1.4/axdd_person_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-04 16:43:48.000000 axdd-person-client-1.1.4/axdd_person_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-04 16:43:48.000000 axdd-person-client-1.1.4/axdd_person_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:48.842678 axdd-person-client-1.1.4/conf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/conf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 16:43:48.846678 axdd-person-client-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:48.842678 axdd-person-client-1.1.4/uw_person_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:48.842678 axdd-person-client-1.1.4/uw_person_client/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25860 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/clients/core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/clients/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3549 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/components.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:48.846678 axdd-person-client-1.1.4/uw_person_client/databases/
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/databases/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/databases/uwpds.py
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:48.846678 axdd-person-client-1.1.4/uw_person_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34221 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/tests/test_core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-05-04 16:43:35.000000 axdd-person-client-1.1.4/uw_person_client/tests/test_mock_client.py
```

### Comparing `axdd-person-client-1.1.3/LICENSE` & `axdd-person-client-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.3/PKG-INFO` & `axdd-person-client-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.3
+Version: 1.1.4
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.3/README.md` & `axdd-person-client-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.3/axdd_person_client.egg-info/PKG-INFO` & `axdd-person-client-1.1.4/axdd_person_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.3
+Version: 1.1.4
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.3/axdd_person_client.egg-info/SOURCES.txt` & `axdd-person-client-1.1.4/axdd_person_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.3/conf/settings.py` & `axdd-person-client-1.1.4/conf/settings.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.3/setup.py` & `axdd-person-client-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.3/uw_person_client/clients/__init__.py` & `axdd-person-client-1.1.4/uw_person_client/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.3/uw_person_client/clients/core_client.py` & `axdd-person-client-1.1.4/uw_person_client/clients/core_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sqlalchemy.orm.exc import NoResultFound
 from uw_person_client.clients import AbstractUWPersonClient
 from uw_person_client.databases.uwpds import UWPDS
 from uw_person_client.exceptions import (
     PersonNotFoundException, AdviserNotFoundException)
 from uw_person_client.components import (
     Person, Student, Employee, Transcript, Major, Sport, Adviser, Term,
-    Transfer)
+    Transfer, Hold)
 
 
 class UWPersonClient(AbstractUWPersonClient):
 
     """
     Public methods
     """
@@ -124,15 +124,16 @@
                     include_employee=True,
                     include_student=True,
                     include_student_transcripts=True,
                     include_student_transfers=True,
                     include_student_sports=True,
                     include_student_advisers=True,
                     include_student_majors=True,
-                    include_student_pending_majors=True):
+                    include_student_pending_majors=True,
+                    include_student_holds=True):
         person = Person()
         person.uwnetid = sqla_person.uwnetid
         person.uwregid = sqla_person.uwregid
         person.prior_uwnetids = sqla_person.prior_uwnetids
         person.prior_uwregids = sqla_person.prior_uwregids
         person.pronouns = sqla_person.pronouns
         person.full_name = sqla_person.full_name
@@ -154,14 +155,15 @@
                     sqla_student,
                     include_student_transcripts=include_student_transcripts,
                     include_student_transfers=include_student_transfers,
                     include_student_sports=include_student_sports,
                     include_student_advisers=include_student_advisers,
                     include_student_majors=include_student_majors,
                     include_student_pending_majors=include_student_pending_majors,  # noqa
+                    include_student_holds=include_student_holds,
                 )
             except NoResultFound:
                 pass
 
         if include_employee:
             try:
                 sqla_employee = self.DB.session.query(self.DB.Employee).filter(
@@ -174,15 +176,16 @@
 
     def _map_student(self, sqla_student,
                      include_student_transcripts=True,
                      include_student_transfers=True,
                      include_student_sports=True,
                      include_student_advisers=True,
                      include_student_majors=True,
-                     include_student_pending_majors=True):
+                     include_student_pending_majors=True,
+                     include_student_holds=True):
         student = Student()
 
         student.system_key = sqla_student.system_key
         student.student_number = sqla_student.student_number
         student.application_status_code = sqla_student.application_status_code
         student.application_status_desc = sqla_student.application_status_desc
         student.application_type_code = sqla_student.application_type_code
@@ -222,18 +225,14 @@
         student.first_generation_4yr_ind = \
             sqla_student.first_generation_4yr_ind
         student.first_generation_ind = sqla_student.first_generation_ind
         student.gender = sqla_student.gender
         student.high_school_gpa = sqla_student.high_school_gpa
         student.high_school_graduation_date = \
             sqla_student.high_school_graduation_date
-        student.hold_office_name_combined = \
-            sqla_student.hold_office_name_combined
-        student.hold_reason_desc_combined = \
-            sqla_student.hold_reason_desc_combined
         student.honors_program_code = sqla_student.honors_program_code
         student.honors_program_ind = sqla_student.honors_program_ind
         student.iss_perm_resident_country = \
             sqla_student.iss_perm_resident_country
         student.jr_col_gpa = sqla_student.jr_col_gpa
         student.last_enrolled_yr_qtr_desc = \
             sqla_student.last_enrolled_yr_qtr_desc
@@ -365,14 +364,21 @@
         if include_student_transfers:
             # map transfers
             student.transfers = []
             for transfer in sqla_student.transfer:
                 transfer = self._map_transfer(transfer)
                 student.transfers.append(transfer)
 
+        if include_student_holds:
+            # map holds
+            student.holds = []
+            for hold in sqla_student.hold:
+                hold = self._map_hold(hold)
+                student.holds.append(hold)
+
         return student
 
     def _map_employee(self, sqla_employee):
         employee = Employee()
         employee.employee_number = sqla_employee.employee_number
         employee.employee_affiliation_state = \
             sqla_employee.employee_affiliation_state
@@ -505,12 +511,23 @@
         transfer.inst_country = sqla_transfer.inst_country
         transfer.inst_postal_cd = sqla_transfer.inst_postal_cd
         transfer.inst_record_stat = sqla_transfer.inst_record_stat
         transfer.two_year = sqla_transfer.two_year
         transfer.wa_cc = sqla_transfer.wa_cc
         return transfer
 
+    def _map_hold(self, sqla_hold):
+        hold = Hold()
+        hold.seq = sqla_hold.seq
+        hold.hold_dt = sqla_hold.hold_dt
+        hold.hold_office = sqla_hold.hold_office
+        hold.hold_office_desc = sqla_hold.hold_office_desc
+        hold.hold_reason = sqla_hold.hold_reason
+        hold.hold_type = sqla_hold.hold_type
+        hold.hold_type_desc = Hold.TYPE_DESCRIPTIONS.get(sqla_hold.hold_type)
+        return hold
+
     def _map_term(self, sqla_term):
         term = Term()
         term.year = sqla_term.year
         term.quarter = sqla_term.quarter
         return term
```

### Comparing `axdd-person-client-1.1.3/uw_person_client/clients/mock_client.py` & `axdd-person-client-1.1.4/uw_person_client/clients/mock_client.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.3/uw_person_client/components.py` & `axdd-person-client-1.1.4/uw_person_client/components.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,14 +66,16 @@
                     obj_cls = Adviser
                 elif key == "transcripts":
                     obj_cls = Transcript
                 elif key == "transfers":
                     obj_cls = Transfer
                 elif key == "sports":
                     obj_cls = Sport
+                elif key == "holds":
+                    obj_cls = Hold
                 items = []
                 for list_value in value:
                     if isinstance(list_value, dict):
                         new_obj = obj_cls()
                         items.append(
                             new_obj.from_dict(list_value, obj=new_obj))
                     else:
@@ -100,14 +102,22 @@
     pass
 
 
 class Transfer(AbstractBase):
     pass
 
 
+class Hold(AbstractBase):
+    TYPE_DESCRIPTIONS = {
+        1: "REGISTRATION HOLD",
+        2: "TRANSCRIPT HOLD",
+        3: "REGISTRATION AND TRANSCRIPT HOLD"
+    }
+
+
 class Major(AbstractBase):
     pass
 
 
 class Sport(AbstractBase):
     pass
```

### Comparing `axdd-person-client-1.1.3/uw_person_client/databases/__init__.py` & `axdd-person-client-1.1.4/uw_person_client/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.3/uw_person_client/databases/postgres.py` & `axdd-person-client-1.1.4/uw_person_client/databases/postgres.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.3/uw_person_client/databases/uwpds.py` & `axdd-person-client-1.1.4/uw_person_client/databases/uwpds.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         self.Student = UWPDS.Base.classes.student
         self.Major = UWPDS.Base.classes.major
         self.Sport = UWPDS.Base.classes.sport
         self.StudentToSport = UWPDS.Base.classes.student_to_sport
         self.StudentToAdviser = UWPDS.Base.classes.student_to_adviser
         self.Transcript = UWPDS.Base.classes.transcript
         self.Transfer = UWPDS.Base.classes.transfer
+        self.Hold = UWPDS.Base.classes.hold
         self.Term = UWPDS.Base.classes.term
 
     def initialize_relationships(self):
         student_to_sport = Table(
             'student_to_sport',
             UWPDS.Base.metadata,
             autoload=True,
@@ -85,19 +86,22 @@
             pending_major_3_id = Column(
                 'pending_major_3_id',
                 ForeignKey('major.id', ondelete="CASCADE"))
             pending_major_3 = \
                 relationship("major", foreign_keys=[pending_major_3_id],
                              viewonly=True)
             transcript = relationship(
-                "Transcript", back_populates="student", uselist=True,
+                "transcript", back_populates="student", uselist=True,
                 viewonly=True)
             transfer = relationship(
                 "transfer", back_populates="student", uselist=True,
                 viewonly=True)
+            hold = relationship(
+                "student_hold", back_populates="student", uselist=True,
+                order_by="student_hold.seq", viewonly=True)
             academic_term_id = Column(
                 'academic_term_id', ForeignKey('term.id', ondelete="CASCADE"))
             academic_term = \
                 relationship("term", foreign_keys=[academic_term_id],
                              viewonly=True)
 
         class Employee(UWPDS.Base):
```

### Comparing `axdd-person-client-1.1.3/uw_person_client/tests/test_core_client.py` & `axdd-person-client-1.1.4/uw_person_client/tests/test_core_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from unittest import TestCase
 from unittest.mock import patch, MagicMock
 from uw_person_client.exceptions import (
     AdviserNotFoundException, PersonNotFoundException)
 from uw_person_client.clients.core_client import UWPersonClient
 from uw_person_client.components import (
     Adviser, Employee, Major, Person, Sport, Student, Term, Transcript,
-    Transfer)
+    Transfer, Hold)
 from sqlalchemy.orm.exc import NoResultFound
 
 
 class UWPersonClientTest(TestCase):
 
     @patch('uw_person_client.clients.core_client.UWPDS')
     def get_mock_person_client(self, mock_uwpds):
@@ -411,16 +411,14 @@
         mock_student.exemption_desc = MagicMock()
         mock_student.external_email = MagicMock()
         mock_student.first_generation_4yr_ind = MagicMock()
         mock_student.first_generation_ind = MagicMock()
         mock_student.gender = MagicMock()
         mock_student.high_school_gpa = MagicMock()
         mock_student.high_school_graduation_date = MagicMock()
-        mock_student.hold_office_name_combined = MagicMock()
-        mock_student.hold_reason_desc_combined = MagicMock()
         mock_student.honors_program_code = MagicMock()
         mock_student.honors_program_ind = MagicMock()
         mock_student.iss_perm_resident_country = MagicMock()
         mock_student.jr_col_gpa = MagicMock()
         mock_student.last_enrolled_yr_qtr_desc = MagicMock()
         mock_student.last_enrolled_yr_qtr_id = MagicMock()
         mock_student.local_addr_4digit_zip = MagicMock()
@@ -673,14 +671,31 @@
         mock_dict = self._mock_to_dict(mock_transfer)
         transfer = client._map_transfer(mock_transfer)
 
         # assertions
         self.assertIsInstance(transfer, Transfer)
         self.assertDictContainsSubset(mock_dict, transfer.to_dict())
 
+    def test_map_hold(self):
+        client = self.get_mock_person_client()
+        mock_hold = MagicMock()
+        mock_hold.seq = MagicMock()
+        mock_hold.hold_dt = MagicMock()
+        mock_hold.hold_office = MagicMock()
+        mock_hold.hold_office_desc = MagicMock()
+        mock_hold.hold_reason = MagicMock()
+        mock_hold.hold_type = MagicMock()
+
+        mock_dict = self._mock_to_dict(mock_hold)
+        hold = client._map_hold(mock_hold)
+
+        # assertions
+        self.assertIsInstance(hold, Hold)
+        self.assertDictContainsSubset(mock_dict, hold.to_dict())
+
     def test_map_term(self):
         client = self.get_mock_person_client()
         mock_term = MagicMock()
         mock_term.year = MagicMock()
         mock_term.quarter = MagicMock()
 
         mock_dict = self._mock_to_dict(mock_term)
```

### Comparing `axdd-person-client-1.1.3/uw_person_client/tests/test_mock_client.py` & `axdd-person-client-1.1.4/uw_person_client/tests/test_mock_client.py`

 * *Files identical despite different names*

