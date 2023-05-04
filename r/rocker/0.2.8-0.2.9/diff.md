# Comparing `tmp/rocker-0.2.8.tar.gz` & `tmp/rocker-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocker-0.2.8.tar", last modified: Mon Feb 14 22:28:07 2022, max compression
+gzip compressed data, was "dist/rocker-0.2.9.tar", last modified: Thu Mar 24 08:54:32 2022, max compression
```

## Comparing `rocker-0.2.8.tar` & `rocker-0.2.9.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 tfoote    (1000) tfoote    (1000)        0 2022-02-14 22:28:07.813253 rocker-0.2.8/
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      563 2022-02-14 22:28:07.813253 rocker-0.2.8/PKG-INFO
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     5439 2022-02-14 22:16:40.000000 rocker-0.2.8/README.md
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)       38 2022-02-14 22:28:07.813253 rocker-0.2.8/setup.cfg
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     2549 2022-02-14 22:26:38.000000 rocker-0.2.8/setup.py
-drwxrwxr-x   0 tfoote    (1000) tfoote    (1000)        0 2022-02-14 22:28:07.813253 rocker-0.2.8/src/
-drwxrwxr-x   0 tfoote    (1000) tfoote    (1000)        0 2022-02-14 22:28:07.813253 rocker-0.2.8/src/rocker/
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)        0 2022-01-28 12:03:23.000000 rocker-0.2.8/src/rocker/__init__.py
--rwxrwxr-x   0 tfoote    (1000) tfoote    (1000)     3260 2022-02-12 00:52:02.000000 rocker-0.2.8/src/rocker/cli.py
--rwxrwxr-x   0 tfoote    (1000) tfoote    (1000)    13112 2022-01-28 12:03:23.000000 rocker-0.2.8/src/rocker/core.py
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     9969 2022-01-28 12:03:23.000000 rocker-0.2.8/src/rocker/extensions.py
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     2291 2022-01-28 12:03:23.000000 rocker-0.2.8/src/rocker/git_extension.py
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     5164 2022-01-28 12:03:23.000000 rocker-0.2.8/src/rocker/nvidia_extension.py
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     3240 2022-01-28 12:03:23.000000 rocker-0.2.8/src/rocker/os_detector.py
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     1541 2022-01-28 12:03:23.000000 rocker-0.2.8/src/rocker/ssh_extension.py
-drwxrwxr-x   0 tfoote    (1000) tfoote    (1000)        0 2022-02-14 22:28:07.813253 rocker-0.2.8/src/rocker/templates/
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)       91 2022-01-28 12:03:23.000000 rocker-0.2.8/src/rocker/templates/Dockerfile.em
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)       14 2022-01-28 12:03:23.000000 rocker-0.2.8/src/rocker/templates/bash_cmd_snippet.Dockerfile.em
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      120 2022-01-28 12:03:23.000000 rocker-0.2.8/src/rocker/templates/dev_helpers_snippet.Dockerfile.em
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      184 2022-01-28 12:03:23.000000 rocker-0.2.8/src/rocker/templates/nvidia_preamble.Dockerfile.em
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     1480 2022-01-28 12:03:23.000000 rocker-0.2.8/src/rocker/templates/nvidia_snippet.Dockerfile.em
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      352 2022-01-28 12:03:23.000000 rocker-0.2.8/src/rocker/templates/pulse_snippet.Dockerfile.em
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     1648 2022-02-14 22:16:40.000000 rocker-0.2.8/src/rocker/templates/user_snippet.Dockerfile.em
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     2575 2022-02-14 22:16:40.000000 rocker-0.2.8/src/rocker/volume_extension.py
-drwxrwxr-x   0 tfoote    (1000) tfoote    (1000)        0 2022-02-14 22:28:07.813253 rocker-0.2.8/src/rocker.egg-info/
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      563 2022-02-14 22:28:07.000000 rocker-0.2.8/src/rocker.egg-info/PKG-INFO
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      977 2022-02-14 22:28:07.000000 rocker-0.2.8/src/rocker.egg-info/SOURCES.txt
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)        1 2022-02-14 22:28:07.000000 rocker-0.2.8/src/rocker.egg-info/dependency_links.txt
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      616 2022-02-14 22:28:07.000000 rocker-0.2.8/src/rocker.egg-info/entry_points.txt
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)       30 2022-02-14 22:28:07.000000 rocker-0.2.8/src/rocker.egg-info/requires.txt
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)        7 2022-02-14 22:28:07.000000 rocker-0.2.8/src/rocker.egg-info/top_level.txt
-drwxrwxr-x   0 tfoote    (1000) tfoote    (1000)        0 2022-02-14 22:28:07.813253 rocker-0.2.8/test/
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     6160 2022-01-28 12:03:23.000000 rocker-0.2.8/test/test_core.py
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)    17226 2022-02-14 22:16:40.000000 rocker-0.2.8/test/test_extension.py
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     3270 2022-01-28 12:03:23.000000 rocker-0.2.8/test/test_file_writing.py
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     3805 2022-01-28 12:03:23.000000 rocker-0.2.8/test/test_git_extension.py
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     8789 2022-01-28 12:03:23.000000 rocker-0.2.8/test/test_nvidia.py
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     1893 2022-01-28 12:03:23.000000 rocker-0.2.8/test/test_os_detect.py
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     2720 2022-01-28 12:03:23.000000 rocker-0.2.8/test/test_ssh_extension.py
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     2880 2022-01-28 12:03:23.000000 rocker-0.2.8/test/test_volume.py
+drwxr-xr-x   0 tfoote    (1000) tfoote    (1000)        0 2022-03-24 08:54:32.000000 rocker-0.2.9/
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     2549 2022-03-23 23:13:27.000000 rocker-0.2.9/setup.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)    11358 2021-05-20 02:08:06.000000 rocker-0.2.9/LICENSE
+drwxr-xr-x   0 tfoote    (1000) tfoote    (1000)        0 2022-03-24 08:54:32.000000 rocker-0.2.9/test/
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     6160 2021-02-08 07:39:52.000000 rocker-0.2.9/test/test_core.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     3805 2021-04-10 01:48:00.000000 rocker-0.2.9/test/test_git_extension.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     8789 2021-01-06 21:30:12.000000 rocker-0.2.9/test/test_nvidia.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)    17226 2022-02-15 00:15:59.000000 rocker-0.2.9/test/test_extension.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     2880 2021-06-09 01:50:00.000000 rocker-0.2.9/test/test_volume.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     3270 2020-11-04 01:36:44.000000 rocker-0.2.9/test/test_file_writing.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     1893 2021-02-04 19:54:55.000000 rocker-0.2.9/test/test_os_detect.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     2720 2020-08-11 01:21:07.000000 rocker-0.2.9/test/test_ssh_extension.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     5531 2022-03-23 23:13:15.000000 rocker-0.2.9/README.md
+-rw-r--r--   0 tfoote    (1000) tfoote    (1000)       38 2022-03-24 08:54:32.000000 rocker-0.2.9/setup.cfg
+drwxr-xr-x   0 tfoote    (1000) tfoote    (1000)        0 2022-03-24 08:54:32.000000 rocker-0.2.9/src/
+drwxr-xr-x   0 tfoote    (1000) tfoote    (1000)        0 2022-03-24 08:54:32.000000 rocker-0.2.9/src/rocker.egg-info/
+-rw-r--r--   0 tfoote    (1000) tfoote    (1000)      616 2022-03-24 08:54:32.000000 rocker-0.2.9/src/rocker.egg-info/entry_points.txt
+-rw-r--r--   0 tfoote    (1000) tfoote    (1000)        1 2022-03-24 08:54:32.000000 rocker-0.2.9/src/rocker.egg-info/dependency_links.txt
+-rw-r--r--   0 tfoote    (1000) tfoote    (1000)      985 2022-03-24 08:54:32.000000 rocker-0.2.9/src/rocker.egg-info/SOURCES.txt
+-rw-r--r--   0 tfoote    (1000) tfoote    (1000)      574 2022-03-24 08:54:32.000000 rocker-0.2.9/src/rocker.egg-info/PKG-INFO
+-rw-r--r--   0 tfoote    (1000) tfoote    (1000)       30 2022-03-24 08:54:32.000000 rocker-0.2.9/src/rocker.egg-info/requires.txt
+-rw-r--r--   0 tfoote    (1000) tfoote    (1000)        7 2022-03-24 08:54:32.000000 rocker-0.2.9/src/rocker.egg-info/top_level.txt
+drwxr-xr-x   0 tfoote    (1000) tfoote    (1000)        0 2022-03-24 08:54:32.000000 rocker-0.2.9/src/rocker/
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     2291 2021-04-10 01:48:00.000000 rocker-0.2.9/src/rocker/git_extension.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     9969 2021-12-01 07:22:07.000000 rocker-0.2.9/src/rocker/extensions.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     5173 2022-03-23 23:13:15.000000 rocker-0.2.9/src/rocker/nvidia_extension.py
+drwxr-xr-x   0 tfoote    (1000) tfoote    (1000)        0 2022-03-24 08:54:32.000000 rocker-0.2.9/src/rocker/templates/
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)       91 2020-08-11 01:21:07.000000 rocker-0.2.9/src/rocker/templates/Dockerfile.em
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)       14 2020-08-11 01:21:07.000000 rocker-0.2.9/src/rocker/templates/bash_cmd_snippet.Dockerfile.em
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     1480 2020-08-11 01:21:07.000000 rocker-0.2.9/src/rocker/templates/nvidia_snippet.Dockerfile.em
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      352 2020-08-11 01:21:07.000000 rocker-0.2.9/src/rocker/templates/pulse_snippet.Dockerfile.em
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      120 2020-08-11 01:21:07.000000 rocker-0.2.9/src/rocker/templates/dev_helpers_snippet.Dockerfile.em
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     1648 2022-02-15 00:15:59.000000 rocker-0.2.9/src/rocker/templates/user_snippet.Dockerfile.em
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      184 2020-08-11 01:21:07.000000 rocker-0.2.9/src/rocker/templates/nvidia_preamble.Dockerfile.em
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     1541 2020-08-11 01:21:07.000000 rocker-0.2.9/src/rocker/ssh_extension.py
+-rwxrwxr-x   0 tfoote    (1000) tfoote    (1000)    13112 2022-03-23 22:31:37.000000 rocker-0.2.9/src/rocker/core.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     3240 2021-10-05 01:05:22.000000 rocker-0.2.9/src/rocker/os_detector.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     2575 2022-02-15 00:15:59.000000 rocker-0.2.9/src/rocker/volume_extension.py
+-rwxrwxr-x   0 tfoote    (1000) tfoote    (1000)     3235 2021-02-08 07:39:51.000000 rocker-0.2.9/src/rocker/cli.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)        0 2020-08-11 01:21:07.000000 rocker-0.2.9/src/rocker/__init__.py
+-rw-r--r--   0 tfoote    (1000) tfoote    (1000)      574 2022-03-24 08:54:32.000000 rocker-0.2.9/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `rocker-0.2.8/PKG-INFO` & `rocker-0.2.9/src/rocker.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: rocker
-Version: 0.2.8
+Version: 0.2.9
 Summary: A tool to run docker containers with customized extras
 Home-page: https://github.com/osrf/rocker
 Author: Tully Foote
 Author-email: tfoote@osrfoundation.org
 License: Apache License 2.0
-Description: A tool to run docker containers with customized extra added like nvidia gui support overlayed.
 Keywords: Docker
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.0
+License-File: LICENSE
+
+A tool to run docker containers with customized extra added like nvidia gui support overlayed.
+
```

### Comparing `rocker-0.2.8/README.md` & `rocker-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 For the NVIDIA option this has been tested on the following systems using nvidia docker2:
 
 | Ubuntu distribution | Linux Kernel | Nvidia drivers                                    |
 | ------------------- | ------------ | ------------------------------------------------- |
 | 16.04               | 4.15         | nvidia-384 (works) <br> nvidia-340 (doesn't work) |
 | 18.04               |              | nvidia-390 (works)                                |
 | 20.04               | 5.4.0        | nvidia-driver-460 (works)                         |
+| 22.04               | 5.13.0        | nvidia-driver-470 (works)                         |
 
 Install nvidia-docker 2: https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html#docker
 
 ### Additional Configuration for rootless mode
 For executing Docker as a non-root user, separate installation instructions are provided here: https://docs.docker.com/engine/security/rootless/
 
 After installing Rootless Docker, the nvidia-docker2 package can be installed as usual from the website above.
```

### Comparing `rocker-0.2.8/setup.py` & `rocker-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     if int(ver[0]) < 2:
         docker_package = 'docker-py'
 
 install_requires.append(docker_package)
 
 kwargs = {
     'name': 'rocker',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'packages': ['rocker'],
     'package_dir': {'': 'src'},
     'package_data': {'rocker': ['templates/*.em']},
     'entry_points': {
         'console_scripts': [
             'rocker = rocker.cli:main',
             'detect_docker_image_os = rocker.cli:detect_image_os',
```

### Comparing `rocker-0.2.8/src/rocker/cli.py` & `rocker-0.2.9/src/rocker/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     dig = DockerImageGenerator(active_extensions, args_dict, base_image)
     exit_code = dig.build(**vars(args))
     if exit_code != 0:
         print("Build failed exiting")
         return exit_code
     # Convert command into string
-    args.command = ' '.join(args.command) ## TODO(tfoote) Unused??
+    args.command = ' '.join(args.command)
     return dig.run(**args_dict)
 
 
 def detect_image_os():
     parser = argparse.ArgumentParser(description='Detect the os in an image')
     parser.add_argument('image')
     parser.add_argument('--verbose', action='store_true',
```

### Comparing `rocker-0.2.8/src/rocker/core.py` & `rocker-0.2.9/src/rocker/core.py`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/src/rocker/extensions.py` & `rocker-0.2.9/src/rocker/extensions.py`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/src/rocker/git_extension.py` & `rocker-0.2.9/src/rocker/git_extension.py`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/src/rocker/nvidia_extension.py` & `rocker-0.2.9/src/rocker/nvidia_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     def get_name():
         return 'nvidia'
 
     def __init__(self):
         self._env_subs = None
         self.name = Nvidia.get_name()
         self.supported_distros = ['Ubuntu', 'Debian GNU/Linux']
-        self.supported_versions = ['16.04', '18.04', '20.04', '10']
+        self.supported_versions = ['16.04', '18.04', '20.04', '10', '22.04']
 
 
     def get_environment_subs(self, cliargs={}):
         if not self._env_subs:
             self._env_subs = {}
             self._env_subs['user_id'] = os.getuid()
             self._env_subs['username'] = getpass.getuser()
```

### Comparing `rocker-0.2.8/src/rocker/os_detector.py` & `rocker-0.2.9/src/rocker/os_detector.py`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/src/rocker/ssh_extension.py` & `rocker-0.2.9/src/rocker/ssh_extension.py`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/src/rocker/templates/nvidia_snippet.Dockerfile.em` & `rocker-0.2.9/src/rocker/templates/nvidia_snippet.Dockerfile.em`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/src/rocker/templates/user_snippet.Dockerfile.em` & `rocker-0.2.9/src/rocker/templates/user_snippet.Dockerfile.em`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/src/rocker/volume_extension.py` & `rocker-0.2.9/src/rocker/volume_extension.py`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/src/rocker.egg-info/PKG-INFO` & `rocker-0.2.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: rocker
-Version: 0.2.8
+Version: 0.2.9
 Summary: A tool to run docker containers with customized extras
 Home-page: https://github.com/osrf/rocker
 Author: Tully Foote
 Author-email: tfoote@osrfoundation.org
 License: Apache License 2.0
-Description: A tool to run docker containers with customized extra added like nvidia gui support overlayed.
 Keywords: Docker
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.0
+License-File: LICENSE
+
+A tool to run docker containers with customized extra added like nvidia gui support overlayed.
+
```

### Comparing `rocker-0.2.8/src/rocker.egg-info/SOURCES.txt` & `rocker-0.2.9/src/rocker.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 src/rocker/__init__.py
 src/rocker/cli.py
 src/rocker/core.py
 src/rocker/extensions.py
 src/rocker/git_extension.py
```

### Comparing `rocker-0.2.8/src/rocker.egg-info/entry_points.txt` & `rocker-0.2.9/src/rocker.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/test/test_core.py` & `rocker-0.2.9/test/test_core.py`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/test/test_extension.py` & `rocker-0.2.9/test/test_extension.py`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/test/test_file_writing.py` & `rocker-0.2.9/test/test_file_writing.py`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/test/test_git_extension.py` & `rocker-0.2.9/test/test_git_extension.py`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/test/test_nvidia.py` & `rocker-0.2.9/test/test_nvidia.py`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/test/test_os_detect.py` & `rocker-0.2.9/test/test_os_detect.py`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/test/test_ssh_extension.py` & `rocker-0.2.9/test/test_ssh_extension.py`

 * *Files identical despite different names*

### Comparing `rocker-0.2.8/test/test_volume.py` & `rocker-0.2.9/test/test_volume.py`

 * *Files identical despite different names*

