# Comparing `tmp/SDTcloud-0.1.2.tar.gz` & `tmp/SDTcloud-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SDTcloud-0.1.2.tar", last modified: Thu May  4 06:26:21 2023, max compression
+gzip compressed data, was "SDTcloud-0.1.3.tar", last modified: Thu May  4 06:33:55 2023, max compression
```

## Comparing `SDTcloud-0.1.2.tar` & `SDTcloud-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 06:26:21.950447 SDTcloud-0.1.2/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 06:26:21.950311 SDTcloud-0.1.2/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)       12 2023-05-04 01:12:59.000000 SDTcloud-0.1.2/README.md
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 06:26:21.949254 SDTcloud-0.1.2/SDTcloud/
--rw-r--r--   0 june       (501) staff       (20)       75 2023-05-04 01:12:59.000000 SDTcloud-0.1.2/SDTcloud/__init__.py
--rw-r--r--   0 june       (501) staff       (20)    10543 2023-05-04 06:26:04.000000 SDTcloud-0.1.2/SDTcloud/sdtcloud.py
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 06:26:21.950092 SDTcloud-0.1.2/SDTcloud.egg-info/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 06:26:21.000000 SDTcloud-0.1.2/SDTcloud.egg-info/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)      188 2023-05-04 06:26:21.000000 SDTcloud-0.1.2/SDTcloud.egg-info/SOURCES.txt
--rw-r--r--   0 june       (501) staff       (20)        1 2023-05-04 06:26:21.000000 SDTcloud-0.1.2/SDTcloud.egg-info/dependency_links.txt
--rw-r--r--   0 june       (501) staff       (20)        9 2023-05-04 06:26:21.000000 SDTcloud-0.1.2/SDTcloud.egg-info/top_level.txt
--rw-r--r--   0 june       (501) staff       (20)       38 2023-05-04 06:26:21.950485 SDTcloud-0.1.2/setup.cfg
--rw-r--r--   0 june       (501) staff       (20)      656 2023-05-04 06:26:17.000000 SDTcloud-0.1.2/setup.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 06:33:55.048390 SDTcloud-0.1.3/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 06:33:55.048246 SDTcloud-0.1.3/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)       12 2023-05-04 01:12:59.000000 SDTcloud-0.1.3/README.md
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 06:33:55.046188 SDTcloud-0.1.3/SDTcloud/
+-rw-r--r--   0 june       (501) staff       (20)       75 2023-05-04 01:12:59.000000 SDTcloud-0.1.3/SDTcloud/__init__.py
+-rw-r--r--   0 june       (501) staff       (20)    10599 2023-05-04 06:33:45.000000 SDTcloud-0.1.3/SDTcloud/sdtcloud.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 06:33:55.048039 SDTcloud-0.1.3/SDTcloud.egg-info/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 06:33:55.000000 SDTcloud-0.1.3/SDTcloud.egg-info/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)      188 2023-05-04 06:33:55.000000 SDTcloud-0.1.3/SDTcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 june       (501) staff       (20)        1 2023-05-04 06:33:55.000000 SDTcloud-0.1.3/SDTcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 june       (501) staff       (20)        9 2023-05-04 06:33:55.000000 SDTcloud-0.1.3/SDTcloud.egg-info/top_level.txt
+-rw-r--r--   0 june       (501) staff       (20)       38 2023-05-04 06:33:55.048425 SDTcloud-0.1.3/setup.cfg
+-rw-r--r--   0 june       (501) staff       (20)      656 2023-05-04 06:33:52.000000 SDTcloud-0.1.3/setup.py
```

### Comparing `SDTcloud-0.1.2/SDTcloud/sdtcloud.py` & `SDTcloud-0.1.3/SDTcloud/sdtcloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,14 @@
     # TODO
     #  - object 생성 후, 로그인을 하도록 설계 해야 함 - ok 
     #  - url도 입력해서 로그인할 수 있도록 설계 해야 함 - ok
     #  - config함수에서 필요한 변수들 정의할 수 있도록 설계 해야 함 - ok
     #  - 예외처리 함수를 추가해서 예외 처리하는게 이쁘다. - ok
     #  - 리턴 값 포맷 정의
 
-    def config(self, address, port):
-        """ Setting config information.
-
-        Args:
-            address (Str): API Address
-            port (Str): API Port
-        """
-        self.url = f"http://{address}:{port}"
-
     def successMessage(self, codeValue):
         if codeValue == 1:
             print("Ok!!!, Status: 200")
         elif codeValue == 2:
             print("Created!!!, Status: 201")
         elif codeValue == 3:
             print("No Content!!!, Status: 204")
@@ -61,15 +52,23 @@
         elif status_code == 201:
             return 2, "Created!!!, Status: 200"
         elif status_code == 204:
             return 3, "No Content!!!, Status: 200"
         else:
             return 0, ""
            
+    def config(self, address, port):
+        """ Setting config information.
 
+        Args:
+            address (Str): API Address
+            port (Str): API Port
+        """
+        self.url = f"http://{address}:{port}"
+        print("Ok!!!")
 
     # 로그인
     def login(self):
         """ login of stackbase. 
 
         Raises:
             Exception: _description_
@@ -87,15 +86,15 @@
             "password": userPassword
         }
         
         response = requests.request('post',f"{self.url}/oauth/token", headers=headers, data=bodys)
         respStatus, returnMessage = self.checkStatusCode(response.status_code)
 
         if respStatus == 0:
-            exceptionHandle(response)
+            self.exceptionHandle(response)
         
         result = json.loads(response.content)
 
         self.userToken = f"Bearer {result['accessToken']}"
 
         print(returnMessage)
 
@@ -123,15 +122,15 @@
             "tag": tag
         })
 
         response = requests.request('post',f"{self.url}/stackbase/v1/storages", headers=headers, data=bodys)
         respStatus, returnMessage = self.checkStatusCode(response.status_code)
 
         if respStatus == 0:
-            exceptionHandle(response)
+            self.exceptionHandle(response)
 
         result = json.loads(response.content)
         result['createdAt'] = datetime.fromtimestamp(int(result['createdAt']/1000), timezone(timedelta(hours=9)))
         result['updatedAt'] = datetime.fromtimestamp(int(result['updatedAt']/1000), timezone(timedelta(hours=9)))
         
         print(returnMessage)
         return result
@@ -155,15 +154,15 @@
             "Authorization": self.userToken
         }
 
         response = requests.request('get',f"{self.url}/stackbase/v1/storages", headers=headers)
         respStatus, returnMessage = self.checkStatusCode(response.status_code)
 
         if respStatus == 0:
-            exceptionHandle(response)
+            self.exceptionHandle(response)
         
         result = json.loads(response.content)
         df = pd.DataFrame(result)
         for n in range(len(df)):
             df.loc[n, 'createdAt'] = datetime.fromtimestamp(int(df.loc[n, 'createdAt']/1000), timezone(timedelta(hours=9)))
             df.loc[n, 'updatedAt'] = datetime.fromtimestamp(int(df.loc[n, 'updatedAt']/1000), timezone(timedelta(hours=9)))
 
@@ -204,15 +203,15 @@
             "storageId": storageId
         })
 
         response = requests.request('post',f"{self.url}/stackbase/v1/folder", headers=headers, data=bodys)
         respStatus, returnMessage = self.checkStatusCode(response.status_code)
 
         if respStatus == 0:
-            exceptionHandle(response)
+            self.exceptionHandle(response)
 
         result = json.loads(response.content)
         result['createdAt'] = datetime.fromtimestamp(int(result['createdAt']/1000), timezone(timedelta(hours=9)))
         
         print(returnMessage)
         return result
     
@@ -240,15 +239,15 @@
             "parentId": parentId
         }
 
         response = requests.request('get',f"{self.url}/stackbase/v1/trees", headers=headers, params=param)
         respStatus, returnMessage = self.checkStatusCode(response.status_code)
 
         if respStatus == 0:
-            exceptionHandle(response)
+            self.exceptionHandle(response)
         
         result = json.loads(response.content)
         df1 = pd.DataFrame(result)
         df2 = pd.DataFrame(result['trees'])
         
         df = pd.concat([df1.drop(['trees'], axis=1), df2], axis=1)
         df['modifiedAt'] = datetime.fromtimestamp(int(df['modifiedAt']/1000), timezone(timedelta(hours=9)))
@@ -291,15 +290,15 @@
             "Authorization": self.userToken
         }
 
         response = requests.request('get',f"{self.url}/stackbase/v1/contents/download/{fileId}", headers=headers)
         respStatus, returnMessage = self.checkStatusCode(response.status_code)
 
         if respStatus == 0:
-            exceptionHandle(response)
+            self.exceptionHandle(response)
         
         with open(getPath, "wb") as f:
             f.write(response.content)
         
         print(returnMessage)
     
     # 컨텐츠 등록
@@ -339,15 +338,15 @@
             "content": (filePath.split("/")[-1], file_open, 'application/octet-stream')
         }
 
         response = requests.request("POST", f"{self.url}/stackbase/v1/contents", headers=headers, files=files)
         respStatus, returnMessage = self.checkStatusCode(response.status_code)
 
         if respStatus == 0:
-            exceptionHandle(response)
+            self.exceptionHandle(response)
 
         result = json.loads(response.content)
         result['createdAt'] = datetime.fromtimestamp(int(result['createdAt']/1000), timezone(timedelta(hours=9)))
         result['modifiedAt'] = datetime.fromtimestamp(int(result['modifiedAt']/1000), timezone(timedelta(hours=9)))
         
         print(returnMessage)
         return result
```

### Comparing `SDTcloud-0.1.2/setup.py` & `SDTcloud-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SDTcloud", # Replace with your own username
-    version="0.1.2",
+    version="0.1.3",
     author="sujune",
     author_email="hoakw@sdt.inc",
     description="SDT cloud API Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

