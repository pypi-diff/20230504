# Comparing `tmp/pa-dlna-0.4.tar.gz` & `tmp/pa-dlna-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pa-dlna-0.4.tar", last modified: Sat Apr  1 09:31:17 2023, max compression
+gzip compressed data, was "pa-dlna-0.5.tar", last modified: Thu May  4 09:51:01 2023, max compression
```

## Comparing `pa-dlna-0.4.tar` & `pa-dlna-0.5.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0       94 2023-02-22 15:13:35.485494 pa-dlna-0.4/.coveragerc
--rw-r--r--   0        0        0       53 2023-03-11 14:12:56.457976 pa-dlna-0.4/.gitignore
--rw-r--r--   0        0        0     1069 2023-03-26 14:17:19.707970 pa-dlna-0.4/.gitlab-ci.yml
--rw-r--r--   0        0        0      594 2023-01-03 10:16:37.856552 pa-dlna-0.4/.gitlab/issue_templates/Default.md
--rw-r--r--   0        0        0      372 2023-01-02 10:51:58.608445 pa-dlna-0.4/.readthedocs.yaml
--rw-r--r--   0        0        0     1081 2022-03-09 16:46:11.925010 pa-dlna-0.4/LICENSE
--rw-r--r--   0        0        0     2162 2023-04-01 09:04:08.592267 pa-dlna-0.4/README.rst
--rw-r--r--   0        0        0      638 2022-12-06 09:56:11.643760 pa-dlna-0.4/docs/Makefile
--rw-r--r--   0        0        0       38 2023-01-02 11:02:52.279913 pa-dlna-0.4/docs/requirements.txt
--rw-r--r--   0        0        0      945 2023-04-01 09:14:04.889355 pa-dlna-0.4/docs/source/_static/coverage.svg
--rw-r--r--   0        0        0      681 2022-12-29 10:19:08.013752 pa-dlna-0.4/docs/source/common.txt
--rw-r--r--   0        0        0     1595 2023-01-02 08:47:10.253567 pa-dlna-0.4/docs/source/conf.py
--rw-r--r--   0        0        0     6050 2023-04-01 08:11:51.640987 pa-dlna-0.4/docs/source/configuration.rst
--rw-r--r--   0        0        0     5417 2023-04-01 09:13:50.696085 pa-dlna-0.4/docs/source/default-config.rst
--rw-r--r--   0        0        0     7658 2023-04-01 09:13:18.069563 pa-dlna-0.4/docs/source/development.rst
--rw-r--r--   0        0        0     2104 2023-04-01 08:11:51.640987 pa-dlna-0.4/docs/source/history.rst
--rw-r--r--   0        0        0      608 2023-03-24 09:34:45.455574 pa-dlna-0.4/docs/source/index.rst
--rw-r--r--   0        0        0     1969 2022-12-29 10:19:08.043751 pa-dlna-0.4/docs/source/pa-dlna.rst
--rw-r--r--   0        0        0     1156 2022-12-29 10:19:08.043751 pa-dlna-0.4/docs/source/upnp-cmd.rst
--rw-r--r--   0        0        0     5958 2023-01-02 10:46:43.319274 pa-dlna-0.4/docs/source/usage.rst
--rw-r--r--   0        0        0      303 2023-04-01 09:16:31.612017 pa-dlna-0.4/pa_dlna/__init__.py
--rw-r--r--   0        0        0     9850 2023-04-01 08:11:51.640987 pa-dlna-0.4/pa_dlna/config.py
--rw-r--r--   0        0        0    12511 2023-04-01 08:11:51.640987 pa-dlna-0.4/pa_dlna/encoders.py
--rw-r--r--   0        0        0    20319 2023-04-01 08:11:51.640987 pa-dlna-0.4/pa_dlna/http_server.py
--rw-r--r--   0        0        0     9757 2023-03-26 14:17:19.711304 pa-dlna-0.4/pa_dlna/init.py
--rw-r--r--   0        0        0    27994 2023-03-29 13:45:15.174594 pa-dlna-0.4/pa_dlna/pa_dlna.py
--rw-r--r--   0        0        0     8567 2023-03-13 13:54:39.691087 pa-dlna-0.4/pa_dlna/pulseaudio.py
--rw-r--r--   0        0        0     2205 2023-02-23 08:20:26.926423 pa-dlna-0.4/pa_dlna/tests/__init__.py
-lrwxr-xr-x   0        0        0        0 2023-02-23 08:02:35.850765 pa-dlna-0.4/pa_dlna/tests/encoder.py -> streams.py
-lrwxr-xr-x   0        0        0        0 2023-02-23 08:46:33.657873 pa-dlna-0.4/pa_dlna/tests/parec.py -> streams.py
--rw-r--r--   0        0        0     5866 2023-03-07 16:06:40.148810 pa-dlna-0.4/pa_dlna/tests/pulsectl.py
--rwxr-xr-x   0        0        0    12183 2023-03-02 14:02:18.102736 pa-dlna-0.4/pa_dlna/tests/streams.py
--rw-r--r--   0        0        0    11740 2023-04-01 08:11:51.640987 pa-dlna-0.4/pa_dlna/tests/test_config.py
--rw-r--r--   0        0        0    12559 2023-03-29 10:10:16.924957 pa-dlna-0.4/pa_dlna/tests/test_http_server.py
--rw-r--r--   0        0        0    10270 2023-03-26 14:17:19.711304 pa-dlna-0.4/pa_dlna/tests/test_init.py
--rw-r--r--   0        0        0    26233 2023-03-28 08:55:56.283983 pa-dlna-0.4/pa_dlna/tests/test_pa_dlna.py
--rw-r--r--   0        0        0     7392 2023-03-09 16:03:30.493896 pa-dlna-0.4/pa_dlna/tests/test_pulseaudio.py
--rw-r--r--   0        0        0      566 2023-03-05 14:40:23.562964 pa-dlna-0.4/pa_dlna/upnp/__init__.py
--rw-r--r--   0        0        0    14956 2023-03-07 08:32:35.882778 pa-dlna-0.4/pa_dlna/upnp/network.py
--rw-r--r--   0        0        0     4655 2023-03-07 09:11:50.377493 pa-dlna-0.4/pa_dlna/upnp/tests/__init__.py
--rw-r--r--   0        0        0     4444 2023-01-30 09:51:40.021976 pa-dlna-0.4/pa_dlna/upnp/tests/device_resps.py
--rw-r--r--   0        0        0    12067 2023-03-05 16:09:03.890581 pa-dlna-0.4/pa_dlna/upnp/tests/test_network.py
--rw-r--r--   0        0        0    19485 2023-03-07 14:51:16.810453 pa-dlna-0.4/pa_dlna/upnp/tests/test_upnp.py
--rw-r--r--   0        0        0     3535 2023-01-29 10:05:34.085986 pa-dlna-0.4/pa_dlna/upnp/tests/test_util.py
--rw-r--r--   0        0        0     5073 2023-01-29 08:56:25.682591 pa-dlna-0.4/pa_dlna/upnp/tests/test_xml.py
--rw-r--r--   0        0        0    28269 2023-04-01 08:52:07.063073 pa-dlna-0.4/pa_dlna/upnp/upnp.py
--rw-r--r--   0        0        0     2804 2023-02-26 08:14:41.129014 pa-dlna-0.4/pa_dlna/upnp/util.py
--rw-r--r--   0        0        0     7571 2023-01-27 11:19:33.383315 pa-dlna-0.4/pa_dlna/upnp/xml.py
--rw-r--r--   0        0        0    19754 2023-03-06 10:47:27.242654 pa-dlna-0.4/pa_dlna/upnp_cmd.py
--rw-r--r--   0        0        0     1010 2023-01-02 16:11:27.189096 pa-dlna-0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-05 15:19:20.393000 pa-dlna-0.4/tools/__init__.py
--rw-r--r--   0        0        0     1554 2022-11-05 15:19:20.393000 pa-dlna-0.4/tools/build_didl_lite.py
--rw-r--r--   0        0        0     1790 2023-01-02 08:45:32.674009 pa-dlna-0.4/tools/gendoc_default_config.py
--rw-r--r--   0        0        0     2968 1970-01-01 00:00:00.000000 pa-dlna-0.4/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-02-22 15:13:35.485494 pa-dlna-0.5/.coveragerc
+-rw-r--r--   0        0        0       53 2023-03-11 14:12:56.457976 pa-dlna-0.5/.gitignore
+-rw-r--r--   0        0        0     1069 2023-03-26 14:17:19.707970 pa-dlna-0.5/.gitlab-ci.yml
+-rw-r--r--   0        0        0      594 2023-01-03 10:16:37.856552 pa-dlna-0.5/.gitlab/issue_templates/Default.md
+-rw-r--r--   0        0        0      372 2023-01-02 10:51:58.608445 pa-dlna-0.5/.readthedocs.yaml
+-rw-r--r--   0        0        0     1081 2022-03-09 16:46:11.925010 pa-dlna-0.5/LICENSE
+-rw-r--r--   0        0        0     2162 2023-04-01 09:04:08.592267 pa-dlna-0.5/README.rst
+-rw-r--r--   0        0        0      638 2023-04-13 13:35:50.730833 pa-dlna-0.5/docs/Makefile
+-rw-r--r--   0        0        0       38 2023-01-02 11:02:52.279913 pa-dlna-0.5/docs/requirements.txt
+-rw-r--r--   0        0        0      945 2023-05-04 09:42:53.490836 pa-dlna-0.5/docs/source/_static/coverage.svg
+-rw-r--r--   0        0        0      681 2022-12-29 10:19:08.013752 pa-dlna-0.5/docs/source/common.txt
+-rw-r--r--   0        0        0     1595 2023-04-20 10:04:24.742324 pa-dlna-0.5/docs/source/conf.py
+-rw-r--r--   0        0        0     6050 2023-04-01 08:11:51.640987 pa-dlna-0.5/docs/source/configuration.rst
+-rw-r--r--   0        0        0     5417 2023-05-04 09:41:57.204462 pa-dlna-0.5/docs/source/default-config.rst
+-rw-r--r--   0        0        0     8586 2023-04-20 10:04:24.742324 pa-dlna-0.5/docs/source/development.rst
+-rw-r--r--   0        0        0     2443 2023-04-20 10:04:24.742324 pa-dlna-0.5/docs/source/history.rst
+-rw-r--r--   0        0        0      608 2023-04-14 07:08:07.571321 pa-dlna-0.5/docs/source/index.rst
+-rw-r--r--   0        0        0     2319 2023-04-20 10:04:24.742324 pa-dlna-0.5/docs/source/pa-dlna.rst
+-rw-r--r--   0        0        0     1506 2023-04-20 10:04:24.742324 pa-dlna-0.5/docs/source/upnp-cmd.rst
+-rw-r--r--   0        0        0     6732 2023-04-20 10:04:24.742324 pa-dlna-0.5/docs/source/usage.rst
+-rw-r--r--   0        0        0      304 2023-05-04 09:40:53.444795 pa-dlna-0.5/pa_dlna/__init__.py
+-rw-r--r--   0        0        0    10026 2023-04-20 10:04:24.742324 pa-dlna-0.5/pa_dlna/config.py
+-rw-r--r--   0        0        0    12511 2023-04-01 08:11:51.640987 pa-dlna-0.5/pa_dlna/encoders.py
+-rw-r--r--   0        0        0    20319 2023-04-16 09:29:00.631641 pa-dlna-0.5/pa_dlna/http_server.py
+-rw-r--r--   0        0        0    10700 2023-04-20 10:04:24.742324 pa-dlna-0.5/pa_dlna/init.py
+-rw-r--r--   0        0        0    26964 2023-04-20 10:04:24.742324 pa-dlna-0.5/pa_dlna/pa_dlna.py
+-rw-r--r--   0        0        0     8567 2023-03-13 13:54:39.691087 pa-dlna-0.5/pa_dlna/pulseaudio.py
+-rw-r--r--   0        0        0     2205 2023-02-23 08:20:26.926423 pa-dlna-0.5/pa_dlna/tests/__init__.py
+lrwxr-xr-x   0        0        0        0 2023-02-23 08:02:35.850765 pa-dlna-0.5/pa_dlna/tests/encoder.py -> streams.py
+lrwxr-xr-x   0        0        0        0 2023-02-23 08:46:33.657873 pa-dlna-0.5/pa_dlna/tests/parec.py -> streams.py
+-rw-r--r--   0        0        0     5866 2023-03-07 16:06:40.148810 pa-dlna-0.5/pa_dlna/tests/pulsectl.py
+-rwxr-xr-x   0        0        0    12183 2023-03-02 14:02:18.102736 pa-dlna-0.5/pa_dlna/tests/streams.py
+-rw-r--r--   0        0        0    12208 2023-04-20 10:04:24.742324 pa-dlna-0.5/pa_dlna/tests/test_config.py
+-rw-r--r--   0        0        0    12559 2023-03-29 10:10:16.924957 pa-dlna-0.5/pa_dlna/tests/test_http_server.py
+-rw-r--r--   0        0        0    10953 2023-04-20 10:04:24.742324 pa-dlna-0.5/pa_dlna/tests/test_init.py
+-rw-r--r--   0        0        0    25268 2023-04-20 10:04:24.742324 pa-dlna-0.5/pa_dlna/tests/test_pa_dlna.py
+-rw-r--r--   0        0        0     7392 2023-03-09 16:03:30.493896 pa-dlna-0.5/pa_dlna/tests/test_pulseaudio.py
+-rw-r--r--   0        0        0      568 2023-04-20 10:04:24.742324 pa-dlna-0.5/pa_dlna/upnp/__init__.py
+-rw-r--r--   0        0        0    15384 2023-04-20 10:04:24.742324 pa-dlna-0.5/pa_dlna/upnp/network.py
+-rw-r--r--   0        0        0     4677 2023-04-20 10:04:24.742324 pa-dlna-0.5/pa_dlna/upnp/tests/__init__.py
+-rw-r--r--   0        0        0     4444 2023-01-30 09:51:40.021976 pa-dlna-0.5/pa_dlna/upnp/tests/device_resps.py
+-rw-r--r--   0        0        0    15827 2023-04-20 10:04:24.742324 pa-dlna-0.5/pa_dlna/upnp/tests/test_network.py
+-rw-r--r--   0        0        0    20989 2023-04-20 10:04:24.742324 pa-dlna-0.5/pa_dlna/upnp/tests/test_upnp.py
+-rw-r--r--   0        0        0     3535 2023-01-29 10:05:34.085986 pa-dlna-0.5/pa_dlna/upnp/tests/test_util.py
+-rw-r--r--   0        0        0     5073 2023-01-29 08:56:25.682591 pa-dlna-0.5/pa_dlna/upnp/tests/test_xml.py
+-rw-r--r--   0        0        0    30661 2023-04-20 10:04:24.745657 pa-dlna-0.5/pa_dlna/upnp/upnp.py
+-rw-r--r--   0        0        0     2804 2023-02-26 08:14:41.129014 pa-dlna-0.5/pa_dlna/upnp/util.py
+-rw-r--r--   0        0        0     7571 2023-01-27 11:19:33.383315 pa-dlna-0.5/pa_dlna/upnp/xml.py
+-rw-r--r--   0        0        0    20322 2023-04-20 10:04:24.745657 pa-dlna-0.5/pa_dlna/upnp_cmd.py
+-rw-r--r--   0        0        0     1010 2023-01-02 16:11:27.189096 pa-dlna-0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-05 15:19:20.393000 pa-dlna-0.5/tools/__init__.py
+-rw-r--r--   0        0        0     1554 2022-11-05 15:19:20.393000 pa-dlna-0.5/tools/build_didl_lite.py
+-rw-r--r--   0        0        0     1790 2023-01-02 08:45:32.674009 pa-dlna-0.5/tools/gendoc_default_config.py
+-rw-r--r--   0        0        0      740 2023-04-20 10:04:24.745657 pa-dlna-0.5/tools/set_devpt_version_name.py
+-rw-r--r--   0        0        0     2968 1970-01-01 00:00:00.000000 pa-dlna-0.5/PKG-INFO
```

### Comparing `pa-dlna-0.4/.gitlab-ci.yml` & `pa-dlna-0.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/.gitlab/issue_templates/Default.md` & `pa-dlna-0.5/.gitlab/issue_templates/Default.md`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/LICENSE` & `pa-dlna-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/README.rst` & `pa-dlna-0.5/README.rst`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/docs/Makefile` & `pa-dlna-0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/docs/source/_static/coverage.svg` & `pa-dlna-0.5/docs/source/_static/coverage.svg`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/docs/source/common.txt` & `pa-dlna-0.5/docs/source/common.txt`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/docs/source/conf.py` & `pa-dlna-0.5/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath('../..'))
 from pa_dlna import __version__
 
 project = 'pa-dlna'
-copyright = '2022, Xavier de Gaye'
+copyright = '2023, Xavier de Gaye'
 author = 'Xavier de Gaye'
 
 # The short X.Y version
 version = __version__
 # The full version, including alpha/beta/rc tags
 release = __version__
```

### Comparing `pa-dlna-0.4/docs/source/configuration.rst` & `pa-dlna-0.5/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/docs/source/default-config.rst` & `pa-dlna-0.5/docs/source/default-config.rst`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/docs/source/development.rst` & `pa-dlna-0.5/docs/source/development.rst`

 * *Files 8% similar despite different names*

```diff
@@ -117,61 +117,85 @@
     belongs to one of the subnets of the network interfaces. That is, the DLNA
     device and the host belong to the same subnet on this interface and the
     local IP address on this subnet is the address that is being looked for.
 
     The `UPnP Device Architecture`_ specification does not specify the
     periodicity of NOTIFY SSDPs sent by DLNA devices.
 
-Development process
--------------------
+Development process [#]_
+------------------------
 
 Requirements
 """"""""""""
 
 Development:
-    * `curl`_ is needed to run the full test suite. If missing then the tests
-      using curl are skipped.
-    * `coverage`_ may be used to get the test suite coverage.
-    * `flit`_ to publish pa-dlna to PyPi. Use the following command to install
-      pa-dlna locally and have the changes in the source code reflected by the
-      ``pa-dlna`` command::
-
-        $ flit install --symlink [--python path/to/python_version]
+    * `curl`_ is used to run the full test suite. When missing, the tests
+      using curl are skipped. It is needed when releasing a new version to fetch
+      the GitLab test coverage badge.
+    * `coverage`_ is used to get the test suite coverage.
+    * `flit`_ is used to install pa-dlna or to publish it to PyPi.
+
+      At the root of pa-dlna local git repository, use the following command to
+      install pa-dlna locally::
+
+        $ flit install --symlink [--python path/to/python]
+
+      This symlinks pa-dlna into site-packages rather than copying it, so that
+      you can test changes by running the ``pa-dlna`` and ``upnp-cmd`` commands
+      without reinstalling the package.
 
 Documentation:
     * `Sphinx`_ [#]_.
     * `Read the Docs theme`_.
 
 Documentation
 """""""""""""
 
-To build locally the documentation, generate the ``default-config.rst`` file,
-fetch the test coverage badge and build the html documentation and the man
-pages::
+To build locally the documentation and:
+
+  - Generate the ``default-config.rst`` file.
+  - Fetch the GitLab test coverage badge.
+  - Build the html documentation and the man pages.
+
+Run the following commands::
 
-  $ python -m tools.gendoc_default_config
-  $ curl -o docs/source/_static/coverage.svg\
+    $ python -m tools.gendoc_default_config
+    $ curl -o docs/source/_static/coverage.svg\
     "https://gitlab.com/xdegaye/pa-dlna/badges/master/coverage.svg?min_medium=85&min_acceptable=90&min_good=95"
-  $ make -C docs clean html man
+    $ make -C docs clean html man
+
+Updating development version
+""""""""""""""""""""""""""""
+
+In order to update the version at the `latest documentation`_ during
+development, after a change in the functionality or in the features, run the
+following commands::
+
+    $ python -m tools.set_devpt_version_name
+    $ make -C docs clean html man
+    $ git commit -m "Update version"
+    $ git push
 
 Releasing
 """""""""
 
 * Run the test suite from the root of the project [#]_::
 
     $ python -m unittest --verbose --catch --failfast
 
-* Optionally get the test suite coverage::
+* Get the test suite coverage::
 
     $ coverage run -m unittest
     $ coverage report -m
 
 * Update ``__version__`` in pa_dlna/__init__.py.
-* Update docs/source/history.rst
-* Build locally the documentation (fetch the latest test coverage badge).
+* Update docs/source/history.rst.
+* Build locally the documentation and possibly create a new version of
+  ``default-config.rst`` or create a new GitLab test coverage badge (see
+  above).
 * Commit the changes::
 
     $ git commit -m 'Version 0.n'
     $ git push
 
 * Tag the release and push::
 
@@ -190,15 +214,19 @@
     https://docs.readthedocs.io/en/stable/faq.html#i-want-to-use-the-read-the-docs-theme-locally
 .. _Sphinx: https://www.sphinx-doc.org/
 .. _curl: https://curl.se/
 .. _`coverage`: https://pypi.org/project/coverage/
 .. _flit: https://pypi.org/project/flit/
 .. _unittest command line options:
     https://docs.python.org/3/library/unittest.html#command-line-options
+.. _latest documentation:
+    https://pa-dlna.readthedocs.io/en/latest/
 
 .. rubric:: Footnotes
 
 .. [#] All sockets bound to the notify multicast address receive the datagram
        sent by a DLNA device, even though it has been received by only one
        interface at the physical layer.
+.. [#] The shell commands in this section are all run from the root of the
+       repository.
 .. [#] Required versions at ``docs/requirements.txt``.
 .. [#] See `unittest command line options`_.
```

### Comparing `pa-dlna-0.4/docs/source/history.rst` & `pa-dlna-0.5/docs/source/history.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Release history
 ===============
 
+Version 0.5
+  - Log a warning upon an empty body in the HTTP response from a DLNA device.
+  - UPnP discovery is triggered by NICs [#]_ state changes.
+  - Add the ``--ip-addresses``, ``-a`` command line argument.
+  - Fix changing the ``args`` encoder option is ignored.
+
 Version 0.4
   - ``sample_format`` is a new encoder configuration option.
-  - The encoders sample format is 's16le' except for the 'audio/l16' encoder.
+  - The encoders sample format is ``s16le`` except for the ``audio/l16``
+    encoder.
   - The encoder command line is now updated with ``pa-dlna.conf`` user
     configuration.
   - Fix the parec command line length keeps increasing at each new track when
     the encoder is set to track metadata.
   - Fix failing to start a new stream session while the device is still playing
     when the encoder is set to not track metadata.
   - Fix ``pa-dlna`` hangs when one types <Control-S> in the terminal where the
@@ -40,7 +47,11 @@
     network.Notify.manage_membership().
   - Fix removing multicast membership when the socket is closed.
   - Don't print a stack traceback upon error parsing the configuration file.
   - Abort on error setting the file logging handler with ``--logfile PATH``.
 
 Version 0.1
   - Publish the project on PyPi.
+
+.. rubric:: Footnotes
+
+.. [#] Network Interface Controller.
```

### Comparing `pa-dlna-0.4/docs/source/index.rst` & `pa-dlna-0.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/docs/source/pa-dlna.rst` & `pa-dlna-0.5/docs/source/pa-dlna.rst`

 * *Files 17% similar despite different names*

```diff
@@ -4,31 +4,39 @@
 =======
 
 Synopsis
 --------
 
 :program:`pa-dlna` [*options*]
 
+UPnP discovery is run on all the networks (except the loopbak interface ``lo``)
+when the ``--ip-addresses`` and ``--nics`` command line arguments are not used
+or empty. Otherwise both arguments may be used indifferently or even jointly.
+
 Options
 -------
 
 .. option::  -h, --help
 
    Show this help message and exit.
 
 .. option::  --version, -v
 
    Show program's version number and exit.
 
+.. option:: --ip-addresses IP_ADDRESSES, -a IP_ADDRESSES
+
+   IP_ADDRESSES is a comma separated list of the IPv4 addresses of the networks
+   where UPnP devices may be discovered (default: ``''``).
+
 .. option:: --nics NICS, -n NICS
 
    NICS is a comma separated list of the names of network interface controllers
    where UPnP devices may be discovered, such as ``wlan0,enp5s0`` for
-   example. All the interfaces are used when this option is an empty string or
-   the option is missing (default: ``''``)
+   example (default: ``''``).
 
 .. option::  --msearch-interval MSEARCH_INTERVAL, -m MSEARCH_INTERVAL
 
    Set the time interval in seconds between the sending of the MSEARCH datagrams
    used for device discovery (default: 60)
 
 .. option::  --ttl TTL
@@ -51,23 +59,23 @@
 
 .. option::  --loglevel {debug,info,warning,error}, -l {debug,info,warning,error}
 
    Set the log level of the stderr logging console (default: info).
 
 .. option::  --logfile PATH, -f PATH
 
-   Add a file logging handler set at 'debug' log level whose path name is PATH.
+   Add a file logging handler set at ``debug`` log level whose path name is PATH.
 
 .. option::  --nolog-upnp, -u
 
-   Ignore UPnP log entries at 'debug' log level.
+   Ignore UPnP log entries at ``debug`` log level.
 
-.. option::  --log-aio, -a
+.. option::  --log-aio, -y
 
-   Do not ignore asyncio log entries at 'debug' log level; the default is to
+   Do not ignore asyncio log entries at ``debug`` log level; the default is to
    ignore those verbose logs.
 
 .. option::  --test-devices MIME-TYPES, -t MIME-TYPES
 
    MIME-TYPES is a comma separated list of distinct audio mime types. A
    DLNATestDevice is instantiated for each one of these mime types and
    registered as a virtual DLNA device. Mostly for testing.
```

### Comparing `pa-dlna-0.4/docs/source/usage.rst` & `pa-dlna-0.5/docs/source/usage.rst`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,24 @@
 Once the encoder is selected, a new sink is registered with pulseaudio and an
 HTTP server is started.
 
 Then when there is an association between a pulseaudio source and this sink (see
 below), ``pa-dlna`` sends an URL to the device so that the device may fetch the
 corresponding audio stream by issuing an HTTP GET for this URL.
 
+UPnP discovery is triggered by NICs [#]_ state changes, that is, whenever a
+configured NIC or the NIC of a configured IP address becomes up. Some examples
+of events triggering UPnP discovery on an IP address after ``pa-dlna`` or
+``upnp-cmd`` [#]_ has been started:
+
+  - A wifi controller connects to a hotspot and acquires a new IP address
+    through DHCP, possibly a different address from the previous one.
+  - A static IP address has been configured on an ethernet card connected to an
+    ethernet switch and the switch is turned on.
+
 See the :ref:`pa-dlna` man page.
 
 Source-sink association
 """""""""""""""""""""""
 
 ``pa-dlna`` registers a new sink with pulseaudio upon the discovery of a DLNA
 device. The sink appears in the ``Output Devices`` tab of the ``pavucontrol``
@@ -136,14 +146,18 @@
 .. _Default/fallback devices:
         https://www.freedesktop.org/wiki/Software/PulseAudio/Documentation/User/DefaultDevice/
 .. _Automatic setup and routing:
         https://gavv.net/articles/pulseaudio-under-the-hood/#automatic-setup-and-routing
 
 .. rubric:: Footnotes
 
+.. [#] Network Interface Controller.
+.. [#] The list of the IP addresses where UPnP discovery is currently activated
+       can be listed on ``upnp-cmd`` by printing the value of the
+       ``ip_monitored`` variable in the main menu.
 .. [#] ``pavucontrol`` and ``pacmd`` are  part of pulseaudio and installed with
        pulseaudio.
 .. [#] A source is called a sink-input by pulseaudio.
 .. [#] An UPnP device implements the `UPnP Device Architecture`_ specification.
 .. [#] A DLNA device is an UPnP device and implements the `MediaRenderer
        Device`_ specification and the `ConnectionManager`_, `AVTransport`_ and
        `RenderingControl`_ services.
```

### Comparing `pa-dlna-0.4/pa_dlna/config.py` & `pa-dlna-0.5/pa_dlna/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,18 +101,18 @@
                     self.parser.set(section, f"# {attr[1:]}: {val}")
                 elif (not hasattr(root, attr) or
                       getattr(root, attr) != getattr(encoder, attr)):
                     if write_separator:
                         write_separator = False
                         self.write_empty_comment(section)
                     self.parser.set(section, attr, val)
-            if isinstance(self, DefaultConfig):
-                encoder.set_args()
-                if encoder.args:
-                    self.parser.set(section, 'args', encoder.args)
+
+            encoder.set_args()
+            if encoder.args:
+                self.parser.set(section, 'args', encoder.args)
 
     def get_value(self, section, encoder, option, new_val):
         old_val = getattr(encoder, option)
         if old_val is not True and old_val is not False:
             for t in (int, float):
                 if isinstance(old_val, t):
                     try:
@@ -122,14 +122,17 @@
         try:
             return self.parser.getboolean(section, option)
         except ValueError:
             pass
         return new_val
 
     def override_options(self, encoder, section, defaults):
+        encoder.set_args()
+        default_args = encoder.args
+
         for option, value in self.parser.items(section):
             if option.startswith("#") or option == 'selection':
                 continue
             if (hasattr(encoder, option) and
                     not option.startswith('_')):
                 new_val = self.get_value(section, encoder,
                                          option, value)
@@ -140,15 +143,19 @@
                             'audio/l16' not in
                                 (mtype.lower() for mtype in
                                  encoder._mime_types)):
                         setattr(encoder, option, new_val)
             elif option not in defaults:
                 raise ParsingError(f'Unknown option'
                                    f" '{section}.{option}'")
-        encoder.set_args()
+
+        # Re-evaluate 'args' with possibly modified options, as 'args' itself
+        # has not been customized by the user.
+        if default_args == encoder.args:
+            encoder.set_args()
 
     def write(self, fileobject):
         """Write the configuration to a text file object."""
 
         for comment in comments_from_doc(self.root_class.__doc__):
             fileobject.write(comment + '\n')
         fileobject.write('\n')
```

### Comparing `pa-dlna-0.4/pa_dlna/encoders.py` & `pa-dlna-0.5/pa_dlna/encoders.py`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/pa_dlna/http_server.py` & `pa-dlna-0.5/pa_dlna/http_server.py`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/pa_dlna/init.py` & `pa-dlna-0.5/pa_dlna/init.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Utilities for starting an UPnPApplication."""
 
 import sys
 import os
 import argparse
+import ipaddress
 import logging
 import asyncio
 import threading
 import struct
 import atexit
 try:
     import termios
@@ -79,15 +80,21 @@
             logfile_hdler.setFormatter(formatter)
             root.addHandler(logfile_hdler)
             return logfile_hdler
 
     return None
 
 def parse_args(doc, pa_dlna=True, argv=sys.argv[1:]):
-    """Parse the command line."""
+    """Parse the command line.
+
+    UPnP discovery is run on all the networks (except the loopbak interface
+    'lo') when the '--ip-addresses' and '--nics' command line arguments are
+    not used or empty. Otherwise both arguments may be used indifferently or
+    even jointly.
+    """
 
     def pack_B(ttl):
         try:
             ttl = int(ttl)
             return struct.pack('B', ttl)
         except (struct.error, ValueError) as e:
             parser.error(f"Bad 'ttl' argument: {e!r}")
@@ -98,26 +105,41 @@
             parser.error('The mime types in MIME-TYPES must be different')
         for mtype in mtypes:
             mtype_split = mtype.split('/')
             if len(mtype_split) != 2 or mtype_split[0] != 'audio':
                 parser.error(f"'{mtype}' is not an audio mime type")
         return mtypes
 
-    parser = argparse.ArgumentParser(description=doc)
+    def ipv4_addresses(ip_addresses):
+        ipv4_addrs = []
+        for addr in (x.strip() for x in ip_addresses.split(',')):
+            if addr:
+                try:
+                    ipaddress.IPv4Address(addr)
+                except ValueError as e:
+                    parser.error(e)
+                ipv4_addrs.append(addr)
+        return ipv4_addrs
+
+    parser = argparse.ArgumentParser(description=doc,
+                        epilog=' '.join(parse_args.__doc__.split('\n')[2:]))
     prog = 'pa-dlna' if pa_dlna else 'upnp-cmd'
     parser.prog = prog
     parser.add_argument('--version', '-v', action='version',
                         version='%(prog)s: version ' + __version__)
+    parser.add_argument('--ip-addresses', '-a', default='',
+                        type=ipv4_addresses,
+                        help='IP_ADDRESSES is a comma separated list of the'
+                        ' IPv4 addresses of the networks where UPnP devices'
+                        " may be discovered (default: '%(default)s')")
     parser.add_argument('--nics', '-n', default='',
                         help='NICS is a comma separated list of the names of'
                         ' network interface controllers where UPnP devices'
-                        " may be discovered, such as 'wlan0,enp5s0' for"
-                        ' example. All the interfaces are used when this'
-                        ' option is an empty string or the option is missing'
-                        " (default: '%(default)s')")
+                        " may be discovered such as 'wlan0,enp5s0' for"
+                        " example (default: '%(default)s')")
     parser.add_argument('--msearch-interval', '-m', type=int, default=60,
                         help='set the time interval in seconds between the'
                         ' sending of the MSEARCH datagrams used for device'
                         ' discovery (default: %(default)s)')
     parser.add_argument('--ttl', type=pack_B, default=b'\x02',
                         help='set the IP packets time to live to TTL'
                         ' (default: 2)')
@@ -138,15 +160,15 @@
                             help='set the log level of the stderr logging'
                             ' console (default: %(default)s)')
     parser.add_argument('--logfile', '-f', metavar='PATH',
                         help='add a file logging handler set at '
                         "'debug' log level whose path name is PATH")
     parser.add_argument('--nolog-upnp', '-u', action='store_true',
                         help="ignore UPnP log entries at 'debug' log level")
-    parser.add_argument('--log-aio', '-a', action='store_true',
+    parser.add_argument('--log-aio', '-y', action='store_true',
                         help='do not ignore asyncio log entries at'
                         " 'debug' log level; the default is to ignore those"
                         ' verbose logs')
     if pa_dlna:
         parser.add_argument('--test-devices', '-t', metavar='MIME-TYPES',
                             type=mime_types, default='',
                             help='MIME-TYPES is a comma separated list of'
@@ -167,14 +189,15 @@
         return options, None
 
     logfile_hdler = setup_logging(options)
     if options['logfile'] is not None and logfile_hdler is None:
         logging.shutdown()
         sys.exit(2)
 
+    logger.info('pa-dlna version ' + __version__)
     logger.info('Python version ' + sys.version)
     options['nics'] = [nic for nic in
                        (x.strip() for x in options['nics'].split(',')) if nic]
     logger.info(f'Options {options}')
     return options, logfile_hdler
 
 # Classes.
```

### Comparing `pa-dlna-0.4/pa_dlna/pa_dlna.py` & `pa-dlna-0.5/pa_dlna/pa_dlna.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 
 import sys
 import shutil
 import asyncio
 import logging
 import re
 import hashlib
-from ipaddress import IPv4Interface, IPv4Address
 from signal import SIGINT, SIGTERM
 from collections import namedtuple
 
 from .init import padlna_main, UPnPApplication, ControlPointAbortError
 from .pulseaudio import Pulse
 from .http_server import StreamSessions, HTTPServer
 from .encoders import select_encoder
 from .upnp import (UPnPControlPoint, UPnPClosedDeviceError,
-                   UPnPSoapFaultError, ipv4_addresses, NL_INDENT, shorten,
+                   UPnPSoapFaultError, NL_INDENT, shorten,
                    log_exception, AsyncioTasks, QUEUE_CLOSED)
 
 logger = logging.getLogger('pa-dlna')
 
 AUDIO_URI_PREFIX = '/audio-content'
 MEDIARENDERER = 'urn:schemas-upnp-org:device:MediaRenderer:'
 AVTRANSPORT = 'urn:upnp-org:serviceId:AVTransport'
@@ -62,17 +61,17 @@
 
     See the Standardized DCP (SDCP) specifications:
       'AVTransport:3 Service'
       'RenderingControl:3 Service'
       'ConnectionManager:3 Service'
     """
 
-    def __init__(self, control_point, local_ipaddress, root_device):
+    def __init__(self, control_point, root_device):
         self.control_point = control_point
-        self.local_ipaddress = local_ipaddress
+        self.local_ipaddress = root_device.local_ipaddress
         self.root_device = root_device
         udn_tail = root_device.udn[-5:]
         self.name = f'{root_device.modelName}-{udn_tail}'
         self.description = f'{root_device.friendlyName} - {udn_tail}'
         self.curtask = None             # Renderer.run() task
         self.closing = False
         self.nullsink = None            # NullSink instance
@@ -458,25 +457,25 @@
 
         def __init__(self, renderer, mime_type, control_point):
             self.control_point = control_point
             self.renderer = renderer
             self.mime_type = mime_type
             self.closed = True
             self.peer_ipaddress = self.LOOPBACK
+            self.local_ipaddress = self.LOOPBACK
 
             match = re.match(r'audio/([^;]+)', mime_type)
             name = match.group(1)
             self.modelName = f'DLNATest_{name}'
             self.friendlyName = self.modelName
             self.udn = get_udn(name.encode())
 
     def __init__(self, control_point, mime_type):
         root_device = self.RootDevice(self, mime_type, control_point)
-        super().__init__(control_point, root_device.peer_ipaddress,
-                         root_device)
+        super().__init__(control_point, root_device)
         self.mime_type = mime_type
 
     async def play(self, speed=1):
         pass
 
     async def soap_action(self, serviceId, action, args='unused'):
         if action == 'GetProtocolInfo':
@@ -628,35 +627,17 @@
 
             if notif == 'alive':
                 if self.upnp_control_point.is_disabled(root_device):
                     logger.debug(f'Ignore disabled {root_device}')
                     continue
 
                 if renderer is None:
-                    local_ipaddress = root_device.local_ipaddress
-
-                    # Find the local_ipaddress when processing a notify SSDP.
-                    # Check that the root device peer_ipaddress belongs to
-                    # one of the networks of our local network interfaces.
-                    if local_ipaddress is None:
-                        ip_addr = IPv4Address(root_device.peer_ipaddress)
-                        for obj in ipv4_addresses(self.nics, yield_str=False):
-                            if (isinstance(obj, IPv4Interface) and
-                                    ip_addr in obj.network):
-                                local_ipaddress = str(obj.ip)
-                                break
-                        else:
-                            logger.warning(
-                                f'Ignored: {root_device.peer_ipaddress} does'
-                                f' not belong to one of the known network'
-                                f' interfaces')
-                            continue
-
-                    renderer = Renderer(self, local_ipaddress, root_device)
-                    await self.register(renderer)
+                    if root_device.local_ipaddress is not None:
+                        renderer = Renderer(self, root_device)
+                        await self.register(renderer)
             else:
                 if renderer is not None:
                     await renderer.close()
                 else:
                     logger.warning("Got a 'byebye' notification for no"
                                    ' existing Renderer')
 
@@ -680,16 +661,17 @@
             self.cp_tasks.create_task(self.shutdown(end_event),
                                       name='shutdown')
             loop = asyncio.get_running_loop()
             for sig in (SIGINT, SIGTERM):
                 loop.add_signal_handler(sig, end_event.set)
 
             # Run the UPnP control point.
-            with UPnPControlPoint(self.nics, self.msearch_interval,
-                                  self.ttl) as self.upnp_control_point:
+            with UPnPControlPoint(
+                    self.ip_addresses, self.nics, self.msearch_interval,
+                    self.ttl) as self.upnp_control_point:
                 # Create the Pulse task.
                 self.pulse = Pulse(self)
                 self.cp_tasks.create_task(self.pulse.run(), name='pulse')
 
                 # Wait for the connection to PulseAudio to be ready.
                 await self.start_event.wait()
```

### Comparing `pa-dlna-0.4/pa_dlna/pulseaudio.py` & `pa-dlna-0.5/pa_dlna/pulseaudio.py`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/pa_dlna/tests/__init__.py` & `pa-dlna-0.5/pa_dlna/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/pa_dlna/tests/pulsectl.py` & `pa-dlna-0.5/pa_dlna/tests/pulsectl.py`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/pa_dlna/tests/streams.py` & `pa-dlna-0.5/pa_dlna/tests/streams.py`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/pa_dlna/tests/test_config.py` & `pa-dlna-0.5/pa_dlna/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     @property
     def available(self):
         if hasattr(self, '_available'):
             return self._available
         return True
 
     def set_args(self):
-        pass
+        raise NotImplementedError
 
 class StandAloneEncoder(Encoder):
     def __init__(self):
         super().__init__()
 
 class TestEncoder(StandAloneEncoder):
     def __init__(self):
@@ -123,14 +123,27 @@
                 mock.patch('builtins.open', mock.mock_open(
                     read_data=pa_dlna_conf)):
             cfg = UserConfig()
 
         self.assertEqual(cfg.encoders['TestEncoder'].__dict__,
                          {'args': 'command line: 2', 'option': 2})
 
+    def test_customize_args_option(self):
+        pa_dlna_conf = """
+        [FFMpegMp3Encoder]
+          bitrate = 320
+          args = foo
+        """
+
+        with mock.patch('builtins.open', mock.mock_open(
+                                                    read_data=pa_dlna_conf)):
+            cfg = UserConfig()
+
+        self.assertEqual(cfg.encoders['FFMpegMp3Encoder'].args, 'foo')
+
     def test_command_qscale(self):
         pa_dlna_conf = """
         [FFMpegMp3Encoder]
           bitrate = 0
           qscale = 2
         """
 
@@ -196,14 +209,17 @@
 
     def test_not_available(self):
         class UnAvailableEncoder(StandAloneEncoder):
             def __init__(self):
                 super().__init__()
                 self._available = False
 
+            def set_args(self):
+                pass
+
         with mock.patch('pa_dlna.config.encoders_module',
                         new=encoders_module(encoder=UnAvailableEncoder)),\
                 mock.patch('builtins.open', mock.mock_open()) as m_open,\
                 redirect_stdout(io.StringIO()) as output:
             m_open.side_effect = FileNotFoundError()
             cfg = UserConfig()
             cfg.print_internal_config()
```

### Comparing `pa-dlna-0.4/pa_dlna/tests/test_http_server.py` & `pa-dlna-0.5/pa_dlna/tests/test_http_server.py`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/pa_dlna/tests/test_init.py` & `pa-dlna-0.5/pa_dlna/tests/test_init.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Command line test cases."""
 
 import sys
 import os
 import io
 import struct
+import ipaddress
 import logging
 import unittest
 try:
     import termios
     import pty
 except ImportError:
     pass
@@ -97,24 +98,38 @@
 class Argv(BaseTestCase):
     """Command line tests."""
 
     def test_no_args(self):
         options, _ = parse_args(self.__doc__, argv=[])
         self.assertEqual(options, {'dump_default': False,
                                    'dump_internal': False,
+                                   'ip_addresses': [],
                                    'log_aio': False,
                                    'logfile': None,
                                    'loglevel': 'info',
                                    'msearch_interval': 60,
                                    'nics': [],
                                    'nolog_upnp': False,
                                    'port': 8080,
                                    'test_devices': [],
                                    'ttl': b'\x02'})
 
+    def test_ip_addresses(self):
+        options, _ = parse_args(self.__doc__,
+                                argv=['--ip-addresses', '192.168.0.1'])
+        self.assertEqual(options['ip_addresses'], ['192.168.0.1'])
+
+    def test_invalid_ip_addresses(self):
+        with self.assertRaises(SystemExit) as cm:
+            options, _ = parse_args(self.__doc__,
+                                argv=['--ip-addresses', '192.168.0.999'])
+        self.assertEqual(cm.exception.args[0], 2)
+        self.assertTrue(isinstance(cm.exception.__context__,
+                                   ipaddress.AddressValueError))
+
     def test_ttl(self):
         options, _ = parse_args(self.__doc__, argv=['--ttl', '255'])
         self.assertEqual(options['ttl'], b'\xff')
 
     def test_invalid_ttl(self):
         with self.assertRaises(SystemExit) as cm:
             options, _ = parse_args(self.__doc__, argv=['--ttl', '256'])
```

### Comparing `pa-dlna-0.4/pa_dlna/tests/test_pa_dlna.py` & `pa-dlna-0.5/pa_dlna/tests/test_pa_dlna.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,17 +104,17 @@
         # control_point.run_control_point() is cancelled by the Pulse task
         # closing the AVControlPoint instance 'control_point'.
         with mock.patch.object(Renderer,
                                'handle_pulse_event', handle_pulse_event),\
                 mock.patch.object(shutil, 'which', which),\
                 self.assertLogs(level=logging.DEBUG) as m_logs:
 
-            control_point = AVControlPoint(nics='lo', port=8080, ttl=2,
-                                           msearch_interval=60,
-                                           test_devices=test_devices)
+            control_point = AVControlPoint(ip_addresses=[], nics='lo',
+                                        port=8080, ttl=2, msearch_interval=60,
+                                        test_devices=test_devices)
             set_control_point(control_point)
             PulseAsync.add_sink_inputs([])
 
             try:
                 return_code = await wait_for(
                                         control_point.run_control_point())
             except asyncio.TimeoutError:
@@ -243,15 +243,16 @@
         self.assertTrue(search_in_logs(logs.output, 'pulse',
                         re.compile('Unload null-sink module DLNATest_foo')))
 
 class PatchGetNotificationTests(IsolatedAsyncioTestCase):
     """Test cases using patch_get_notification()."""
 
     def setUp(self):
-        self.upnp_control_point = UPnPControlPoint([], 60)
+        self.upnp_control_point = UPnPControlPoint(nics=[],
+                                                   msearch_interval=60)
         self.control_point = AVControlPoint(nics=['lo'], port=8080)
         self.control_point.upnp_control_point = self.upnp_control_point
 
         # PulseAsync must be instantiated after the call to the
         # add_sink_inputs() class method.
         PulseAsync.add_sink_inputs([])
         self.control_point.pulse = pulseaudio.Pulse(self.control_point)
@@ -362,37 +363,14 @@
                                                   ('alive', mpeg_root_device)
                                                   ],
                                                  alive_count=1)
 
         self.assertEqual(len(self.control_point.renderers), 1)
         self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
                                 re.compile('Ignore disabled UPnPRootDevice')))
-    async def test_local_ipaddress(self):
-        root_device = RootDevice(self.upnp_control_point)
-        root_device.local_ipaddress = None
-
-        logs = await self.patch_get_notification([('alive', root_device),],
-                                                 alive_count=1)
-
-        self.assertEqual(len(self.control_point.renderers), 1)
-        renderer = self.control_point.renderers.pop()
-        self.assertEqual(renderer.local_ipaddress, '127.0.0.1')
-
-    async def test_no_local_ipaddress(self):
-        root_device = RootDevice(self.upnp_control_point)
-        root_device.local_ipaddress = None
-        self.control_point.nics = ['an unknown network interface cards']
-
-        logs = await self.patch_get_notification([('alive', root_device),],
-                                                 alive_count=0)
-
-        self.assertEqual(len(self.control_point.renderers), 0)
-        self.assertTrue(find_in_logs(logs.output, 'pa-dlna',
-                'Ignored: 127.0.0.1 does not belong to one of the known'
-                ' network interfaces'))
 
 class PulseEventContext:
     """The context set before running handle_pulse_event() tests.
 
     The context is made of 'renderer', 'sink' and 'sink_input'.
     'sink' and 'sink_input' are either both None or both not None.
     In the last case, this is interpreted as a change of the pulseaudio state.
@@ -407,21 +385,21 @@
                  sink_input_proplist=None):
 
         is_index = isinstance(sink_input_index, int)
         assert (all((sink_state, is_index)) or
                 all((not sink_state, not is_index)))
 
         # Build the renderer.
-        upnp_control_point = UPnPControlPoint([], 60)
+        upnp_control_point = UPnPControlPoint(nics=[], msearch_interval=60)
         control_point = AVControlPoint()
         control_point.upnp_control_point = upnp_control_point
         _set_control_point(control_point)
 
         root_device = RootDevice(upnp_control_point)
-        self.renderer = Renderer(control_point, None, root_device)
+        self.renderer = Renderer(control_point, root_device)
         self.renderer.previous_idx = previous_idx
 
         # Set the value of Renderer.nullsink.
         prev_sink = Sink(prev_sink_state)
         nullsink = pulseaudio.NullSink(prev_sink)
         if prev_sink_input_index is not None:
             nullsink.sink_input = SinkInput(prev_sink_input_index)
```

### Comparing `pa-dlna-0.4/pa_dlna/tests/test_pulseaudio.py` & `pa-dlna-0.5/pa_dlna/tests/test_pulseaudio.py`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/pa_dlna/upnp/network.py` & `pa-dlna-0.5/pa_dlna/upnp/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,29 +33,39 @@
         f'',
         ])
 
 class UPnPInvalidSsdpError(UPnPError): pass
 class UPnPInvalidHttpError(UPnPError): pass
 
 # Networking helper functions.
-def ipv4_addresses(ifaces, yield_str=True):
-    """Yield IPv4 addresses on 'ifaces' network interface cards.
+def ipaddr_from_nics(nics, skip_loopback=False, as_string=True):
+    """Yield the IPv4 addresses of NICS in the UP state.
 
-    Use all existing network interface cards when 'ifaces' is empty.
+    Use all existing network interface when 'nics' is empty, except the
+    loopback interface when 'skip_loopback' is true.
     """
 
-    nics = psutil.net_if_addrs()
-    for nic in filter(lambda x: not ifaces or x in ifaces, nics):
-        for addr in filter(lambda x: x.family == socket.AF_INET, nics[nic]):
+    # Get the IP addresses of each NIC in the UP state.
+    all_nics = {}
+    nics_stats = psutil.net_if_stats()
+    for nic, val in psutil.net_if_addrs().items():
+        if nic in nics_stats and nics_stats[nic].isup:
+            all_nics[nic] = val
+
+    for nic in filter(lambda x:
+                      not nics and (not skip_loopback or x != 'lo') or
+                      x in nics, all_nics):
+        for addr in filter(lambda x:
+                           x.family == socket.AF_INET, all_nics[nic]):
             if addr.netmask is not None:
-                ipadd = IPv4Interface(f'{addr.address}/{addr.netmask}')
-                if ipadd.network.prefixlen != 32:
-                    yield addr.address if yield_str else ipadd
+                ip_addr = IPv4Interface(f'{addr.address}/{addr.netmask}')
+                if ip_addr.network.prefixlen != 32:
+                    yield addr.address if as_string else ip_addr
             else:
-                yield addr.address if yield_str else IPv4Address(addr.address)
+                yield addr.address if as_string else IPv4Address(addr.address)
 
 def http_header_as_dict(header):
     """Return the http header as a dict."""
 
     def normalize(args):
         """Return a normalized (key, value) tuple."""
         return args[0].strip().upper(), args[1].strip()
@@ -198,21 +208,21 @@
 
 async def http_query(method, url, header='', body=''):
     """An HTTP 1.0 GET or POST request."""
 
     assert method in ('GET', 'POST')
     writer = None
     try:
-        url = urllib.parse.urlsplit(url)
-        host = url.hostname
-        port = url.port if url.port is not None else 80
+        urlobj = urllib.parse.urlsplit(url)
+        host = urlobj.hostname
+        port = urlobj.port if urlobj.port is not None else 80
         reader, writer = await asyncio.open_connection(host, port)
 
         # Send the request.
-        request = url._replace(scheme='')._replace(netloc='').geturl()
+        request = urlobj._replace(scheme='')._replace(netloc='').geturl()
         query = (
             f"{method} {request or '/'} HTTP/1.0\r\n"
             f"Host: {host}:{port}\r\n"
         )
         query = query + header + '\r\n'
         writer.write(query.encode('latin-1'))
         writer.write(body.encode())
@@ -234,24 +244,27 @@
             raise UPnPInvalidHttpError(f'Empty http header from {host}')
 
         header_dict = http_header_as_dict(header[1:])
         content_length = header_dict.get('CONTENT-LENGTH')
         if content_length is not None:
             content_length = int(content_length)
             if content_length == 0:
+                logger.warning(f'Got content_length = 0 from {url}')
                 return header, b'', host
 
         body = await reader.read()
 
         # Check that we have received the whole body.
         if content_length is not None:
             if len(body) != content_length:
                 raise UPnPInvalidHttpError(f'Content-Length and actual length'
                                 f' mismatch ({content_length} != {len(body)})'
                                 f' from {host}')
+        if not body:
+            logger.warning(f'Got empty body from {url}')
         return header, body, host
 
     finally:
         if writer is not None:
             writer.close()
             await writer.wait_closed()
 
@@ -294,25 +307,24 @@
         self.process_datagram = process_datagram
         self.failed_memberships = set()
 
         # Create the socket.
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self.sock.setblocking(False)
 
-        self.ip_addresses = set()
         self.manage_membership(ip_addresses)
 
         # Future used by the test suite.
         loop = asyncio.get_running_loop()
         self.startup = loop.create_future()
 
     def close(self):
         self.sock.close()
 
-    def manage_membership(self, ip_addresses):
+    def manage_membership(self, new_ips, stale_ips=None):
         def member(ip, option):
             msg = ('member of' if option == socket.IP_ADD_MEMBERSHIP else
                    'dropped from')
             try:
                 mreq = struct.pack('4s4s', socket.inet_aton(MCAST_GROUP),
                                    socket.inet_aton(ip))
                 self.sock.setsockopt(socket.IPPROTO_IP, option, mreq)
@@ -327,21 +339,20 @@
                         ip not in self.failed_memberships):
                     logger.warning(f'SSDP notify: {ip} cannot be {msg}'
                                    f' {MCAST_GROUP}: {e!r}')
                     self.failed_memberships.add(ip)
                 return False
             return True
 
-        for ip in ip_addresses.difference(self.ip_addresses):
-            if member(ip, socket.IP_ADD_MEMBERSHIP):
-                self.ip_addresses.add(ip)
-
-        for ip in self.ip_addresses.difference(ip_addresses):
-            if member(ip, socket.IP_DROP_MEMBERSHIP):
-                self.ip_addresses.remove(ip)
+        for ip in new_ips:
+            member(ip, socket.IP_ADD_MEMBERSHIP)
+
+        if stale_ips is not None:
+            for ip in stale_ips:
+                member(ip, socket.IP_DROP_MEMBERSHIP)
 
     async def run(self):
         # Allow other processes to bind to the same multicast group and port.
         self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
         # Bind to the multicast (group, port).
         # Binding to (INADDR_ANY, port) would also work, except
@@ -424,12 +435,12 @@
             self.process_datagram(data, addr[0], None)
         except Exception as exc:
             if not self.on_con_lost.done():
                 self.on_con_lost.set_result(True)
             self.error_received(exc)
 
     def error_received(self, exc):
-        logger.error(f'Error received by NotifyServerProtocol: {exc!r}')
+        logger.exception(f'Error received by NotifyServerProtocol: {exc!r}')
 
     def connection_lost(self, exc):
         if exc:
             logger.warning(f'Connection lost by NotifyServerProtocol: {exc!r}')
```

### Comparing `pa-dlna-0.4/pa_dlna/upnp/tests/__init__.py` & `pa-dlna-0.5/pa_dlna/upnp/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             if mock.called:
                 return True
 
     if asyncio.iscoroutinefunction(datagrams):
         coro = datagrams
     else:
         coro = send_datagrams
-    control_point = UPnPControlPoint(['lo'], 3600)
+    control_point = UPnPControlPoint(nics=['lo'], msearch_interval=3600)
     with mock.patch.object(control_point,
                            '_ssdp_msearch') as ssdp_msearch:
         if patch_method is not None:
             patcher = mock.patch.object(control_point, patch_method)
             method = patcher.start()
 
         # Prevent the msearch task to run UPnPControlPoint._ssdp_msearch.
```

### Comparing `pa-dlna-0.4/pa_dlna/upnp/tests/device_resps.py` & `pa-dlna-0.5/pa_dlna/upnp/tests/device_resps.py`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/pa_dlna/upnp/tests/test_network.py` & `pa-dlna-0.5/pa_dlna/upnp/tests/test_network.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Network test cases."""
 
 import re
 import asyncio
+import psutil
 import logging
 import socket
-from unittest import IsolatedAsyncioTestCase, mock
+from collections import namedtuple
+from ipaddress import IPv4Address
+from unittest import TestCase, IsolatedAsyncioTestCase, mock
+
+from ..network import ipaddr_from_nics
 
 # Load the tests in the order they are declared.
 from . import load_ordered_tests as load_tests
 
 from . import (find_in_logs, search_in_logs, loopback_datagrams, URL,
                MSEARCH_PORT, HOST, HTTP_PORT, SSDP_PARAMS, SSDP_NOTIFY,
                SSDP_ALIVE)
@@ -34,24 +39,29 @@
 NOT_FOUND_REASON = 'A dummy reason'
 NOT_FOUND = '\r\n'.join([
     f'HTTP/1.1 404 {NOT_FOUND_REASON}',
     'Content-Length: 0',
     '', '',
 ])
 
+# A shortened psutil address.
+snicaddr = namedtuple('snicaddr', ['address', 'netmask', 'family'],
+                      defaults=[socket.AF_INET])
+snicstats = namedtuple('snicstats', ['isup'])
+NICS_STAT = {'lo': snicstats(True)}
+
 class HTTPServer:
     def __init__(self, body, content_length=None, start_line=None):
         self.body = body.encode()
         self.body_length = len(self.body)
-        content_length = (self.body_length if content_length is None else
-                          content_length)
 
         header = ['HTTP/1.1 200 OK' if start_line is None else
                   start_line]
-        header.append(f'Content-Length: {content_length}')
+        if content_length is not None:
+            header.append(f'Content-Length: {content_length}')
         header.extend(['', ''])
         self.header = '\r\n'.join(header).encode('latin-1')
 
         loop = asyncio.get_running_loop()
         self.startup = loop.create_future()
 
     async def client_connected(self, reader, writer):
@@ -75,14 +85,70 @@
     async def run(self):
         aio_server = await asyncio.start_server(self.client_connected,
                                                 HOST, HTTP_PORT)
         async with aio_server:
             self.startup.set_result(None)
             await aio_server.serve_forever()
 
+class AddrFromNics(TestCase):
+    """network.ipaddr_from_nics() tests."""
+
+    def test_cfg_skip_loopback_true(self):
+        # Test that '127.0.0.1' is returned when 'lo' is configured, even
+        # though 'skip_loopback' is true.
+        nics_addr = {'lo': [snicaddr('127.0.0.1', '255.0.0.0')]}
+        with mock.patch.object(psutil,'net_if_addrs') as net_if_addrs,\
+                mock.patch.object(psutil, 'net_if_stats') as net_if_stats:
+            net_if_addrs.return_value = nics_addr
+            net_if_stats.return_value = NICS_STAT
+            result = list(ipaddr_from_nics(['lo'], skip_loopback=True))
+            self.assertEqual(result, ['127.0.0.1'])
+
+    def test_cfg_skip_loopback_false(self):
+        # Test that '127.0.0.1' is returned when 'lo' is not configured
+        # and 'skip_loopback' is false.
+        nics_addr = {'lo': [snicaddr('127.0.0.1', '255.0.0.0')]}
+        with mock.patch.object(psutil,'net_if_addrs') as net_if_addrs,\
+                mock.patch.object(psutil, 'net_if_stats') as net_if_stats:
+            net_if_stats.return_value = NICS_STAT
+            net_if_addrs.return_value = nics_addr
+            result = list(ipaddr_from_nics(['lo'], skip_loopback=False))
+            self.assertEqual(result, ['127.0.0.1'])
+
+    def test_nocfg_skip_loopback_true(self):
+        # Test that '127.0.0.1' is ignored when 'lo' is not configured
+        # and 'skip_loopback' is true.
+        nics_addr = {'lo': [snicaddr('127.0.0.1', '255.0.0.0')]}
+        with mock.patch.object(psutil,'net_if_addrs') as net_if_addrs,\
+                mock.patch.object(psutil, 'net_if_stats') as net_if_stats:
+            net_if_stats.return_value = NICS_STAT
+            net_if_addrs.return_value = nics_addr
+            result = list(ipaddr_from_nics([], skip_loopback=True))
+            self.assertEqual(result, [])
+
+    def test_nocfg_skip_loopback_false(self):
+        # Test that '127.0.0.1' is returned when 'lo' is not configured
+        # and 'skip_loopback' is false.
+        nics_addr = {'lo': [snicaddr('127.0.0.1', '255.0.0.0')]}
+        with mock.patch.object(psutil,'net_if_addrs') as net_if_addrs,\
+                mock.patch.object(psutil, 'net_if_stats') as net_if_stats:
+            net_if_addrs.return_value = nics_addr
+            net_if_stats.return_value = NICS_STAT
+            result = list(ipaddr_from_nics([], skip_loopback=False))
+            self.assertEqual(result, ['127.0.0.1'])
+
+    def test_no_netmask(self):
+        nics_addr = {'lo': [snicaddr('127.0.0.1', None)]}
+        with mock.patch.object(psutil,'net_if_addrs') as net_if_addrs,\
+                mock.patch.object(psutil, 'net_if_stats') as net_if_stats:
+            net_if_addrs.return_value = nics_addr
+            net_if_stats.return_value = NICS_STAT
+            result = list(ipaddr_from_nics(['lo'], as_string=False))
+            self.assertEqual(result, [IPv4Address('127.0.0.1')])
+
 class SSDP_notify(IsolatedAsyncioTestCase):
     """SSDP notify test cases.
 
     These tests use the fact that multicast datagrams sent to the loopback
     interface are looped back to the notify task.
     """
 
@@ -264,16 +330,28 @@
         body = 'Some content.'
         received_body = await self._loopback_get(body)
 
         self.assertEqual(body, received_body.decode())
 
     async def test_zero_length(self):
         body = 'Some content.'
-        received_body = await self._loopback_get(body, content_length=0)
+        with self.assertLogs(level=logging.DEBUG) as m_logs:
+            received_body = await self._loopback_get(body, content_length=0)
 
+        self.assertTrue(search_in_logs(m_logs.output, 'network',
+                                       re.compile('Got content_length = 0')))
+        self.assertEqual(received_body, b'')
+
+    async def test_empty_body(self):
+        body = ''
+        with self.assertLogs(level=logging.DEBUG) as m_logs:
+            received_body = await self._loopback_get(body)
+
+        self.assertTrue(search_in_logs(m_logs.output, 'network',
+                                       re.compile('Got empty body')))
         self.assertEqual(received_body, b'')
 
     async def test_length_mismatch(self):
         body = 'Some content.'
         with self.assertRaises(UPnPInvalidHttpError) as cm:
             received_body = await self._loopback_get(body, content_length=1)
```

### Comparing `pa-dlna-0.4/pa_dlna/upnp/tests/test_upnp.py` & `pa-dlna-0.5/pa_dlna/upnp/tests/test_upnp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """UPnP test cases."""
 
 import re
 import asyncio
+import psutil
 import logging
 import urllib
 from unittest import mock, IsolatedAsyncioTestCase
 
 # Load the tests in the order they are declared.
 from . import load_ordered_tests as load_tests
 
 from . import (loopback_datagrams, find_in_logs, search_in_logs, UDN, HOST,
                HTTP_PORT, SSDP_NOTIFY, SSDP_PARAMS, SSDP_ALIVE, URL,
                bind_mcast_address)
+from .test_network import snicaddr, snicstats
 from .device_resps import device_description, scpd, soap_response, soap_fault
 from ..util import HTTPRequestHandler, shorten
 from ..upnp import (UPnPControlPoint, UPnPRootDevice, UPnPService,
                     UPnPSoapFaultError, UPnPClosedDeviceError)
 from ..xml import UPnPXMLError
 
 SSDP_BYEBYE = SSDP_NOTIFY.format(nts='NTS: ssdp:byebye', **SSDP_PARAMS)
@@ -210,76 +212,99 @@
     async def test_close(self):
         async def is_called(mock):
             while True:
                 await asyncio.sleep(0)
                 if mock.called:
                     return True
 
-        control_point = UPnPControlPoint(['lo'], 3600)
+        control_point = UPnPControlPoint(nics=['lo'], msearch_interval=3600)
         with mock.patch.object(UPnPControlPoint, 'msearch_once') as msearch,\
                 self.assertLogs(level=logging.DEBUG) as m_logs:
             msearch.side_effect = OSError('FOO')
             control_point.open()
             await asyncio.wait_for(is_called(msearch), 1)
 
         self.assertTrue(search_in_logs(m_logs.output, 'upnp',
                                        re.compile("OSError\('FOO'\)")))
         self.assertTrue(find_in_logs(m_logs.output, 'upnp',
                                      'Close UPnPControlPoint'))
 
     @bind_mcast_address()
-    async def test_ssdp_race(self):
+    async def test_local_ip_address(self):
         header = { 'LOCATION': URL }
-        control_point = UPnPControlPoint(['lo'], 3600)
-        with mock.patch.object(control_point, '_put_notification') as notify,\
+        control_point = UPnPControlPoint(nics=['lo'], msearch_interval=3600)
+        with mock.patch.object(control_point, '_put_notification'),\
                 self.assertLogs(level=logging.DEBUG) as m_logs:
             await start_http_server()
             # The SSDP notification.
-            control_point._create_root_device(header, UDN, HOST, False, None)
-            # The SSDP msearch.
-            control_point._create_root_device(header, UDN, HOST, True, HOST)
-
-        root_device = control_point._devices[UDN]
-        notify.assert_called_with('alive', root_device)
-        self.assertEqual(root_device.local_ipaddress, HOST)
-
-    @bind_mcast_address()
-    async def test_ssdp_no_race(self):
-        header = { 'LOCATION': URL }
-        control_point = UPnPControlPoint(['lo'], 3600)
-        with mock.patch.object(control_point, '_put_notification') as notify,\
-                self.assertLogs(level=logging.DEBUG) as m_logs:
-            await start_http_server()
-            # The SSDP notification.
-            control_point._create_root_device(header, UDN, HOST, False, None)
-
+            # Using '192.168.0.1' instead of HOST to prevent the root device
+            # local_ipaddress to be found by matching the network of 'lo'.
+            control_point._create_root_device(header, UDN, '192.168.0.1',
+                                              False, None)
             root_device = control_point._devices[UDN]
-            with mock.patch.object(root_device, '_age_root_device') as age:
-                 # Make the UPnPRootDevice._run() coroutine terminate.
-                age.side_effect = [None]
-                for task in control_point._upnp_tasks:
-                    if task.get_name() == str(root_device):
-                        break
-                else:
-                    raise AssertionError(f'Root device task {root_device}'
-                                         ' not found')
-                await task
+            self.assertEqual(root_device.local_ipaddress, None)
 
-            # The SSDP msearch.
+            # The SSDP msearch provides the local_ipaddress.
             control_point._create_root_device(header, UDN, HOST, True, HOST)
-            notify.assert_called()
+            self.assertEqual(root_device.local_ipaddress, HOST)
 
-        self.assertEqual(root_device.local_ipaddress, HOST)
+    def test_update_ip_addresses(self):
+        init_nics = {
+            'eth0': [snicaddr('192.168.0.1', '255.255.255.0')],
+            'eth1': [snicaddr('192.168.1.1', '255.255.255.0')],
+        }
+        next_nics = {
+            'eth0': [snicaddr('192.168.0.1', '255.255.255.0')],
+            'wlan2': [snicaddr('192.168.2.1', '255.255.255.0')],
+        }
+        nics_stat = {
+            'eth0': snicstats(True),
+            'eth1': snicstats(True),
+            'wlan2': snicstats(True),
+        }
+        with mock.patch.object(psutil,'net_if_addrs') as net_if_addrs,\
+                mock.patch.object(psutil, 'net_if_stats') as net_if_stats:
+            net_if_addrs.side_effect = [init_nics, init_nics,
+                                        next_nics, next_nics]
+            net_if_stats.side_effect = [nics_stat, nics_stat,
+                                        nics_stat, nics_stat]
+            control_point = UPnPControlPoint(ip_addresses=['192.168.1.1'],
+                                             nics=['eth0', 'wlan2'])
+            new_ips, stale_ips = control_point._update_ip_addresses()
+            self.assertEqual(new_ips, {'192.168.2.1'})
+            self.assertEqual(stale_ips, {'192.168.1.1'})
+
+    @bind_mcast_address()
+    async def test_stale_ip_address(self):
+        ip = '192.168.0.1'
+        nics = {'eth0': [snicaddr(ip, '255.255.255.0')]}
+        nics_stat = {'eth0': snicstats(True)}
+        next_nics_stat = {'eth0': snicstats(False)}
+        with mock.patch.object(psutil,'net_if_addrs') as net_if_addrs,\
+                mock.patch.object(psutil, 'net_if_stats') as net_if_stats:
+            net_if_addrs.side_effect = [nics, nics]
+            net_if_stats.side_effect = [nics_stat, next_nics_stat]
+            control_point = UPnPControlPoint(nics=['eth0'])
+
+            header = { 'LOCATION': URL }
+            with mock.patch.object(control_point, '_put_notification'),\
+                    self.assertLogs(level=logging.DEBUG) as m_logs:
+                await start_http_server()
+                control_point._create_root_device(header, UDN, ip, True, ip)
+                self.assertTrue(UDN in control_point._devices)
+                await control_point.msearch_once(None, do_msearch=False)
+                self.assertTrue(UDN not in control_point._devices)
 
 @bind_mcast_address()
 class RootDevice(IsolatedAsyncioTestCase):
     """Root device test cases."""
 
     def setUp(self):
-        self.control_point = UPnPControlPoint(['lo'], 3600)
+        self.control_point = UPnPControlPoint(nics=['lo'],
+                                              msearch_interval=3600)
         self.root_device = UPnPRootDevice(self.control_point, UDN, HOST, HOST,
                                           URL, 1800)
 
     async def test_OSError(self):
         exc = OSError('FOO')
         with self.assertLogs(level=logging.DEBUG) as m_logs,\
                 mock.patch.object(self.root_device,
```

### Comparing `pa-dlna-0.4/pa_dlna/upnp/tests/test_util.py` & `pa-dlna-0.5/pa_dlna/upnp/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/pa_dlna/upnp/tests/test_xml.py` & `pa-dlna-0.5/pa_dlna/upnp/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/pa_dlna/upnp/upnp.py` & `pa-dlna-0.5/pa_dlna/upnp/upnp.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 The library does not have any external dependency.
 Here is an example of using the Control Point. Allow it a few seconds to
 discover an UPnP device on the 'enp0s31f6' ethernet interface.
 
 >>> import asyncio
 >>> import upnp
 >>>
->>> async def main(nics, interval):
-...   with upnp.UPnPControlPoint(nics, interval) as control_point:
+>>> async def main(nics):
+...   with upnp.UPnPControlPoint(nics=nics) as control_point:
 ...     notification, root_device = await control_point.get_notification()
 ...     print(f"  Got '{notification}' from {root_device.peer_ipaddress}")
 ...     print(f'  deviceType: {root_device.deviceType}')
 ...     print(f'  friendlyName: {root_device.friendlyName}')
 ...     for service in root_device.serviceList.values():
 ...       print(f'    serviceId: {service.serviceId}')
 ...
 >>> try:
-...   asyncio.run(main(['enp0s31f6'], 10))
+...   asyncio.run(main(['enp0s31f6']))
 ... except KeyboardInterrupt:
 ...   pass
 ...
   Got 'alive' from 192.168.0.212
   deviceType: urn:schemas-upnp-org:device:MediaRenderer:1
   friendlyName: Yamaha RN402D
     serviceId: urn:upnp-org:serviceId:AVTransport
@@ -45,20 +45,21 @@
 
 import asyncio
 import sys
 import logging
 import time
 import collections
 import urllib.parse
+from ipaddress import IPv4Interface, IPv4Address
 from signal import SIGINT, SIGTERM, strsignal
 
 from . import UPnPError, TEST_LOGLEVEL
 from .util import NL_INDENT, shorten, log_exception, AsyncioTasks
-from .network import (ipv4_addresses, parse_ssdp, msearch, send_mcast, Notify,
-                      http_get, http_soap)
+from .network import (ipaddr_from_nics, parse_ssdp, msearch, send_mcast,
+                      Notify, http_get, http_soap)
 from .xml import (upnp_org_etree, build_etree, xml_of_subelement,
                   findall_childless, scpd_actionlist, scpd_servicestatetable,
                   dict_to_xml, parse_soap_response, parse_soap_fault,
                   UPnPXMLError)
 
 logger = logging.getLogger('upnp')
 
@@ -490,16 +491,20 @@
         return f'UPnPRootDevice {shorten(self.udn)}'
 
 # UPnP control point.
 class UPnPControlPoint:
     """An UPnP control point.
 
     Attributes:
+      ip_configured List of the IPv4 addresses of the networks where UPnP
+                    devices may be discovered.
       nics          List of the network interfaces where UPnP devices may be
                     discovered.
+      ip_monitored  List of the IPv4 addresses currently monitored by UPnP
+                    discovery.
       msearch_interval
                     The time interval in seconds between the sending of the
                     MSEARCH datagrams used for device discovery.
       ttl           The IP packets time to live.
 
     Methods:
       open          Coroutine - start the UPnP Control Point.
@@ -510,53 +515,57 @@
       get_notification
                     Coroutine - return a notification and the corresponding
                     UPnPRootDevice instance.
       __enter__     UPnPControlPoint supports the context manager protocol.
       __close__
     """
 
-    def __init__(self, nics, msearch_interval, ttl=2):
+    def __init__(self, ip_addresses=[], nics=[], msearch_interval=60, ttl=2):
+        self.ip_configured = ip_addresses
         self.nics = nics
         self.msearch_interval = msearch_interval
         self.ttl = ttl
 
+        # Get the list of active IPv4 addresses used for UPnP discovery.
+        self.ip_monitored = set()
+        self._update_ip_addresses()
+
         self._closed = False
         self._notify = None
         self._upnp_queue = asyncio.Queue()
         self._devices = {}              # {udn: UPnPRootDevice}
         self._faulty_devices = set()    # set of the udn of root devices
                                         # permanently disabled
-        self.msearch_task = None
-        self.notify_task = None
+        self._msearch_task = None
+        self._notify_task = None
         self._upnp_tasks = AsyncioTasks()
 
     def open(self):
         """Start the UPnP Control Point."""
 
         # Start the msearch task.
-        self.msearch_task = self._upnp_tasks.create_task(self._ssdp_msearch(),
-                                                         name='ssdp msearch')
+        self._msearch_task = self._upnp_tasks.create_task(
+                                    self._ssdp_msearch(), name='ssdp msearch')
 
         # Start the notify task.
-        self._notify = Notify(self._process_ssdp,
-                              set(ipv4_addresses(self.nics)))
-        self.notify_task = self._upnp_tasks.create_task(self._ssdp_notify(),
+        self._notify = Notify(self._process_ssdp, self.ip_monitored)
+        self._notify_task = self._upnp_tasks.create_task(self._ssdp_notify(),
                                                         name='ssdp notify')
 
     def close(self):
         """Close the UPnP Control Point."""
 
         if not self._closed:
             self._closed = True
 
             self._put_notification(*QUEUE_CLOSED)
-            if self.msearch_task is not None:
-                self.msearch_task.cancel()
-            if self.notify_task is not None:
-                self.notify_task.cancel()
+            if self._msearch_task is not None:
+                self._msearch_task.cancel()
+            if self._notify_task is not None:
+                self._notify_task.cancel()
                 self._notify.close()
 
             for root_device in list(self._devices.values()):
                 root_device.close()
 
             logger.info('Close UPnPControlPoint')
 
@@ -605,14 +614,25 @@
                 logger.warning(
                     f'Invalid CACHE-CONTROL field in'
                     f' SSDP notify from {peer_ipaddress}:\n{header}')
                 return
 
         if udn not in self._devices:
             # Instantiate the UPnPDevice and start its task.
+            if local_ipaddress is None:
+                ip_addr = IPv4Address(peer_ipaddress)
+                for obj in ipaddr_from_nics(self.nics, as_string=False):
+                    if (isinstance(obj, IPv4Interface) and
+                            ip_addr in obj.network):
+                        local_ipaddress = str(obj.ip)
+                        break
+                else:
+                    logger.info(f'{peer_ipaddress} does not belong to one'
+                                f' of the known network interfaces')
+
             root_device = UPnPRootDevice(self, udn, peer_ipaddress,
                                 local_ipaddress, header['LOCATION'], max_age)
             self._upnp_tasks.create_task(root_device._run(),
                                          name=str(root_device))
             self._devices[udn] = root_device
 
         else:
@@ -648,19 +668,43 @@
             root_device.close()
             logger.debug(f'{root_device} has been deleted')
             self._put_notification('byebye', root_device)
 
         if exc is not None:
             self.disable_root_device(root_device)
 
+    def _update_ip_addresses(self):
+        """Set the new IPv4 addresses set."""
+
+        current_ips = set()
+        if self.ip_configured:
+            all_ips = list(ipaddr_from_nics(nics=[]))
+            for ip in self.ip_configured:
+                if ip in all_ips:
+                    current_ips.add(ip)
+
+        if self.nics or not self.ip_configured:
+            for ip in ipaddr_from_nics(nics=self.nics, skip_loopback=True):
+                current_ips.add(ip)
+
+        new_ips = current_ips.difference(self.ip_monitored)
+        if new_ips:
+            logger.info(f'Start UPnP discovery on new IPs {new_ips}')
+        stale_ips =  self.ip_monitored.difference(current_ips)
+        if stale_ips:
+            logger.info(f'Stop UPnP discovery on stale IPs {stale_ips}')
+        self.ip_monitored = current_ips
+
+        return new_ips, stale_ips
+
     def _process_ssdp(self, datagram, peer_ipaddress, local_ipaddress):
         """Process the received datagrams."""
 
         if (local_ipaddress is not None and local_ipaddress not in
-                                                ipv4_addresses(self.nics)):
+                                                self.ip_monitored):
             logger.warning(
                 f'Ignore msearch SSDP received on {local_ipaddress}')
             return
 
         logger.log(TEST_LOGLEVEL, datagram.decode())
 
         # 'is_msearch' is True when processing a msearch response,
@@ -688,22 +732,31 @@
                 logger.warning(f'Ignore not supported {nts} notification'
                                f' from {peer_ipaddress}')
 
             else:
                 logger.warning(f"Unknown NTS field '{nts}' in SSDP notify"
                                ' from {peer_ipaddress}')
 
-    async def msearch_once(self, coro, port=None):
-        ip_addresses = set(ipv4_addresses(self.nics))
+    async def msearch_once(self, coro, port=None, do_msearch=True):
+        new_ips, stale_ips = self._update_ip_addresses()
+
+        for ip in stale_ips:
+            for root_device in self._devices.values():
+                if ip == root_device.local_ipaddress:
+                    root_device.close()
+                    break
 
-        # Update the notify task with the ip addresses.
+        # Update the notify task with the new and stale sets.
         if self._notify is not None:
-            self._notify.manage_membership(ip_addresses)
+            self._notify.manage_membership(new_ips, stale_ips)
+
+        if not do_msearch and not new_ips:
+            return
 
-        for ip_addr in ip_addresses:
+        for ip_addr in self.ip_monitored:
             # 'coro' is a coroutine *function*.
             result = await send_mcast(ip_addr, port=port, ttl=self.ttl,
                                       coro=coro)
             if result:
                 for (data, peer_addr, local_addr) in result:
                     self._process_ssdp(data, peer_addr, local_addr)
             else:
@@ -712,17 +765,24 @@
                              f' {self.msearch_interval} seconds')
 
     @log_exception(logger)
     async def _ssdp_msearch(self, coro=msearch):
         """Send msearch multicast SSDPs and process unicast responses."""
 
         try:
+            last_time = -1
             while True:
-                await self.msearch_once(coro)
-                await asyncio.sleep(self.msearch_interval)
+                do_msearch = False
+                cur_time = time.time()
+                if (last_time == -1 or
+                        cur_time - last_time >= self.msearch_interval):
+                    do_msearch = True
+                    last_time = cur_time
+                await self.msearch_once(coro, do_msearch=do_msearch)
+                await asyncio.sleep(1)
         except asyncio.CancelledError:
             pass
         except Exception as e:
             logger.exception(f'{e!r}')
         finally:
             self.close()
```

### Comparing `pa-dlna-0.4/pa_dlna/upnp/util.py` & `pa-dlna-0.5/pa_dlna/upnp/util.py`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/pa_dlna/upnp/xml.py` & `pa-dlna-0.5/pa_dlna/upnp/xml.py`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/pa_dlna/upnp_cmd.py` & `pa-dlna-0.5/pa_dlna/upnp_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     for key, value in vars(obj).items():
         if key.startswith('_') or key in exclude:
             continue
         funcname = f'do_{key}'
         if not hasattr(instance, funcname):
             setattr(instance, funcname, DoMethod(print, value,
-                                            f"Print the value of '{key}'"))
+                                            f"Print the value of '{key}'."))
 
 def check_required(obj, attributes):
     """Check that all in 'attributes' are attributes of 'obj'."""
 
     for name in attributes:
         if not hasattr(obj, name):
             msg = ''
@@ -135,15 +135,15 @@
             print()
         except Exception as e:
             print(f'*** {e!r}')
         else:
             return  dev
 
     def do_EOF(self, unused):
-        """Quit the application"""
+        """Quit the application."""
         print()
         return self.do_quit(unused)
 
     def get_names(self):
         return dir(self)
 
     def do_help(self, arg):
@@ -232,37 +232,37 @@
             funcname = f'do_{action}'
             setattr(self, funcname, DoMethod(self.soap_action, action))
 
         self.prompt = f'[{str(self.upnp_service)}] '
         self.quit = False
 
     def do_quit(self, unused):
-        """Quit the application"""
+        """Quit the application."""
 
         # Tell cmdloop() to return True.
         self.quit = True
         # Stop the current interpreter and return to the previous one.
         return True
 
     def do_previous(self, unused):
-        """Return to the device"""
+        """Return to the device."""
         return True
 
     def help_parent_device(self):
-        print('Shortened UDN of the parent device')
+        print('Shortened UDN of the parent device.')
 
     def do_description(self, unused):
-        """Print the xml 'description'"""
+        """Print the xml 'description'."""
         print(pformat_xml(self.upnp_service.description))
 
     def help_root_device(self):
-        print('Shortened UDN of the root device')
+        print('Shortened UDN of the root device.')
 
     def help_actionList(self):
-        print(_dedent("""Print an action or list actions
+        print(_dedent("""Print an action or list actions.
 
         With a numeric argument such as 'actionList DEPTH':
           When DEPTH is 1, print the list of the actions.
           When DEPTH is 2, print the list of the actions with their arguments.
           When DEPTH is 3, print the list of the actions with their arguments
             and the values of 'direction' and 'relatedStateVariable' for each
             argument.
@@ -296,15 +296,15 @@
             try:
                 action = {arg: self.upnp_service.actionList[arg]}
                 pprint_pprint(action)
             except KeyError:
                 print(f"*** '{arg}' is not an action")
 
     def help_serviceStateTable(self):
-        print(_dedent("""Print a stateVariable or list the stateVariables
+        print(_dedent("""Print a stateVariable or list the stateVariables.
 
         With a numeric argument such as 'serviceStateTable DEPTH':
           When DEPTH is 1, print the list of the stateVariables.
           When DEPTH is 2, print the list of the stateVariables with their
             parameters.
           When DEPTH is 3, print also the list of the 'allowedValueList' or
            'allowedValuerange' parameter if any.
@@ -391,28 +391,28 @@
         self.loop = loop
         build_commands_from(self, upnp_device,
                             exclude=('deviceList', 'serviceList'))
         self.prompt = f'[{device_name(upnp_device)}] '
         self.quit = False
 
     def do_quit(self, unused):
-        """Quit the application"""
+        """Quit the application."""
 
         # Tell cmdloop() to return True.
         self.quit = True
         # Stop the current interpreter and return to the previous one.
         return True
 
     def do_embedded_list(self, unused):
         """List the embedded UPnP devices"""
         print([device_name(dev) for dev in
                self.upnp_device.deviceList.values()])
 
     def help_embedded(self):
-        print(_dedent(f"""Select an embedded device
+        print(_dedent(f"""Select an embedded device.
 
         Use the command 'embedded IDX' to select the device at index IDX
         (starting at zero) in the list printed by the 'embedded_list' command.
         With no argument, do this for the device at index 0.
 
         """))
 
@@ -421,24 +421,24 @@
         selected = self.select_device(dev_list, idx)
         if selected is not None:
             interpreter = UPnPDeviceCmd(selected)
             if interpreter.cmdloop():
                 return self.do_quit(None)
 
     def do_service_list(self, unused):
-        """List the services"""
+        """List the services."""
         print([str(serv) for serv in self.upnp_device.serviceList.values()])
 
     def complete_service(self, text, line, begidx, endidx):
         return [s for s in
                 (str(serv) for serv in self.upnp_device.serviceList.values())
                     if s.startswith(text)]
 
     def help_service(self):
-        print(_dedent("""Select a service
+        print(_dedent("""Select a service.
 
         Use the command 'service NAME' to select the service named NAME.
         Completion is enabled on the service names.
 
         """))
 
     def do_service(self, arg):
@@ -469,42 +469,42 @@
 
         interpreter = UPnPServiceCmd(serv, self.loop)
         if interpreter.cmdloop():
             return self.do_quit(None)
 
     def help_previous(self):
         if self.upnp_device.parent_device is self.upnp_device.root_device:
-            print('Return to the control point')
+            print('Return to the control point.')
         else:
-            print('Return to the previous device')
+            print('Return to the previous device.')
 
     def do_previous(self, unused):
         return True
 
     def help_peer_ipaddress(self):
-        print('Print the IP address of the UPnP device')
+        print('Print the IP address of the UPnP device.')
 
     def help_parent_device(self):
-        print('Shortened UDN of the parent device')
+        print('Shortened UDN of the parent device.')
 
     def do_description(self, unused):
-        """Print the xml 'description'"""
+        """Print the xml 'description'."""
         print(pformat_xml(self.upnp_device.description))
 
     def do_iconList(self, unused):
-        """Print the value of 'iconList'"""
+        """Print the value of 'iconList'."""
 
         device = self.upnp_device
         if hasattr(device, 'iconList'):
             pprint_pprint(device.iconList, indent=2)
         else:
             print('None')
 
     def help_root_device(self):
-        print('Shortened UDN of the root device')
+        print('Shortened UDN of the root device.')
 
     def cmdloop(self):
         super().cmdloop()
         # Tell the previous interpreter to just quit when self.quit is True.
         return self.quit
 
 class UPnPControlCmd(UPnPApplication, _Cmd):
@@ -529,24 +529,24 @@
         self.cp_thread = None
         self.devices = set()
 
         # Cmd attributes.
         self.prompt = '[Control Point] '
 
     def do_quit(self, unused):
-        """Quit the application"""
+        """Quit the application."""
         self.close()
         return True
 
     def do_device_list(self, unused):
-        """List the discovered UPnP devices"""
+        """List the discovered UPnP devices."""
         print([device_name(dev) for dev in self.devices])
 
     def help_device(self):
-        print(_dedent(f"""Select a discovered device
+        print(_dedent(f"""Select a discovered device.
 
         Use the command 'device IDX' to select the device at index IDX
         (starting at zero) in the list printed by the 'device_list' command.
         With no argument, do this for the device at index 0.
 
         """))
 
@@ -555,21 +555,33 @@
         selected = self.select_device(dev_list, idx)
         if selected is not None:
             interpreter = UPnPDeviceCmd(selected, self.loop)
             if interpreter.cmdloop():
                 self.close()
                 return True
 
+    def help_ip_configured (self):
+        print(_dedent("""Print the list of the configured IPv4 addresses of
+        the networks where UPnP devices may be discovered. All addresses may
+        be monitored when both 'ip_configured' and 'nics' are empty.
+        """))
+
     def help_nics(self):
-        print(_dedent("""Print the list of the network interfaces where
-        UPnP devices may be discovered
+        print(_dedent("""Print the list of the network interfaces where UPnP
+        devices may be discovered. All IPv4 addresses may be monitored when
+        both 'ip_configured' and 'nics' are empty.
+        """))
+
+    def help_ip_monitored(self):
+        print(_dedent("""Print the list of the IPv4 addresses currently
+        monitored by UPnP discovery.
         """))
 
     def help_ttl(self):
-        print('Print the the IP packets time to live')
+        print('Print the IP packets time to live.')
 
     def close(self):
         if self.control_point is not None:
             if threading.current_thread() is not self.cp_thread:
                 if self.loop is not None and not self.loop.is_closed():
                     self.loop.call_soon_threadsafe(self.control_point.close)
                 self.cp_thread.join(timeout=5)
@@ -587,16 +599,17 @@
             self.close()
 
     @log_exception(logger)
     async def run_control_point(self, event):
         self.loop = asyncio.get_running_loop()
         try:
             # Run the UPnP control point.
-            with UPnPControlPoint(self.nics, self.msearch_interval,
-                                  self.ttl) as self.control_point:
+            with UPnPControlPoint(
+                    self.ip_addresses, self.nics, self.msearch_interval,
+                    self.ttl) as self.control_point:
                 event.set()
                 while True:
                     notif, root_device = (await
                                           self.control_point.get_notification())
                     if (notif, root_device) == QUEUE_CLOSED:
                         logger.debug('UPnP queue is closed')
                         break
```

### Comparing `pa-dlna-0.4/pyproject.toml` & `pa-dlna-0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/tools/build_didl_lite.py` & `pa-dlna-0.5/tools/build_didl_lite.py`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/tools/gendoc_default_config.py` & `pa-dlna-0.5/tools/gendoc_default_config.py`

 * *Files identical despite different names*

### Comparing `pa-dlna-0.4/PKG-INFO` & `pa-dlna-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pa-dlna
-Version: 0.4
+Version: 0.5
 Summary: Forward pulseaudio streams to DLNA devices.
 Keywords: pulseaudio,DLNA,UPnP,asyncio,pulsectl
 Author-email: Xavier de Gaye <xdegaye@gmail.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: AsyncIO
```

