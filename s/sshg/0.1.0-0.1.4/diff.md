# Comparing `tmp/sshg-0.1.0.tar.gz` & `tmp/sshg-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshg-0.1.0.tar", max compression
+gzip compressed data, was "sshg-0.1.4.tar", max compression
```

## Comparing `sshg-0.1.0.tar` & `sshg-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1068 2023-05-04 03:09:43.907914 sshg-0.1.0/LICENSE
--rw-r--r--   0        0        0     1939 2023-05-04 05:39:30.827422 sshg-0.1.0/README.md
--rw-r--r--   0        0        0      681 2023-05-04 05:39:52.793197 sshg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    11223 2023-05-04 05:39:52.793439 sshg-0.1.0/sshg.py
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 sshg-0.1.0/setup.py
--rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 sshg-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-04 07:53:20.678888 sshg-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2318 2023-05-04 07:53:20.678888 sshg-0.1.4/README.md
+-rw-r--r--   0        0        0      629 2023-05-04 07:53:40.471302 sshg-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    11223 2023-05-04 07:53:40.471302 sshg-0.1.4/sshg.py
+-rw-r--r--   0        0        0     3027 1970-01-01 00:00:00.000000 sshg-0.1.4/PKG-INFO
```

### Comparing `sshg-0.1.0/LICENSE` & `sshg-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sshg-0.1.0/README.md` & `sshg-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # sshg
 先说为什么起这个名字呢？
 因为我之前起的几个名字sshx, sshs 都被别人捷足先登了，而且项目写的还不错。可他们的项目又不能满足我快速选择要连接的设备和远程配置的需求，所以我就只起sshg这个名字了
 
+[![codecov](https://codecov.io/gh/codeskyblue/sshg/branch/master/graph/badge.svg?token=RUS38DVMCR)](https://codecov.io/gh/codeskyblue/sshg)
+[![PyPI version](https://badge.fury.io/py/sshg.svg)](https://badge.fury.io/py/sshg)
+
 ## 支持的功能
 - [x] 支持将ip,user,password写入到配置文件中，并快速的键盘选择上下选择功能(VIM的hj也支持)
 - [x] 支持ssh跳板机的功能
 - [ ] 远程配置的功能
 
 ## 安装
 ```bash
-pip install sshg
+pip3 install sshg
 ```
 
 ## 使用
 创建配置文件 `~/.sshg.yml`
 
 文件内容例子
 
 ```yaml
 - name: inner-server
   user: appuser
   host: 192.168.8.35
   port: 22
   password: 123456 # login password
-  gateway:
-    user: gateway-server
+  via:
+    user: via-server
     host: 10.0.0.38
     port: 2222
 - name: dev server fully configured
   user: appuser
   host: 192.168.1.1
   keypath: ~/.ssh/id_rsa
   password: abcdefghijklmn # passphrase
@@ -64,15 +67,17 @@
 # 没安装就装一下，项目依赖poetry发布
 # pip install poetry
 
 poetry self add "poetry-dynamic-versioning[plugin]"
 poetry publish --build
 ```
 
+
 # Refs
 - https://poetry.eustace.io/docs/
 - https://pypi.org/project/poetry-dynamic-versioning/
 - https://github.com/yinheli/sshw UI风格基本都是参考这个项目
 - https://github.com/WqyJh/sshx 本来用这个名字的，发现跟它重复了
+- https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/ 如何使用Github Actions发布
 
 # LICENSE
 [MIT](LICENSE)
```

### Comparing `sshg-0.1.0/pyproject.toml` & `sshg-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "sshg"
-version = "0.1.0"
+version = "0.1.4"
 description = "ssh from config with arrow select support"
 authors = ["codeskyblue <codeskyblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Jinja2 = "^3.1.2"
 requests = "*"
 dataclasses-json = "*"
 pyyaml = "*"
 prompt_toolkit = "*"
 pexpect = "*"
 
 [tool.poetry.scripts]
-gen_supervisor_conf = "py3toolkit.gen_supervisor_conf:main"
-sshg = "py3toolkit.sshg:main"
+sshg = "sshg:main"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
+pytest-cov = "^2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `sshg-0.1.0/sshg.py` & `sshg-0.1.4/sshg.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from prompt_toolkit.key_binding import KeyBindings, KeyPressEvent
 from prompt_toolkit.keys import Keys
 from prompt_toolkit.layout.containers import HSplit, Window
 from prompt_toolkit.layout.controls import FormattedTextControl
 from prompt_toolkit.layout.layout import Layout
 from prompt_toolkit.styles import Style
 
-__version__ = "0.1.0"
+__version__ = "0.1.4"
 
 def make_field(field_name: str = None,
                mm_field=None,
                decorder: typing.Callable = None,
                default=dataclasses.MISSING,
                default_factory=dataclasses.MISSING, **kwargs) -> dataclasses.field:
     return dataclasses.field(metadata=dconfig(field_name=field_name,
```

### Comparing `sshg-0.1.0/PKG-INFO` & `sshg-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sshg
-Version: 0.1.0
+Version: 0.1.4
 Summary: ssh from config with arrow select support
 License: MIT
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,37 +20,40 @@
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # sshg
 先说为什么起这个名字呢？
 因为我之前起的几个名字sshx, sshs 都被别人捷足先登了，而且项目写的还不错。可他们的项目又不能满足我快速选择要连接的设备和远程配置的需求，所以我就只起sshg这个名字了
 
+[![codecov](https://codecov.io/gh/codeskyblue/sshg/branch/master/graph/badge.svg?token=RUS38DVMCR)](https://codecov.io/gh/codeskyblue/sshg)
+[![PyPI version](https://badge.fury.io/py/sshg.svg)](https://badge.fury.io/py/sshg)
+
 ## 支持的功能
 - [x] 支持将ip,user,password写入到配置文件中，并快速的键盘选择上下选择功能(VIM的hj也支持)
 - [x] 支持ssh跳板机的功能
 - [ ] 远程配置的功能
 
 ## 安装
 ```bash
-pip install sshg
+pip3 install sshg
 ```
 
 ## 使用
 创建配置文件 `~/.sshg.yml`
 
 文件内容例子
 
 ```yaml
 - name: inner-server
   user: appuser
   host: 192.168.8.35
   port: 22
   password: 123456 # login password
-  gateway:
-    user: gateway-server
+  via:
+    user: via-server
     host: 10.0.0.38
     port: 2222
 - name: dev server fully configured
   user: appuser
   host: 192.168.1.1
   keypath: ~/.ssh/id_rsa
   password: abcdefghijklmn # passphrase
@@ -86,15 +89,17 @@
 # 没安装就装一下，项目依赖poetry发布
 # pip install poetry
 
 poetry self add "poetry-dynamic-versioning[plugin]"
 poetry publish --build
 ```
 
+
 # Refs
 - https://poetry.eustace.io/docs/
 - https://pypi.org/project/poetry-dynamic-versioning/
 - https://github.com/yinheli/sshw UI风格基本都是参考这个项目
 - https://github.com/WqyJh/sshx 本来用这个名字的，发现跟它重复了
+- https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/ 如何使用Github Actions发布
 
 # LICENSE
 [MIT](LICENSE)
```

