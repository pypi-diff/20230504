# Comparing `tmp/navalmartin_mir_aws_utils-0.0.28.tar.gz` & `tmp/navalmartin_mir_aws_utils-0.0.9.tar.gz`

## Comparing `navalmartin_mir_aws_utils-0.0.28.tar` & `navalmartin_mir_aws_utils-0.0.9.tar`

### file list

```diff
@@ -1,51 +1,28 @@
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/.pre-commit-config.yaml
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/requirements.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/.idea/.gitignore
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/.idea/misc.xml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/.idea/modules.xml
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/.idea/navalmartin_mir_aws_utils.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/.idea/vcs.xml
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/.idea/.gitignore
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/.idea/modules.xml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/.idea/src.iml
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/.idea/vcs.xml
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/__init__.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/aws_credentials.py
--rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/boto3_client.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/cognito_idp_utils.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/env_utils.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/exceptions.py
--rw-r--r--   0        0        0     9475 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/file_s3_batch.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/s3_utils.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/sqs_queue_config.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/sqs_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/examples/__init__.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/examples/create_image_batch.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/examples/lamda_task_decorator.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/examples/working_with_cognito.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/examples/working_with_s3.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/examples/working_with_secrets_manager.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/examples/working_with_ses.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/examples/working_with_sqs.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/tasks/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/tasks/ses_tasks/__init__.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/tasks/ses_tasks/ses_tasks.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/tasks_lambdas/__init__.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/tasks_lambdas/aws_tasks_decorator.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/tasks_lambdas/tasks_lambdas_utils.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/utils/__init__.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/utils/cognito_user_data.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/utils/sfn_utils.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/utils/simple_email.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/utils/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/LICENSE
--rw-r--r--   0        0        0    10654 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/README.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/pyproject.toml
--rw-r--r--   0        0        0    11264 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.28/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/requirements.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/setup.cfg
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/setup.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/.idea/.gitignore
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/.idea/modules.xml
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/.idea/src.iml
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/.idea/vcs.xml
+-rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/.idea/workspace.xml
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/navalmartin_mir_aws_utils/__init__.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/navalmartin_mir_aws_utils/aws_credentials.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/navalmartin_mir_aws_utils/boto3_client.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/navalmartin_mir_aws_utils/env_utils.py
+-rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/navalmartin_mir_aws_utils/image_s3_batch.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/navalmartin_mir_aws_utils/s3_utils.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/navalmartin_mir_aws_utils/sqs_queue_config.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/navalmartin_mir_aws_utils/sqs_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/navalmartin_mir_aws_utils/examples/__init__.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/navalmartin_mir_aws_utils/examples/create_image_batch.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/src/navalmartin_mir_aws_utils/examples/send_sqs_message.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/README.md
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 navalmartin_mir_aws_utils-0.0.9/PKG-INFO
```

### Comparing `navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/env_utils.py` & `navalmartin_mir_aws_utils-0.0.9/src/navalmartin_mir_aws_utils/env_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 
     A dictionary with the values of the environment variables
     """
 
     variables = {}
 
     for name in var_names:
+
         if name in variables:
-            raise ValueError(f"Duplicate variable {name} found")
+            raise ValueError(f'Duplicate variable {name} found')
         value = os.getenv(name, default=None)
 
         if value is None:
             raise ValueError(f"Environment variable {name} is not set")
 
         variables[name] = value
```

### Comparing `navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/file_s3_batch.py` & `navalmartin_mir_aws_utils-0.0.9/src/navalmartin_mir_aws_utils/image_s3_batch.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,320 +1,163 @@
 """module image_s3_batch. Represents
 a batch of images on S3
 
 """
 import os
-from typing import List, Any, Union, Callable
+from typing import List, Any, Union
 from navalmartin_mir_aws_utils.aws_credentials import AWSCredentials_S3
 from navalmartin_mir_aws_utils.boto3_client import get_aws_s3_client
-from navalmartin_mir_aws_utils.s3_utils import (
-    expand_s3_iterator_contents,
-    expand_s3_iterator_common_prefixes,
-)
-
-S3_URI = "s3://"
+from navalmartin_mir_aws_utils.s3_utils import expand_s3_iterator_contents, expand_s3_iterator_common_prefixes
 
 
-class FilePathBatch(object):
-    def __init__(
-        self,
-        s3_credentials: AWSCredentials_S3,
-        delimiter: str = "/",
-        do_build_client: bool = True,
-    ):
+class ImagePathBatch(object):
+
+    def __init__(self, s3_credentials: AWSCredentials_S3, delimiter: str = '/',
+                 do_build_client: bool = True):
         self.aws_bucket_credentials = s3_credentials
-        self.files: List[Any] = []
+        self.images: List[dict] = []
         self.delimiter = delimiter
         self._current_pos: int = -1
         self._client: Any = None
 
         if do_build_client:
             self.build_client()
 
     def __len__(self):
-        return len(self.files)
+        return len(self.images)
 
     def __iter__(self):
         self._current_pos = 0
         return self
 
     def __next__(self):
-        if len(self.files) == 0:
+        if len(self.images) == 0:
             raise StopIteration
 
-        if self._current_pos < len(self.files):
-            result = self.files[self._current_pos]
+        if self._current_pos < len(self.images):
+            result = self.images[self._current_pos]
             self._current_pos += 1
             return result
         else:
             self._current_pos = -1
             raise StopIteration
 
-    def __getitem__(self, key: Union[int, str]) -> str:
-        """Returns the image that corresponds to the given key
-
-        Parameters
-        ----------
-        key
-
-        Returns
-        -------
-
-        A string representing the image in the batch
-        """
-        if type(key) == int:
-            if key >= len(self.files):
-                raise ValueError(
-                    f"Invalid key. Integer key {key} cannot be >= {len(self.files)}"
-                )
-
-            key = self.files[key]
-            return key
-        elif type(key) == str:
-            if key not in self.files:
-                raise ValueError(f"key={key} not in {self.files}")
-            return key
-        else:
-            raise ValueError(f"key type {type(key)} is not valid")
-
-    def reinit(
-        self,
-        s3_credentials: AWSCredentials_S3,
-        delimiter: str = "/",
-        do_build_client: bool = True,
-    ):
-        """Set the file batch to the state just after the constructor
-        was called
-
-        Parameters
-        ----------
-        s3_credentials
-        delimiter
-        do_build_client
-
-        Returns
-        -------
-
-        """
-
-        self.aws_bucket_credentials = s3_credentials
-        self.files: List[Any] = []
-        self.delimiter = delimiter
-        self._current_pos: int = -1
-        self._client: Any = None
-
-        if do_build_client:
-            self.build_client()
-
     def build_client(self) -> Any:
-        """Build an S3 client from the given AWS S3 credentials
-
-        Returns
-        -------
-
-        """
         self._client = get_aws_s3_client(credentials=self.aws_bucket_credentials)
 
-    def load_from_list(self, files: List[str], delimiter="/"):
-        self.files = files
+    def load_from_list(self, images: List[str], delimiter="/"):
+        self.images = images
         self.delimiter = delimiter
 
-    def read_file_byte_string(
-        self,
-        key: Union[int, str],
-        read_from_local_host: bool = False,
-        file_reader: Callable = None,
-    ) -> str:
-        """Returns the byte string associated with the given key
+    def read(self, prefixes: tuple, valid_image_extensions: tuple,
+             delimiter: str = '/'):
 
-        Parameters
-        ----------
-        file_reader
-        read_from_local_host
-        key: The key of the object to read
-
-        Returns
-        -------
-
-        The byte string of the object that is represented by the
-        given key
-
-        """
-
-        if read_from_local_host:
-            image = self[key]
-            return file_reader(image)
-
-        file_obj = self.get_object(key=key)
-
-        if "Body" not in file_obj:
-            raise ValueError("Body is missing from file object response")
-
-        return file_obj["Body"].read()
-
-    def read(
-        self, prefixes: tuple, valid_image_extensions: tuple, delimiter: str = "/"
-    ):
         self.delimiter = delimiter
 
-        # empty the files as we will read new ones
-        self.files = []
-
-        if self._client is None:
-            self.build_client()
-
         # get the object that lists the objects
         # on S3
-        paginator = self._client.get_paginator("list_objects")
+        paginator = self._client.get_paginator('list_objects')
 
         for prefix in prefixes:
-            s3_iterator = paginator.paginate(
-                Bucket=self.aws_bucket_credentials.aws_s3_bucket_name,
-                Delimiter=self.delimiter,
-                Prefix=prefix,
-            )
+            s3_iterator = paginator.paginate(Bucket=self.aws_bucket_credentials.aws_s3_bucket_name,
+                                             Delimiter=self.delimiter,
+                                             Prefix=prefix)
 
             contents = expand_s3_iterator_contents(s3_iterator)
 
             if len(contents) != 0:
-                self.read_from_contents(
-                    contents=contents, valid_image_extensions=valid_image_extensions
-                )
-
-            common_prefixes = expand_s3_iterator_common_prefixes(
-                s3_iterator=s3_iterator
-            )
+                self.read_from_contents(contents=contents,
+                                        valid_image_extensions=valid_image_extensions)
+
+            common_prefixes = expand_s3_iterator_common_prefixes(s3_iterator=s3_iterator)
             if len(common_prefixes) != 0:
-                self.read_from_common_prefixes(
-                    common_prefixes=common_prefixes,
-                    valid_image_extensions=valid_image_extensions,
-                )
+                self.read_from_common_prefixes(common_prefixes=common_prefixes,
+                                               valid_image_extensions=valid_image_extensions)
 
     def copy_to(self, s3_credentials_to: AWSCredentials_S3) -> None:
         """Copy the images in the bucket to the S3 bucket specified
         by the provided credentials
 
         Parameters
         ----------
         s3_credentials_to: The credentials to use for the bucket to copy
 
         Returns
         -------
 
         """
 
-        if len(self.files) == 0:
+        if len(self.images) == 0:
             print("WARNING: Image batch is empty...")
             return
 
         raise NotImplementedError("The function is not implemented")
 
-    def copy_file_to(
-        self,
-        key: Union[int, str],
-        s3_credentials_to: AWSCredentials_S3,
-        new_filename: str = "",
-        **kwargs,
-    ) -> dict:
-        """Copies the specified file identified by the given key
-        into the bucket specified in the given AWSCredentials_S3 credentials
-
-        Parameters
-        ----------
-        key: The index of the file to copy to
-        s3_credentials_to: Credentials for accessing the new bucket
-        kwargs: Arguments to orchestrate how the copy is done
-
-        Returns
-        -------
-
-        """
-
-        item_to_copy = self[key]
-
-        if new_filename == "":
-            new_filename = item_to_copy
-
-        if self._client is None:
-            self.build_client()
-
-        copy_source = (
-            self.aws_bucket_credentials.aws_s3_bucket_name + "/" + item_to_copy
-        )
-        copy_response = self._client.copy_object(
-            Bucket=s3_credentials_to.aws_s3_bucket_name,
-            Key=new_filename,
-            CopySource=copy_source,
-            **kwargs,
-        )
-        return copy_response
-
     def get_object(self, key: Union[int, str]) -> Any:
         """Returns the object specified with the given key.
 
         Parameters
         ----------
         key: The key of the object to return
 
         Returns
         -------
 
         """
 
         if type(key) == int:
-            if key >= len(self.files):
-                raise ValueError(
-                    f"Invalid key. Integer key {key} cannot be >= {len(self.files)}"
-                )
 
-            key = self.files[key]
+            if key >= len(self.images):
+                raise ValueError(f"Invalid key. Integer key {key} cannot be >= {len(self.images)}")
+
+            key = self.images[key]
         elif type(key) == str:
-            if key not in self.files:
-                raise ValueError(f"key={key} not in {self.files}")
+            if key not in self.images:
+                raise ValueError(f"key={key} not in {self.images}")
         else:
-            raise ValueError(f"key type {type(key)} is not valid")
+            raise ValueError(f"key type {type(key)} is not valie")
 
         if self._client is None:
             raise ValueError("S3 client is not built")
 
-        file_byte_string = self._client.get_object(
-            Bucket=self.aws_bucket_credentials.aws_s3_bucket_name, Key=key
-        )
+        file_byte_string = self._client.get_object(Bucket=self.aws_bucket_credentials.aws_s3_bucket_name,
+                                                   Key=key)
 
         return file_byte_string
 
-    def read_from_contents(
-        self, contents: List[dict], valid_image_extensions: tuple
-    ) -> None:
+    def read_from_contents(self, contents: List[dict], valid_image_extensions: tuple) -> None:
         """Read the contents of the S3 bucket
 
         Parameters
         ----------
         contents: The contents to use for reading the images
         valid_image_extensions: The valid_image_extensions to look for
 
         Returns
         -------
 
         """
 
         n_extensions = len(valid_image_extensions)
         for content in contents:
-            image = content.get("Key")
+
+            image = content.get('Key')
 
             if n_extensions != 0:
+
                 img_extension = os.path.splitext(image)[1]
                 if img_extension in valid_image_extensions:
-                    self.files.append(content.get("Key"))
+                    self.images.append({'img': content.get('Key'),
+                                        'bucket': self.aws_bucket_credentials.aws_s3_bucket_name})
             else:
-                self.files.append(content.get("Key"))
+                self.images.append({'img': content.get('Key'),
+                                    'bucket': self.aws_bucket_credentials.aws_s3_bucket_name})
 
-    def read_from_common_prefixes(
-        self, common_prefixes: List[dict], valid_image_extensions: tuple
-    ) -> None:
+    def read_from_common_prefixes(self, common_prefixes: List[dict],
+                                  valid_image_extensions: tuple) -> None:
         """Read from the common_prefixes
 
         Parameters
         ----------
         common_prefixes: The common_prefixes to use for reading
         valid_image_extensions: The valid_image_extensions to look for
 
@@ -322,21 +165,18 @@
         -------
 
         """
 
         if self._client is None:
             raise ValueError("S3 client is not built")
 
-        paginator = self._client.get_paginator("list_objects")
+        paginator = self._client.get_paginator('list_objects')
         for item in common_prefixes:
-            prefix = item["Prefix"]
+            prefix = item['Prefix']
 
-            s3_iterator = paginator.paginate(
-                Bucket=self.aws_bucket_credentials.aws_s3_bucket_name,
-                Delimiter=self.delimiter,
-                Prefix=prefix,
-            )
+            s3_iterator = paginator.paginate(Bucket=self.aws_bucket_credentials.aws_s3_bucket_name,
+                                             Delimiter=self.delimiter,
+                                             Prefix=prefix)
 
             contents = expand_s3_iterator_contents(s3_iterator)
-            self.read_from_contents(
-                contents=contents, valid_image_extensions=valid_image_extensions
-            )
+            self.read_from_contents(contents=contents,
+                                    valid_image_extensions=valid_image_extensions)
```

### Comparing `navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/sqs_queue_config.py` & `navalmartin_mir_aws_utils-0.0.9/src/navalmartin_mir_aws_utils/sqs_queue_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from typing import List, Union
 
 
 class MessageAttributes:
     def __init__(self):
         self.string_value: str = ""
-        self.binary_value: bytes = b"bytes"
+        self.binary_value: bytes = b'bytes'
         self.string_list_values: List[str]
-        self.binary_list_values: List[b"bytes"]
+        self.binary_list_values: List[b'bytes']
         self.data_type: str
 
 
 class SQSMessageConfig(object):
-    def __init__(
-        self,
-        message_body: str,
-        message_group_id: str,
-        message_attributes: Union[MessageAttributes, None],
-        message_deduplication_id: str,
-        delay_seconds: int = 123,
-    ):
+    def __init__(self, message_body: str,
+                 message_group_id: str,
+                 message_attributes: Union[MessageAttributes, None],
+                 message_deduplication_id: str,
+                 delay_seconds: int = 123):
         self.message_body: str = message_body
         self.message_group_id = message_group_id
         self.message_deduplication_id = message_deduplication_id
         self.message_attributes = message_attributes
         self.delay_seconds = delay_seconds
```

### Comparing `navalmartin_mir_aws_utils-0.0.28/src/navalmartin_mir_aws_utils/sqs_utils.py` & `navalmartin_mir_aws_utils-0.0.9/src/navalmartin_mir_aws_utils/sqs_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,108 +1,91 @@
 from typing import Any
 from navalmartin_mir_aws_utils.aws_credentials import AWSCredentials_SQS
 from navalmartin_mir_aws_utils.boto3_client import get_aws_sqs_client
 from navalmartin_mir_aws_utils.sqs_queue_config import SQSMessageConfig
 
 
-def send_sqs_message(
-    sqs_credentials: AWSCredentials_SQS,
-    sqs_msg: SQSMessageConfig,
-    sqs_client: Any = None,
-) -> dict:
+def send_sqs_message(sqs_credentials: AWSCredentials_SQS,
+                     sqs_msg: SQSMessageConfig, sqs_client: Any = None) -> dict:
     """Send a message to the SQS queue specified
     under the sqs credentials
 
     Parameters
     ----------
     sqs_credentials: The credentials to use to send the message
     sqs_msg: The message configuration
 
     Returns
     -------
     A dictionary with the response attributes
     """
 
     if sqs_client is not None:
-        response = sqs_client.send_message(
-            QueueUrl=sqs_credentials.queue_url,
-            MessageBody=sqs_msg.message_body,
-            # DelaySeconds=sqs_msg.delay_seconds,
-            MessageAttributes=sqs_msg.message_attributes
-            if sqs_msg.message_attributes is not None
-            else {},
-            MessageGroupId=sqs_msg.message_group_id,
-            MessageDeduplicationId=sqs_msg.message_deduplication_id,
-        )
+        response = sqs_client.send_message(QueueUrl=sqs_credentials.queue_url,
+                                           MessageBody=sqs_msg.message_body,
+                                           # DelaySeconds=sqs_msg.delay_seconds,
+                                           MessageAttributes=sqs_msg.message_attributes if sqs_msg.message_attributes is not None else {},
+                                           MessageGroupId=sqs_msg.message_group_id,
+                                           MessageDeduplicationId=sqs_msg.message_deduplication_id)
         return response
 
     new_sqs_client = get_aws_sqs_client(credentials=sqs_credentials)
-    response: dict = new_sqs_client.send_message(
-        QueueUrl=sqs_credentials.queue_url,
-        MessageBody=sqs_msg.message_body,
-        # DelaySeconds=sqs_msg.delay_seconds,
-        MessageAttributes=sqs_msg.message_attributes
-        if sqs_msg.message_attributes is not None
-        else {},
-        MessageGroupId=sqs_msg.message_group_id,
-        MessageDeduplicationId=sqs_msg.message_deduplication_id,
-    )
+    response: dict = new_sqs_client.send_message(QueueUrl=sqs_credentials.queue_url,
+                                                 MessageBody=sqs_msg.message_body,
+                                                 # DelaySeconds=sqs_msg.delay_seconds,
+                                                 MessageAttributes=sqs_msg.message_attributes if sqs_msg.message_attributes is not None else {},
+                                                 MessageGroupId=sqs_msg.message_group_id,
+                                                 MessageDeduplicationId=sqs_msg.message_deduplication_id)
     return response
 
 
-def read_one_sqs_message(
-    sqs_credentials: AWSCredentials_SQS, sqs_client: Any = None
-) -> dict:
+def read_one_sqs_message(sqs_credentials: AWSCredentials_SQS,
+                         sqs_client: Any = None) -> dict:
     """
 
     Parameters
     ----------
     sqs_client: The SQS client to use for the operation
     sqs_credentials: The credentials to use for the queue
 
     Returns
     -------
 
     A dictionary of the response
     """
 
     if sqs_client is not None:
-        response = sqs_client.receive_message(
-            QueueUrl=sqs_credentials.queue_url, MaxNumberOfMessages=1
-        )
+        response = sqs_client.receive_message(QueueUrl=sqs_credentials.queue_url,
+                                              MaxNumberOfMessages=1)
         return response
 
     new_sqs_client = get_aws_sqs_client(credentials=sqs_credentials)
-    response = new_sqs_client.receive_message(
-        QueueUrl=sqs_credentials.queue_url, MaxNumberOfMessages=1
-    )
+    response = new_sqs_client.receive_message(QueueUrl=sqs_credentials.queue_url,
+                                              MaxNumberOfMessages=1)
 
     return response
 
 
-def delete_sqs_message(
-    sqs_credentials: AWSCredentials_SQS, receipt_handle: str, sqs_client: Any = None
-) -> dict:
+def delete_sqs_message(sqs_credentials: AWSCredentials_SQS, receipt_handle: str,
+                       sqs_client: Any = None) -> dict:
     """Deletes the message from the queue
 
     Parameters
     ----------
     sqs_client: The SQS client to use for the operation
     sqs_credentials: The credentials to use for the queue
     receipt_handle: This is the handle received when receiving the message
 
     Returns
     -------
 
     """
 
     if sqs_client is not None:
-        response = sqs_client.delete_message(
-            QueueUrl=sqs_credentials.queue_url, ReceiptHandle=receipt_handle
-        )
+        response = sqs_client.delete_message(QueueUrl=sqs_credentials.queue_url,
+                                             ReceiptHandle=receipt_handle)
         return response
 
     new_sqs_client = get_aws_sqs_client(credentials=sqs_credentials)
-    response = new_sqs_client.delete_message(
-        QueueUrl=sqs_credentials.queue_url, ReceiptHandle=receipt_handle
-    )
+    response = new_sqs_client.delete_message(QueueUrl=sqs_credentials.queue_url,
+                                             ReceiptHandle=receipt_handle)
     return response
```

### Comparing `navalmartin_mir_aws_utils-0.0.28/.gitignore` & `navalmartin_mir_aws_utils-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_aws_utils-0.0.28/LICENSE` & `navalmartin_mir_aws_utils-0.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `navalmartin_mir_aws_utils-0.0.28/pyproject.toml` & `navalmartin_mir_aws_utils-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
-requires = ["hatchling", "boto3", "pydantic", "pydantic[email]",]
+requires = ["hatchling", "boto3"]
 build-backend = "hatchling.build"
 [project]
 name = "navalmartin_mir_aws_utils"
-version = "0.0.28"
+version = "0.0.9"
 authors = [
   { name="Alexandros Giavaras", email="a.giavaras@gmail.com" },
 ]
 description = "Various utilities for working with AWS in Python 3. for the mir project"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 [project.urls]
 "Homepage" = "https://github.com/Navalmartin/navalmartin_mir_aws_utils"
```

