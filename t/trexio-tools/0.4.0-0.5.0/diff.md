# Comparing `tmp/trexio-tools-0.4.0.tar.gz` & `tmp/trexio-tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trexio-tools-0.4.0.tar", last modified: Thu Jun 16 14:27:59 2022, max compression
+gzip compressed data, was "trexio-tools-0.5.0.tar", last modified: Thu May  4 13:24:08 2023, max compression
```

## Comparing `trexio-tools-0.4.0.tar` & `trexio-tools-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:27:59.057443 trexio-tools-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2275 2022-06-16 14:27:59.057443 trexio-tools-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1730 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-06-16 14:27:59.057443 trexio-tools-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:27:59.053443 trexio-tools-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:27:59.053443 trexio-tools-0.4.0/src/converters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/src/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28003 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/src/converters/cart_sphe.py
--rw-r--r--   0 runner    (1001) docker     (121)     6726 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/src/converters/convert_back_end.py
--rw-r--r--   0 runner    (1001) docker     (121)    13802 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/src/converters/convert_from.py
--rw-r--r--   0 runner    (1001) docker     (121)     8665 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/src/converters/convert_to.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:27:59.053443 trexio-tools-0.4.0/src/group_tools/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/src/group_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2815 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/src/group_tools/ao.py
--rw-r--r--   0 runner    (1001) docker     (121)     3543 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/src/group_tools/basis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/src/group_tools/check_basis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/src/group_tools/check_mos.py
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/src/group_tools/determinant.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/src/group_tools/mo.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/src/group_tools/nucleus.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:27:59.053443 trexio-tools-0.4.0/src/trexio_tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/src/trexio_tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4099 2022-06-16 14:27:46.000000 trexio-tools-0.4.0/src/trexio_tools/trexio_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:27:59.057443 trexio-tools-0.4.0/src/trexio_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2275 2022-06-16 14:27:58.000000 trexio-tools-0.4.0/src/trexio_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-06-16 14:27:59.000000 trexio-tools-0.4.0/src/trexio_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-16 14:27:58.000000 trexio-tools-0.4.0/src/trexio_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-06-16 14:27:58.000000 trexio-tools-0.4.0/src/trexio_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-16 14:27:57.000000 trexio-tools-0.4.0/src/trexio_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-06-16 14:27:58.000000 trexio-tools-0.4.0/src/trexio_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-06-16 14:27:58.000000 trexio-tools-0.4.0/src/trexio_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:24:08.914435 trexio-tools-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-04 13:24:08.914435 trexio-tools-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-04 13:24:08.914435 trexio-tools-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:24:08.910435 trexio-tools-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:24:08.910435 trexio-tools-0.5.0/src/trexio_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:24:08.910435 trexio-tools-0.5.0/src/trexio_tools/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38003 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/converters/cart_sphe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/converters/convert_back_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24649 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/converters/convert_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/converters/convert_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26677 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/converters/pyscf_to_trexio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:24:08.914435 trexio-tools-0.5.0/src/trexio_tools/group_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/group_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/group_tools/ao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/group_tools/basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/group_tools/check_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/group_tools/check_mos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/group_tools/determinant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/group_tools/mo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/group_tools/nucleus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4316 2023-05-04 13:23:59.000000 trexio-tools-0.5.0/src/trexio_tools/trexio_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:24:08.910435 trexio-tools-0.5.0/src/trexio_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-04 13:24:08.000000 trexio-tools-0.5.0/src/trexio_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-04 13:24:08.000000 trexio-tools-0.5.0/src/trexio_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:24:08.000000 trexio-tools-0.5.0/src/trexio_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 13:24:08.000000 trexio-tools-0.5.0/src/trexio_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:24:08.000000 trexio-tools-0.5.0/src/trexio_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 13:24:08.000000 trexio-tools-0.5.0/src/trexio_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 13:24:08.000000 trexio-tools-0.5.0/src/trexio_tools.egg-info/top_level.txt
```

### Comparing `trexio-tools-0.4.0/LICENSE` & `trexio-tools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trexio-tools-0.4.0/PKG-INFO` & `trexio-tools-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trexio-tools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Set of tools for TREXIO files
 Home-page: https://github.com/TREX-CoE/trexio_tools
 Author: TREX-CoE
 Author-email: posenitskiy@irsamc.ups-tlse.fr
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/TREX-CoE/trexio_tools/issues
 Classifier: Programming Language :: Python :: 3
@@ -24,35 +24,35 @@
 ## Requirements
 
 - python3 (>=3.6)
 - trexio (>=1.0.0) [Python API]
 - numpy (>=1.17.3)
 - resultsFile [for GAMESS/GAU$$IAN conversion]
 - docopt [for CLI]
+- pyscf [only if you use the pyscf->trexio converter]
 
 
 ## Installation
 
-0. Clone the repository
+### Installation via PyPI, periodically updated
+
+`pip install trexio-tools` 
+
+### Installation from source code
+
+1. Clone the repository
 - `git clone https://github.com/TREX-CoE/trexio_tools.git`
-1. Create an isolated virtual environment, for example using
+2. Create an isolated virtual environment, for example using
 - `python3 -m venv trexio_tools`
-2. Activate the previously created environment, for example using
+3. Activate the previously created environment, for example using
 - `source trexio_tools/bin/activate`
-3. Install/upgrade the Python setup tools
-- `pip install --upgrade setuptools wheel build`
 4. Install the Python packages that are required for `trexio-tools` to work
 - `pip install -r requirements.txt`
-5. Install the `trexio-tools` package using one of the following methods:
-- `pip install trexio-tools` (installation from PyPI, periodically updated)
-- `pip install .` (installation from source, always contains recent updates)
-
-Only the last step has to be repeated to upgrade the `trexio-tools` package.
-This means that the virtual environment can stay the same, unless there have been
-critical updates in `trexio` or `resultsFile` packages.
+5. Install `trexio-tools` via `pip` (also works in `--editable` mode)
+- `pip install .` 
 
 
 ## Instructions for users
 
 After installation, `trexio-tools` provides an entry point, which can be accessed via CLI:
 
 `trexio --help`
```

### Comparing `trexio-tools-0.4.0/README.md` & `trexio-tools-0.5.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 ## Requirements
 
 - python3 (>=3.6)
 - trexio (>=1.0.0) [Python API]
 - numpy (>=1.17.3)
 - resultsFile [for GAMESS/GAU$$IAN conversion]
 - docopt [for CLI]
+- pyscf [only if you use the pyscf->trexio converter]
 
 
 ## Installation
 
-0. Clone the repository
+### Installation via PyPI, periodically updated
+
+`pip install trexio-tools` 
+
+### Installation from source code
+
+1. Clone the repository
 - `git clone https://github.com/TREX-CoE/trexio_tools.git`
-1. Create an isolated virtual environment, for example using
+2. Create an isolated virtual environment, for example using
 - `python3 -m venv trexio_tools`
-2. Activate the previously created environment, for example using
+3. Activate the previously created environment, for example using
 - `source trexio_tools/bin/activate`
-3. Install/upgrade the Python setup tools
-- `pip install --upgrade setuptools wheel build`
 4. Install the Python packages that are required for `trexio-tools` to work
 - `pip install -r requirements.txt`
-5. Install the `trexio-tools` package using one of the following methods:
-- `pip install trexio-tools` (installation from PyPI, periodically updated)
-- `pip install .` (installation from source, always contains recent updates)
-
-Only the last step has to be repeated to upgrade the `trexio-tools` package.
-This means that the virtual environment can stay the same, unless there have been
-critical updates in `trexio` or `resultsFile` packages.
+5. Install `trexio-tools` via `pip` (also works in `--editable` mode)
+- `pip install .` 
 
 
 ## Instructions for users
 
 After installation, `trexio-tools` provides an entry point, which can be accessed via CLI:
 
 `trexio --help`
```

### Comparing `trexio-tools-0.4.0/setup.cfg` & `trexio-tools-0.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trexio-tools
-version = 0.4.0
+version = 0.5.0
 author = TREX-CoE
 author_email = posenitskiy@irsamc.ups-tlse.fr
 description = Set of tools for TREXIO files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TREX-CoE/trexio_tools
 project_urls =
```

### Comparing `trexio-tools-0.4.0/src/converters/convert_back_end.py` & `trexio-tools-0.5.0/src/trexio_tools/converters/convert_back_end.py`

 * *Files identical despite different names*

### Comparing `trexio-tools-0.4.0/src/converters/convert_to.py` & `trexio-tools-0.5.0/src/trexio_tools/converters/convert_to.py`

 * *Files 14% similar despite different names*

```diff
@@ -168,127 +168,181 @@
     out_file.write("\n".join(out))
 
     return
 
 
 
 
-def run_cart_phe(inp, filename, cartesian):
+def run_cart_phe(inp, filename, to_cartesian):
     out = trexio.File(filename, 'u', inp.back_end)
 
     shell_ang_mom = trexio.read_basis_shell_ang_mom(inp)
 
-    # Build rotation matrix
+    # Build transformation matrix
     count_sphe = 0
     count_cart = 0
     accu = []
     shell = []
     for i, l in enumerate(shell_ang_mom):
       p, r = count_cart, count_sphe
       (x,y) = cart_sphe.data[l].shape
       count_cart += x
       count_sphe += y
       q, s = count_cart, count_sphe
       accu.append( (l, p,q, r,s) )
-      if cartesian > 0: n = x
+      if to_cartesian != 0: n = x
       else: n = y
       for _ in range(n):
           shell.append(i)
 
+    cart_normalization = np.ones(count_cart)
     R = np.zeros( (count_cart, count_sphe) )
     for (l, p,q, r,s) in accu:
       R[p:q,r:s] = cart_sphe.data[l]
+      cart_normalization[p:q] = cart_sphe.normalization[l]
 
-    if cartesian > 0:
-      R = R.T
-    else:
-      R = np.linalg.pinv(R)
+    S = np.eye(count_sphe)
+
+    ao_num_in  = trexio.read_ao_num(inp)
+
+
+    if to_cartesian == 0:
+        print("Transformation from cartesian to spherical is not implemented")
+        return
+
+#        # See http://users.df.uba.ar/dmitnik/estructura3/bases/biblio/transformationGaussianSpherical.pdf
+#        # If S is the overlap of cartesian functions, R @ S @ R.T = I, so R^{-1} = S @ R.T
+#        if trexio.has_ao_1e_int_overlap(inp):
+#            X = trexio.read_ao_1e_int_overlap(inp)
+#        else:
+#            print("Transformation from Cartesian to Spherical requires AO overlap matrix.")
+#            return -1
+#
+#        S = np.zeros((count_cart, count_cart))
+#        for (l, p,q, r,s) in accu:
+#            S[p:q,p:q] = X[p:q,p:q]
+#
+#        R = R.T @ S
+
+    elif to_cartesian == -1:
+        R = np.eye(ao_num_in)
 
     # Update AOs
-    trexio.write_ao_cartesian(out, cartesian)
-    trexio.write_ao_num(out, len(shell))
+    ao_num_out = R.shape[0]
+    trexio.write_ao_cartesian(out, to_cartesian)
+    trexio.write_ao_num(out, ao_num_out)
     trexio.write_ao_shell(out, shell)
 
+    normalization = np.array( [ 1. ] * ao_num_in )
     if trexio.has_ao_normalization(inp):
-      X = trexio.read_ao_normalization(inp)
-      trexio.write_ao_normalization(out, X @ R)
+      normalization = trexio.read_ao_normalization(inp)
+
+    trexio.write_ao_normalization(out, cart_normalization)
+
+    R_norm_inv = np.array(R)
 
     # Update MOs
     if trexio.has_mo_coefficient(inp):
       X = trexio.read_mo_coefficient(inp)
-      trexio.write_mo_coefficient(out, X @ R )
+      for i in range(R.shape[1]):
+         if normalization[i] != 1.:
+            X[:,i] *= normalization[i]
+      Y  = X @ R.T
+      trexio.write_mo_coefficient(out, Y)
 
     # Update 1e Integrals
     if trexio.has_ao_1e_int_overlap(inp):
       X = trexio.read_ao_1e_int_overlap(inp)
-      trexio.write_ao_1e_int_overlap(out, X @ R)
+      for i in range(R.shape[1]):
+            X[:,i] /= normalization[i]
+      for i in range(R.shape[1]):
+            X[i,:] /= normalization[i]
+      Y = R_norm_inv @ X @ R_norm_inv.T
+      trexio.write_ao_1e_int_overlap(out, Y)
+
 
     if trexio.has_ao_1e_int_kinetic(inp):
       X = trexio.read_ao_1e_int_kinetic(inp)
-      trexio.write_ao_1e_int_kinetic(out, X @ R)
+      for i in range(R.shape[1]):
+         if normalization[i] != 1.:
+            X[:,i] /= normalization[i]
+            X[i,:] /= normalization[i]
+      trexio.write_ao_1e_int_kinetic(out, R_norm_inv @ X @ R_norm_inv.T)
 
     if trexio.has_ao_1e_int_potential_n_e(inp):
       X = trexio.read_ao_1e_int_potential_n_e(inp)
-      trexio.write_ao_1e_int_potential_n_e(out, X @ R)
+      for i in range(R.shape[1]):
+         if normalization[i] != 1.:
+            X[:,i] /= normalization[i]
+            X[i,:] /= normalization[i]
+      trexio.write_ao_1e_int_potential_n_e(out, R_norm_inv @ X @ R_norm_inv.T)
 
     if trexio.has_ao_1e_int_ecp(inp):
       X = trexio.read_ao_1e_int_ecp(inp)
-      trexio.write_ao_1e_int_ecp(out, X @ R)
+      for i in range(R.shape[1]):
+         if normalization[i] != 1.:
+            X[:,i] /= normalization[i]
+            X[i,:] /= normalization[i]
+      trexio.write_ao_1e_int_ecp(out, R_norm_inv @ X @ R_norm_inv.T)
 
     if trexio.has_ao_1e_int_core_hamiltonian(inp):
       X = trexio.read_ao_1e_int_core_hamiltonian(inp)
-      trexio.write_ao_1e_int_core_hamiltonian(out, X @ R)
+      for i in range(R.shape[1]):
+         if normalization[i] != 1.:
+            X[:,i] /= normalization[i]
+            X[i,:] /= normalization[i]
+      trexio.write_ao_1e_int_core_hamiltonian(out, R_norm_inv @ X @ R_norm_inv.T)
 
-    # Remove 2e integrals
+    # Remove 2e integrals: too expensive to transform
     if trexio.has_ao_2e_int_eri(inp):
+      print("Warning: Two-electron integrals are not converted")
       trexio.delete_ao_2e_int_eri(out)
 
     if trexio.has_ao_2e_int_eri_lr(inp):
       trexio.delete_ao_2e_int_eri_lr(out)
 
 
+def run_normalized_aos(t, filename):
+    # Start by copying the file
+    os.system('cp -r %s %s' % (t.filename, filename))
+    run_cart_phe(t, filename, to_cartesian=-1)
+    return
+
+
 def run_cartesian(t, filename):
     # Start by copying the file
-    os.system('cp %s %s' % (t.filename, filename))
+    os.system('cp -r %s %s' % (t.filename, filename))
     cartesian = trexio.read_ao_cartesian(t)
     if cartesian > 0:
         return
 
-    run_cart_phe(t, filename, cartesian=1)
+    run_cart_phe(t, filename, to_cartesian=1)
     return
 
-
 def run_spherical(t, filename):
     # Start by copying the file
-    os.system('cp %s %s' % (t.filename, filename))
+    os.system('cp -r %s %s' % (t.filename, filename))
     cartesian = trexio.read_ao_cartesian(t)
     if cartesian == 0:
         return
 
-    run_cart_phe(t, filename, cartesian=0)
+    run_cart_phe(t, filename, to_cartesian=0)
     return
 
 
-
 def run(trexio_filename, filename, filetype):
 
-    try:
-        trexio_file = trexio.File(trexio_filename,mode='r',back_end=trexio.TREXIO_TEXT)
-    except:
-        trexio_file = trexio.File(trexio_filename,mode='r',back_end=trexio.TREXIO_HDF5)
+    trexio_file = trexio.File(trexio_filename,mode='r',back_end=trexio.TREXIO_AUTO)
 
     if filetype.lower() == "molden":
         run_molden(trexio_file, filename)
     elif filetype.lower() == "cartesian":
         run_cartesian(trexio_file, filename)
     elif filetype.lower() == "spherical":
         run_spherical(trexio_file, filename)
-#    elif filetype.lower() == "gamess":
-#    elif filetype.lower() == "gamess":
-#        run_resultsFile(trexio_file, filename)
+#    elif filetype.lower() == "normalized_aos":
+#        run_normalized_aos(trexio_file, filename)
 #    elif filetype.lower() == "fcidump":
 #        run_fcidump(trexio_file, filename)
-#    elif filetype.lower() == "molden":
-#        run_fcidump(trexio_file, filename)
     else:
-        raise TypeError("Unknown file type")
+        raise NotImplementedError(f"Conversion from TREXIO to {filetype} is not supported.")
```

### Comparing `trexio-tools-0.4.0/src/group_tools/ao.py` & `trexio-tools-0.5.0/src/trexio_tools/group_tools/ao.py`

 * *Files identical despite different names*

### Comparing `trexio-tools-0.4.0/src/group_tools/basis.py` & `trexio-tools-0.5.0/src/trexio_tools/group_tools/basis.py`

 * *Files identical despite different names*

### Comparing `trexio-tools-0.4.0/src/group_tools/check_basis.py` & `trexio-tools-0.5.0/src/trexio_tools/group_tools/check_basis.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,57 +2,120 @@
 
 import trexio
 import numpy as np
 from . import nucleus as trexio_nucleus
 from . import basis as trexio_basis
 from . import ao as trexio_ao
 
-def run(trexio_file, n_points):
-    """
-    Computes numerically the overlap matrix in the AO basis and compares it to
-    the matrix stored in the file.
-    """
-
-    if not trexio.has_ao_1e_int_overlap(trexio_file):
-      raise Exception(
-        "One-electron overlap integrals are missing in the TREXIO file. Required for check-basis."
-        )
-
-    ao = trexio_ao.read(trexio_file)
-    basis = ao["basis"]
-    nucleus = basis["nucleus"]
-    assert basis["type"] == "Gaussian"
-
-    rmin = np.array( list([ np.min(nucleus["coord"][:,a]) for a in range(3) ]) )
-    rmax = np.array( list([ np.max(nucleus["coord"][:,a]) for a in range(3) ]) )
-
-    shift = np.array([5.,5.,5.])
-    linspace = [ None for i in range(3) ]
-    step = [ None for i in range(3) ]
-    for a in range(3):
-      linspace[a], step[a] = np.linspace(rmin[a]-shift[a], rmax[a]+shift[a], num=n_points, retstep=True)
-      
-    print("Integration steps:", step)
-    dv = step[0]*step[1]*step[2]
-
-    S = np.zeros( [ ao["num"], ao["num"]] )
-    for x in linspace[0]:
-      #print(".",end='',flush=True)
-      for y in linspace[1]:
-        for z in linspace[2]:
-           chi = trexio_ao.value(ao, np.array( [x,y,z] ) )
-           S += np.outer(chi, chi)*dv
-    print()
-
-    ao_num = ao["num"]
-    S_ex = trexio.read_ao_1e_int_overlap(trexio_file)
-    S_diff = S - S_ex
-    print("Norm of the error: %f"%(np.linalg.norm(S_diff)))
-    #print(S_diff)
-
-    # This produces a lot of output for large molecules, maybe wrap up in ``if debug`` statement ?
-    for i in range(ao_num):
-      for j in range(i,ao_num):
-        print("%3d %3d %15f %15f"%(i,j,S[i][j],S_ex[i,j]))
+try:
+    import qmckl
+    def run(trexio_file, n_points):
+        """
+        Computes numerically the overlap matrix in the AO basis and compares it to
+        the matrix stored in the file.
+        """
+
+        if not trexio.has_ao_1e_int_overlap(trexio_file):
+          raise Exception(
+            "One-electron overlap integrals are missing in the TREXIO file. Required for check-basis."
+            )
+
+        trexio_filename = trexio_file.filename
+        context = qmckl.context_create()
+        qmckl.trexio_read(context, trexio_filename)
+
+        ao = trexio_ao.read(trexio_file)
+        basis = ao["basis"]
+        nucleus = basis["nucleus"]
+        assert basis["type"] == "Gaussian"
+
+        rmin = np.array( list([ np.min(nucleus["coord"][:,a]) for a in range(3) ]) )
+        rmax = np.array( list([ np.max(nucleus["coord"][:,a]) for a in range(3) ]) )
+
+        shift = np.array([8.,8.,8.])
+        linspace = [ None for i in range(3) ]
+        step = [ None for i in range(3) ]
+        for a in range(3):
+          linspace[a], step[a] = np.linspace(rmin[a]-shift[a], rmax[a]+shift[a], num=n_points, retstep=True)
+
+        print("Integration steps:", step)
+        dv = step[0]*step[1]*step[2]
+
+        point = []
+        for x in linspace[0]:
+          #print(".",end='',flush=True)
+          for y in linspace[1]:
+            for z in linspace[2]:
+               point += [ [x, y, z] ]
+        point = np.array(point)
+        point_num = len(point)
+        ao_num = ao["num"]
+
+        qmckl.set_point(context, 'N', point_num, np.reshape(point, (point_num*3)))
+        chi = qmckl.get_ao_basis_ao_value(context, point_num*ao_num)
+        chi = np.reshape( chi, (point_num,ao_num) )
+        S = chi.T @ chi * dv
+        print()
+
+        S_ex = trexio.read_ao_1e_int_overlap(trexio_file)
+
+        # This produces a lot of output for large molecules, maybe wrap up in ``if debug`` statement ?
+        for i in range(ao_num):
+          for j in range(i,ao_num):
+            print("%3d %3d %15f %15f"%(i,j,S[i,j],S_ex[i,j]))
+        S_diff = S - S_ex
+        print("Norm of the error: %f"%(np.linalg.norm(S_diff)))
+
+
+
+
+except ImportError:
+
+    def run(trexio_file, n_points):
+        """
+        Computes numerically the overlap matrix in the AO basis and compares it to
+        the matrix stored in the file.
+        """
+
+        if not trexio.has_ao_1e_int_overlap(trexio_file):
+          raise Exception(
+            "One-electron overlap integrals are missing in the TREXIO file. Required for check-basis."
+            )
+
+        ao = trexio_ao.read(trexio_file)
+        basis = ao["basis"]
+        nucleus = basis["nucleus"]
+        assert basis["type"] == "Gaussian"
+
+        rmin = np.array( list([ np.min(nucleus["coord"][:,a]) for a in range(3) ]) )
+        rmax = np.array( list([ np.max(nucleus["coord"][:,a]) for a in range(3) ]) )
+
+        shift = np.array([8.,8.,8.])
+        linspace = [ None for i in range(3) ]
+        step = [ None for i in range(3) ]
+        for a in range(3):
+          linspace[a], step[a] = np.linspace(rmin[a]-shift[a], rmax[a]+shift[a], num=n_points, retstep=True)
+
+        print("Integration steps:", step)
+        dv = step[0]*step[1]*step[2]
+
+        S = np.zeros( [ ao["num"], ao["num"]] )
+        for x in linspace[0]:
+          #print(".",end='',flush=True)
+          for y in linspace[1]:
+            for z in linspace[2]:
+               chi = trexio_ao.value(ao, np.array( [x,y,z] ) )
+               S += np.outer(chi, chi)*dv
+        print()
+
+        S_ex = trexio.read_ao_1e_int_overlap(trexio_file)
+        ao_num = ao["num"]
+
+        # This produces a lot of output for large molecules, maybe wrap up in ``if debug`` statement ?
+        for i in range(ao_num):
+          for j in range(i,ao_num):
+            print("%3d %3d %15f %15f"%(i,j,S[i][j],S_ex[i,j]))
+        S_diff = S - S_ex
+        print("Norm of the error: %f"%(np.linalg.norm(S_diff)))
```

### Comparing `trexio-tools-0.4.0/src/group_tools/check_mos.py` & `trexio-tools-0.5.0/src/trexio_tools/group_tools/check_mos.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,52 +3,109 @@
 import trexio
 import numpy as np
 from . import nucleus as trexio_nucleus
 from . import basis as trexio_basis
 from . import ao as trexio_ao
 from . import mo as trexio_mo
 
-def run(trexio_file, n_points):
-    """
-    Computes numerically the overlap matrix in the AO basis and compares it to
-    the matrix stored in the file.
-    """
-
-    mo = trexio_mo.read(trexio_file)
-    ao = mo["ao"]
-    basis = ao["basis"]
-    nucleus = basis["nucleus"]
-    assert basis["type"] == "Gaussian"
-
-    rmin = np.array( list([ np.min(nucleus["coord"][:,a]) for a in range(3) ]) )
-    rmax = np.array( list([ np.max(nucleus["coord"][:,a]) for a in range(3) ]) )
-
-    shift = np.array([5.,5.,5.])
-    linspace = [ None for i in range(3) ]
-    step = [ None for i in range(3) ]
-    for a in range(3):
-      linspace[a], step[a] = np.linspace(rmin[a]-shift[a], rmax[a]+shift[a], num=n_points, retstep=True)
-
-    print("Integration steps:", step)
-    dv = step[0]*step[1]*step[2]
-
-    mo_num = mo["num"]
-    S = np.zeros( [ mo_num, mo_num ] )
-    for x in linspace[0]:
-      #print(".",end='',flush=True)
-      for y in linspace[1]:
-        for z in linspace[2]:
-           chi = trexio_mo.value(mo, np.array( [x,y,z] ) )
-           S += np.outer(chi, chi)*dv
-    print()
-
-    S_ex = np.eye(mo_num)
-    S_diff = S - S_ex
-    print ("Norm of the error: %f"%(np.linalg.norm(S_diff)))
-    #print(S_diff)
-
-    for i in range(mo_num):
-      for j in range(i,mo_num):
-        print("%3d %3d %15f %15f"%(i,j,S[i][j],S_ex[i,j]))
+try:
+    import qmckl
+    def run(trexio_file, n_points):
+        """
+        Computes numerically the overlap matrix in the AO basis and compares it to
+        the matrix stored in the file.
+        """
+
+        trexio_filename = trexio_file.filename
+        context = qmckl.context_create()
+        qmckl.trexio_read(context, trexio_filename)
+
+        mo = trexio_mo.read(trexio_file)
+        ao = mo["ao"]
+        basis = ao["basis"]
+        nucleus = basis["nucleus"]
+        assert basis["type"] == "Gaussian"
+
+        rmin = np.array( list([ np.min(nucleus["coord"][:,a]) for a in range(3) ]) )
+        rmax = np.array( list([ np.max(nucleus["coord"][:,a]) for a in range(3) ]) )
+
+        shift = np.array([8.,8.,8.])
+        linspace = [ None for i in range(3) ]
+        step = [ None for i in range(3) ]
+        for a in range(3):
+          linspace[a], step[a] = np.linspace(rmin[a]-shift[a], rmax[a]+shift[a], num=n_points, retstep=True)
+
+        print("Integration steps:", step)
+        dv = step[0]*step[1]*step[2]
+
+        point = []
+        for x in linspace[0]:
+          #print(".",end='',flush=True)
+          for y in linspace[1]:
+            for z in linspace[2]:
+               point += [ [x, y, z] ]
+        point = np.array(point)
+        point_num = len(point)
+        mo_num = mo["num"]
+
+        qmckl.set_point(context, 'N', point_num, np.reshape(point, (point_num*3)))
+        chi = qmckl.get_mo_basis_mo_value(context, point_num*mo_num)
+        chi = np.reshape( chi, (point_num,mo_num) )
+        S = chi.T @ chi * dv
+        print()
+
+        S_ex = np.eye(mo_num)
+
+        for i in range(mo_num):
+          for j in range(i,mo_num):
+            print("%3d %3d %15f %15f"%(i,j,S[i][j],S_ex[i,j]))
+        S_diff = S - S_ex
+        print ("Norm of the error: %f"%(np.linalg.norm(S_diff)))
+
+except ImportError:
+
+    def run(trexio_file, n_points):
+        """
+        Computes numerically the overlap matrix in the AO basis and compares it to
+        the matrix stored in the file.
+        """
+
+        mo = trexio_mo.read(trexio_file)
+        ao = mo["ao"]
+        basis = ao["basis"]
+        nucleus = basis["nucleus"]
+        assert basis["type"] == "Gaussian"
+
+        rmin = np.array( list([ np.min(nucleus["coord"][:,a]) for a in range(3) ]) )
+        rmax = np.array( list([ np.max(nucleus["coord"][:,a]) for a in range(3) ]) )
+
+        shift = np.array([8.,8.,8.])
+        linspace = [ None for i in range(3) ]
+        step = [ None for i in range(3) ]
+        for a in range(3):
+          linspace[a], step[a] = np.linspace(rmin[a]-shift[a], rmax[a]+shift[a], num=n_points, retstep=True)
+
+        print("Integration steps:", step)
+        dv = step[0]*step[1]*step[2]
+
+        mo_num = mo["num"]
+        S = np.zeros( [ mo_num, mo_num ] )
+        for x in linspace[0]:
+          #print(".",end='',flush=True)
+          for y in linspace[1]:
+            for z in linspace[2]:
+               chi = trexio_mo.value(mo, np.array( [x,y,z] ) )
+               S += np.outer(chi, chi)*dv
+        print()
+
+        S_ex = np.eye(mo_num)
+        S_diff = S - S_ex
+        print ("%e %e"%(np.linalg.norm(S), np.linalg.norm(S_ex) ))
+        print ("Norm of the error: %e"%(np.linalg.norm(S_diff)))
+        #print(S_diff)
+
+        for i in range(mo_num):
+          for j in range(i,mo_num):
+            print("%3d %3d %15f %15f"%(i,j,S[i][j],S_ex[i,j]))
```

### Comparing `trexio-tools-0.4.0/src/group_tools/determinant.py` & `trexio-tools-0.5.0/src/trexio_tools/group_tools/determinant.py`

 * *Files identical despite different names*

### Comparing `trexio-tools-0.4.0/src/group_tools/mo.py` & `trexio-tools-0.5.0/src/trexio_tools/group_tools/mo.py`

 * *Files identical despite different names*

### Comparing `trexio-tools-0.4.0/src/trexio_tools/trexio_run.py` & `trexio-tools-0.5.0/src/trexio_tools/trexio_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 """
 Set of tools to interact with trexio files.
 
 Usage:
       trexio check-basis      [-n N_POINTS]  [-b BACK_END]  TREXIO_FILE
       trexio check-mos        [-n N_POINTS]  [-b BACK_END]  TREXIO_FILE
       trexio convert-to       -t TYPE -o OUTPUT_FILE        TREXIO_FILE
-      trexio convert-from     -t TYPE -i INPUT_FILE  [-b BACK_END]  TREXIO_FILE
+      trexio convert-from     -t TYPE -i INPUT_FILE  [-b BACK_END]  [-x MO_TYPE]  TREXIO_FILE
       trexio convert-backend  -i INPUT_FILE  -o OUTPUT_FILE  -b BACK_END  -j TREX_JSON_FILE  [-s BACK_END_FROM]  [-w OVERWRITE]
       trexio (-h | --help)
 
 Options:
       -h, --help                    Print help message.
       -n, --n_points=N_POINTS       Number of integration points.  [default: 81]
       -i, --input=INPUT_FILE        Name of the input file.
       -o, --output=OUTPUT_FILE      Name of the output file.
-      -b, --back_end=BACK_END       [hdf5 | text]  The TREXIO back end.  [default: hdf5]
+      -b, --back_end=BACK_END       [hdf5 | text | auto]  The TREXIO back end.  [default: hdf5]
       -s, --back_end_from=BACK_END  [hdf5 | text | auto]  The input TREXIO back end.  [default: auto]
       -j, --json=TREX_JSON_FILE     TREX configuration file (in JSON format).
       -w, --overwrite=OVERWRITE     Overwrite flag for the conversion of back ends.  [default: True]
-      -t, --type=TYPE               [gaussian | gamess | fcidump | molden | cartesian | spherical ] File format.
+      -t, --type=TYPE               [gaussian | gamess | pyscf | fcidump | molden | cartesian ] File format.
+      -x, --motype=MO_TYPE          [natural | initial | guga-initial | guga-natural] The type of the molecular orbitals.
 """
 
 from docopt import docopt
 import trexio
 import os
 
 
@@ -47,21 +48,21 @@
             print(f'File {args["--output"]} will be overwritten.')
 
     if args["--back_end"]:
         if str(args["--back_end"]).lower() == "hdf5":
             back_end = trexio.TREXIO_HDF5
         elif str(args["--back_end"]).lower() == "text":
             back_end = trexio.TREXIO_TEXT
+        elif str(args["--back_end"]).lower() == "auto":
+            back_end = trexio.TREXIO_AUTO
         else:
-            raise ValueError("Supported back ends: text, hdf5.")
+            raise ValueError("Supported back ends: text, hdf5, auto.")
     else:
         if args["convert-backend"]:
             raise Exception("Missing argument for the target back end: specify --back_end or -b.")
-        else:
-            back_end = trexio.TREXIO_HDF5
 
     if args["--back_end_from"]:
         if str(args["--back_end_from"]).lower() == "hdf5":
             back_end_from = trexio.TREXIO_HDF5
         elif str(args["--back_end_from"]).lower() == "text":
             back_end_from = trexio.TREXIO_TEXT
         elif str(args["--back_end_from"]).lower() == "auto":
@@ -73,35 +74,35 @@
 
 
     if args["check-basis"]:
         trexio_file = trexio.File(filename, 'r', back_end=back_end)
         if trexio_file is None:
             raise IOError
 
-        from group_tools.check_basis import run
+        from .group_tools.check_basis import run
         run(trexio_file,n_points)
 
     elif args["check-mos"]:
         trexio_file = trexio.File(filename, 'r', back_end=back_end)
         if trexio_file is None:
             raise IOError
 
-        from group_tools.check_mos import run
+        from .group_tools.check_mos import run
         run(trexio_file,n_points)
 
     elif args["convert-from"]:
-        from converters.convert_from import run
-        run(args["TREXIO_FILE"], args["--input"], args["--type"], back_end=back_end)
+        from .converters.convert_from import run
+        run(args["TREXIO_FILE"], args["--input"], args["--type"], back_end=back_end, motype=args["--motype"])
 
     elif args["convert-to"]:
-        from converters.convert_to import run
+        from .converters.convert_to import run
         run(args["TREXIO_FILE"], args["--output"], args["--type"])
 
     elif args["convert-backend"]:
-        from converters.convert_back_end import run
+        from .converters.convert_back_end import run
         run(
             args["--input"],
             args["--output"],
             back_end_to=back_end,
             back_end_from=back_end_from,
             overwrite=overwrite,
             json_filename=args["--json"]
```

### Comparing `trexio-tools-0.4.0/src/trexio_tools.egg-info/PKG-INFO` & `trexio-tools-0.5.0/src/trexio_tools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trexio-tools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Set of tools for TREXIO files
 Home-page: https://github.com/TREX-CoE/trexio_tools
 Author: TREX-CoE
 Author-email: posenitskiy@irsamc.ups-tlse.fr
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/TREX-CoE/trexio_tools/issues
 Classifier: Programming Language :: Python :: 3
@@ -24,35 +24,35 @@
 ## Requirements
 
 - python3 (>=3.6)
 - trexio (>=1.0.0) [Python API]
 - numpy (>=1.17.3)
 - resultsFile [for GAMESS/GAU$$IAN conversion]
 - docopt [for CLI]
+- pyscf [only if you use the pyscf->trexio converter]
 
 
 ## Installation
 
-0. Clone the repository
+### Installation via PyPI, periodically updated
+
+`pip install trexio-tools` 
+
+### Installation from source code
+
+1. Clone the repository
 - `git clone https://github.com/TREX-CoE/trexio_tools.git`
-1. Create an isolated virtual environment, for example using
+2. Create an isolated virtual environment, for example using
 - `python3 -m venv trexio_tools`
-2. Activate the previously created environment, for example using
+3. Activate the previously created environment, for example using
 - `source trexio_tools/bin/activate`
-3. Install/upgrade the Python setup tools
-- `pip install --upgrade setuptools wheel build`
 4. Install the Python packages that are required for `trexio-tools` to work
 - `pip install -r requirements.txt`
-5. Install the `trexio-tools` package using one of the following methods:
-- `pip install trexio-tools` (installation from PyPI, periodically updated)
-- `pip install .` (installation from source, always contains recent updates)
-
-Only the last step has to be repeated to upgrade the `trexio-tools` package.
-This means that the virtual environment can stay the same, unless there have been
-critical updates in `trexio` or `resultsFile` packages.
+5. Install `trexio-tools` via `pip` (also works in `--editable` mode)
+- `pip install .` 
 
 
 ## Instructions for users
 
 After installation, `trexio-tools` provides an entry point, which can be accessed via CLI:
 
 `trexio --help`
```

### Comparing `trexio-tools-0.4.0/src/trexio_tools.egg-info/SOURCES.txt` & `trexio-tools-0.5.0/src/trexio_tools.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
-src/converters/__init__.py
-src/converters/cart_sphe.py
-src/converters/convert_back_end.py
-src/converters/convert_from.py
-src/converters/convert_to.py
-src/group_tools/__init__.py
-src/group_tools/ao.py
-src/group_tools/basis.py
-src/group_tools/check_basis.py
-src/group_tools/check_mos.py
-src/group_tools/determinant.py
-src/group_tools/mo.py
-src/group_tools/nucleus.py
 src/trexio_tools/__init__.py
 src/trexio_tools/trexio_run.py
 src/trexio_tools.egg-info/PKG-INFO
 src/trexio_tools.egg-info/SOURCES.txt
 src/trexio_tools.egg-info/dependency_links.txt
 src/trexio_tools.egg-info/entry_points.txt
 src/trexio_tools.egg-info/not-zip-safe
 src/trexio_tools.egg-info/requires.txt
-src/trexio_tools.egg-info/top_level.txt
+src/trexio_tools.egg-info/top_level.txt
+src/trexio_tools/converters/__init__.py
+src/trexio_tools/converters/cart_sphe.py
+src/trexio_tools/converters/convert_back_end.py
+src/trexio_tools/converters/convert_from.py
+src/trexio_tools/converters/convert_to.py
+src/trexio_tools/converters/pyscf_to_trexio.py
+src/trexio_tools/group_tools/__init__.py
+src/trexio_tools/group_tools/ao.py
+src/trexio_tools/group_tools/basis.py
+src/trexio_tools/group_tools/check_basis.py
+src/trexio_tools/group_tools/check_mos.py
+src/trexio_tools/group_tools/determinant.py
+src/trexio_tools/group_tools/mo.py
+src/trexio_tools/group_tools/nucleus.py
```

