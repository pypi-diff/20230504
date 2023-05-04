# Comparing `tmp/caikit-tgis-backend-0.1.0.tar.gz` & `tmp/caikit-tgis-backend-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-tgis-backend-0.1.0.tar", last modified: Tue May  2 21:29:34 2023, max compression
+gzip compressed data, was "caikit-tgis-backend-0.1.1.tar", last modified: Thu May  4 18:54:33 2023, max compression
```

## Comparing `caikit-tgis-backend-0.1.0.tar` & `caikit-tgis-backend-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       65 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/.coveragerc
--rw-r--r--   0        0        0      676 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      105 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1280 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1141 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1144 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      183 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/.gitignore
--rw-r--r--   0        0        0      318 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/.isort.cfg
--rw-r--r--   0        0        0      440 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       24 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/.prettierignore
--rw-r--r--   0        0        0       12 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/.prettierrc.yaml
--rw-r--r--   0        0        0    21406 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/.pylintrc
--rw-r--r--   0        0        0       78 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/.whitesource
--rw-r--r--   0        0        0      314 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/CODEOWNERS
--rw-r--r--   0        0        0     7269 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/LICENSE
--rw-r--r--   0        0        0      138 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/README.md
--rw-r--r--   0        0        0      152 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/SECURITY.md
--rw-r--r--   0        0        0      723 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/caikit_tgis_backend/__init__.py
--rw-r--r--   0        0        0     5727 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/caikit_tgis_backend/generation.proto
--rw-r--r--   0        0        0      840 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/caikit_tgis_backend/protobufs/__init__.py
--rw-r--r--   0        0        0    13426 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/caikit_tgis_backend/protobufs/generation_pb2.py
--rw-r--r--   0        0        0     5685 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/caikit_tgis_backend/protobufs/generation_pb2_grpc.py
--rw-r--r--   0        0        0    12520 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/caikit_tgis_backend/tgis_backend.py
--rw-r--r--   0        0        0      169 2023-05-02 21:29:20.997342 caikit-tgis-backend-0.1.0/code-of-conduct.md
--rw-r--r--   0        0        0      655 2023-05-02 21:29:28.154269 caikit-tgis-backend-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0      720 2023-05-02 21:29:21.001342 caikit-tgis-backend-0.1.0/scripts/fmt.sh
--rwxr-xr-x   0        0        0      393 2023-05-02 21:29:21.001342 caikit-tgis-backend-0.1.0/scripts/gen_tgis_protos.sh
--rw-r--r--   0        0        0       33 2023-05-02 21:29:21.001342 caikit-tgis-backend-0.1.0/setup_requirements.txt
--rw-r--r--   0        0        0        0 2023-05-02 21:29:21.001342 caikit-tgis-backend-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      342 2023-05-02 21:29:21.001342 caikit-tgis-backend-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     9063 2023-05-02 21:29:21.001342 caikit-tgis-backend-0.1.0/tests/test_tgis_backend.py
--rw-r--r--   0        0        0     7629 2023-05-02 21:29:21.001342 caikit-tgis-backend-0.1.0/tests/tgis_mock.py
--rw-r--r--   0        0        0     1209 2023-05-02 21:29:21.001342 caikit-tgis-backend-0.1.0/tox.ini
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 caikit-tgis-backend-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.coveragerc
+-rw-r--r--   0        0        0      676 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      105 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1280 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1141 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1144 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      183 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.gitignore
+-rw-r--r--   0        0        0      318 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.isort.cfg
+-rw-r--r--   0        0        0      440 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       24 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.prettierignore
+-rw-r--r--   0        0        0       12 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.prettierrc.yaml
+-rw-r--r--   0        0        0    21406 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.pylintrc
+-rw-r--r--   0        0        0       78 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.whitesource
+-rw-r--r--   0        0        0      314 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/CODEOWNERS
+-rw-r--r--   0        0        0     7269 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/LICENSE
+-rw-r--r--   0        0        0      138 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/README.md
+-rw-r--r--   0        0        0      152 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/SECURITY.md
+-rw-r--r--   0        0        0      723 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/caikit_tgis_backend/__init__.py
+-rw-r--r--   0        0        0     5727 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/caikit_tgis_backend/generation.proto
+-rw-r--r--   0        0        0      840 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/caikit_tgis_backend/protobufs/__init__.py
+-rw-r--r--   0        0        0    13426 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/caikit_tgis_backend/protobufs/generation_pb2.py
+-rw-r--r--   0        0        0     5685 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/caikit_tgis_backend/protobufs/generation_pb2_grpc.py
+-rw-r--r--   0        0        0    12520 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/caikit_tgis_backend/tgis_backend.py
+-rw-r--r--   0        0        0      169 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/code-of-conduct.md
+-rw-r--r--   0        0        0      655 2023-05-04 18:54:29.651985 caikit-tgis-backend-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0      720 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/scripts/fmt.sh
+-rwxr-xr-x   0        0        0      393 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/scripts/gen_tgis_protos.sh
+-rw-r--r--   0        0        0       33 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/setup_requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      342 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     9063 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/tests/test_tgis_backend.py
+-rw-r--r--   0        0        0     7629 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/tests/tgis_mock.py
+-rw-r--r--   0        0        0     1209 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/tox.ini
+-rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 caikit-tgis-backend-0.1.1/PKG-INFO
```

### Comparing `caikit-tgis-backend-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-tgis-backend-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-tgis-backend-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-tgis-backend-0.1.1/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/.github/workflows/build-library.yml` & `caikit-tgis-backend-0.1.1/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/.github/workflows/lint-code.yml` & `caikit-tgis-backend-0.1.1/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/.github/workflows/publish-library.yml` & `caikit-tgis-backend-0.1.1/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/.pylintrc` & `caikit-tgis-backend-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/CONTRIBUTING.md` & `caikit-tgis-backend-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/LICENSE` & `caikit-tgis-backend-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/caikit_tgis_backend/__init__.py` & `caikit-tgis-backend-0.1.1/caikit_tgis_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/caikit_tgis_backend/generation.proto` & `caikit-tgis-backend-0.1.1/caikit_tgis_backend/generation.proto`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/caikit_tgis_backend/protobufs/__init__.py` & `caikit-tgis-backend-0.1.1/caikit_tgis_backend/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/caikit_tgis_backend/protobufs/generation_pb2.py` & `caikit-tgis-backend-0.1.1/caikit_tgis_backend/protobufs/generation_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/caikit_tgis_backend/protobufs/generation_pb2_grpc.py` & `caikit-tgis-backend-0.1.1/caikit_tgis_backend/protobufs/generation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/caikit_tgis_backend/tgis_backend.py` & `caikit-tgis-backend-0.1.1/caikit_tgis_backend/tgis_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/pyproject.toml` & `caikit-tgis-backend-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit-tgis-backend"
 # Not the actual current version: overwritten by CI
-version = "0.1.0"
+version = "0.1.1"
 description = "Caikit module backend for models run in TGIS"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
-    "caikit>=0.2.0,<0.3.0", # Core abstractions
+    "caikit>=0.2.0,<0.4.0", # Core abstractions
     "grpcio>=1.35.0,<2.0", # Client calls to TGIS
     "requests>=2.28.2,<3", # Health check calls to TGIS
 ]
 
 [project.urls]
 Source = "https://github.com/caikit/caikit-tgis-backend"
```

### Comparing `caikit-tgis-backend-0.1.0/scripts/fmt.sh` & `caikit-tgis-backend-0.1.1/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/tests/test_tgis_backend.py` & `caikit-tgis-backend-0.1.1/tests/test_tgis_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/tests/tgis_mock.py` & `caikit-tgis-backend-0.1.1/tests/tgis_mock.py`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/tox.ini` & `caikit-tgis-backend-0.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.0/PKG-INFO` & `caikit-tgis-backend-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: caikit-tgis-backend
-Version: 0.1.0
+Version: 0.1.1
 Summary: Caikit module backend for models run in TGIS
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: caikit>=0.2.0,<0.3.0
+Requires-Dist: caikit>=0.2.0,<0.4.0
 Requires-Dist: grpcio>=1.35.0,<2.0
 Requires-Dist: requests>=2.28.2,<3
 Project-URL: Source, https://github.com/caikit/caikit-tgis-backend
 
 ## Caikit Text Generation Inference Service (TGIS) Backend
 
 This project provides a Caikit module backend that manages models run in TGIS
```

