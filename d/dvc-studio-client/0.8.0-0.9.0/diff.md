# Comparing `tmp/dvc-studio-client-0.8.0.tar.gz` & `tmp/dvc-studio-client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-studio-client-0.8.0.tar", last modified: Thu Apr 20 17:44:58 2023, max compression
+gzip compressed data, was "dvc-studio-client-0.9.0.tar", last modified: Thu May  4 14:50:32 2023, max compression
```

## Comparing `dvc-studio-client-0.8.0.tar` & `dvc-studio-client-0.9.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-20 17:44:58.971891 dvc-studio-client-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.963891 dvc-studio-client-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/src/dvc_studio_client/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/src/dvc_studio_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/src/dvc_studio_client/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/src/dvc_studio_client/post_live_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/src/dvc_studio_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/src/dvc_studio_client/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-20 17:44:58.000000 dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-20 17:44:58.000000 dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 17:44:58.000000 dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 17:44:58.000000 dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-20 17:44:58.000000 dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 17:44:58.000000 dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/tests/test_post_live_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.575607 dvc-studio-client-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.575607 dvc-studio-client-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.github/workflows/leaked-secrets-scan.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.575607 dvc-studio-client-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/src/dvc_studio_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/src/dvc_studio_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/src/dvc_studio_client/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/src/dvc_studio_client/post_live_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/src/dvc_studio_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/src/dvc_studio_client/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-04 14:50:32.000000 dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-04 14:50:32.000000 dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:50:32.000000 dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:50:32.000000 dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-04 14:50:32.000000 dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 14:50:32.000000 dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/tests/test_post_live_metrics.py
```

### Comparing `dvc-studio-client-0.8.0/.cruft.json` & `dvc-studio-client-0.9.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/.github/dependabot.yml` & `dvc-studio-client-0.9.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/.github/workflows/docs.yml` & `dvc-studio-client-0.9.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/.github/workflows/pre-commit.yml` & `dvc-studio-client-0.9.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/.github/workflows/release.yml` & `dvc-studio-client-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/.github/workflows/tests.yml` & `dvc-studio-client-0.9.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/.gitignore` & `dvc-studio-client-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/.pre-commit-config.yaml` & `dvc-studio-client-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/CODE_OF_CONDUCT.rst` & `dvc-studio-client-0.9.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/CONTRIBUTING.rst` & `dvc-studio-client-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/LICENSE` & `dvc-studio-client-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/PKG-INFO` & `dvc-studio-client-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dvc-studio-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: Small library to post data from DVC/DVCLive to Iterative Studio
-Home-page: https://github.com/iterative/DVC Studio Client
+Home-page: https://github.com/iterative/dvc-studio-client
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dvc-studio-client-0.8.0/README.rst` & `dvc-studio-client-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/docs/assets/logo.svg` & `dvc-studio-client-0.9.0/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/docs/gen_ref_pages.py` & `dvc-studio-client-0.9.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/mkdocs.yml` & `dvc-studio-client-0.9.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/pyproject.toml` & `dvc-studio-client-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.8.0/setup.cfg` & `dvc-studio-client-0.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 description = Small library to post data from DVC/DVCLive to Iterative Studio
 name = dvc-studio-client
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 license = Apache-2.0
 license_file = LICENSE
-url = https://github.com/iterative/DVC Studio Client
+url = https://github.com/iterative/dvc-studio-client
 platforms = any
 authors = Iterative
 maintainer_email = support@dvc.org
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
```

### Comparing `dvc-studio-client-0.8.0/src/dvc_studio_client/post_live_metrics.py` & `dvc-studio-client-0.9.0/src/dvc_studio_client/post_live_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,21 +64,22 @@
     studio_repo_url = studio_repo_url or getenv(STUDIO_REPO_URL, None)
     if studio_repo_url is None:
         logger.debug(f"`{STUDIO_REPO_URL}` not found. Trying to automatically find it.")
         studio_repo_url = get_studio_repo_url()
     return studio_token, studio_repo_url
 
 
-def post_live_metrics(
+def post_live_metrics(  # noqa: C901
     event_type: Literal["start", "data", "done"],
     baseline_sha: str,
     name: str,
     client: Literal["dvc", "dvclive"],
     experiment_rev: Optional[str] = None,
     machine: Optional[Dict[str, Any]] = None,
+    message: Optional[str] = None,
     metrics: Optional[Dict[str, Any]] = None,
     params: Optional[Dict[str, Any]] = None,
     plots: Optional[Dict[str, Any]] = None,
     step: Optional[int] = None,
     studio_token: Optional[str] = None,
     studio_repo_url: Optional[str] = None,
 ) -> Optional[bool]:
@@ -106,14 +107,16 @@
             machine={
                 "cpu": 0.94
                 "memory": 0.99
                 "cloud": "aws"
                 "instance": "t2.micro"
             }
             ```
+        message: (Optional[str]): Custom message to be displayed as the commit
+            message in Studio UI.
         metrics (Optional[Dict[str, Any]]): Updates to DVC metric files.
             Defaults to `None`.
             Only used when `event_type="data"`.
             ```
             metrics={
                 "dvclive/metrics.json": {
                     "data": {
@@ -174,15 +177,19 @@
 
     if metrics:
         body["metrics"] = metrics
 
     if machine:
         body["machine"] = machine
 
-    if event_type == "data":
+    if event_type == "start":
+        if message:
+            # Cutting the message to match the commit title length limit.
+            body["message"] = message[:72]
+    elif event_type == "data":
         if step is None:
             logger.warning("Missing `step` in `data` event.")
             return None
         body["step"] = step
         if plots:
             body["plots"] = plots
```

### Comparing `dvc-studio-client-0.8.0/src/dvc_studio_client/schema.py` & `dvc-studio-client-0.9.0/src/dvc_studio_client/schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,19 @@
         "params": {str: dict},
         "metrics": {str: {"data": dict, "error": ERROR_SCHEMA}},
         "machine": dict,
         # Required("timestamp"): iso_datetime,  # TODO: decide if we need this
     }
 )
 SCHEMAS_BY_TYPE = {
-    "start": BASE_SCHEMA,
+    "start": BASE_SCHEMA.extend(
+        {
+            "message": str,
+        }
+    ),
     "data": BASE_SCHEMA.extend(
         {
             Required("step"): int,
             "plots": {
                 str: {
                     Exclusive("data", "data"): [dict],
                     "props": dict,
```

### Comparing `dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/PKG-INFO` & `dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dvc-studio-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: Small library to post data from DVC/DVCLive to Iterative Studio
-Home-page: https://github.com/iterative/DVC Studio Client
+Home-page: https://github.com/iterative/dvc-studio-client
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/SOURCES.txt` & `dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 LICENSE
 README.rst
 mkdocs.yml
 pyproject.toml
 setup.cfg
 .github/dependabot.yml
 .github/workflows/docs.yml
+.github/workflows/leaked-secrets-scan.yaml
 .github/workflows/pre-commit.yml
 .github/workflows/release.yml
 .github/workflows/tests.yml
 .github/workflows/update-template.yaml
 .vscode/settings.json
 docs/gen_ref_pages.py
 docs/index.md
```

### Comparing `dvc-studio-client-0.8.0/tests/test_post_live_metrics.py` & `dvc-studio-client-0.9.0/tests/test_post_live_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -374,7 +374,68 @@
         },
         headers={
             "Authorization": "token FOO_TOKEN",
             "Content-type": "application/json",
         },
         timeout=5,
     )
+
+
+def test_post_live_metrics_message(mocker, monkeypatch):
+    monkeypatch.setenv(DVC_STUDIO_URL, "https://0.0.0.0")
+    monkeypatch.setenv(DVC_STUDIO_TOKEN, "FOO_TOKEN")
+    monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
+
+    mocked_response = mocker.MagicMock()
+    mocked_response.status_code = 200
+    mocked_post = mocker.patch("requests.post", return_value=mocked_response)
+
+    assert post_live_metrics(
+        "start",
+        "f" * 40,
+        "fooname",
+        "fooclient",
+        message="FOO_MESSAGE",
+    )
+
+    mocked_post.assert_called_with(
+        "https://0.0.0.0/api/live",
+        json={
+            "type": "start",
+            "repo_url": "FOO_REPO_URL",
+            "baseline_sha": "f" * 40,
+            "name": "fooname",
+            "client": "fooclient",
+            "message": "FOO_MESSAGE",
+        },
+        headers={
+            "Authorization": "token FOO_TOKEN",
+            "Content-type": "application/json",
+        },
+        timeout=5,
+    )
+
+    # Test message length limit
+    assert post_live_metrics(
+        "start",
+        "f" * 40,
+        "fooname",
+        "fooclient",
+        message="X" * 100,
+    )
+
+    mocked_post.assert_called_with(
+        "https://0.0.0.0/api/live",
+        json={
+            "type": "start",
+            "repo_url": "FOO_REPO_URL",
+            "baseline_sha": "f" * 40,
+            "name": "fooname",
+            "client": "fooclient",
+            "message": "X" * 72,
+        },
+        headers={
+            "Authorization": "token FOO_TOKEN",
+            "Content-type": "application/json",
+        },
+        timeout=5,
+    )
```

