# Comparing `tmp/pywaterflood-0.3.0.tar.gz` & `tmp/pywaterflood-0.3.0rc1.tar.gz`

## Comparing `pywaterflood-0.3.0.tar` & `pywaterflood-0.3.0rc1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      326 1970-01-01 00:00:00.000000 pywaterflood-0.3.0/Cargo.toml
--rw-r--r--   0     1001      123     1239 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/.dockerignore
--rw-r--r--   0     1001      123       68 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/.git-blame-ignore-revs
--rw-r--r--   0     1001      123      317 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/.github/dependabot.yml
--rw-r--r--   0     1001      123     2762 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0     1001      123     1174 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/.github/workflows/tests.yml
--rw-r--r--   0     1001      123     2121 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/.gitignore
--rw-r--r--   0     1001      123     1870 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      123      194 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/.readthedocs.yml
--rw-r--r--   0     1001      123      547 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/CHANGELOG.md
--rw-r--r--   0     1001      123     3053 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/CONDUCT.md
--rw-r--r--   0     1001      123     2481 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/CONTRIBUTING.md
--rw-r--r--   0     1001      123      497 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/Dockerfile
--rw-r--r--   0     1001      123     1326 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/LICENSE
--rw-r--r--   0     1001      123     2983 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/README.md
--rw-r--r--   0     1001      123      668 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/docs/Makefile
--rw-r--r--   0     1001      123       34 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/docs/changelog.md
--rw-r--r--   0     1001      123       32 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/docs/conduct.md
--rw-r--r--   0     1001      123     1616 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/docs/conf.py
--rw-r--r--   0     1001      123       37 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/docs/contributing.md
--rw-r--r--   0     1001      123   191830 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/docs/example.ipynb
--rw-r--r--   0     1001      123      724 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/docs/index.md
--rw-r--r--   0     1001      123     1721 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/noxfile.py
--rw-r--r--   0     1001      123     2945 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/pyproject.toml
--rw-r--r--   0     1001      123      807 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/pywaterflood/__init__.py
--rw-r--r--   0     1001      123    27993 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/pywaterflood/crm.py
--rw-r--r--   0     1001      123     5445 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/pywaterflood/multiwellproductivity.py
--rw-r--r--   0     1001      123      153 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/requirements.yml
--rw-r--r--   0     1001      123     5208 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/__init__.py
--rw-r--r--   0     1001      123       79 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/conftest.py
--rw-r--r--   0     1001      123      104 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/data/gain_producer.csv
--rw-r--r--   0     1001      123      504 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/data/gains.csv
--rw-r--r--   0     1001      123    37548 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/data/injection.csv
--rw-r--r--   0     1001      123    29800 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/data/prediction_noprimary_per-pair.csv
--rw-r--r--   0     1001      123    29800 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/data/prediction_noprimary_per-producer.csv
--rw-r--r--   0     1001      123    29800 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/data/prediction_primary_per-pair.csv
--rw-r--r--   0     1001      123    29800 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/data/prediction_primary_per-producer.csv
--rw-r--r--   0     1001      123    30098 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/data/production.csv
--rw-r--r--   0     1001      123      104 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/data/tau_producer.csv
--rw-r--r--   0     1001      123      104 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/data/taus.csv
--rw-r--r--   0     1001      123      504 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/data/taus_per-pair.csv
--rw-r--r--   0     1001      123     7748 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/data/time.csv
--rw-r--r--   0     1001      123     1971 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/regenerate_results.py
--rw-r--r--   0     1001      123    14400 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/test_CRM.py
--rw-r--r--   0     1001      123     3926 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/testing/test_mpi.py
--rw-r--r--   0     1001      123     8413 2023-05-04 01:42:55.000000 pywaterflood-0.3.0/Cargo.lock
--rw-r--r--   0        0        0     4438 1970-01-01 00:00:00.000000 pywaterflood-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      326 1970-01-01 00:00:00.000000 pywaterflood-0.3.0rc1/Cargo.toml
+-rw-r--r--   0     1001      123     1239 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/.dockerignore
+-rw-r--r--   0     1001      123       68 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/.git-blame-ignore-revs
+-rw-r--r--   0     1001      123      317 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/.github/dependabot.yml
+-rw-r--r--   0     1001      123     2684 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0     1001      123     1174 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/.github/workflows/tests.yml
+-rw-r--r--   0     1001      123     2121 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/.gitignore
+-rw-r--r--   0     1001      123     1870 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123      194 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/.readthedocs.yml
+-rw-r--r--   0     1001      123      547 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/CHANGELOG.md
+-rw-r--r--   0     1001      123     3053 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/CONDUCT.md
+-rw-r--r--   0     1001      123     2481 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/CONTRIBUTING.md
+-rw-r--r--   0     1001      123      497 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/Dockerfile
+-rw-r--r--   0     1001      123     1326 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/LICENSE
+-rw-r--r--   0     1001      123     2983 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/README.md
+-rw-r--r--   0     1001      123      668 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/docs/Makefile
+-rw-r--r--   0     1001      123       34 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/docs/changelog.md
+-rw-r--r--   0     1001      123       32 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/docs/conduct.md
+-rw-r--r--   0     1001      123     1616 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/docs/conf.py
+-rw-r--r--   0     1001      123       37 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/docs/contributing.md
+-rw-r--r--   0     1001      123   191830 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/docs/example.ipynb
+-rw-r--r--   0     1001      123      724 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/docs/index.md
+-rw-r--r--   0     1001      123     1721 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/noxfile.py
+-rw-r--r--   0     1001      123     2948 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/pyproject.toml
+-rw-r--r--   0     1001      123      807 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/pywaterflood/__init__.py
+-rw-r--r--   0     1001      123    27993 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/pywaterflood/crm.py
+-rw-r--r--   0     1001      123     5445 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/pywaterflood/multiwellproductivity.py
+-rw-r--r--   0     1001      123      153 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/requirements.yml
+-rw-r--r--   0     1001      123     5208 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/__init__.py
+-rw-r--r--   0     1001      123       79 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/conftest.py
+-rw-r--r--   0     1001      123      104 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/data/gain_producer.csv
+-rw-r--r--   0     1001      123      504 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/data/gains.csv
+-rw-r--r--   0     1001      123    37548 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/data/injection.csv
+-rw-r--r--   0     1001      123    29800 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/data/prediction_noprimary_per-pair.csv
+-rw-r--r--   0     1001      123    29800 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/data/prediction_noprimary_per-producer.csv
+-rw-r--r--   0     1001      123    29800 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/data/prediction_primary_per-pair.csv
+-rw-r--r--   0     1001      123    29800 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/data/prediction_primary_per-producer.csv
+-rw-r--r--   0     1001      123    30098 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/data/production.csv
+-rw-r--r--   0     1001      123      104 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/data/tau_producer.csv
+-rw-r--r--   0     1001      123      104 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/data/taus.csv
+-rw-r--r--   0     1001      123      504 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/data/taus_per-pair.csv
+-rw-r--r--   0     1001      123     7748 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/data/time.csv
+-rw-r--r--   0     1001      123     1971 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/regenerate_results.py
+-rw-r--r--   0     1001      123    14400 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/test_CRM.py
+-rw-r--r--   0     1001      123     3926 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/testing/test_mpi.py
+-rw-r--r--   0     1001      123     8413 2023-03-09 04:28:05.000000 pywaterflood-0.3.0rc1/Cargo.lock
+-rw-r--r--   0        0        0     4441 1970-01-01 00:00:00.000000 pywaterflood-0.3.0rc1/PKG-INFO
```

### Comparing `pywaterflood-0.3.0/.dockerignore` & `pywaterflood-0.3.0rc1/.dockerignore`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/.github/workflows/publish-to-pypi.yml` & `pywaterflood-0.3.0rc1/.github/workflows/publish-to-pypi.yml`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "curl https://sh.rustup.rs -sSf | sh -s -- --default-toolchain stable -y"
       CIBW_ENVIRONMENT: 'PATH="$PATH:$HOME/.cargo/bin"'
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.12.3
+        uses: pypa/cibuildwheel@v2.12.0
 
       - uses: actions/upload-artifact@v3
         with:
           path: ./wheelhouse/*.whl
 
   build:
     name: Build source distribution
@@ -48,53 +48,49 @@
       - uses: actions/upload-artifact@v3
         with:
           path: dist/
 
   upload_testpypi:
     needs: [build, build_wheels]
     runs-on: ubuntu-latest
-    permissions:
-      id-token: write
     steps:
       - name: get artifacts
         uses: actions/download-artifact@v3
         with:
           # unpacks default artifact into dist/
           # if `name: artifact` is omitted, the action will create extra parent dir
           name: artifact
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@v1.8.5
+      - uses: pypa/gh-action-pypi-publish@v1.6.4
         with:
           # If you've already pushed this version to TestPyPI, don't fail the job
-          skip-existing: true
+          skip_existing: true
           user: __token__
           password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-          repository-url: https://test.pypi.org/legacy/
+          repository_url: https://test.pypi.org/legacy/
 
   upload_pypi:
     needs: [build, build_wheels]
     runs-on: ubuntu-latest
-    permissions:
-      id-token: write
     # Publish when a GitHub Release is created, use the following rule:
     if: github.event_name == 'release' && github.event.action == 'published'
     steps:
       - name: get artifacts
         uses: actions/download-artifact@v3
         with:
           # unpacks default artifact into dist/
           # if `name: artifact` is omitted, the action will create extra parent dir
           name: artifact
           path: dist
 
       - run: pipx run twine check dist/*
 
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.5
+        uses: pypa/gh-action-pypi-publish@v1.6.4
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
 
       - name: Upload artifacts to release
         uses: softprops/action-gh-release@v1
         with:
```

### Comparing `pywaterflood-0.3.0/.github/workflows/tests.yml` & `pywaterflood-0.3.0rc1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/.gitignore` & `pywaterflood-0.3.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/.pre-commit-config.yaml` & `pywaterflood-0.3.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/CHANGELOG.md` & `pywaterflood-0.3.0rc1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/CONDUCT.md` & `pywaterflood-0.3.0rc1/CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/CONTRIBUTING.md` & `pywaterflood-0.3.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/LICENSE` & `pywaterflood-0.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/README.md` & `pywaterflood-0.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/docs/Makefile` & `pywaterflood-0.3.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/docs/conf.py` & `pywaterflood-0.3.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/docs/example.ipynb` & `pywaterflood-0.3.0rc1/docs/example.ipynb`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/docs/index.md` & `pywaterflood-0.3.0rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/noxfile.py` & `pywaterflood-0.3.0rc1/noxfile.py`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/pyproject.toml` & `pywaterflood-0.3.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pywaterflood"
-version = "0.3.0"
+version = "0.3.0rc1"
 description = "Physics-inspired waterflood performance modeling"
 authors = [{name = "Frank Male", email ="frmale@utexas.edu"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
```

### Comparing `pywaterflood-0.3.0/pywaterflood/__init__.py` & `pywaterflood-0.3.0rc1/pywaterflood/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/pywaterflood/crm.py` & `pywaterflood-0.3.0rc1/pywaterflood/crm.py`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/pywaterflood/multiwellproductivity.py` & `pywaterflood-0.3.0rc1/pywaterflood/multiwellproductivity.py`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/src/lib.rs` & `pywaterflood-0.3.0rc1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/testing/data/injection.csv` & `pywaterflood-0.3.0rc1/testing/data/injection.csv`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/testing/data/prediction_noprimary_per-pair.csv` & `pywaterflood-0.3.0rc1/testing/data/prediction_noprimary_per-pair.csv`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/testing/data/prediction_noprimary_per-producer.csv` & `pywaterflood-0.3.0rc1/testing/data/prediction_noprimary_per-producer.csv`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/testing/data/prediction_primary_per-pair.csv` & `pywaterflood-0.3.0rc1/testing/data/prediction_primary_per-pair.csv`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/testing/data/prediction_primary_per-producer.csv` & `pywaterflood-0.3.0rc1/testing/data/prediction_primary_per-producer.csv`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/testing/data/production.csv` & `pywaterflood-0.3.0rc1/testing/data/production.csv`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/testing/data/time.csv` & `pywaterflood-0.3.0rc1/testing/data/time.csv`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/testing/regenerate_results.py` & `pywaterflood-0.3.0rc1/testing/regenerate_results.py`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/testing/test_CRM.py` & `pywaterflood-0.3.0rc1/testing/test_CRM.py`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/testing/test_mpi.py` & `pywaterflood-0.3.0rc1/testing/test_mpi.py`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/Cargo.lock` & `pywaterflood-0.3.0rc1/Cargo.lock`

 * *Files identical despite different names*

### Comparing `pywaterflood-0.3.0/PKG-INFO` & `pywaterflood-0.3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: pywaterflood
-Version: 0.3.0
+Version: 0.3.0rc1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Dist: numpy >=1.21
 Requires-Dist: scipy >=1.4
 Requires-Dist: pandas >=1.3.5
 Requires-Dist: openpyxl >=3.0.9
 Requires-Dist: joblib >=1.1.0
+Requires-Dist: ipykernel; extra == 'devwork'
+Requires-Dist: seaborn; extra == 'devwork'
 Requires-Dist: myst-nb; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autoapi; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme; extra == 'docs'
 Requires-Dist: pytest >=6.2.5; extra == 'test'
 Requires-Dist: pytest-cov >=3.0.0; extra == 'test'
 Requires-Dist: coverage[toml] >=6.3.3; extra == 'test'
-Requires-Dist: ipykernel; extra == 'devwork'
-Requires-Dist: seaborn; extra == 'devwork'
+Provides-Extra: devwork
 Provides-Extra: docs
 Provides-Extra: test
-Provides-Extra: devwork
 License-File: LICENSE
 Summary: Physics-inspired waterflood performance modeling
 Author-email: Frank Male <frmale@utexas.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Bug Tracker, https://github.com/frank1010111/pywaterflood/issues
 Project-URL: repository, https://github.com/frank1010111/pywaterflood
 Project-URL: documentation, https://pywaterflood.readthedocs.io
-Project-URL: Bug Tracker, https://github.com/frank1010111/pywaterflood/issues
 
 # `pywaterflood`: Waterflood Connectivity Analysis
 
 [![PyPI version](https://badge.fury.io/py/pywaterflood.svg)](https://badge.fury.io/py/pywaterflood)
 [![Documentation Status](https://readthedocs.org/projects/pywaterflood/badge/?version=latest)](https://pywaterflood.readthedocs.io/en/latest/?badge=latest)
 
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
```

