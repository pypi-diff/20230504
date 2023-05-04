# Comparing `tmp/addons_installer-2.1.0.tar.gz` & `tmp/addons_installer-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addons_installer-2.1.0.tar", last modified: Tue Jul  5 15:58:53 2022, max compression
+gzip compressed data, was "addons_installer-3.0.0.tar", last modified: Thu May  4 14:52:13 2023, max compression
```

## Comparing `addons_installer-2.1.0.tar` & `addons_installer-3.0.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-05 15:58:53.287328 addons_installer-2.1.0/
--rw-r--r--   0 root         (0) root         (0)     5792 2022-07-05 15:58:53.287328 addons_installer-2.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5014 2022-06-29 09:05:54.000000 addons_installer-2.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-05 15:58:53.287328 addons_installer-2.1.0/addons_installer/
--rw-rw-rw-   0 root         (0) root         (0)      442 2022-06-25 14:55:41.000000 addons_installer-2.1.0/addons_installer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-25 14:55:41.000000 addons_installer-2.1.0/addons_installer/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2022-07-05 15:57:49.000000 addons_installer-2.1.0/addons_installer/addons_installer.py
--rw-rw-rw-   0 root         (0) root         (0)     4466 2022-06-30 13:08:12.000000 addons_installer-2.1.0/addons_installer/api.py
--rw-rw-rw-   0 root         (0) root         (0)     7123 2022-06-25 14:55:41.000000 addons_installer-2.1.0/addons_installer/git_addons.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2022-06-25 14:55:41.000000 addons_installer-2.1.0/addons_installer/local_addons.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-05 15:58:53.287328 addons_installer-2.1.0/addons_installer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5792 2022-07-05 15:58:53.000000 addons_installer-2.1.0/addons_installer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2022-07-05 15:58:53.000000 addons_installer-2.1.0/addons_installer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-05 15:58:53.000000 addons_installer-2.1.0/addons_installer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2022-07-05 15:58:53.000000 addons_installer-2.1.0/addons_installer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-07-05 15:58:53.000000 addons_installer-2.1.0/addons_installer.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1275 2022-06-25 14:55:41.000000 addons_installer-2.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      946 2022-07-05 15:58:53.291328 addons_installer-2.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 14:52:13.614966 addons_installer-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      249 2023-05-04 14:52:13.614966 addons_installer-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5014 2023-05-02 13:47:14.000000 addons_installer-3.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      699 2023-05-02 13:47:14.000000 addons_installer-3.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 14:52:13.614966 addons_installer-3.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 14:52:13.610966 addons_installer-3.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 14:52:13.610966 addons_installer-3.0.0/src/addons_installer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 13:47:14.000000 addons_installer-3.0.0/src/addons_installer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5279 2023-05-02 13:47:14.000000 addons_installer-3.0.0/src/addons_installer/addons_installer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5139 2023-05-03 09:51:05.000000 addons_installer-3.0.0/src/addons_installer/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     7097 2023-05-03 09:51:05.000000 addons_installer-3.0.0/src/addons_installer/git_addons.py
+-rw-rw-rw-   0 root         (0) root         (0)     1231 2023-05-03 09:51:05.000000 addons_installer-3.0.0/src/addons_installer/local_addons.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 14:52:13.610966 addons_installer-3.0.0/src/addons_installer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      249 2023-05-04 14:52:13.000000 addons_installer-3.0.0/src/addons_installer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-04 14:52:13.000000 addons_installer-3.0.0/src/addons_installer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 14:52:13.000000 addons_installer-3.0.0/src/addons_installer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-04 14:52:13.000000 addons_installer-3.0.0/src/addons_installer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-04 14:52:13.000000 addons_installer-3.0.0/src/addons_installer.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 14:52:13.614966 addons_installer-3.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    12315 2023-05-03 09:51:05.000000 addons_installer-3.0.0/tests/test_addons_finder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8632 2023-05-02 13:47:14.000000 addons_installer-3.0.0/tests/test_git_addons.py
+-rw-rw-rw-   0 root         (0) root         (0)     7323 2023-05-03 09:51:05.000000 addons_installer-3.0.0/tests/test_local_addons.py
```

### Comparing `addons_installer-2.1.0/PKG-INFO` & `addons_installer-3.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: addons_installer
-Version: 2.1.0
-Summary: Allow to find Odoo addons from Environment Variables
-Home-page: https://gitlab.ndp-systemes.fr/python-libs/addons_launcher
-Author: NDP Systemes
-Author-email: opensource@ndp-systemes.fr
-License: GPLv3
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,>=2.7
-Description-Content-Type: text/markdown
-
 # Odoo Addons Installer
 
 The purpose of this lib is to watch environment variable and find [Odoo](https://github.com/odoo/odoo) extra addons_path.
 The addons path can be `git` project (private or not, see [The protocole and the credential](#_private_git_project)) or local dir.
 
 Install
 =======
```

### Comparing `addons_installer-2.1.0/addons_installer/api.py` & `addons_installer-3.0.0/src/addons_installer/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,149 +1,158 @@
-import abc
-import sys
-from typing import Dict, List, Optional
-
-if sys.version_info[0] == 2:  # Python 2
-
-    class ABC(object):
-        __meta_class__ = abc.ABCMeta
-        __slots__ = ()
+from __future__ import annotations
 
-else:
-    ABC = abc.ABC
+import abc
+import os
+from typing import Dict, List, Optional, Type, TypeVar
 
 
 class KeySuffix(object):
-    def __init__(self, addons, name, default=None, have_default=True):
-        # type: (AddonsSuffix, str, str, bool) -> KeySuffix
+    def __init__(self, addons: AddonsSuffix, name: str, default: str = None, have_default: bool = True):
         self.name = name
         self.prefix = addons.prefix
         self.base_key = addons.identifier
         self.default_value = default
         self.have_default = have_default
 
-    def get_value(self, env_vars, with_default=True):
+    def get_value(self, env_vars: Dict[str, str], with_default: bool = True) -> Optional[str]:
         return (
             env_vars.get(self.full_key, env_vars.get(self.default_key, with_default and self.default_value or None))
             or None
         )
 
-    def get_key(self, *args):
-        # type: (List[str]) -> str
+    @staticmethod
+    def get_key(*args: str) -> str:
         return "_".join([s for s in args if s]).upper()
 
     @property
-    def full_key(self):
+    def full_key(self) -> str:
         return self.get_key(self.prefix, self.base_key, self.name)
 
     @property
-    def default_key(self):  # type: ()-> Optional[str]
+    def default_key(self) -> Optional[str]:
         return self.have_default and self.get_key(self.prefix, AddonsSuffix.ADDONS_DEFAULT, self.name) or None
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "%s(%s, default=%s)" % (type(self).__name__, self.full_key, self.default_key)
 
 
-class AddonsSuffix(ABC):
+class AddonsSuffix(abc.ABC):
     ADDONS_DEFAULT = "DEFAULT"
     ADDONS_SUFFIX_EXCLUDE = "EXCLUDE"
 
-    def __init__(self, prefix, base_key):
-        # type: (str, str) -> AddonsSuffix
+    prefix: str = None
+
+    def __init__(self, base_key: str):
         super(AddonsSuffix, self).__init__()
+        assert self.prefix, "Set the prefix attribute in %s" % type(self)
         self.base_key = base_key
-        self.prefix = prefix
         self._key_registry = {}
         self._values = {}
         self.NAME = self.create_key("", have_default=False)
 
     @property
-    def identifier(self):
+    def identifier(self) -> str:
         return self.base_key.replace(self.prefix, "").strip("_")
 
-    def extract(self, env_vars):
-        # type: (Dict[str, str]) -> OdooAddonsDef
+    @abc.abstractmethod
+    def extract(self, env_vars: Dict[str, str]) -> OdooAddonsDef:
         raise NotImplementedError()
 
-    def to_dict(self, env_vars):
-        # type: (Dict[str, str]) -> Dict[KeySuffix, str]
+    def to_dict(self, env_vars: Dict[str, str]) -> Dict[KeySuffix, str]:
         return {key: key.get_value(env_vars) for key_name, key in self._key_registry.items()}
 
-    def get_suffix_keys(self):
-        # type: () -> List[str]
+    def get_suffix_keys(self) -> List[str]:
         return list(self._key_registry.keys())
 
-    def create_key(self, name, default=None, have_default=True):
+    def create_key(self, name: str, default: str = None, have_default: bool = True):
         key = KeySuffix(addons=self, name=name, default=default, have_default=have_default)
         self._key_registry[name] = key
         return key
 
-    def is_valid(self):
+    def is_valid(self) -> bool:
         return (
             self.base_key.startswith(self.prefix)
             and self.identifier != self.base_key
             and not any(self.base_key.endswith(suffix) for suffix in self.get_suffix_keys() if suffix)
             and not self.base_key.endswith(self.ADDONS_SUFFIX_EXCLUDE)
         )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "%s(%s)" % (type(self).__name__, self.identifier)
 
-    def __eq__(self, other):
+    def __eq__(self, other: AddonsSuffix) -> bool:
         return isinstance(other, AddonsSuffix) and other.identifier == self.identifier
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash(self.identifier)
 
 
-class OdooAddonsDef(ABC):
-    def __init__(self, name):
+class OdooAddonsDef(abc.ABC):
+    def __init__(self, name: str):
         self.name = name
 
     @property
-    def addons_path(self):
+    @abc.abstractmethod
+    def addons_path(self) -> str:
         raise NotImplementedError()
 
-    def install_cmd(self):
-        # type: () -> List[List[str]]
+    @abc.abstractmethod
+    def install_cmd(self) -> List[List[str]]:
         raise NotImplementedError()
 
-    def arg_cmd(self):
-        # type: () -> List[str]
+    @abc.abstractmethod
+    def arg_cmd(self) -> List[str]:
         raise NotImplementedError()
 
 
-class ABCSubDirAddons(AddonsSuffix, ABC):
-    _identifier = None
+PT = TypeVar("PT", bound="AddonsSuffix")
+
 
-    def __init__(self, base_key):
+class ABCSubDirAddons(AddonsSuffix, abc.ABC):
+    parent_addons: PT
+
+    _parent_type: Type[PT] = None
+
+    def __init__(self, base_key: str):
+        assert self._parent_type, "Set _parent_type in %s" % type(self)
+        super(ABCSubDirAddons, self).__init__(base_key)
         of_ref = base_key.split("_OF_")[-1]
-        super(ABCSubDirAddons, self).__init__(self._identifier, base_key)
         self.parent_addons = None
         if of_ref and self.is_valid():
-            tmp = self.get_parent("")
+            tmp = self._parent_type("")
             key_git = tmp.prefix + "_" + of_ref
-            self.parent_addons = self.get_parent(key_git)
+            self.parent_addons = self._parent_type(key_git)
             assert self.parent_addons.is_valid(), "The key %s is not a Addons valid key" % key_git
 
-    def get_parent(self, key):
-        raise NotImplementedError
+    def is_valid(self) -> bool:
+        return super().is_valid() and "_OF_" in self.base_key
 
-    def extract(self, env_vars):  # type: (Dict[str, str]) -> LocalAddonsResult
-        raise NotImplementedError
+    @property
+    def identifier(self) -> str:
+        return super().identifier
 
+    def extract(self, env_vars: Dict[str, str]) -> BaseAddonsResult:
+        res = self.to_dict(env_vars)
+        parent_extract = self.parent_addons.extract(env_vars)
+        sub_path = res[self.NAME]
+
+        if os.path.isabs(sub_path):
+            sub_path = sub_path[1:]  # Remove '/' at first, removeprefix don't exist in 3.8
+        full_path = os.path.join(parent_extract.addons_path, sub_path)
+        return BaseAddonsResult(name=self.NAME.full_key, full_path=full_path)
+
+
+class BaseAddonsResult(OdooAddonsDef):
+    def __init__(self, name: str, full_path: str):
+        super().__init__(name)
+        self.name = name
+        self._full_path = full_path
 
-class LocalAddonsResult(OdooAddonsDef):
-    def install_cmd(self):
+    def install_cmd(self) -> List[List[str]]:
         return []
 
-    def arg_cmd(self):
+    def arg_cmd(self) -> List[str]:
         return []
 
     @property
-    def addons_path(self):
-        return self.full_path
-
-    def __init__(self, name, full_path):
-        super(LocalAddonsResult, self).__init__(name)
-        self.name = name
-        self.full_path = full_path
+    def addons_path(self) -> str:
+        return self._full_path
```

### Comparing `addons_installer-2.1.0/addons_installer/git_addons.py` & `addons_installer-3.0.0/src/addons_installer/git_addons.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,49 @@
+from __future__ import annotations
 import logging
 from os.path import exists as path_exists
 from os.path import expanduser
 from os.path import join as path_join
 from typing import Dict, List
-
-from .api import (
-    ABCSubDirAddons,
-    AddonsSuffix,
-    KeySuffix,
-    LocalAddonsResult,
-    OdooAddonsDef,
-)
+from .api import ABCSubDirAddons, AddonsSuffix, BaseAddonsResult, OdooAddonsDef, KeySuffix
 
 _logger = logging.getLogger(__name__)
 _logger.setLevel(logging.INFO)
 
 
 class GitOdooAddons(AddonsSuffix):
-    _prefix = "ADDONS_GIT"
+    """
+    Represent a Git remote url to clone to get Odoo Addons.
+
+    """
+
     PROTOCLE_HTTPS = "https"
     PROTOCLE_SSH = "ssh"
     PROTOCLE_PUBLIC = "public"
     FORMAT_GIT_CLONE = {
         PROTOCLE_HTTPS: "https://%(login)s:%(password)s@%(server)s/%(git_path)s.git",
         PROTOCLE_SSH: "git@%(server)s:%(git_path)s.git",
         PROTOCLE_PUBLIC: "https://%(server)s/%(git_path)s.git",
     }
 
     def __init__(self, base_key):
-        super(GitOdooAddons, self).__init__(GitOdooAddons._prefix, base_key)
+        super(GitOdooAddons, self).__init__(base_key)
         self.BRANCH = self.create_key("BRANCH", default="master")
         self.CLONE_PATH = self.create_key("CLONE_PATH")
         self.PULL_OPTIONS = self.create_key("PULL_OPTIONS", default="--depth=1,--quiet,--single-branch")
         self.HTTPS_LOGIN = self.create_key("HTTPS_LOGIN")
         self.HTTPS_PASSWORD = self.create_key("HTTPS_PASSWORD")
         self.PROTOCOLE = self.create_key("PROTOCOLE", default=self.PROTOCLE_PUBLIC)
         self.SERVER = self.create_key("SERVER")
 
-    def extract(self, env_vars):
-        # type: (Dict[str, str]) -> GitOdooAddonsResult
+    @property
+    def prefix(self):
+        return "ADDONS_GIT"
+
+    def extract(self, env_vars: Dict[str, str]) -> GitOdooAddonsResult:
         res = self.to_dict(env_vars)
         # Remove de '/' at the end and the beginning of the name '/p1/p2' become 'p1/p2'
         self._apply_check(env_vars, res)
 
         res[self.NAME] = res[self.NAME].strip("/")
 
         protocole = self._get_protocole(env_vars, res)
@@ -61,26 +62,24 @@
             pull_options=pull_option,
             https_login=res.get(self.HTTPS_LOGIN),
             https_password=res.get(self.HTTPS_PASSWORD),
             protocole=protocole,
             server=res[self.SERVER],
         )
 
-    def _get_protocole(self, env_vars, res):
-        # type: (Dict[str, str], Dict[KeySuffix, str]) -> str
+    def _get_protocole(self, env_vars: Dict[str, str], res: Dict[KeySuffix, str]):
         if (
             not self.PROTOCOLE.get_value(env_vars, with_default=False)
             and res[self.HTTPS_LOGIN]
             and res[self.HTTPS_PASSWORD]
         ):
             return self.PROTOCLE_HTTPS
         return res[self.PROTOCOLE]
 
-    def _apply_check(self, env_vars, res):
-        # type: (Dict[str, str], Dict[KeySuffix, str]) -> None
+    def _apply_check(self, env_vars: Dict[str, str], res: Dict[KeySuffix, str]):
         if not res[self.SERVER]:
             raise ValueError(
                 "Not git server is provided, key [%s] or [%s]" % (self.SERVER.full_key, self.SERVER.default_key)
             )
         if res[self.PROTOCOLE] not in self.FORMAT_GIT_CLONE.keys():
             raise ValueError(
                 "The selected protocole %s is not supported, possible values are %s"
@@ -143,54 +142,52 @@
         self.pull_options = pull_options
         self.https_login = https_login
         self.https_password = https_password
         self.protocole = protocole
         self.server = server
         self.format = GitOdooAddons.FORMAT_GIT_CLONE[protocole]
 
-    def install_cmd(self):
-        # type: () -> List[List[str]]
+    def install_cmd(self) -> List[List[str]]:
         if path_exists(self.clone_path):
             _logger.info("Path %s not empty to clone %s", self.clone_path, self)
             return []
         clone_cmd = ["git", "clone"]
         clone_cmd.extend(self.arg_cmd())
         clone_cmd.append(self.clone_path)
         return [clone_cmd]
 
-    def arg_cmd(self):
-        # type: () -> List[str]
+    def arg_cmd(self) -> List[str]:
         clone_cmd = []
         if self.pull_options:
             clone_cmd.extend(self.pull_options)
         if self.branch:
             clone_cmd.append("-b")
             clone_cmd.append(self.branch)
         clone_cmd.append(self.git_url)
         return clone_cmd
 
     @property
-    def addons_path(self):
+    def addons_path(self) -> str:
         return self.clone_path
 
     @property
-    def git_url(self):
+    def git_url(self) -> str:
         return self.format % {
             "login": self.https_login,
             "password": self.https_password,
             "server": self.server,
             "git_path": self.git_path,
         }
 
 
 class GitSubDirOdooAddons(ABCSubDirAddons):
-    _identifier = "ADDONS_SUBDIR_GIT"
+    _parent_type = GitOdooAddons
 
-    def get_parent(self, key):
-        return GitOdooAddons(key)
+    @property
+    def prefix(self):
+        return "ADDONS_SUBDIR_GIT"
 
-    def extract(self, env_vars):
-        # type: (Dict[str, str]) -> LocalAddonsResult
+    def extract(self, env_vars: Dict[str, str]) -> BaseAddonsResult:
         res = self.to_dict(env_vars)
-        git_res = self.parent_addons.to_dict(env_vars)
-        full_path = path_join(git_res[self.parent_addons.CLONE_PATH], res[self.NAME])
-        return LocalAddonsResult(name=self.NAME.full_key, full_path=full_path)
+        git_res = self.parent_addons.extract(env_vars)
+        full_path = path_join(git_res.addons_path, res[self.NAME])
+        return BaseAddonsResult(name=self.NAME.full_key, full_path=full_path)
```

