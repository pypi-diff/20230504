# Comparing `tmp/sipiiiii-0.8.7.tar.gz` & `tmp/sipiiiii-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipiiiii-0.8.7.tar", last modified: Wed May  3 13:54:29 2023, max compression
+gzip compressed data, was "sipiiiii-0.8.8.tar", last modified: Thu May  4 03:44:11 2023, max compression
```

## Comparing `sipiiiii-0.8.7.tar` & `sipiiiii-0.8.8.tar`

### file list

```diff
@@ -1,41 +1,35 @@
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 13:54:29.814745 sipiiiii-0.8.7/
--rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-0.8.7/MANIFEST.in
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 13:54:29.813823 sipiiiii-0.8.7/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.8.7/README.md
--rw-r--r--   0 j0hn       (501) staff       (20)      634 2023-05-03 13:52:10.000000 sipiiiii-0.8.7/pyproject.toml
--rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-03 13:54:29.815147 sipiiiii-0.8.7/setup.cfg
--rw-r--r--   0 j0hn       (501) staff       (20)     3401 2023-05-03 13:52:10.000000 sipiiiii-0.8.7/setup.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 13:54:29.750854 sipiiiii-0.8.7/sipiiiii/
--rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.8.7/sipiiiii/__init__.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 13:54:29.769438 sipiiiii-0.8.7/sipiiiii/app/
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.8.7/sipiiiii/app/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)    10430 2023-05-03 13:38:34.000000 sipiiiii-0.8.7/sipiiiii/app/core.py
--rw-r--r--   0 j0hn       (501) staff       (20)    22947 2023-05-03 13:54:08.000000 sipiiiii-0.8.7/sipiiiii/app/new_app.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 13:54:29.780680 sipiiiii-0.8.7/sipiiiii/app/utils/
--rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-0.8.7/sipiiiii/app/utils/HttpSDK.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 13:54:29.803602 sipiiiii-0.8.7/sipiiiii/app/utils/PPI/
--rw-rw-r--   0 j0hn       (501) staff       (20)      174 2018-04-19 14:27:03.000000 sipiiiii-0.8.7/sipiiiii/app/utils/PPI/__init__.py
--rw-rw-r--   0 j0hn       (501) staff       (20)      524 2018-04-19 14:27:03.000000 sipiiiii-0.8.7/sipiiiii/app/utils/PPI/generator_factory.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     6829 2023-04-10 15:58:16.000000 sipiiiii-0.8.7/sipiiiii/app/utils/PPI/prog_class.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     3470 2018-04-19 14:27:03.000000 sipiiiii-0.8.7/sipiiiii/app/utils/PPI/progbar.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     2460 2018-04-19 14:27:03.000000 sipiiiii-0.8.7/sipiiiii/app/utils/PPI/progpercent.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1598 2023-05-03 13:30:01.000000 sipiiiii-0.8.7/sipiiiii/app/utils/Tools.py
--rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.8.7/sipiiiii/app/utils/ZipFileTool.py
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.8.7/sipiiiii/app/utils/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-03 08:02:36.000000 sipiiiii-0.8.7/sipiiiii/app/utils/config.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.8.7/sipiiiii/app/utils/formatConversion.py
--rw-r--r--   0 j0hn       (501) staff       (20)       17 2023-05-03 13:52:10.000000 sipiiiii-0.8.7/sipiiiii/app/version.py
--rw-r--r--   0 j0hn       (501) staff       (20)     8501 2023-05-03 12:18:55.000000 sipiiiii-0.8.7/sipiiiii/main.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 13:54:29.762226 sipiiiii-0.8.7/sipiiiii.egg-info/
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 13:54:29.000000 sipiiiii-0.8.7/sipiiiii.egg-info/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)      887 2023-05-03 13:54:29.000000 sipiiiii-0.8.7/sipiiiii.egg-info/SOURCES.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-03 13:54:29.000000 sipiiiii-0.8.7/sipiiiii.egg-info/dependency_links.txt
--rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-03 13:54:29.000000 sipiiiii-0.8.7/sipiiiii.egg-info/entry_points.txt
--rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-03 13:54:29.000000 sipiiiii-0.8.7/sipiiiii.egg-info/requires.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-03 13:54:29.000000 sipiiiii-0.8.7/sipiiiii.egg-info/top_level.txt
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 13:54:29.811391 sipiiiii-0.8.7/template/
--rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-0.8.7/template/python_fastapi.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-04-18 15:46:06.000000 sipiiiii-0.8.7/template/python_flask.j2
--rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-0.8.7/template/python_openai.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      795 2023-05-03 13:15:30.000000 sipiiiii-0.8.7/template/template_openai.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-0.8.7/template/template_other.yaml
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-04 03:44:11.136856 sipiiiii-0.8.8/
+-rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-0.8.8/MANIFEST.in
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-04 03:44:11.135774 sipiiiii-0.8.8/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.8.8/README.md
+-rw-r--r--   0 j0hn       (501) staff       (20)      634 2023-05-04 03:34:11.000000 sipiiiii-0.8.8/pyproject.toml
+-rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-04 03:44:11.137224 sipiiiii-0.8.8/setup.cfg
+-rw-r--r--   0 j0hn       (501) staff       (20)     3401 2023-05-04 03:34:43.000000 sipiiiii-0.8.8/setup.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-04 03:44:11.099174 sipiiiii-0.8.8/sipiiiii/
+-rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.8.8/sipiiiii/__init__.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-04 03:44:11.114184 sipiiiii-0.8.8/sipiiiii/app/
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.8.8/sipiiiii/app/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    11056 2023-05-04 03:25:50.000000 sipiiiii-0.8.8/sipiiiii/app/core.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    21799 2023-05-04 03:34:11.000000 sipiiiii-0.8.8/sipiiiii/app/new_app.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-04 03:44:11.127700 sipiiiii-0.8.8/sipiiiii/app/utils/
+-rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-0.8.8/sipiiiii/app/utils/HttpSDK.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1565 2023-05-04 03:09:45.000000 sipiiiii-0.8.8/sipiiiii/app/utils/Tools.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.8.8/sipiiiii/app/utils/ZipFileTool.py
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.8.8/sipiiiii/app/utils/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-03 08:02:36.000000 sipiiiii-0.8.8/sipiiiii/app/utils/config.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.8.8/sipiiiii/app/utils/formatConversion.py
+-rw-r--r--   0 j0hn       (501) staff       (20)       17 2023-05-04 03:34:11.000000 sipiiiii-0.8.8/sipiiiii/app/version.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     8632 2023-05-04 03:31:44.000000 sipiiiii-0.8.8/sipiiiii/main.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-04 03:44:11.107385 sipiiiii-0.8.8/sipiiiii.egg-info/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-04 03:44:10.000000 sipiiiii-0.8.8/sipiiiii.egg-info/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)      699 2023-05-04 03:44:10.000000 sipiiiii-0.8.8/sipiiiii.egg-info/SOURCES.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-04 03:44:10.000000 sipiiiii-0.8.8/sipiiiii.egg-info/dependency_links.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-04 03:44:10.000000 sipiiiii-0.8.8/sipiiiii.egg-info/entry_points.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-04 03:44:10.000000 sipiiiii-0.8.8/sipiiiii.egg-info/requires.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-04 03:44:10.000000 sipiiiii-0.8.8/sipiiiii.egg-info/top_level.txt
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-04 03:44:11.134295 sipiiiii-0.8.8/template/
+-rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-0.8.8/template/python_fastapi.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-04-18 15:46:06.000000 sipiiiii-0.8.8/template/python_flask.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-0.8.8/template/python_openai.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      795 2023-05-03 13:15:30.000000 sipiiiii-0.8.8/template/template_openai.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-0.8.8/template/template_other.yaml
```

### Comparing `sipiiiii-0.8.7/PKG-INFO` & `sipiiiii-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.8.7
+Version: 0.8.8
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-0.8.7/README.md` & `sipiiiii-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.7/pyproject.toml` & `sipiiiii-0.8.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sipiiiii"
-version = "0.8.7"
+version = "0.8.8"
 authors = [
   { name="DeplRun", email="sipiiiii@example.com" },
 ]
 description = "sipiiiii定位为简单易用的云应用托管平台"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `sipiiiii-0.8.7/setup.py` & `sipiiiii-0.8.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     print(msg)
     sys.exit(1)
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="sipiiiii",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="0.8.7",
+    version="0.8.8",
     # 作者名
     author="sipiiiii@admin",
     # 作者邮箱
     author_email="j0hn.wahahaha@gmail.com",
     # 包的简介描述
     description="depl sipiiiii, App Development Framework",
     # 包的详细介绍(一般通过加载README.md)
```

### Comparing `sipiiiii-0.8.7/sipiiiii/app/core.py` & `sipiiiii-0.8.8/sipiiiii/app/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,78 +38,90 @@
         self.app_name = app_name
         self.app_yaml = app_yaml
         self.app_dir = app_dir
 
     def __create_app_path(self):
         if os.path.exists(self.app_name):
             print(f"{self.app_name} 路径已存在，无法在不删除的情况下创建新项目.")
-            is_rm = input("是否需要删除(y/n)?")
+            is_rm = input("是否需要删除, 不删除则会退出程序(y/n)?")
             is_rm = is_rm.lower()
             if is_rm == "y":
                 rmtree(self.app_name)
             elif is_rm == "n":
                 return True, "退出"
 
         path = Path(f"{self.app_name}")
         path.mkdir(parents=True, exist_ok=True)
 
     def __create_code(self, code_type, app_type):
-        if not create_framework_code(self.app_dir, self.app_name, self.app_yaml, code_type, app_type):
-            return False, "创建框架出错，请检查yaml文件."
-        return True, ""
+        status, msg = create_framework_code(
+            self.app_dir, self.app_name, self.app_yaml, code_type, app_type)
+        if not status:
+            return False, "创建框架代码出错, {msg}"
+        return True, msg
 
-    def __create_python_requirements(self):
+    def __create_python_requirements(self, app_type):
         requirements = input("输入导入的库(多个库用逗号分隔):")
-        if requirements is None:
+        if requirements is None or requirements == "":
             requirements = ""
 
         if requirements.find(",") > -1:
             requirements = requirements.split(",")
         else:
             if requirements == "":
                 requirements = []
             else:
                 requirements = [requirements]
 
+        if app_type == "fastapi":
+            requirements.append('fastapi')
+        if app_type == "flask":
+            requirements.append('flask')
+        if app_type == "openai":
+            requirements.append('quart')
+            requirements.append('quart_cors')
+
         status, requirements_file_path = create_requirements(
             self.app_name, requirements)
         if not status:
             return False, requirements_file_path
 
     def create_flask_app(self, code_type):
         self.__create_app_path()
 
         if code_type == "python":
-            self.__create_python_requirements()
+            self.__create_python_requirements("flask")
 
         status, openapi_file_path = create_app_yaml(
             self.app_name, self.app_yaml, "flask")
         if not status:
             return False, openapi_file_path
 
-        if not self.__create_code(code_type, "flask"):
-            return False, "创建框架出错，请检查yaml文件."
+        ststus, msg = self.__create_code(code_type, "flask")
+        if not ststus:
+            return False, msg
 
-        return True, "创建flask框架成功."
+        return True, f"创建flask框架代码成功, 项目目录: ./{self.app_name}"
 
     def create_fastapi_app(self, code_type):
         self.__create_app_path()
 
         if code_type == "python":
-            self.__create_python_requirements()
+            self.__create_python_requirements("fastapi")
 
         status, openapi_file_path = create_app_yaml(
             self.app_name, self.app_yaml, "fastapi")
         if not status:
             return False, openapi_file_path
 
-        if not self.__create_code(code_type, "fastapi"):
-            return False, "创建框架出错，请检查yaml文件."
+        ststus, msg = self.__create_code(code_type, "fastapi")
+        if not ststus:
+            return False, msg
 
-        return True, "创建fastapi框架成功."
+        return True, f"创建fastapi框架代码成功, 项目目录: ./{self.app_name}"
 
     def create_openai_app(self, code_type):
         ai_plugin_json = {
             "schema_version": "",
             "name_for_human": "",
             "name_for_model": "",
             "description_for_human": "",
@@ -140,30 +152,31 @@
                 'info', {}).get('description')
         except Exception as e:
             return False, str(e)
 
         self.__create_app_path()
 
         if code_type == "python":
-            self.__create_python_requirements()
+            self.__create_python_requirements("openai")
 
         status, openapi_file_path = create_app_yaml(
             self.app_name, self.app_yaml, "openai")
         if not status:
             return False, openapi_file_path
 
         status, plugin_json_file_path = create_app_config(
             self.app_name, ai_plugin_json, "openai")
         if not status:
             return False, plugin_json_file_path
 
-        if not self.__create_code(code_type, "openai"):
-            return False, "创建框架出错，请检查yaml文件."
+        ststus, msg = self.__create_code(code_type, "openai")
+        if not ststus:
+            return False, msg
 
-        return True, "创建openai框架成功."
+        return True, f"创建openai框架代码成功, 项目目录: ./{self.app_name}"
 
 
 def get_app_name(app_name, is_yaml=False):
     if app_name is None:
         while True:
             app_yaml_file = ""
             try:
@@ -171,22 +184,23 @@
             except KeyboardInterrupt:
                 print("\r\n")
                 sys.exit(1)
 
             if app_yaml_file == "":
                 continue
             status, app_name, openapi_yaml, aiapi_dir = yaml_app_info(
-                app_yaml_file)
+                app_yaml_file, None)
             if not status:
                 return False, app_name, openapi_yaml, aiapi_dir
 
             return True, app_name, openapi_yaml, aiapi_dir
 
     elif app_name.find(".yaml") > -1:
-        status, app_name, openapi_yaml, aiapi_dir = yaml_app_info(app_name)
+        status, app_name, openapi_yaml, aiapi_dir = yaml_app_info(
+            app_name, None)
         if not status:
             return False, app_name, openapi_yaml, aiapi_dir
         return True, app_name, openapi_yaml, aiapi_dir
     else:
         if is_yaml:
             return False, app_name, "", ""
         return True, app_name, "", ""
@@ -302,19 +316,21 @@
 
 def create_framework_code(directory_path, app_path, openapi_yaml, code_type, app_type):
     env = Environment(loader=FileSystemLoader(f"{directory_path}"))
     # template.j2
     # if app_type != "openai":
     #     app_type = "other"
     j2_file = f"{code_type}_{app_type}"
-    template = env.get_template(f'{j2_file}.j2')
-    output = template.render(paths=openapi_yaml['paths'])
+    try:
+        template = env.get_template(f'{j2_file}.j2')
+        output = template.render(paths=openapi_yaml['paths'])
+    except Exception as e:
+        return False, str(e)
     _fix = fix.get(code_type, None)
     if _fix is None:
-        return False
+        return False, "没有获取到应用类型"
     # Write the output to a Python file
     app_file = os.path.join(app_path, f"app.{_fix}")
     with open(app_file, 'w', encoding="utf-8") as f:
         f.write(output)
 
-    return True
-    
+    return True, "创建框架代码成功"
```

### Comparing `sipiiiii-0.8.7/sipiiiii/app/new_app.py` & `sipiiiii-0.8.8/sipiiiii/app/new_app.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 import prettytable as pt
 import sys
 import time
 import yaml
 
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 from pathlib import Path
-from shutil import copyfile
 
 from .core import CreateAppTypeClass, yaml_app_info, ExecAppClass, get_app_code_type, get_app_name
 
-# from .utils.PPI import ProgPercent
 from .utils.ZipFileTool import zip_folder
 from .utils.HttpSDK import https_get, https_post, https_file
-from .utils.Tools import get_outside_ip, is_encomm_char, write_new_yaml, get_current_path
+from .utils.Tools import get_outside_ip, is_encomm_char, write_new_yaml
 from .utils.config import app_all_types, server_host, fix
 
 
 def process_update_outside_ip(domain, _token):
     while True:
         time.sleep(60 * 30)
         outside_ip = get_outside_ip()
@@ -41,15 +39,15 @@
 def get_token():
     _token = ""
     home_dir_file = os.path.join(Path.home(), ".sipitoken")
     if os.path.exists(home_dir_file):
         with open(home_dir_file, 'r', encoding='utf8') as f:
             _token = f.read()
     if _token == "":
-        return False, "请登录 sipiiiii."
+        return False, "请登录 sipiiiii, 使用 sipiiiii -L 进行登录, 使用 sipiiiii -h 获得帮助"
 
     return True, _token
 
 
 # 创建项目
 def create_app_project():
     status, _token = get_token()
@@ -58,75 +56,72 @@
 
     print("""
     *** 应用名称必须英文
     *** 可以使用向导模式创建应用和使用模版创建应用
         """)
 
     while True:
-        is_ai_create = input("是否使用向导创建应用(y/n):")
-        is_ai_create = is_ai_create.lower()
+        is_wizard_create = input("是否使用向导创建应用(y/n):")
+        is_wizard_create = is_wizard_create.lower()
 
-        if is_ai_create == "y":
+        if is_wizard_create == "y":
             app_name = input("请输入应用名:")
-            if app_name == "":
-                print("项目名不能为空")
-                continue
-            if not is_encomm_char(app_name):
-                print("项目名必须是英文")
+            if app_name == "" or not is_encomm_char(app_name):
+                print("应用名不能为空, 并且应用名只能使用英文字母")
                 continue
 
             app_desc = input("请输入应用说明:")
-            app_version = input("请输入应用版本(不输入默认 v1.0):")
+            app_version = input("请输入应用版本(默认 v1.0):")
             if app_version == "":
                 app_version = "v1.0"
-            print(f"项目名: {app_name}, 项目说明: {app_desc}, 项目版本: {app_version}")
+            print(f"应用名: {app_name}, 应用说明: {app_desc}, 应用版本: {app_version}")
 
             status, yaml_data = create_yaml(
                 app_name, app_version, app_desc)
             if not status:
                 print(yaml_data)
                 continue
 
             with open(f"{os.getcwd()}{os.sep}aiapi.yaml", "w", encoding="utf-8") as f:
                 f.write(yaml_data)
 
-            status, msg, app_name = create_app(
+            status, msg, app_name, app_type = create_app(
                 f"{os.getcwd()}{os.sep}aiapi.yaml")
             if status:
                 write_new_yaml(
-                    f"{os.getcwd()}{os.sep}{app_name}{os.sep}aiapi.yaml")
+                    f"{os.getcwd()}{os.sep}{app_name}{os.sep}aiapi.yaml", app_type)
 
             os.remove(f"{os.getcwd()}{os.sep}aiapi.yaml")
-            return status, msg, app_name
-        elif is_ai_create == "n":
-            status, msg, app_name = create_app(None)
-            # if status:
-            #     write_new_yaml(f"{msg}{os.sep}aiapi.yaml")
             break
 
+        elif is_wizard_create == "n":
+            status, msg, app_name, _ = create_app(None)
+            break
+        else:
+            continue
+
     return status, msg, app_name
 
 
 # 创建yaml模版
 def create_yaml(app_name, app_version, app_desc):
     status, _token = get_token()
     if not status:
         return False, _token
 
-    # yaml_name = input("请输入Yaml文件名:")
-    # if not is_encomm_char(yaml_name):
-    #     return False, "yaml文件名必须是英文"
-    route_num = input("请输入有多少个接口(输入数字,不输入则1个):")
-    if route_num == "":
-        route_num = 1
+    while True:
+        route_num = input("请输入有多少个接口(默认1个接口):")
+        if route_num == "":
+            route_num = 1
 
-    try:
-        route_num = int(route_num)
-    except Exception as _:
-        return False, "请输入数字"
+        try:
+            route_num = int(route_num)
+            break
+        except Exception as _:
+            print("接口数量必须为数字")
 
     route_json = {
         "swagger": "2.0",
         "info": {
             "title": app_name,
             "description": app_desc,
             "version": app_version
@@ -171,60 +166,60 @@
 
 # 通过yaml直接创建APP
 
 
 def create_app(yaml_file=None):
     status, _token = get_token()
     if not status:
-        return False, _token, ""
+        return False, _token, "", ""
 
-    code_type = input(
-        f"请输入创建编程语言{list(fix.keys())}: "
-    )
-
-    _code_type = app_all_types.get(code_type, None)
-    if _code_type is None:
-        return False, f"输入的编程语言的范围: {list(fix.keys())}", ""
-
-    app_type = input(
-        f"请创建应用程序类型({', '.join(app_all_types[code_type])}): "
-    )
+    while True:
+        code_type = input(
+            f"请输入创建编程语言{list(fix.keys())}(默认第一个): "
+        )
+
+        if code_type == "":
+            code_type = list(fix.keys())[0]
+
+        _code_type = app_all_types.get(code_type, None)
+        if _code_type is None:
+            print(f"编程语言的范围为: {list(fix.keys())}")
+            continue
+        break
 
-    if app_type not in app_all_types[code_type]:
-        return False, f"输入应用程序的范围: {app_all_types[code_type]}", ""
+    while True:
+        app_type = input(
+            f"请创建应用程序类型{app_all_types[code_type]}(默认第一个): "
+        )
+        if app_type == "":
+            app_type = app_all_types[code_type][0]
+        if app_type not in app_all_types[code_type]:
+            print(f"应用程序类型的范围为: {app_all_types[code_type]}")
+            continue
+        break
 
     status, app_name, app_yaml, app_dir = yaml_app_info(yaml_file, app_type)
     if not status:
-        return False, app_name, ""
+        return False, f"创建应用失败: {app_name}", "", ""
 
     catc = CreateAppTypeClass(app_name, app_yaml, app_dir)
     method_of_catc = getattr(catc, f"create_{app_type}_app")
     status, msg = method_of_catc(code_type)
-    return status, msg, app_name
+    return status, msg, app_name, app_type
 
 
 def dev_app():
     print("测试运行....\r\n")
     run_main = input("请输入APP运行文件:")
     cwd = os.getcwd()
-    # file_path = os.path.join(cwd, "ai-plugin.json")
-    # file_path = Path(f'{file_path}')
-    # if not file_path.exists():
-    #     print("Error: dont sipiiiii project path.")
-    #     sys.exit(1)
-
-    # file_path = os.path.join(cwd, "openapi.yaml")
-    # file_path = Path(f'{file_path}')
-    # if not file_path.exists():
-    #     return False, "Error: dont sipiiiii project path."
 
     file_path = os.path.join(cwd, run_main)
     file_path = Path(f'{file_path}')
     if not file_path.exists():
-        return False, "错误: 不存在sipiiiii项目路径, 请到项目路径下运行"
+        return False, "错误: 不存在项目路径, 请到项目路径下运行"
 
     status, code_type = get_app_code_type(file_path)
     if not status:
         return False, code_type
 
     eac = ExecAppClass(cwd, file_path, code_type)
 
@@ -237,15 +232,15 @@
 def localdepl(yaml_file_name):
     status, _token = get_token()
     if not status:
         return False, _token
 
     status, app_name, app_yaml, _ = get_app_name(yaml_file_name, True)
     if not status:
-        return False, "获取应用名错误"
+        return False, f"获取应用名错误: {app_name}"
 
     app_cn_name = input("请输出应用别名:")
     if app_cn_name == "":
         app_cn_name = app_name
 
     print(f"本地部署: {app_name} 项目\r\n")
 
@@ -254,46 +249,41 @@
         description = app_yaml.get(
             'info', {}).get('description')
     except Exception as e:
         return False, str(e)
 
     outside_ip = get_outside_ip()
     if outside_ip == "":
-        return False, "你无法访问互联网"
+        return False, "无法访问互联网"
 
-    print(f"你的外网IP: {outside_ip}")
+    print(f"本机外网IP: {outside_ip}")
     status, _token = get_token()
     if not status:
         return False, _token
 
     run_main = input("请输入APP运行文件:")
 
     if run_main.find(".") == 0:
         return False, "APP运行文件必须是文件名加文件后缀"
 
-    cwd = os.getcwd()
-    file_path = os.path.join(cwd, run_main)
-    file_path = Path(f'{file_path}')
-    if not file_path.exists():
-        return False, "错误: 不存在sipiiiii项目路径, 请到项目路径下运行"
-
     run_main_fix = run_main.split(".")
     if len(run_main_fix) != 2:
         return False, "APP运行文件输入不合法"
 
     if run_main_fix[-1] not in list(fix.keys()):
         return False, f"APP运行文件不在允许的列表范围内: {list(fix.keys())}"
 
+    cwd = os.getcwd()
+    file_path = os.path.join(cwd, run_main)
+    file_path = Path(f'{file_path}')
+    if not file_path.exists():
+        return False, "错误: 不存在项目路径, 请到项目路径下运行"
+
     app_language = [k for k, v in fix.items() if v == run_main_fix[-1]][0]
 
-    '''
-    需要两个接口
-    1）本地部署上传应用信息，并且申请个二级域名
-    2）通过应用名和用户EMAIL对二级域名的IP进行更新IP地址
-    '''
     url = f"{server_host}/system/openapi/app/local/deployment"
     headers = {
         "Content-type": "application/json",
         "authorization": _token
     }
     data = {
         "app_name": app_name,
@@ -324,24 +314,24 @@
     method_of_catc = getattr(eac, f"run_{code_type}_app")
     status, msg = method_of_catc()
 
     return status, msg
 
 
 def stop_app(app_name=None):
+    status, _token = get_token()
+    if not status:
+        return False, _token
+
     status, app_name, _, _ = get_app_name(app_name)
     if not status:
-        return False, "获取应用名错误"
+        return False, f"获取应用名错误: {app_name}"
 
     data = {"app_name": app_name}
 
-    status, _token = get_token()
-    if not status:
-        return False, _token
-
     headers = {
         "Content-type": "application/json",
         "authorization": _token
     }
     url = f"{server_host}/system/openapi/app/stop"
     response = https_post(url, json_data=data, headers=headers)
     if not response.success:
@@ -350,66 +340,64 @@
     return True, response.msg
 
 
 def deployed():
     status, _token = get_token()
     if not status:
         return False, _token
-
+    print("""
+    *** 必须在项目目录下进行操作
+    *** 暴露的端口必须为8000
+    """)
     headers = {
         "Content-type": "application/json",
         "authorization": _token
     }
 
     url = f"{server_host}/system/openapi/users/check/token"
     # response = requests.get(url,headers=headers, timeout=20)
     response = https_get(url, headers=headers)
 
     if not response.success:
-        return False, "用户令牌无效，请登录sipiiiiii."
+        return False, "用户令牌无效，请登录使用 sipiiiiii -L 登录."
 
     if not response.data["exist"]:
-        return False, "用户令牌无效或超时，请登录sipiiiiii."
+        return False, "用户令牌无效或超时，请登录使用 sipiiiiii -L 登录."
 
     app_cn_name = input("请输入APP别名:")
     # input("please input APP docking party(chatgpt, other):")
     app_dock = "other"
     run_main = input("请输入APP运行文件:")
-    # is_run_params = input("Whether there are operating parameters(y/n):")
-    # is_run_params = is_run_params.lower()
-    # run_params = ""
-    # if is_run_params == "y":
-    #     run_params = input("Please enter operating parameters")
 
     if app_cn_name == "" or run_main == "":
         return False, "APP别名 或者 APP运行文件的不能为空."
 
     if run_main.find(".") == 0:
         return False, "APP运行文件必须是文件名加文件后缀"
-    
+
+    run_main_fix = run_main.split(".")
+    if len(run_main_fix) != 2:
+        return False, "APP运行文件输入不合法"
+
     cwd = os.getcwd()
     file_path = os.path.join(cwd, run_main)
     file_path = Path(f'{file_path}')
     if not file_path.exists():
-        return False, "错误: 不存在sipiiiii项目路径, 请到项目路径下运行"
-    
-    run_main_fix = run_main.split(".")
-    if len(run_main_fix) != 2:
-        return False, "APP运行文件输入不合法"
+        return False, "错误: 不存在项目路径, 请到项目路径下运行, 或者使用sipiiiii -n 创建项目"
 
     if run_main_fix[-1] not in list(fix.values()):
         return False, f"APP运行文件不在允许的列表范围内: {list(fix.keys())}"
 
     app_language = [k for k, v in fix.items() if v == run_main_fix[-1]][0]
 
-    app_dir = os.getcwd()
-    zip_file_path = zip_folder(app_dir)
+    zip_file_path = zip_folder(cwd)
     if zip_file_path is None:
         return False, "应用程序打包失败。请检查应用程序目录中是否存在异常文件或文件夹"
-    filename = os.path.basename(app_dir)
+
+    filename = os.path.basename(cwd)
     print(f"远程部署: {filename} 项目\r\n")
     # filename = ""#os.path.basename(zip_file_path)
     files = MultipartEncoder(fields={
         'file': (f"{filename}.zip", open(zip_file_path, 'rb'), 'application/octet-stream'),
     })
 
     url = f"{server_host}/system/openapi/app/upload"
@@ -482,107 +470,80 @@
     if not response.success:
         return False, response.msg
 
     home_dir_file = os.path.join(Path.home(), ".sipitoken")
     with open(home_dir_file, 'w', encoding='utf-8') as f:
         f.write(response.data['token'])
 
-    status, tally = get_tally()
+    status, tally, info = get_tally()
     if status:
-        return True, f"登录成功, 登录有效期3天, 剩余积分: {tally}"
+        return True, f"登录成功, 登录有效期3天, 剩余积分: {tally}, {info}"
 
     return False, "登录成功, 登录有效期3天, 获取积分失败."
 
 
-# def init_framework():
-#     aiapi_dir = get_current_path()
-
-#     # Replace 'template/template.yaml' with the path to the file you want to copy
-#     # src_file = f'sipiiiii{os.sep}template/template.yaml'
-#     src_dir = os.path.join("sipiiiii", "template")
-
-#     template_files = os.listdir(src_dir)
-#     for tFIle in template_files:
-#         src_file = os.path.join(src_dir, tFIle)
-
-#         # Use Path().resolve() to get the absolute path of the source file
-#         src_path = Path(src_file).resolve()
-
-#         # Use Path().joinpath() to get the destination path
-#         dest_path = Path(aiapi_dir).joinpath(tFIle)
-#         # Use Path().replace() to copy the file
-#         try:
-#             copyfile(src_path, dest_path)
-#         except Exception as e:
-#             print(str(e))
-#             continue
-
-#         # Check if the file was copied successfully
-#         if not dest_path.exists():
-#             continue
-
-#     return True, "初始化成功"
-
-
 def get_tally():
     status, _token = get_token()
     if not status:
         return False, _token
 
     url = f"{server_host}/system/openapi/user/tally"
     headers = {
         "Content-type": "application/json",
         "authorization": _token
     }
     response = https_get(url, headers=headers)
     # response = requests.get(url, headers=headers, timeout=20)
     if response.code != 200:
-        return False, "服务器错误."
+        return False, "服务器内部错误, 请稍后再试", ""
 
     if not response.success:
-        return False, response.msg
+        return False, response.msg, ""
 
-    return True, response.data['tally']
+    tally = response.data['tally']
+    tally = int(tally)
+    info = f"可以部署{int(tally/20)}个远程应用或{int(tally/5)}个本地应用"
+    return True, response.data['tally'], info
 
 
 def restart_app(app_name):
     status, _token = get_token()
     if not status:
         return False, _token
 
     url = f"{server_host}/system/openapi/app/restart"
     headers = {
         "Content-type": "application/json",
         "authorization": _token
     }
     status, app_name, _, _ = get_app_name(app_name)
     if not status:
-        return False, "获取应用名错误"
+        return False, f"获取应用名错误: {app_name}"
 
     response = https_post(
         url, json_data={"app_name": app_name}, headers=headers)
     if response.code != 200:
-        return False, "服务器错误."
+        return False, "服务器内部错误, 请稍后再试"
 
     if not response.success:
         return False, response.msg
 
     return True, response.msg
 
 
 def delete_app(app_name):
-    status, app_name, _, _ = get_app_name(app_name)
-    if not status:
-        return False, "获取应用名错误"
-
-    data = {"app_name": app_name}
     status, _token = get_token()
     if not status:
         return False, _token
 
+    status, app_name, _, _ = get_app_name(app_name)
+    if not status:
+        return False, f"获取应用名错误: {app_name}"
+
+    data = {"app_name": app_name}
     headers = {
         "Content-type": "application/json",
         "authorization": _token
     }
     url = f"{server_host}/system/openapi/app/del"
     response = https_post(url, json_data=data, headers=headers)
     if not response.success:
@@ -599,21 +560,21 @@
     url = f"{server_host}/system/openapi/app/status"
     headers = {
         "Content-type": "application/json",
         "authorization": _token
     }
     status, app_name, _, _ = get_app_name(app_name)
     if not status:
-        return False, {}, "获取应用名错误"
+        return False, {}, f"获取应用名错误: {app_name}"
 
     data = {"app_name": app_name}
 
     response = https_post(url, json_data=data, headers=headers)
     if response.code != 200:
-        return False, {}, "服务器错误."
+        return False, {}, "服务器内部错误, 请稍后再试"
 
     if not response.success:
         return False, {}, response.msg
 
     app_info = response.data
     app_info = app_info['data']
     app_info_str = f"""
@@ -637,15 +598,15 @@
         "Content-type": "application/json",
         "authorization": _token
     }
 
     #response = requests.get(url, headers=headers, timeout=20)
     response = https_get(url, headers=headers)
     if response.code != 200:
-        return False, "服务器错误."
+        return False, "服务器内部错误, 请稍后再试"
 
     if not response.success:
         return False, response.msg
 
     app_list = response.data['data']
     table = pt.PrettyTable(
         ['应用名', '应用别名', '域名', '服务状态', '应用状态', '创建时间'])
@@ -653,15 +614,15 @@
         table.add_row((app['AppName'], app['AppCnName'], app['Domain'],
                       app['ServerStatus'], app['AppStast'], app['CreateTime']))
 
     return True, table
 
 
 def get_cli_server_version():
-    return "0.8.7"
+    return "0.8.8"
 
 
 def update_template():
     pass
 
 
 def activate_account():
@@ -674,15 +635,15 @@
         "authorization": _token
     }
 
     url = f"{server_host}/system/openapi/user/verify/code"
 
     response = https_get(url, headers=headers)
     if response.code != 200:
-        return False, "服务器连接异常"
+        return False, "服务器内部错误, 请稍后再试"
 
     if not response.success:
         return False, f"获取验证码异常: {response.msg}"
 
     verify_code = ""
     while True:
         try:
@@ -699,15 +660,15 @@
         break
 
     url = f"{server_host}/system/openapi/user/verify/code"
 
     response = https_post(
         url, json_data={"code": verify_code}, headers=headers)
     if response.code != 200:
-        return False, "服务器连接异常"
+        return False, "服务器内部错误, 请稍后再试"
 
     if not response.success:
         return False, f"获取验证码异常: {response.msg}"
 
     return True, response.msg
 
 
@@ -722,15 +683,15 @@
         "password": password,
         "email": email
     }
 
     response = https_post(url, json_data=data, headers=headers)
 
     if response.code != 200:
-        return False, "服务器连接异常"
+        return False, "服务器内部错误, 请稍后再试"
 
     if not response.success:
         return False, f"注册异常: {response.msg}"
 
     print(f"用户: {username} 注册成功, 注册后需要接受邮件验证码并且输入验证码后才能使用")
     print("验证码也可以之后使用 -V 进行重新验证")
 
@@ -739,15 +700,15 @@
         f.write(response.data['token'])
 
     headers["authorization"] = response.data['token']
     url = f"{server_host}/system/openapi/user/verify/code"
 
     response = https_get(url, headers=headers)
     if response.code != 200:
-        return False, "服务器连接异常"
+        return False, "服务器内部错误, 请稍后再试"
 
     if not response.success:
         return False, f"获取验证码异常: {response.msg}"
 
     ststus, msg = activate_account()
 
     return ststus, msg
```

### Comparing `sipiiiii-0.8.7/sipiiiii/app/utils/HttpSDK.py` & `sipiiiii-0.8.8/sipiiiii/app/utils/HttpSDK.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.7/sipiiiii/app/utils/Tools.py` & `sipiiiii-0.8.8/sipiiiii/app/utils/Tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,20 +42,17 @@
         openapi_yaml = yaml.safe_load(openapi_yaml)
     except Exception as e:
         print(e)
         return ""
     return openapi_yaml
 
 
-def write_new_yaml(yaml_file):
+def write_new_yaml(yaml_file, app_type):
+    if app_type != "openai":
+        return
     with open(yaml_file, "r", encoding="utf-8") as f:
         openapi_yaml = f.read()
     openapi_yaml = yaml.safe_load(openapi_yaml)
     openapi_yaml['openapi'] = "3.0.1"
     del openapi_yaml['swagger']
     with open(f"{os.getcwd()}{os.sep}aiapi.yaml", "w", encoding="utf") as f:
         yaml.dump(openapi_yaml, stream=f, allow_unicode=True)
-
-    # try:
-    #     os.remove(yaml_file)
-    # except Exception as _:
-    #     pass
```

### Comparing `sipiiiii-0.8.7/sipiiiii/app/utils/ZipFileTool.py` & `sipiiiii-0.8.8/sipiiiii/app/utils/ZipFileTool.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.7/sipiiiii/app/utils/formatConversion.py` & `sipiiiii-0.8.8/sipiiiii/app/utils/formatConversion.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.7/sipiiiii/main.py` & `sipiiiii-0.8.8/sipiiiii/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,20 +75,22 @@
       sipiiiii -r <test.yaml> 或 --restart <test.yaml>
       
     删除你的应用(非本地部署):
       sipiiiii -DE <app name> 或 --delete <app name>
       sipiiiii -DE <test.yaml> 或 --delete <test.yaml>
 
   示例:
-    sipiiiii -n test.yaml
-    sipiiiii -LD test.yaml
-    sipiiiii -LD your-app-name
+    使用注册邮箱和密码进行登录
+    sipiiiii -L 
+    创建一个新的应用, 创建后编写相关的业务代码
+    sipiiiii -n 
+    进入到应用目录后, 进行部署
     sipiiiii -D
-    sipiiiii -L
-    sipiiiii -i your-app-name
+    查看应用详情信息 
+    sipiiiii -i 应用名
 
 '''
     return _log
 
 
 def main():
     parser = argparse.ArgumentParser(description='说明', add_help=False)
@@ -141,15 +143,15 @@
     elif args['new']:
         # execute new code here
         status = False
         msg = ""
         if args['new'] == "default_value":
             status, msg, app_name = create_app_project()
         else:
-            status, msg, app_name = create_app(args['new'])
+            status, msg, app_name, _ = create_app(args['new'])
 
         if status:
             print(f"{msg} 项目目录在当前文件夹下的: {app_name}")
         else:
             print(msg)
 
     elif args['login']:
@@ -184,19 +186,19 @@
         _, msg = activate_account()
         print(msg)
 
     elif args['list']:
         _, apps = show_list()
         print(apps)
     elif args['tally']:
-        status, tally = get_tally()
+        status, tally, info = get_tally()
         if not status:
             print(tally)
         else:
-            print(f"你的积分: {tally}")
+            print(f"你的积分: {tally}, {info}")
 
     elif args['info']:
         status = False
         app_info = ""
         if args['info'] == "default_value":
             status, _, app_info = get_app_info()
         else:
```

### Comparing `sipiiiii-0.8.7/sipiiiii.egg-info/PKG-INFO` & `sipiiiii-0.8.8/sipiiiii.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.8.7
+Version: 0.8.8
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-0.8.7/sipiiiii.egg-info/SOURCES.txt` & `sipiiiii-0.8.8/sipiiiii.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -16,17 +16,12 @@
 sipiiiii/app/version.py
 sipiiiii/app/utils/HttpSDK.py
 sipiiiii/app/utils/Tools.py
 sipiiiii/app/utils/ZipFileTool.py
 sipiiiii/app/utils/__init__.py
 sipiiiii/app/utils/config.py
 sipiiiii/app/utils/formatConversion.py
-sipiiiii/app/utils/PPI/__init__.py
-sipiiiii/app/utils/PPI/generator_factory.py
-sipiiiii/app/utils/PPI/prog_class.py
-sipiiiii/app/utils/PPI/progbar.py
-sipiiiii/app/utils/PPI/progpercent.py
 template/python_fastapi.j2
 template/python_flask.j2
 template/python_openai.j2
 template/template_openai.yaml
 template/template_other.yaml
```

### Comparing `sipiiiii-0.8.7/template/python_openai.j2` & `sipiiiii-0.8.8/template/python_openai.j2`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.7/template/template_openai.yaml` & `sipiiiii-0.8.8/template/template_openai.yaml`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.7/template/template_other.yaml` & `sipiiiii-0.8.8/template/template_other.yaml`

 * *Files identical despite different names*

