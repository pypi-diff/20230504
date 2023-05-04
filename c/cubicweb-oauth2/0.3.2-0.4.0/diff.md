# Comparing `tmp/cubicweb-oauth2-0.3.2.tar.gz` & `tmp/cubicweb-oauth2-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-oauth2-0.3.2.tar", last modified: Tue May  3 21:47:06 2022, max compression
+gzip compressed data, was "cubicweb-oauth2-0.4.0.tar", last modified: Thu May  4 09:33:52 2023, max compression
```

## Comparing `cubicweb-oauth2-0.3.2.tar` & `cubicweb-oauth2-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 21:47:06.585714 cubicweb-oauth2-0.3.2/
--rw-rw-rw-   0 root         (0) root         (0)      436 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2860 2022-05-03 21:47:06.585714 cubicweb-oauth2-0.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2438 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 21:47:06.585714 cubicweb-oauth2-0.3.2/cubicweb_oauth2/
--rw-rw-rw-   0 root         (0) root         (0)      243 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/cubicweb_oauth2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/cubicweb_oauth2/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     8335 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/cubicweb_oauth2/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 21:47:06.585714 cubicweb-oauth2-0.3.2/cubicweb_oauth2/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      298 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/cubicweb_oauth2/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      298 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/cubicweb_oauth2/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      298 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/cubicweb_oauth2/i18n/fr.po
--rw-rw-rw-   0 root         (0) root         (0)     5123 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/cubicweb_oauth2/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     2702 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/cubicweb_oauth2/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 21:47:06.585714 cubicweb-oauth2-0.3.2/cubicweb_oauth2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2860 2022-05-03 21:47:05.000000 cubicweb-oauth2-0.3.2/cubicweb_oauth2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      629 2022-05-03 21:47:06.000000 cubicweb-oauth2-0.3.2/cubicweb_oauth2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-03 21:47:05.000000 cubicweb-oauth2-0.3.2/cubicweb_oauth2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2022-05-03 21:47:05.000000 cubicweb-oauth2-0.3.2/cubicweb_oauth2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-03 21:47:05.000000 cubicweb-oauth2-0.3.2/cubicweb_oauth2.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       34 2022-05-03 21:47:06.000000 cubicweb-oauth2-0.3.2/cubicweb_oauth2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-05-03 21:47:06.000000 cubicweb-oauth2-0.3.2/cubicweb_oauth2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-03 21:47:06.585714 cubicweb-oauth2-0.3.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2637 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 21:47:06.585714 cubicweb-oauth2-0.3.2/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 21:47:06.585714 cubicweb-oauth2-0.3.2/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     3243 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/test/jwt.key
--rw-rw-rw-   0 root         (0) root         (0)      800 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/test/jwt.pub
--rw-rw-rw-   0 root         (0) root         (0)     6970 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/test/test_oauth2.py
--rw-rw-rw-   0 root         (0) root         (0)       25 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/test-requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1916 2022-05-03 21:46:15.000000 cubicweb-oauth2-0.3.2/tox.ini
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-04 09:33:52.133850 cubicweb-oauth2-0.4.0/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      436 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/MANIFEST.in
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2840 2023-05-04 09:33:52.133850 cubicweb-oauth2-0.4.0/PKG-INFO
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2438 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/README.rst
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-04 09:33:52.129850 cubicweb-oauth2-0.4.0/cubicweb_oauth2/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      243 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/__init__.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      693 2023-05-04 08:51:51.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/__pkginfo__.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     8335 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/auth.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-04 09:33:52.133850 cubicweb-oauth2-0.4.0/cubicweb_oauth2/i18n/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      298 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/i18n/en.po
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      298 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/i18n/es.po
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      298 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/i18n/fr.po
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     5123 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/site_cubicweb.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2701 2023-03-21 09:36:29.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/views.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-04 09:33:52.129850 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2840 2023-05-04 09:33:52.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/PKG-INFO
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      646 2023-05-04 09:33:52.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/SOURCES.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-05-04 09:33:52.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/dependency_links.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       42 2023-05-04 09:33:52.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/entry_points.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-03-21 09:16:50.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/not-zip-safe
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       72 2023-05-04 09:33:52.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/requires.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       16 2023-05-04 09:33:52.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/top_level.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       38 2023-05-04 09:33:52.133850 cubicweb-oauth2-0.4.0/setup.cfg
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2637 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/setup.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-04 09:33:52.133850 cubicweb-oauth2-0.4.0/test/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-03-21 09:36:32.000000 cubicweb-oauth2-0.4.0/test/__init__.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-04 09:33:52.133850 cubicweb-oauth2-0.4.0/test/data/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        7 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/test/data/bootstrap_cubes
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     3243 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/test/jwt.key
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      800 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/test/jwt.pub
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     6935 2023-03-21 09:36:32.000000 cubicweb-oauth2-0.4.0/test/test_oauth2.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       25 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/test-requirements.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1916 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/tox.ini
```

### Comparing `cubicweb-oauth2-0.3.2/PKG-INFO` & `cubicweb-oauth2-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-oauth2
-Version: 0.3.2
+Version: 0.4.0
 Summary: Oauth2/OpenID authentication for cubicweb
 Home-page: http://www.cubicweb.org/project/cubicweb-oauth2
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
 
 Summary
 -------
@@ -70,9 +69,7 @@
      oauth2-enabled=yes
      oauth2-server-url=https://keycloak/auth/realms/master
      oauth2-client-id=<client_id>
      oauth2-client-secret=<client_secret>
 6. Start your instance, go to login page and click on "Log in with Oauth2"
 
 
-
-
```

### Comparing `cubicweb-oauth2-0.3.2/README.rst` & `cubicweb-oauth2-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-oauth2-0.3.2/cubicweb_oauth2/auth.py` & `cubicweb-oauth2-0.4.0/cubicweb_oauth2/auth.py`

 * *Files identical despite different names*

### Comparing `cubicweb-oauth2-0.3.2/cubicweb_oauth2/site_cubicweb.py` & `cubicweb-oauth2-0.4.0/cubicweb_oauth2/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-oauth2-0.3.2/cubicweb_oauth2/views.py` & `cubicweb-oauth2-0.4.0/cubicweb_oauth2/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """cubicweb-oauth2 views/forms/actions/components for web ui"""
 
 from pyramid.httpexceptions import HTTPFound
 
 from cubicweb import _
-from cubicweb.web.views.basetemplates import LogFormView, LogForm
-from cubicweb.web.formwidgets import Button
+from cubicweb_web.views.basetemplates import LogFormView, LogForm
+from cubicweb_web.formwidgets import Button
 from cubicweb import tags
 
 
 class LoginWithOauth2Button(Button):
     def __init__(self, label, url):
         super().__init__(label=label)
         self._url = url
@@ -50,15 +50,14 @@
     )
 
 
 class Oauth2LogFormView(LogFormView):
     def call(self, *args, **kwargs):
         config = self._cw.vreg.config
         if config["oauth2-enabled"]:
-
             if config["oauth2-auto-login"]:
                 raise HTTPFound(start_login_url(self._cw))
 
             cw = self._cw
             form = cw.vreg["forms"].select("logform", cw)
             if not any(isinstance(b, LoginWithOauth2Button) for b in form.form_buttons):
                 form.form_buttons.append(login_button(self._cw))
```

### Comparing `cubicweb-oauth2-0.3.2/cubicweb_oauth2.egg-info/PKG-INFO` & `cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-oauth2
-Version: 0.3.2
+Version: 0.4.0
 Summary: Oauth2/OpenID authentication for cubicweb
 Home-page: http://www.cubicweb.org/project/cubicweb-oauth2
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
 
 Summary
 -------
@@ -70,9 +69,7 @@
      oauth2-enabled=yes
      oauth2-server-url=https://keycloak/auth/realms/master
      oauth2-client-id=<client_id>
      oauth2-client-secret=<client_secret>
 6. Start your instance, go to login page and click on "Log in with Oauth2"
 
 
-
-
```

### Comparing `cubicweb-oauth2-0.3.2/cubicweb_oauth2.egg-info/SOURCES.txt` & `cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 cubicweb_oauth2.egg-info/entry_points.txt
 cubicweb_oauth2.egg-info/not-zip-safe
 cubicweb_oauth2.egg-info/requires.txt
 cubicweb_oauth2.egg-info/top_level.txt
 cubicweb_oauth2/i18n/en.po
 cubicweb_oauth2/i18n/es.po
 cubicweb_oauth2/i18n/fr.po
+test/__init__.py
 test/jwt.key
 test/jwt.pub
 test/test_oauth2.py
 test/data/bootstrap_cubes
```

### Comparing `cubicweb-oauth2-0.3.2/setup.py` & `cubicweb-oauth2-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-oauth2-0.3.2/test/jwt.key` & `cubicweb-oauth2-0.4.0/test/jwt.key`

 * *Files identical despite different names*

### Comparing `cubicweb-oauth2-0.3.2/test/jwt.pub` & `cubicweb-oauth2-0.4.0/test/jwt.pub`

 * *Files identical despite different names*

### Comparing `cubicweb-oauth2-0.3.2/test/test_oauth2.py` & `cubicweb-oauth2-0.4.0/test/test_oauth2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import os
-import pytest
 import unittest
 import urllib.parse
 
 from authlib.jose import jwt
 import responses
 
 from cubicweb.pyramid.test import PyramidCWTest
@@ -35,14 +34,16 @@
     # openssl rsa -in jwt.key -pubout -outform PEM -out jwt.pub
     with open(os.path.join(HERE, "jwt.key")) as f:
         privkey = f.read()
     return jwt.encode({"alg": "RS256"}, payload, privkey).decode()
 
 
 class AuthenticationTC(PyramidCWTest):
+    settings = {"cubicweb.bwcompat": False}
+
     @classmethod
     def init_config(cls, config):
         super().init_config(config)
         config.global_set_option("oauth2-enabled", True)
         config.global_set_option("oauth2-client-id", "id")
         config.global_set_option("oauth2-client-secret", "secret")
         config.global_set_option("oauth2-authorization-url", "https://provider/auth")
@@ -74,15 +75,14 @@
             self.set_option("oauth2-force-login", False)
         assert resp.body == (
             b'<!DOCTYPE html><html><head><meta http-equiv="refresh" content="0; '
             b'url=https://localhost:80/oauth2/start?rd=https%3A%2F%2Flocalhost%3A80%2F1" />'
             b"</head></html>"
         )
 
-    @pytest.mark.skip(reason="this test is broken for now sadly")
     def test_force_login_signedrequest(self):
         # we should not block requests with signedrequest token authentication
         self.set_option("oauth2-force-login", True)
         try:
             self.webapp.get("/1", headers={"Authorization": "Cubicweb foo"}, status=404)
         finally:
             self.set_option("oauth2-force-login", False)
```

### Comparing `cubicweb-oauth2-0.3.2/tox.ini` & `cubicweb-oauth2-0.4.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 [flake8]
 max-line-length = 100
 exclude = cubicweb_oauth2/migration/*,test/data/*,.tox/*
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
@@ -59,15 +59,15 @@
   twine check dist/*
   twine upload --skip-existing dist/*
 
 [testenv:deb-publish]
 passenv = JENKINS_USER JENKINS_TOKEN
 basepython = python3
 skip_install = true
-whitelist_externals =
+allowlist_externals =
   rm
   sh
   hg
   python3
 deps =
   httpie
 commands =
```

