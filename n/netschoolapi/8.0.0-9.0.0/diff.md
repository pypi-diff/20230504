# Comparing `tmp/netschoolapi-8.0.0-py3-none-any.whl.zip` & `tmp/netschoolapi-9.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,12 @@
-Zip file size: 9260 bytes, number of entries: 11
--rw-r--r--  2.0 unx       68 b- defN 22-Nov-06 16:28 netschoolapi/__init__.py
--rw-r--r--  2.0 unx     2060 b- defN 22-Nov-06 16:28 netschoolapi/async_client_wrapper.py
--rw-r--r--  2.0 unx     2517 b- defN 22-Nov-06 16:28 netschoolapi/data.py
--rw-r--r--  2.0 unx      207 b- defN 22-Nov-06 16:28 netschoolapi/errors.py
--rw-r--r--  2.0 unx    11103 b- defN 22-Nov-06 16:28 netschoolapi/netschoolapi.py
--rw-r--r--  2.0 unx     3133 b- defN 22-Nov-06 16:28 netschoolapi/schemas.py
--rw-r--r--  2.0 unx     1149 b- defN 22-Nov-06 16:29 netschoolapi-8.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2292 b- defN 22-Nov-06 16:29 netschoolapi-8.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-06 16:29 netschoolapi-8.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 22-Nov-06 16:29 netschoolapi-8.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      904 b- defN 22-Nov-06 16:29 netschoolapi-8.0.0.dist-info/RECORD
-11 files, 23538 bytes uncompressed, 7728 bytes compressed:  67.2%
+Zip file size: 8123 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       68 b- defN 22-Nov-24 16:59 netschoolapi/__init__.py
+-rw-r--r--  2.0 unx     2080 b- defN 22-Nov-24 16:59 netschoolapi/async_client_wrapper.py
+-rw-r--r--  2.0 unx      207 b- defN 22-Nov-24 16:59 netschoolapi/errors.py
+-rw-r--r--  2.0 unx    11139 b- defN 22-Nov-24 16:59 netschoolapi/netschoolapi.py
+-rw-r--r--  2.0 unx     3405 b- defN 22-Nov-24 16:59 netschoolapi/schemas.py
+-rw-r--r--  2.0 unx     1149 b- defN 22-Nov-24 16:59 netschoolapi-9.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2252 b- defN 22-Nov-24 16:59 netschoolapi-9.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Nov-24 16:59 netschoolapi-9.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 22-Nov-24 16:59 netschoolapi-9.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      827 b- defN 22-Nov-24 16:59 netschoolapi-9.0.0.dist-info/RECORD
+10 files, 21232 bytes uncompressed, 6707 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -1,34 +1,31 @@
 Filename: netschoolapi/__init__.py
 Comment: 
 
 Filename: netschoolapi/async_client_wrapper.py
 Comment: 
 
-Filename: netschoolapi/data.py
-Comment: 
-
 Filename: netschoolapi/errors.py
 Comment: 
 
 Filename: netschoolapi/netschoolapi.py
 Comment: 
 
 Filename: netschoolapi/schemas.py
 Comment: 
 
-Filename: netschoolapi-8.0.0.dist-info/LICENSE
+Filename: netschoolapi-9.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: netschoolapi-8.0.0.dist-info/METADATA
+Filename: netschoolapi-9.0.0.dist-info/METADATA
 Comment: 
 
-Filename: netschoolapi-8.0.0.dist-info/WHEEL
+Filename: netschoolapi-9.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: netschoolapi-8.0.0.dist-info/top_level.txt
+Filename: netschoolapi-9.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: netschoolapi-8.0.0.dist-info/RECORD
+Filename: netschoolapi-9.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netschoolapi/async_client_wrapper.py

```diff
@@ -50,13 +50,13 @@
 
     async def _infinite_request(
             self, path: str, method: str, params: Optional[dict],
             json: Optional[dict], data: Optional[dict]):
         while True:
             try:
                 response = await self.client.request(
-                    method, path, params=params, json=json, data=data
+                        method, path, params=params, json=json, data=data  # type: ignore
                 )
             except httpx.ReadTimeout:
                 pass
             else:
                 return response
```

## netschoolapi/netschoolapi.py

```diff
@@ -2,15 +2,15 @@
 from hashlib import md5
 from io import BytesIO
 from typing import Optional, Dict, List, Union
 
 import httpx
 from httpx import AsyncClient, Response
 
-from netschoolapi import data, errors, schemas
+from netschoolapi import errors, schemas
 
 __all__ = ['NetSchoolAPI']
 
 from netschoolapi.async_client_wrapper import AsyncClientWrapper, Requester
 
 
 async def _die_on_bad_status(response: Response):
@@ -36,19 +36,20 @@
 
         self._assignment_types: Dict[int, str] = {}
         self._login_data = ()
 
     async def __aenter__(self) -> 'NetSchoolAPI':
         return self
 
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
+    async def __aexit__(self, _exc_type, _exc_val, _exc_tb):
         await self.logout()
 
     async def login(
-            self, user_name: str, password: str, school: str,
+            self, user_name: str, password: str,
+            school_name_or_id: Union[int, str],
             requests_timeout: int = None):
         requester = self._wrapped_client.make_requester(requests_timeout)
         # Getting the `NSSESSIONID` cookie for `auth/getdata`
         await requester('logindata')
 
         # Getting the `NSSESSIONID` cookie for `login`
         response = await requester('auth/getdata', method="POST")
@@ -62,15 +63,15 @@
         pw = pw2[: len(password)]
 
         try:
             response = await requester(
                 'login',
                 data={
                     'loginType': 1,
-                    **(await self._address(school, requester)),
+                    **(await self._address(school_name_or_id, requester)),
                     'un': user_name,
                     'pw': pw,
                     'pw2': pw2,
                     **login_meta,
                 },
                 method="POST"
             )
@@ -108,15 +109,15 @@
             'grade/assignment/types', params={'all': False}
         )
         assignment_reference = response.json()
         self._assignment_types = {
             assignment['id']: assignment['name']
             for assignment in assignment_reference
         }
-        self._login_data = (user_name, password, school)
+        self._login_data = (user_name, password, school_name_or_id)
 
     async def _request_with_optional_relogin(
             self, requests_timeout: Optional[int], path: str,
             method="GET", params: dict = None, json: dict = None):
         try:
             response = await self._wrapped_client.request(
                 requests_timeout, path, method, params, json,
@@ -138,54 +139,48 @@
                     )
             else:
                 raise http_status_error
         else:
             return response
 
     async def download_attachment(
-            self, attachment: data.Attachment,
-            path_or_file: Union[BytesIO, str] = None,
+            self, attachment_id: int,
+            path_or_file: Union[BytesIO, str],
             requests_timeout: int = None):
-        """
-        If `path_to_file` is a string, it should contain absolute path to file
-        """
-        if path_or_file is None:
-            file = open(attachment.name, "wb")
-            file_is_new = True
-        elif isinstance(path_or_file, str):
+        if isinstance(path_or_file, str):
             file = open(path_or_file, "wb")
             file_is_new = True
         else:
             file = path_or_file
             file_is_new = False
         file.write((
             await self._request_with_optional_relogin(
                 requests_timeout,
-                f"attachments/{attachment.id}",
+                f"attachments/{attachment_id}",
             )
         ).content)
         if file_is_new:
             file.close()
 
     async def download_attachment_as_bytes(
-            self, attachment: data.Attachment, requests_timeout: int = None,
+            self, attachment_id: int, requests_timeout: int = None,
     ) -> BytesIO:
         attachment_contents_buffer = BytesIO()
         await self.download_attachment(
-            attachment, path_or_file=attachment_contents_buffer,
+            attachment_id, path_or_file=attachment_contents_buffer,
             requests_timeout=requests_timeout
         )
         return attachment_contents_buffer
 
     async def diary(
         self,
         start: Optional[date] = None,
         end: Optional[date] = None,
         requests_timeout: int = None,
-    ) -> data.Diary:
+    ) -> schemas.Diary:
         if not start:
             monday = date.today() - timedelta(days=date.today().weekday())
             start = monday
         if not end:
             end = start + timedelta(days=5)
 
         response = await self._request_with_optional_relogin(
@@ -196,22 +191,23 @@
                 'yearId': self._year_id,
                 'weekStart': start.isoformat(),
                 'weekEnd': end.isoformat(),
             },
         )
         diary_schema = schemas.Diary()
         diary_schema.context['assignment_types'] = self._assignment_types
-        return data.diary(diary_schema.load(response.json()))
+        diary = diary_schema.load(response.json())
+        return diary  # type: ignore
 
     async def overdue(
         self,
         start: Optional[date] = None,
         end: Optional[date] = None,
         requests_timeout: int = None,
-    ) -> List[data.Assignment]:
+    ) -> List[schemas.Assignment]:
         if not start:
             monday = date.today() - timedelta(days=date.today().weekday())
             start = monday
         if not end:
             end = start + timedelta(days=5)
 
         response = await self._request_with_optional_relogin(
@@ -223,54 +219,51 @@
                 'weekStart': start.isoformat(),
                 'weekEnd': end.isoformat(),
             },
         )
         assignments_schema = schemas.Assignment()
         assignments_schema.context['assignment_types'] = self._assignment_types
         assignments = assignments_schema.load(response.json(), many=True)
-        return [data.Assignment(**assignment) for assignment in assignments]
+        return assignments  # type: ignore
 
     async def announcements(
             self, take: Optional[int] = -1,
-            requests_timeout: int = None) -> List[data.Announcement]:
+            requests_timeout: int = None) -> List[schemas.Announcement]:
         response = await self._request_with_optional_relogin(
             requests_timeout,
             'announcements',
             params={'take': take},
         )
         announcements = schemas.Announcement().load(response.json(), many=True)
-        return [
-            data.announcement(announcement)
-            for announcement in announcements
-        ]
+        return announcements  # type: ignore
 
     async def attachments(
-            self, assignment: data.Assignment,
-            requests_timeout: int = None) -> List[data.Attachment]:
+            self, assignment_id: int,
+            requests_timeout: int = None) -> List[schemas.Attachment]:
         response = await self._request_with_optional_relogin(
             requests_timeout,
             method="POST",
             path='student/diary/get-attachments',
             params={'studentId': self._student_id},
-            json={'assignId': [assignment.id]},
+            json={'assignId': [assignment_id]},
         )
         response = response.json()
         if not response:
             return []
         attachments_json = response[0]['attachments']
         attachments = schemas.Attachment().load(attachments_json, many=True)
-        return [data.Attachment(**attachment) for attachment in attachments]
+        return attachments  # type: ignore
 
-    async def school(self, requests_timeout: int = None):
+    async def school(self, requests_timeout: int = None) -> schemas.School:
         response = await self._request_with_optional_relogin(
             requests_timeout,
             'schools/{0}/card'.format(self._school_id),
         )
         school = schemas.School().load(response.json())
-        return data.School(**school)
+        return school  # type: ignore
 
     async def logout(self, requests_timeout: int = None):
         try:
             await self._wrapped_client.request(
                 requests_timeout,
                 'auth/logout',
                 method="POST",
@@ -287,24 +280,30 @@
             else:
                 raise http_status_error
 
     async def full_logout(self, requests_timeout: int = None):
         await self.logout(requests_timeout)
         await self._wrapped_client.client.aclose()
 
-    async def _address(
-            self, school: str, requester: Requester) -> Dict[str, int]:
-        response = await requester('addresses/schools')
+    async def schools(
+            self, requests_timeout: int = None) -> List[schemas.ShortSchool]:
+        resp = await self._wrapped_client.request(requests_timeout, "addresses/schools")
+        schools = schemas.ShortSchool().load(resp.json(), many=True)
+        return schools  # type: ignore
 
-        schools_reference = response.json()
-        for school_ in schools_reference:
-            if school_['name'] == school or school_['id'] == school:
-                self._school_id = school_['id']
+    async def _address(
+            self, school_name_or_id: Union[int, str],
+            requester: Requester) -> Dict[str, int]:
+        schools = (await requester("addresses/schools")).json()
+
+        for school in schools:
+            if school["name"] == school_name_or_id or school["id"] == school_name_or_id:
+                self._school_id = school['id']
                 return {
-                    'cid': school_['countryId'],
-                    'sid': school_['stateId'],
-                    'pid': school_['municipalityDistrictId'],
-                    'cn': school_['cityId'],
+                    'cid': school['countryId'],
+                    'sid': school['stateId'],
+                    'pid': school['municipalityDistrictId'],
+                    'cn': school['cityId'],
                     'sft': 2,
-                    'scid': school_['id'],
+                    'scid': school['id'],
                 }
-        raise errors.SchoolNotFoundError(school)
+        raise errors.SchoolNotFoundError(school_name_or_id)
```

## netschoolapi/schemas.py

```diff
@@ -13,19 +13,26 @@
 
 class Attachment(NetSchoolAPISchema):
     id = fields.Integer()
     name = fields.String(data_key='originalFileName')
     description = fields.String(allow_none=True, missing='')
 
 
+class Author(NetSchoolAPISchema):
+    id = fields.Integer()
+    full_name = fields.String(data_key="fio")
+    nickname = fields.String(data_key="nickName")
+
+
 class Announcement(NetSchoolAPISchema):
     name = fields.String()
     content = fields.String(data_key='description')
     post_date = fields.DateTime(data_key='postDate')
     attachments = fields.List(fields.Nested(Attachment), missing=[])
+    author = fields.Nested(Author)
 
 
 class Assignment(NetSchoolAPISchema):
     id = fields.Integer()
     type = fields.Function(
         deserialize=(
             lambda type_id, context: context['assignment_types'][type_id]
@@ -69,24 +76,30 @@
 
 class Diary(NetSchoolAPISchema):
     start = fields.Date(data_key='weekStart')
     end = fields.Date(data_key='weekEnd')
     schedule = fields.List(fields.Nested(Day), data_key='weekDays')
 
 
+class ShortSchool(NetSchoolAPISchema):
+    name = fields.String()
+    id = fields.Integer()
+    address = fields.String(data_key="addressString")
+
+
 class School(NetSchoolAPISchema):
     name = fields.String(data_key='fullSchoolName')
-    about = fields.String(data_key='about')
+    about = fields.String()
 
-    address = fields.String(data_key='address')
-    email = fields.String(data_key='email')
+    address = fields.String()
+    email = fields.String()
     site = fields.String(data_key='web')
     phone = fields.String(data_key='phones')
 
-    director = fields.String(data_key='director')
+    director = fields.String()
     AHC = fields.String(data_key='principalAHC')
     IT = fields.String(data_key='principalIT')
     UVR = fields.String(data_key='principalUVR')
 
     @pre_load
     def unwrap_nested_dicts(
             self, school: Dict[str, Any], **_) -> Dict[str, str]:
```

## Comparing `netschoolapi-8.0.0.dist-info/LICENSE` & `netschoolapi-9.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `netschoolapi-8.0.0.dist-info/METADATA` & `netschoolapi-9.0.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: netschoolapi
-Version: 8.0.0
-Summary: =?utf-8?b?0JDRgdC40L3RhdGA0L7QvdC90YvQuSBBUEkt0LrQu9C40LXQvdGCINC00LvRjyDCq9Ch0LXRgtC10LLQvtCz0L4g0LPQvtGA0L7QtNCwwrs=?=
+Version: 9.0.0
+Summary: Асинхронный API-клиент для «Сетевого города»
 Home-page: https://github.com/nm17/netschoolapi/
 Author: nm17
 Author-email: dannevergame@gmail.com
 Maintainer: igorlanov
 Maintainer-email: vonalrogi@ya.ru
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
```

