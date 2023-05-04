# Comparing `tmp/whitetower-0.1-py3-none-any.whl.zip` & `tmp/whitetower-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 6515 bytes, number of entries: 16
--rw-rw-r--  2.0 unx       87 b- defN 23-May-02 14:02 whitetower/__init__.py
--rw-rw-r--  2.0 unx      670 b- defN 23-May-02 13:58 whitetower/callbacks.py
--rw-rw-r--  2.0 unx     4523 b- defN 23-May-02 13:59 whitetower/whitetower.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-27 13:17 whitetower/docker/__init__.py
--rw-rw-r--  2.0 unx     1402 b- defN 23-May-02 13:57 whitetower/docker/docker_compose.py
--rw-rw-r--  2.0 unx        0 b- defN 23-May-02 14:07 whitetower/repositories/__init__.py
--rw-rw-r--  2.0 unx     1445 b- defN 23-May-02 13:57 whitetower/repositories/ecr_repository.py
--rw-rw-r--  2.0 unx      184 b- defN 23-Apr-26 12:09 whitetower/repositories/repository.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-27 13:16 whitetower/types/__init__.py
--rw-rw-r--  2.0 unx      446 b- defN 23-May-02 13:57 whitetower/types/app_image_info.py
--rw-rw-r--  2.0 unx      424 b- defN 23-Apr-26 12:09 whitetower/types/image.py
--rw-rw-r--  2.0 unx      240 b- defN 23-Apr-27 12:17 whitetower/types/update_decision.py
--rw-rw-r--  2.0 unx      228 b- defN 23-May-02 14:46 whitetower-0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-02 14:46 whitetower-0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-May-02 14:46 whitetower-0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1337 b- defN 23-May-02 14:46 whitetower-0.1.dist-info/RECORD
-16 files, 11089 bytes uncompressed, 4277 bytes compressed:  61.4%
+Zip file size: 6720 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat       88 b- defN 23-May-04 11:43 whitetower/__init__.py
+-rw-rw-rw-  2.0 fat      690 b- defN 23-May-04 11:43 whitetower/callbacks.py
+-rw-rw-rw-  2.0 fat     4624 b- defN 23-May-04 11:46 whitetower/whitetower.py
+-rw-rw-rw-  2.0 fat       58 b- defN 23-May-04 11:45 whitetower/docker/__init__.py
+-rw-rw-rw-  2.0 fat     1441 b- defN 23-May-04 11:43 whitetower/docker/docker_compose.py
+-rw-rw-rw-  2.0 fat       64 b- defN 23-May-04 11:45 whitetower/repositories/__init__.py
+-rw-rw-rw-  2.0 fat     1495 b- defN 23-May-04 11:47 whitetower/repositories/ecr_repository.py
+-rw-rw-rw-  2.0 fat      187 b- defN 23-May-04 11:43 whitetower/repositories/repository.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-04 11:43 whitetower/types/__init__.py
+-rw-rw-rw-  2.0 fat      460 b- defN 23-May-04 11:43 whitetower/types/app_image_info.py
+-rw-rw-rw-  2.0 fat      440 b- defN 23-May-04 11:43 whitetower/types/image.py
+-rw-rw-rw-  2.0 fat      251 b- defN 23-May-04 11:43 whitetower/types/update_decision.py
+-rw-rw-rw-  2.0 fat      191 b- defN 23-May-04 11:49 whitetower-0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-04 11:49 whitetower-0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-May-04 11:49 whitetower-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1339 b- defN 23-May-04 11:49 whitetower-0.2.dist-info/RECORD
+16 files, 11431 bytes uncompressed, 4482 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: whitetower/types/image.py
 Comment: 
 
 Filename: whitetower/types/update_decision.py
 Comment: 
 
-Filename: whitetower-0.1.dist-info/METADATA
+Filename: whitetower-0.2.dist-info/METADATA
 Comment: 
 
-Filename: whitetower-0.1.dist-info/WHEEL
+Filename: whitetower-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: whitetower-0.1.dist-info/top_level.txt
+Filename: whitetower-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: whitetower-0.1.dist-info/RECORD
+Filename: whitetower-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## whitetower/__init__.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
-from whitetower.whitetower import WhiteTower
+from whitetower.whitetower import WhiteTower
 from whitetower.callbacks import Callbacks
```

## whitetower/callbacks.py

 * *Ordering differences only*

```diff
@@ -1,20 +1,20 @@
-from typing import Dict
-from whitetower.types.image import Image
-from whitetower.types.update_decision import UpdateDecision
-
-
-class Callbacks:
-    def __init__(self, applications: Dict[str, str]):
-        self.applications = applications
-
-    def get_image_name(self, app_name: str) -> str | None:
-        raise Exception("Abstract")
-    
-    def get_local_version(self, image_name: str) -> int | None:
-        raise Exception("Abstract")
-
-    def on_before_repo_check(self, app_name: str, current_image: Image) -> bool:
-        return True
-
-    def on_new_image_found(self, app_name: str, current_image: Image, new_image: Image) -> UpdateDecision:
-        return True
+from typing import Dict
+from whitetower.types.image import Image
+from whitetower.types.update_decision import UpdateDecision
+
+
+class Callbacks:
+    def __init__(self, applications: Dict[str, str]):
+        self.applications = applications
+
+    def get_image_name(self, app_name: str) -> str | None:
+        raise Exception("Abstract")
+    
+    def get_local_version(self, image_name: str) -> int | None:
+        raise Exception("Abstract")
+
+    def on_before_repo_check(self, app_name: str, current_image: Image) -> bool:
+        return True
+
+    def on_new_image_found(self, app_name: str, current_image: Image, new_image: Image) -> UpdateDecision:
+        return True
```

## whitetower/whitetower.py

 * *Ordering differences only*

```diff
@@ -1,101 +1,101 @@
-import time
-from typing import Dict
-from whitetower.types.app_image_info import AppImageInfo
-from whitetower.callbacks import Callbacks
-from whitetower.types.image import Image
-from whitetower.types.update_decision import UpdateDecision
-from whitetower.docker.docker_compose import DockerCompose
-from whitetower.repositories.repository import Repository
-
-
-class WhiteTower:
-    def __init__(self, docker_compose: DockerCompose, image_repository: Repository, callbacks: Callbacks):
-        self.docker_compose = docker_compose
-        self.image_repository = image_repository
-        self.callbacks = callbacks
-
-    def get_current_image(self, image_name: str) -> Image:
-        result = Image(image_name)
-        ver = self.callbacks.get_local_version(image_name)
-        if ver:
-            result.version = ver
-        if result.version == -1:
-            ver = self.image_repository.get_latest_version(image_name)
-            if ver:
-                result.version = ver
-        return result
-
-    def run(self):
-        applications = self.docker_compose.get_applications()
-        app_names = list(applications.keys())
-        current_images : Dict[str, Image] = dict()
-
-        # Сache image info
-        for app in app_names:
-            image_name = self.callbacks.get_image_name(app)
-            current_images[app] = self.get_current_image(image_name)
-
-        print("Current image versions:")
-        for image in current_images:
-            print("\t", image, " -> ", f"{current_images[image]}")
-
-        apps: Dict[str, AppImageInfo] = {}
-        for image in current_images:
-            apps[image] = AppImageInfo(current_images[image], current_images[image])
-
-        # Start applications
-        application_images_to_run = { k: v.current_image for (k,v) in apps.items() }
-        self.docker_compose.run("app", application_images_to_run)
-
-        # Main loop
-        apps_to_update = []
-        while True:
-            new_apps_to_update = []
-            for app_name in apps:
-                app = apps[app_name]
-                current_image = app.current_image
-                if not self.callbacks.on_before_repo_check(app, current_image):
-                    print("Callback 'on_before_repo_check' returned False, skipping check of", app)
-                    continue
-
-                possibly_new_image_name = self.callbacks.get_image_name(app_name)
-                ver = self.image_repository.get_latest_version(possibly_new_image_name)
-                new_image = Image(possibly_new_image_name, ver)
-
-                if current_image != new_image and not app_name in apps_to_update and (new_image != app.latest_known_image or not app.skip_latest_known_image):
-                    print(f"Found new version of '{app_name}'. Old={current_image}, New={new_image}")
-                    app.latest_known_image = new_image
-                    app.skip_latest_known_image = False
-
-                    update_decision = self.callbacks.on_new_image_found(app_name, current_image, new_image)
-                    if update_decision == UpdateDecision.skip_this_version:
-                        print("Callback 'on_new_image_found' returned 'skip_this_version', skipping update of", app)
-                        continue
-
-                    if update_decision == UpdateDecision.postpone_update:
-                        print("Callback 'on_new_image_found' returned 'postpone_update', so we will check this app again on next iteration", app)
-                        continue
-
-                    new_apps_to_update.append(app_name)
-
-            if new_apps_to_update:
-                # We save these found apps and run next iteration of checks
-                apps_to_update += new_apps_to_update
-                print("Updates found. Waiting for another repo check iteration results.")
-            elif apps_to_update:
-                print("No more updates found. Apply pending updates.")
-                
-                for app_name in apps_to_update:
-                    app = apps[app_name]
-                    app.current_image = app.latest_known_image
-                    app.latest_known_image = None
-                    app.skip_latest_known_image = False
-
-                # Start applications
-                application_images_to_run = { k: v.current_image for (k,v) in apps.items() }
-                self.docker_compose.run("app", application_images_to_run)
-
-                print(f"Applications {apps_to_update} were restarted")
-                apps_to_update.clear()
-
-            time.sleep(10)
+import time
+from typing import Dict
+from whitetower.types.app_image_info import AppImageInfo
+from whitetower.callbacks import Callbacks
+from whitetower.types.image import Image
+from whitetower.types.update_decision import UpdateDecision
+from whitetower.docker.docker_compose import DockerCompose
+from whitetower.repositories.repository import Repository
+
+
+class WhiteTower:
+    def __init__(self, docker_compose: DockerCompose, image_repository: Repository, callbacks: Callbacks):
+        self.docker_compose = docker_compose
+        self.image_repository = image_repository
+        self.callbacks = callbacks
+
+    def get_current_image(self, image_name: str) -> Image:
+        result = Image(image_name)
+        ver = self.callbacks.get_local_version(image_name)
+        if ver:
+            result.version = ver
+        if result.version == -1:
+            ver = self.image_repository.get_latest_version(image_name)
+            if ver:
+                result.version = ver
+        return result
+
+    def run(self):
+        applications = self.docker_compose.get_applications()
+        app_names = list(applications.keys())
+        current_images : Dict[str, Image] = dict()
+
+        # Сache image info
+        for app in app_names:
+            image_name = self.callbacks.get_image_name(app)
+            current_images[app] = self.get_current_image(image_name)
+
+        print("Current image versions:")
+        for image in current_images:
+            print("\t", image, " -> ", f"{current_images[image]}")
+
+        apps: Dict[str, AppImageInfo] = {}
+        for image in current_images:
+            apps[image] = AppImageInfo(current_images[image], current_images[image])
+
+        # Start applications
+        application_images_to_run = { k: v.current_image for (k,v) in apps.items() }
+        self.docker_compose.run("app", application_images_to_run)
+
+        # Main loop
+        apps_to_update = []
+        while True:
+            new_apps_to_update = []
+            for app_name in apps:
+                app = apps[app_name]
+                current_image = app.current_image
+                if not self.callbacks.on_before_repo_check(app, current_image):
+                    print("Callback 'on_before_repo_check' returned False, skipping check of", app)
+                    continue
+
+                possibly_new_image_name = self.callbacks.get_image_name(app_name)
+                ver = self.image_repository.get_latest_version(possibly_new_image_name)
+                new_image = Image(possibly_new_image_name, ver)
+
+                if current_image != new_image and not app_name in apps_to_update and (new_image != app.latest_known_image or not app.skip_latest_known_image):
+                    print(f"Found new version of '{app_name}'. Old={current_image}, New={new_image}")
+                    app.latest_known_image = new_image
+                    app.skip_latest_known_image = False
+
+                    update_decision = self.callbacks.on_new_image_found(app_name, current_image, new_image)
+                    if update_decision == UpdateDecision.skip_this_version:
+                        print("Callback 'on_new_image_found' returned 'skip_this_version', skipping update of", app)
+                        continue
+
+                    if update_decision == UpdateDecision.postpone_update:
+                        print("Callback 'on_new_image_found' returned 'postpone_update', so we will check this app again on next iteration", app)
+                        continue
+
+                    new_apps_to_update.append(app_name)
+
+            if new_apps_to_update:
+                # We save these found apps and run next iteration of checks
+                apps_to_update += new_apps_to_update
+                print("Updates found. Waiting for another repo check iteration results.")
+            elif apps_to_update:
+                print("No more updates found. Apply pending updates.")
+                
+                for app_name in apps_to_update:
+                    app = apps[app_name]
+                    app.current_image = app.latest_known_image
+                    app.latest_known_image = None
+                    app.skip_latest_known_image = False
+
+                # Start applications
+                application_images_to_run = { k: v.current_image for (k,v) in apps.items() }
+                self.docker_compose.run("app", application_images_to_run)
+
+                print(f"Applications {apps_to_update} were restarted")
+                apps_to_update.clear()
+
+            time.sleep(10)
```

## whitetower/docker/__init__.py

```diff
@@ -0,0 +1,4 @@
+00000000: 6672 6f6d 2077 6869 7465 746f 7765 722e  from whitetower.
+00000010: 646f 636b 6572 2e64 6f63 6b65 725f 636f  docker.docker_co
+00000020: 6d70 6f73 6520 696d 706f 7274 2044 6f63  mpose import Doc
+00000030: 6b65 7243 6f6d 706f 7365                 kerCompose
```

## whitetower/docker/docker_compose.py

 * *Ordering differences only*

```diff
@@ -1,40 +1,40 @@
-import copy
-import time
-from typing import Dict
-from subprocess import Popen, PIPE, STDOUT
-import yaml
-
-from whitetower.types.image import Image
-
-class DockerCompose:
-    def __init__(self, docker_compose_template_file_name: str):
-        self.docker_compose_template_file_name = docker_compose_template_file_name
-        with open(docker_compose_template_file_name, "r") as f:
-            try:
-                self.data = yaml.safe_load(f)
-            except yaml.YAMLError as exc:
-                print(exc)
-
-        if "services" in self.data:
-            services = self.data["services"]
-            self.apps = {}
-            for s in services:
-                self.apps[s] = services[s]["image"].split(":")[0]
-
-    def get_applications(self) -> Dict[str, str]:
-        return self.apps
-    
-    def run(self, project_name: str, application_images: Dict[str, Image]):
-        data = copy.deepcopy(self.data)
-        if "services" in data:
-            services = data["services"]
-            for s in services:
-                if s in application_images:
-                    services[s]["image"] = str(application_images[s])
-
-        docker_compose_data = yaml.dump(data)
-
-        p = Popen([ "docker-compose", "-f", "-", "-p", project_name, "up", "-d" ], stdin=PIPE)
-        stdout_data = p.communicate(input=docker_compose_data.encode("utf-8"))[0]
-        time.sleep(5)
+import copy
+import time
+from typing import Dict
+from subprocess import Popen, PIPE, STDOUT
+import yaml
+
+from whitetower.types.image import Image
+
+class DockerCompose:
+    def __init__(self, docker_compose_template_file_name: str):
+        self.docker_compose_template_file_name = docker_compose_template_file_name
+        with open(docker_compose_template_file_name, "r") as f:
+            try:
+                self.data = yaml.safe_load(f)
+            except yaml.YAMLError as exc:
+                print(exc)
+
+        if "services" in self.data:
+            services = self.data["services"]
+            self.apps = {}
+            for s in services:
+                self.apps[s] = services[s]["image"].split(":")[0]
+
+    def get_applications(self) -> Dict[str, str]:
+        return self.apps
+    
+    def run(self, project_name: str, application_images: Dict[str, Image]):
+        data = copy.deepcopy(self.data)
+        if "services" in data:
+            services = data["services"]
+            for s in services:
+                if s in application_images:
+                    services[s]["image"] = str(application_images[s])
+
+        docker_compose_data = yaml.dump(data)
+
+        p = Popen([ "docker-compose", "-f", "-", "-p", project_name, "up", "-d" ], stdin=PIPE)
+        stdout_data = p.communicate(input=docker_compose_data.encode("utf-8"))[0]
+        time.sleep(5)
         print(stdout_data)
```

## whitetower/repositories/__init__.py

```diff
@@ -0,0 +1,4 @@
+00000000: 6672 6f6d 2077 6869 7465 746f 7765 722e  from whitetower.
+00000010: 7265 706f 7369 746f 7269 6573 2e65 6372  repositories.ecr
+00000020: 5f72 6570 6f73 6974 6f72 7920 696d 706f  _repository impo
+00000030: 7274 2045 6372 5265 706f 7369 746f 7279  rt EcrRepository
```

## whitetower/repositories/ecr_repository.py

```diff
@@ -1,38 +1,38 @@
-import boto3
-import re
-from whitetower.repository import Repository
-
-class EcrRepository(Repository):
-    def __init__(self, aws_account_id, aws_account_secret, aws_region):
-        self.aws_args = { 
-            "aws_access_key_id": aws_account_id, 
-            "aws_secret_access_key": aws_account_secret, 
-            "region_name": aws_region
-        }
-        self.__login()
-    
-    def __login(self):
-        self.client = boto3.client('ecr', **self.aws_args)
-
-    def get_latest_version(self, image_name: str) -> int:
-        # Check if image_name is Docker URL instead of ECR repo name
-        # Keep only ECR repo name if so
-        m = re.match(r"[0-9]+\.dkr\.ecr\.[a-z0-9-]+\.amazonaws\.com/([^:]+)", image_name)
-        if m:
-            image_name = m.groups(1)[0]
-
-        response = self.client.describe_images(repositoryName=image_name, imageIds=[{ 'imageTag': 'latest'}])
-        if response and "imageDetails" in response:
-            for image in response["imageDetails"]:
-                if "imageTags" in image:
-                    found = False
-                    for tag in image["imageTags"]:
-                        if tag != "latest":
-                            try:
-                                num = int(tag)
-                                found = True
-                            except:
-                                pass
-                    if found:
-                        return num
+import boto3
+import re
+from whitetower.repositories.repository import Repository
+
+class EcrRepository(Repository):
+    def __init__(self, aws_account_id, aws_account_secret, aws_region):
+        self.aws_args = { 
+            "aws_access_key_id": aws_account_id, 
+            "aws_secret_access_key": aws_account_secret, 
+            "region_name": aws_region
+        }
+        self.__login()
+    
+    def __login(self):
+        self.client = boto3.client('ecr', **self.aws_args)
+
+    def get_latest_version(self, image_name: str) -> int:
+        # Check if image_name is Docker URL instead of ECR repo name
+        # Keep only ECR repo name if so
+        m = re.match(r"[0-9]+\.dkr\.ecr\.[a-z0-9-]+\.amazonaws\.com/([^:]+)", image_name)
+        if m:
+            image_name = m.groups(1)[0]
+
+        response = self.client.describe_images(repositoryName=image_name, imageIds=[{ 'imageTag': 'latest'}])
+        if response and "imageDetails" in response:
+            for image in response["imageDetails"]:
+                if "imageTags" in image:
+                    found = False
+                    for tag in image["imageTags"]:
+                        if tag != "latest":
+                            try:
+                                num = int(tag)
+                                found = True
+                            except:
+                                pass
+                    if found:
+                        return num
         return None
```

## whitetower/repositories/repository.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-class Repository:
-    def get_latest_version(self, image_name: str) -> int:
-        '''Returns latest numeric version by checking the :latest tag'''
+class Repository:
+    def get_latest_version(self, image_name: str) -> int:
+        '''Returns latest numeric version by checking the :latest tag'''
         raise Exception("Abstract")
```

## whitetower/types/app_image_info.py

 * *Ordering differences only*

```diff
@@ -1,14 +1,14 @@
-from dataclasses import dataclass
-from whitetower.types.image import Image
-
-
-@dataclass
-class AppImageInfo:
-    current_image: Image
-    '''Image version, which is currently being run'''
-
-    latest_known_image: Image = None
-    '''Most recent application image version, which we saw in the repository'''
-
-    skip_latest_known_image: bool = False
-    '''If True, then we are not going to use current latest_known_image for application update'''
+from dataclasses import dataclass
+from whitetower.types.image import Image
+
+
+@dataclass
+class AppImageInfo:
+    current_image: Image
+    '''Image version, which is currently being run'''
+
+    latest_known_image: Image = None
+    '''Most recent application image version, which we saw in the repository'''
+
+    skip_latest_known_image: bool = False
+    '''If True, then we are not going to use current latest_known_image for application update'''
```

## whitetower/types/image.py

 * *Ordering differences only*

```diff
@@ -1,17 +1,17 @@
-from dataclasses import dataclass
-
-
-@dataclass 
-class Image:
-    image_name: str
-    version: int = -1
-
-    def __repr__(self):
-        return f"{self.image_name}:{self.version}"
-    
-    def __eq__(self, other: 'Image'):
-        if not self and not other:
-            return True
-        if not self or not other:
-            return False
+from dataclasses import dataclass
+
+
+@dataclass 
+class Image:
+    image_name: str
+    version: int = -1
+
+    def __repr__(self):
+        return f"{self.image_name}:{self.version}"
+    
+    def __eq__(self, other: 'Image'):
+        if not self and not other:
+            return True
+        if not self or not other:
+            return False
         return self.image_name == other.image_name and self.version == other.version
```

## whitetower/types/update_decision.py

 * *Ordering differences only*

```diff
@@ -1,11 +1,11 @@
-import enum
-
-class UpdateDecision(enum.Enum):
-    perform_update = 1
-    """Update as soon as possible"""
-
-    postpone_update = 2
-    """Perform pre-update checks again"""
-
-    skip_this_version = 3
-    """Do not update to this version"""
+import enum
+
+class UpdateDecision(enum.Enum):
+    perform_update = 1
+    """Update as soon as possible"""
+
+    postpone_update = 2
+    """Perform pre-update checks again"""
+
+    skip_this_version = 3
+    """Do not update to this version"""
```

