# Comparing `tmp/maturin-1.0.0b7.tar.gz` & `tmp/maturin-1.0.0b8.tar.gz`

## Comparing `maturin-1.0.0b7.tar` & `maturin-1.0.0b8.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     4442 1970-01-01 00:00:00.000000 maturin-1.0.0b7/Cargo.toml
--rw-r--r--   0     1001      123     1693 2023-04-05 13:40:38.000000 maturin-1.0.0b7/.cirrus.yml
--rw-r--r--   0     1001      123       94 2023-04-05 13:40:38.000000 maturin-1.0.0b7/.codespellrc
--rw-r--r--   0     1001      123      252 2023-04-05 13:40:38.000000 maturin-1.0.0b7/.config/nextest.toml
--rw-r--r--   0     1001      123      180 2023-04-05 13:40:38.000000 maturin-1.0.0b7/.dockerignore
--rw-r--r--   0     1001      123      184 2023-04-05 13:40:38.000000 maturin-1.0.0b7/.gitignore
--rw-r--r--   0     1001      123    65636 2023-04-05 13:40:38.000000 maturin-1.0.0b7/Cargo.lock
--rw-r--r--   0     1001      123    55213 2023-04-05 13:40:38.000000 maturin-1.0.0b7/Changelog.md
--rw-r--r--   0     1001      123     3228 2023-04-05 13:40:38.000000 maturin-1.0.0b7/Code-of-Conduct.md
--rw-r--r--   0     1001      123     2386 2023-04-05 13:40:38.000000 maturin-1.0.0b7/Dockerfile
--rw-r--r--   0     1001      123      245 2023-04-05 13:40:38.000000 maturin-1.0.0b7/MANIFEST.in
--rw-r--r--   0     1001      123    16573 2023-04-05 13:40:38.000000 maturin-1.0.0b7/README.md
--rw-r--r--   0     1001      123       16 2023-04-05 13:40:38.000000 maturin-1.0.0b7/clippy.toml
--rw-r--r--   0     1001      123     9664 2023-04-05 13:40:38.000000 maturin-1.0.0b7/deny.toml
--rw-r--r--   0     1001      123    10847 2023-04-05 13:40:38.000000 maturin-1.0.0b7/license-apache
--rw-r--r--   0     1001      123     1051 2023-04-05 13:40:38.000000 maturin-1.0.0b7/license-mit
--rw-r--r--   0     1001      123     6236 2023-04-05 13:40:38.000000 maturin-1.0.0b7/maturin/__init__.py
--rw-r--r--   0     1001      123      956 2023-04-05 13:40:38.000000 maturin-1.0.0b7/maturin/__main__.py
--rw-r--r--   0     1001      123     5162 2023-04-05 13:40:38.000000 maturin-1.0.0b7/maturin/import_hook.py
--rw-r--r--   0     1001      123      200 2023-04-05 13:40:38.000000 maturin-1.0.0b7/netlify.toml
--rw-r--r--   0     1001      123     2170 2023-04-05 13:40:38.000000 maturin-1.0.0b7/noxfile.py
--rw-r--r--   0     1001      123     1290 2023-04-05 13:40:38.000000 maturin-1.0.0b7/pyproject.toml
--rw-r--r--   0     1001      123     2868 2023-04-05 13:40:38.000000 maturin-1.0.0b7/setup.py
--rw-r--r--   0     1001      123    19412 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/auditwheel/audit.rs
--rw-r--r--   0     1001      123    53261 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/auditwheel/manylinux-policy.json
--rw-r--r--   0     1001      123      242 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/auditwheel/mod.rs
--rw-r--r--   0     1001      123     1862 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/auditwheel/musllinux-policy.json
--rw-r--r--   0     1001      123     1389 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/auditwheel/musllinux.rs
--rw-r--r--   0     1001      123     3777 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/auditwheel/patchelf.rs
--rw-r--r--   0     1001      123     4602 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/auditwheel/platform_tag.rs
--rw-r--r--   0     1001      123     5393 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/auditwheel/policy.rs
--rw-r--r--   0     1001      123     1169 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/auditwheel/repair.rs
--rw-r--r--   0     1001      123    47514 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/build_context.rs
--rw-r--r--   0     1001      123    57254 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/build_options.rs
--rw-r--r--   0     1001      123     5407 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/cargo_toml.rs
--rw-r--r--   0     1001      123    33723 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/ci.rs
--rw-r--r--   0     1001      123    23999 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/compile.rs
--rw-r--r--   0     1001      123     8342 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/cross_compile.rs
--rw-r--r--   0     1001      123     6119 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/develop.rs
--rw-r--r--   0     1001      123     2233 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/lib.rs
--rw-r--r--   0     1001      123    17816 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/main.rs
--rw-r--r--   0     1001      123    32034 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/metadata.rs
--rw-r--r--   0     1001      123    44938 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/module_writer.rs
--rw-r--r--   0     1001      123     8203 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/new_project.rs
--rw-r--r--   0     1001      123    16142 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/project_layout.rs
--rw-r--r--   0     1001      123    16408 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/pyproject_toml.rs
--rw-r--r--   0     1001      123    11820 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/python_interpreter/config.rs
--rw-r--r--   0     1001      123     1595 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/python_interpreter/get_interpreter_metadata.py
--rw-r--r--   0     1001      123    34577 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/python_interpreter/mod.rs
--rw-r--r--   0     1001      123      443 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/python_interpreter/sysconfig-emscripten.json
--rw-r--r--   0     1001      123     3861 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/python_interpreter/sysconfig-freebsd.json
--rw-r--r--   0     1001      123    14124 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/python_interpreter/sysconfig-linux.json
--rw-r--r--   0     1001      123     3812 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/python_interpreter/sysconfig-macos.json
--rw-r--r--   0     1001      123      738 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/python_interpreter/sysconfig-netbsd.json
--rw-r--r--   0     1001      123     2353 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/python_interpreter/sysconfig-openbsd.json
--rw-r--r--   0     1001      123     3341 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/python_interpreter/sysconfig-windows.json
--rw-r--r--   0     1001      123    30697 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/source_distribution.rs
--rw-r--r--   0     1001      123    18478 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/target.rs
--rw-r--r--   0     1001      123      686 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/templates/.gitignore.j2
--rw-r--r--   0     1001      123      518 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/templates/Cargo.toml.j2
--rw-r--r--   0     1001      123      149 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/templates/__init__.py.j2
--rw-r--r--   0     1001      123      123 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/templates/build.rs.j2
--rw-r--r--   0     1001      123       47 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/templates/example.udl.j2
--rw-r--r--   0     1001      123      722 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/templates/lib.rs.j2
--rw-r--r--   0     1001      123       45 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/templates/main.rs.j2
--rw-r--r--   0     1001      123      859 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/templates/pyproject.toml.j2
--rw-r--r--   0     1001      123    20146 2023-04-05 13:40:38.000000 maturin-1.0.0b7/src/upload.rs
--rwxr-xr-x   0     1001      123      974 2023-04-05 13:40:38.000000 maturin-1.0.0b7/test-dockerfile.sh
--rw-r--r--   0        0        0    17757 1970-01-01 00:00:00.000000 maturin-1.0.0b7/PKG-INFO
+-rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 maturin-1.0.0b8/Cargo.toml
+-rw-r--r--   0     1001      123     1692 2023-05-04 14:56:10.000000 maturin-1.0.0b8/.cirrus.yml
+-rw-r--r--   0     1001      123       94 2023-05-04 14:56:10.000000 maturin-1.0.0b8/.codespellrc
+-rw-r--r--   0     1001      123      252 2023-05-04 14:56:10.000000 maturin-1.0.0b8/.config/nextest.toml
+-rw-r--r--   0     1001      123      180 2023-05-04 14:56:10.000000 maturin-1.0.0b8/.dockerignore
+-rw-r--r--   0     1001      123      184 2023-05-04 14:56:10.000000 maturin-1.0.0b8/.gitignore
+-rw-r--r--   0     1001      123    65671 2023-05-04 14:56:10.000000 maturin-1.0.0b8/Cargo.lock
+-rw-r--r--   0     1001      123    55621 2023-05-04 14:56:10.000000 maturin-1.0.0b8/Changelog.md
+-rw-r--r--   0     1001      123     3228 2023-05-04 14:56:10.000000 maturin-1.0.0b8/Code-of-Conduct.md
+-rw-r--r--   0     1001      123     2386 2023-05-04 14:56:10.000000 maturin-1.0.0b8/Dockerfile
+-rw-r--r--   0     1001      123      245 2023-05-04 14:56:10.000000 maturin-1.0.0b8/MANIFEST.in
+-rw-r--r--   0     1001      123    16573 2023-05-04 14:56:10.000000 maturin-1.0.0b8/README.md
+-rw-r--r--   0     1001      123       16 2023-05-04 14:56:10.000000 maturin-1.0.0b8/clippy.toml
+-rw-r--r--   0     1001      123     9664 2023-05-04 14:56:10.000000 maturin-1.0.0b8/deny.toml
+-rw-r--r--   0     1001      123    10847 2023-05-04 14:56:10.000000 maturin-1.0.0b8/license-apache
+-rw-r--r--   0     1001      123     1051 2023-05-04 14:56:10.000000 maturin-1.0.0b8/license-mit
+-rw-r--r--   0     1001      123     6236 2023-05-04 14:56:10.000000 maturin-1.0.0b8/maturin/__init__.py
+-rw-r--r--   0     1001      123      956 2023-05-04 14:56:10.000000 maturin-1.0.0b8/maturin/__main__.py
+-rw-r--r--   0     1001      123     5162 2023-05-04 14:56:10.000000 maturin-1.0.0b8/maturin/import_hook.py
+-rw-r--r--   0     1001      123      200 2023-05-04 14:56:10.000000 maturin-1.0.0b8/netlify.toml
+-rw-r--r--   0     1001      123     2170 2023-05-04 14:56:10.000000 maturin-1.0.0b8/noxfile.py
+-rw-r--r--   0     1001      123     1290 2023-05-04 14:56:10.000000 maturin-1.0.0b8/pyproject.toml
+-rw-r--r--   0     1001      123     2868 2023-05-04 14:56:10.000000 maturin-1.0.0b8/setup.py
+-rw-r--r--   0     1001      123    19534 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/audit.rs
+-rw-r--r--   0     1001      123    53261 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/manylinux-policy.json
+-rw-r--r--   0     1001      123      242 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/mod.rs
+-rw-r--r--   0     1001      123     1862 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/musllinux-policy.json
+-rw-r--r--   0     1001      123     1389 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/musllinux.rs
+-rw-r--r--   0     1001      123     3777 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/patchelf.rs
+-rw-r--r--   0     1001      123     4602 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/platform_tag.rs
+-rw-r--r--   0     1001      123     5393 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/policy.rs
+-rw-r--r--   0     1001      123     1169 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/repair.rs
+-rw-r--r--   0     1001      123    47514 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/build_context.rs
+-rw-r--r--   0     1001      123    57254 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/build_options.rs
+-rw-r--r--   0     1001      123     5407 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/cargo_toml.rs
+-rw-r--r--   0     1001      123    33723 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/ci.rs
+-rw-r--r--   0     1001      123    23999 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/compile.rs
+-rw-r--r--   0     1001      123     8342 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/cross_compile.rs
+-rw-r--r--   0     1001      123     6119 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/develop.rs
+-rw-r--r--   0     1001      123     2233 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/lib.rs
+-rw-r--r--   0     1001      123    17816 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/main.rs
+-rw-r--r--   0     1001      123    32462 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/metadata.rs
+-rw-r--r--   0     1001      123    44938 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/module_writer.rs
+-rw-r--r--   0     1001      123     8203 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/new_project.rs
+-rw-r--r--   0     1001      123    16142 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/project_layout.rs
+-rw-r--r--   0     1001      123    17317 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/pyproject_toml.rs
+-rw-r--r--   0     1001      123    11820 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/config.rs
+-rw-r--r--   0     1001      123     1595 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/get_interpreter_metadata.py
+-rw-r--r--   0     1001      123    34577 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/mod.rs
+-rw-r--r--   0     1001      123      443 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/sysconfig-emscripten.json
+-rw-r--r--   0     1001      123     3861 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/sysconfig-freebsd.json
+-rw-r--r--   0     1001      123    14124 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/sysconfig-linux.json
+-rw-r--r--   0     1001      123     3812 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/sysconfig-macos.json
+-rw-r--r--   0     1001      123      738 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/sysconfig-netbsd.json
+-rw-r--r--   0     1001      123     2353 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/sysconfig-openbsd.json
+-rw-r--r--   0     1001      123     3341 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/sysconfig-windows.json
+-rw-r--r--   0     1001      123    34671 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/source_distribution.rs
+-rw-r--r--   0     1001      123    18478 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/target.rs
+-rw-r--r--   0     1001      123      686 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/.gitignore.j2
+-rw-r--r--   0     1001      123      518 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/Cargo.toml.j2
+-rw-r--r--   0     1001      123      149 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/__init__.py.j2
+-rw-r--r--   0     1001      123      123 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/build.rs.j2
+-rw-r--r--   0     1001      123       47 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/example.udl.j2
+-rw-r--r--   0     1001      123      722 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/lib.rs.j2
+-rw-r--r--   0     1001      123       45 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/main.rs.j2
+-rw-r--r--   0     1001      123      859 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/pyproject.toml.j2
+-rw-r--r--   0     1001      123    22846 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/upload.rs
+-rwxr-xr-x   0     1001      123      974 2023-05-04 14:56:10.000000 maturin-1.0.0b8/test-dockerfile.sh
+-rw-r--r--   0        0        0    17754 1970-01-01 00:00:00.000000 maturin-1.0.0b8/PKG-INFO
```

### Comparing `maturin-1.0.0b7/Cargo.toml` & `maturin-1.0.0b8/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 authors = ["konstin <konstin@mailbox.org>", "messense <messense@icloud.com>"]
 name = "maturin"
-version = "1.0.0-beta.7"
+version = "1.0.0-beta.8"
 description = "Build and publish crates with pyo3, rust-cpython and cffi bindings as well as rust binaries as python packages"
 exclude = ["test-crates/**/*", "sysconfig/*", "test-data/*", "ci/*", "tests/*", "guide/*", ".github/*"]
 homepage = "https://github.com/pyo3/maturin"
 readme = "README.md"
 repository = "https://github.com/pyo3/maturin"
 license = "MIT OR Apache-2.0"
 keywords = ["python", "cffi", "packaging", "pypi", "pyo3"]
@@ -44,33 +44,34 @@
 fs-err = "2.5.0"
 fat-macho = { version = "0.4.6", default-features = false }
 once_cell = "1.7.2"
 rustc_version = "0.4.0"
 semver = "1.0.13"
 target-lexicon = "0.12.0"
 indexmap = "1.9.3"
-pyproject-toml = "0.5.1"
+pyproject-toml = "0.6.0"
 python-pkginfo = "0.5.5"
 textwrap = "0.16.0"
 ignore = "0.4.20"
 itertools = "0.10.5"
 lddtree = "0.3.2"
 cc = "1.0.72"
 dunce = "1.0.2"
 normpath = "1.0.0"
 pep440_rs = { version = "0.3.3", features = ["serde"] }
 pep508_rs = { version = "0.1.1", features = ["serde"] }
+same-file = "1.0.6"
 time = "0.3.17"
 
 # cli
 clap = { version = "4.0.0", features = ["derive", "env", "wrap_help"] }
 clap_complete_command = { version = "0.5.1", optional = true }
 
 # cross compile
-cargo-zigbuild = { version = "0.16.5", default-features = false, optional = true }
+cargo-zigbuild = { version = "0.16.7", default-features = false, optional = true }
 cargo-xwin = { version = "0.14.2", default-features = false, optional = true }
 
 # log
 tracing = "0.1.36"
 tracing-subscriber = { version = "0.3.15", features = ["env-filter"], optional = true }
 
 # project scaffolding, maturin new/init/generate-ci
@@ -78,20 +79,21 @@
 console = { version = "0.15.4", optional = true }
 minijinja = { version = "0.31.0", optional = true }
 
 # upload
 bytesize = { version = "1.0.1", optional = true }
 configparser = { version = "3.0.0", optional = true }
 multipart = { version = "0.18.0", features = ["client"], default-features = false, optional = true }
-ureq = { version = "2.6.1", features = ["gzip", "socks-proxy"], default-features = false, optional = true }
+ureq = { version = "2.6.1", features = ["gzip", "json", "socks-proxy"], default-features = false, optional = true }
 native-tls = { version = "0.2.8", optional = true }
 rustls = { version = "0.20.8", optional = true }
 rustls-pemfile = { version = "1.0.1", optional = true }
 keyring = { version = "2.0.0", default-features = false, features = ["linux-no-secret-service"], optional = true }
 wild = { version = "2.1.0", optional = true }
+url = { version = "2.3.1", optional = true }
 
 [dev-dependencies]
 indoc = "2.0.0"
 pretty_assertions = "1.3.0"
 rustversion = "1.0.9"
 time = { version = "0.3.17", features = ["macros"] }
 trycmd = "0.14.11"
@@ -102,15 +104,15 @@
 
 full = ["cli-completion", "cross-compile", "log", "scaffolding", "upload"]
 
 log = ["tracing-subscriber"]
 
 cli-completion = ["dep:clap_complete_command"]
 
-upload = ["ureq", "multipart", "configparser", "bytesize", "dialoguer/password", "wild"]
+upload = ["ureq", "multipart", "configparser", "bytesize", "dialoguer/password", "url", "wild"]
 # keyring doesn't support *BSD so it's not enabled in `full` by default
 password-storage = ["upload", "keyring"]
 
 rustls = ["dep:rustls", "ureq?/tls", "cargo-xwin?/rustls-tls", "dep:rustls-pemfile"]
 native-tls = ["dep:native-tls", "ureq?/native-tls", "cargo-xwin?/native-tls", "dep:rustls-pemfile"]
 
 # cross compile using zig or xwin
```

### Comparing `maturin-1.0.0b7/.cirrus.yml` & `maturin-1.0.0b8/.cirrus.yml`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,15 @@
   CARGO_TERM_COLOR: always
   CARGO_REGISTRIES_CRATES_IO_PROTOCOL: sparse
 
 build_and_test: &BUILD_AND_TEST
   # only run tasks on pull request or bors related branches
   only_if: $CIRRUS_BRANCH == 'staging' || $CIRRUS_BRANCH == 'trying' || $CIRRUS_PR != ""
   setup_script:
-    - curl https://sh.rustup.rs -sSf --output rustup.sh
-    - sh rustup.sh -y --default-toolchain stable
+    - curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y --default-toolchain stable
     - rustup target add wasm32-wasi
     - python3 -m pip install --upgrade cffi virtualenv
   build_script:
     - cargo build
   test_script:
     - cargo test
 
@@ -25,15 +24,15 @@
     PATH: $HOME/.cargo/bin:$PATH
   target_cache:
     folder: target
     fingerprint_script:
       - echo $CIRRUS_OS
       - cat Cargo.lock
   install_script:
-    - pkg install -y curl bash python
+    - pkg install -y bash git python
     - python3 -m ensurepip
   <<: *BUILD_AND_TEST
 
 macos_arm64_task:
   name: Test (arm64 macOS)
   macos_instance:
     image: ghcr.io/cirruslabs/macos-monterey-xcode
```

### Comparing `maturin-1.0.0b7/Cargo.lock` & `maturin-1.0.0b8/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -141,17 +141,17 @@
 checksum = "c530edf18f37068ac2d977409ed5cd50d53d73bc653c7647b48eb78976ac9ae2"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "cargo-config2"
-version = "0.1.6"
+version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bd8e990edcbebfd43b4d62cb73d4e17e412a1c66a320a393c1de16ff7aa2137"
+checksum = "7ee1e7a7c5bc8f3389f125fb3da214c86d8e21c2b7259923079e0142ac47ffe4"
 dependencies = [
  "cfg-expr",
  "home",
  "once_cell",
  "serde",
  "shell-escape",
  "toml 0.7.3",
@@ -191,17 +191,17 @@
  "path-slash",
  "which",
  "xwin",
 ]
 
 [[package]]
 name = "cargo-zigbuild"
-version = "0.16.5"
+version = "0.16.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91857f14adb5098836a45766d7194d7fa1e24cd1a749e233df843a4451b02091"
+checksum = "00ff7c023d9f668281696d679e2ebc0095275501afb17df6331258c54a9aefda"
 dependencies = [
  "anyhow",
  "cargo-options",
  "cargo_metadata",
  "clap",
  "dirs",
  "fs-err",
@@ -212,17 +212,17 @@
  "serde_json",
  "target-lexicon",
  "which",
 ]
 
 [[package]]
 name = "cargo_metadata"
-version = "0.15.3"
+version = "0.15.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08a1ec454bc3eead8719cb56e15dbbfecdbc14e4b3a3ae4936cc6e31f5fc0d07"
+checksum = "eee4243f1f26fc7a42710e7439c149e2b10b05472f88090acce52632f231a73a"
 dependencies = [
  "camino",
  "cargo-platform",
  "semver",
  "serde",
  "serde_json",
  "thiserror",
@@ -261,17 +261,17 @@
  "byteorder",
  "fnv",
  "uuid",
 ]
 
 [[package]]
 name = "cfg-expr"
-version = "0.14.0"
+version = "0.15.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a35b255461940a32985c627ce82900867c61db1659764d3675ea81963f72a4c6"
+checksum = "c8790cf1286da485c72cf5fc7aeba308438800036ec67d89425924c4807268c9"
 dependencies = [
  "smallvec",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
@@ -440,23 +440,23 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "280a9f2d8b3a38871a3c8a46fb80db65e5e5ed97da80c4d08bf27fb63e35e181"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -464,17 +464,17 @@
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.7"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf2b3e8478797446514c91ef04bafcb59faba183e621ad488df88983cc14128c"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
@@ -533,17 +533,17 @@
 name = "data-encoding"
 version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23d8666cb01533c39dde32bcbab8e227b4ed6679b2c925eba05feabea39508fb"
 
 [[package]]
 name = "dialoguer"
-version = "0.10.3"
+version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af3c796f3b0b408d9fd581611b47fa850821fcb84aa640b83a3c1a5be2d691f2"
+checksum = "59c6f2989294b9a498d3ad5491a79c6deb604617378e1cdc4bfc1c1361fe2f87"
 dependencies = [
  "console",
  "shell-words",
  "zeroize",
 ]
 
 [[package]]
@@ -580,17 +580,17 @@
  "libc",
  "redox_users",
  "winapi",
 ]
 
 [[package]]
 name = "dunce"
-version = "1.0.3"
+version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bd4b30a6560bbd9b4620f4de34c3f14f60848e58a9b7216801afcb4c7b31c3c"
+checksum = "56ce8c6da7551ec6c462cbaf3bfbc75131ebbfa1c944aeaa9dab51ca1c5f0c3b"
 
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
@@ -658,17 +658,17 @@
  "libc",
  "redox_syscall",
  "windows-sys",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.25"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
@@ -714,17 +714,17 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -915,17 +915,17 @@
 checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "keyring"
-version = "2.0.1"
+version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bfd6f156b53b48cd89223a27b11f1cddaa5d9bd298b48af3b644c43a8ae5f0f"
+checksum = "09484a398d672f7332798206e3561dfa022dd4b1fe9d3a638e6bf9cc15a590c5"
 dependencies = [
  "byteorder",
  "lazy_static",
  "linux-keyutils",
  "security-framework",
  "winapi",
 ]
@@ -945,17 +945,17 @@
  "fs-err",
  "glob",
  "goblin",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "linux-keyutils"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f27bb67f6dd1d0bb5ab582868e4f65052e58da6401188a08f0da09cf512b84b"
 dependencies = [
@@ -1012,15 +1012,15 @@
 checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
 dependencies = [
  "regex-automata",
 ]
 
 [[package]]
 name = "maturin"
-version = "1.0.0-beta.7"
+version = "1.0.0-beta.8"
 dependencies = [
  "anyhow",
  "base64 0.13.1",
  "bytesize",
  "cargo-config2",
  "cargo-options",
  "cargo-xwin",
@@ -1058,14 +1058,15 @@
  "pyproject-toml",
  "python-pkginfo",
  "regex",
  "rustc_version",
  "rustls",
  "rustls-pemfile",
  "rustversion",
+ "same-file",
  "semver",
  "serde",
  "serde_json",
  "sha2",
  "tar",
  "target-lexicon",
  "tempfile",
@@ -1074,14 +1075,15 @@
  "time",
  "toml 0.7.3",
  "toml_edit",
  "tracing",
  "tracing-subscriber",
  "trycmd",
  "ureq",
+ "url",
  "which",
  "wild",
  "zip",
 ]
 
 [[package]]
 name = "memchr"
@@ -1112,32 +1114,32 @@
 dependencies = [
  "mime",
  "unicase",
 ]
 
 [[package]]
 name = "minijinja"
-version = "0.31.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "673d1ece89f7e166f43270800d78f9b1a9d21fda92dbcfa3b98b21213cdccbbc"
+checksum = "0b1dbc390e4447b2500c4071d7bc2a808cf07e925bae6b92db8a3c3eae773c58"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.6.2"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "msi"
 version = "0.5.1"
@@ -1236,17 +1238,17 @@
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "openssl"
-version = "0.10.48"
+version = "0.10.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "518915b97df115dd36109bfa429a48b8f737bd05508cf9588977b599648926d2"
+checksum = "7e30d8bc91859781f0a943411186324d580f2bbeb71b452fe91ae344806af3f1"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
@@ -1268,28 +1270,27 @@
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-src"
-version = "111.25.1+1.1.1t"
+version = "111.25.2+1.1.1t"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ef9a9cc6ea7d9d5e7c4a913dc4b48d0e359eddf01af1dfec96ba7064b4aba10"
+checksum = "320708a054ad9b3bf314688b5db87cf4d6683d64cfc835e2337924ae62bf4431"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.83"
+version = "0.9.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "666416d899cf077260dac8698d60a60b435a46d57e82acb1be3d0dad87284e5b"
+checksum = "0d3d193fb1488ad46ffe3aaabc912cc931d02ee8518fe2959aea8ef52718b0c0"
 dependencies = [
- "autocfg",
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -1351,30 +1352,30 @@
 name = "path-slash"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e91099d4268b0e11973f036e885d652fb0b21fedcf69738c627f94db6a44f42"
 
 [[package]]
 name = "pep440_rs"
-version = "0.3.3"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0cbf1fd438eeb1b1e42e8390951ec90d1cf87bbe3d3305b28551bca30b7595a"
+checksum = "aac177a025c60a4dd25d638bf33e746d1ead5f7123f6650f35b4394c7ce1a104"
 dependencies = [
  "lazy_static",
  "regex",
  "serde",
  "tracing",
  "unicode-width",
 ]
 
 [[package]]
 name = "pep508_rs"
-version = "0.1.1"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e566191336ac8cf72db45240583769ab9fb75bd87dd9544cd96a9bc7e28585c4"
+checksum = "969679a29dfdc8278a449f75b3dd45edf57e649bd59f7502429c2840751c46d8"
 dependencies = [
  "once_cell",
  "pep440_rs",
  "regex",
  "serde",
  "thiserror",
  "tracing",
@@ -1462,17 +1463,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.54"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e472a104799c74b514a57226160104aa483546de37e839ec50e3c2e41dd87534"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "psm"
 version = "0.1.21"
@@ -1480,17 +1481,17 @@
 checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pyproject-toml"
-version = "0.5.1"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71c24ad9fa3f11e0b5f45bf86ea6e1ae4dfef288fb7b077a15b6a19ebc87a37f"
+checksum = "f04dbbb336bd88583943c7cd973a32fed323578243a7569f40cb0c7da673321b"
 dependencies = [
  "indexmap",
  "pep440_rs",
  "pep508_rs",
  "serde",
  "toml 0.7.3",
 ]
@@ -1980,17 +1981,17 @@
  "filetime",
  "libc",
  "xattr",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempfile"
 version = "3.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af18f7ae1acd354b992402e9ec5864359d693cd8a79dcbef59f76891701c1e95"
 dependencies = [
@@ -2314,14 +2315,16 @@
 dependencies = [
  "base64 0.13.1",
  "flate2",
  "log",
  "native-tls",
  "once_cell",
  "rustls",
+ "serde",
+ "serde_json",
  "socks",
  "url",
  "webpki",
  "webpki-roots",
 ]
 
 [[package]]
@@ -2334,17 +2337,17 @@
  "idna",
  "percent-encoding",
  "serde",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.3.0"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1674845326ee10d37ca60470760d4288a6f80f304007d92e5c53bab78c9cfd79"
+checksum = "5b55a3fef2a1e3b3a00ce878640918820d3c51081576ac657d23af9fc7928fdb"
 
 [[package]]
 name = "valuable"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
 
@@ -2639,17 +2642,17 @@
 name = "yansi"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "09041cd90cf85f7f8b2df60c646f853b7f535ce68f85244eb6731cf89fa498ec"
 
 [[package]]
 name = "zeroize"
-version = "1.5.7"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c394b5bd0c6f669e7275d9c20aa90ae064cb22e75a1cad54e1b34088034b149f"
+checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
 
 [[package]]
 name = "zip"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0445d0fbc924bb93539b4316c11afb121ea39296f99a3c4c9edad09e3658cdef"
 dependencies = [
```

### Comparing `maturin-1.0.0b7/Changelog.md` & `maturin-1.0.0b8/Changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 * Add Cargo compile targets configuration for filtering multiple bin targets in [#1339](https://github.com/PyO3/maturin/pull/1339)
 * Respect `rustflags` settings in cargo configuration file in [#1405](https://github.com/PyO3/maturin/pull/1405)
 * Add support for uniffi 0.23 in [#1481](https://github.com/PyO3/maturin/pull/1481)
 * Add support for custom TLS certificate authority bundle in [#1483](https://github.com/PyO3/maturin/pull/1483)
 * Bump MSRV to 1.64.0 in [#1528](https://github.com/PyO3/maturin/pull/1528)
 * Add wildcards support to publish/upload commands on Windows in [#1534](https://github.com/PyO3/maturin/pull/1534)
 * Add support for configuring macOS deployment target version in `pyproject.toml` in [#1536](https://github.com/PyO3/maturin/pull/1536)
+* Rewrite platform specific dependencies in `Cargo.toml` by viccie30 in [#1572](https://github.com/PyO3/maturin/pull/1572)
+* Add trusted publisher support in [#1578](https://github.com/PyO3/maturin/pull/1578)
+* Add new `git` source distribution generator in [#1587](https://github.com/PyO3/maturin/pull/1587)
+
+## [0.14.17] - 2023-04-06
+
 * Fix wrong `EXT_SUFFIX` when cross compiling musllinux wheels for Python 3.11 in [#1560](https://github.com/PyO3/maturin/pull/1560)
 
 ## [0.14.16] - 2023-03-26
 
 * Deprecate `package.metadata.maturin.name` in favor of `tool.maturin.module-name` in `pyproject.toml` in [#1531](https://github.com/PyO3/maturin/pull/1531)
 
 ## [0.14.15] - 2023-03-03
@@ -840,15 +846,16 @@
 
  * Show a progress bar for cargo's compile progress
 
 ## 0.1.0 - 2018-08-22
 
  * Initial Release
 
-[Unreleased]: https://github.com/pyo3/maturin/compare/v0.14.16...HEAD
+[Unreleased]: https://github.com/pyo3/maturin/compare/v0.14.17...HEAD
+[0.14.17]: https://github.com/pyo3/maturin/compare/v0.14.16...v0.14.17
 [0.14.16]: https://github.com/pyo3/maturin/compare/v0.14.15...v0.14.16
 [0.14.15]: https://github.com/pyo3/maturin/compare/v0.14.14...v0.14.15
 [0.14.14]: https://github.com/pyo3/maturin/compare/v0.14.13...v0.14.14
 [0.14.13]: https://github.com/pyo3/maturin/compare/v0.14.12...v0.14.13
 [0.14.12]: https://github.com/pyo3/maturin/compare/v0.14.11...v0.14.12
 [0.14.11]: https://github.com/pyo3/maturin/compare/v0.14.10...v0.14.11
 [0.14.10]: https://github.com/pyo3/maturin/compare/v0.14.9...v0.14.10
```

### Comparing `maturin-1.0.0b7/Code-of-Conduct.md` & `maturin-1.0.0b8/Code-of-Conduct.md`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/Dockerfile` & `maturin-1.0.0b8/Dockerfile`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/README.md` & `maturin-1.0.0b8/README.md`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/deny.toml` & `maturin-1.0.0b8/deny.toml`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/license-apache` & `maturin-1.0.0b8/license-apache`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/license-mit` & `maturin-1.0.0b8/license-mit`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/maturin/__init__.py` & `maturin-1.0.0b8/maturin/__init__.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/maturin/__main__.py` & `maturin-1.0.0b8/maturin/__main__.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/maturin/import_hook.py` & `maturin-1.0.0b8/maturin/import_hook.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/noxfile.py` & `maturin-1.0.0b8/noxfile.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/pyproject.toml` & `maturin-1.0.0b8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/setup.py` & `maturin-1.0.0b8/setup.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/auditwheel/audit.rs` & `maturin-1.0.0b8/src/auditwheel/audit.rs`

 * *Files 0% similar despite different names*

```diff
@@ -419,15 +419,19 @@
             .output()
             .with_context(|| format!("Failed to run `{} --print-sysroot`", path.display()))?;
         if out.status.success() {
             let sysroot = String::from_utf8(out.stdout)
                 .context("Failed to read the sysroot path")?
                 .trim()
                 .to_owned();
-            return Ok(PathBuf::from(sysroot));
+            if sysroot.is_empty() {
+                return Ok(PathBuf::from("/"));
+            } else {
+                return Ok(PathBuf::from(sysroot));
+            }
         } else {
             bail!(
                 "Failed to get the sysroot path: {}",
                 String::from_utf8(out.stderr)?
             );
         }
     }
```

### Comparing `maturin-1.0.0b7/src/auditwheel/manylinux-policy.json` & `maturin-1.0.0b8/src/auditwheel/manylinux-policy.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/auditwheel/musllinux-policy.json` & `maturin-1.0.0b8/src/auditwheel/musllinux-policy.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/auditwheel/musllinux.rs` & `maturin-1.0.0b8/src/auditwheel/musllinux.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/auditwheel/patchelf.rs` & `maturin-1.0.0b8/src/auditwheel/patchelf.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/auditwheel/platform_tag.rs` & `maturin-1.0.0b8/src/auditwheel/platform_tag.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/auditwheel/policy.rs` & `maturin-1.0.0b8/src/auditwheel/policy.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/auditwheel/repair.rs` & `maturin-1.0.0b8/src/auditwheel/repair.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/build_context.rs` & `maturin-1.0.0b8/src/build_context.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/build_options.rs` & `maturin-1.0.0b8/src/build_options.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/cargo_toml.rs` & `maturin-1.0.0b8/src/cargo_toml.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/ci.rs` & `maturin-1.0.0b8/src/ci.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/compile.rs` & `maturin-1.0.0b8/src/compile.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/cross_compile.rs` & `maturin-1.0.0b8/src/cross_compile.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/develop.rs` & `maturin-1.0.0b8/src/develop.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/lib.rs` & `maturin-1.0.0b8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/main.rs` & `maturin-1.0.0b8/src/main.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/metadata.rs` & `maturin-1.0.0b8/src/metadata.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use crate::PyProjectToml;
 use anyhow::{bail, format_err, Context, Result};
 use fs_err as fs;
 use indexmap::IndexMap;
 use pep440_rs::{Version, VersionSpecifiers};
 use pep508_rs::{MarkerExpression, MarkerOperator, MarkerTree, MarkerValue, Requirement};
+use pyproject_toml::License;
 use regex::Regex;
 use serde::{Deserialize, Serialize};
 use std::collections::HashMap;
 use std::fmt::Write as _;
 use std::path::{Path, PathBuf};
 use std::str;
 use std::str::FromStr;
@@ -176,24 +177,29 @@
                 None => {}
             }
 
             if let Some(requires_python) = &project.requires_python {
                 self.requires_python = Some(requires_python.clone());
             }
 
-            if let Some(pyproject_toml::License { file, text }) = &project.license {
-                if file.is_some() && text.is_some() {
-                    bail!("file and text fields of 'project.license' are mutually-exclusive, only one of them should be specified");
-                }
-                if let Some(license_path) = file {
-                    let license_path = pyproject_dir.join(license_path);
-                    self.license_files.push(license_path);
-                }
-                if let Some(license_text) = text {
-                    self.license = Some(license_text.clone());
+            if let Some(license) = &project.license {
+                match license {
+                    // TODO: switch to License-Expression core metadata, see https://peps.python.org/pep-0639/#add-license-expression-field
+                    License::String(license_expr) => self.license = Some(license_expr.clone()),
+                    License::Table { file, text } => match (file, text) {
+                        (Some(_), Some(_)) => {
+                            bail!("file and text fields of 'project.license' are mutually-exclusive, only one of them should be specified");
+                        }
+                        (Some(license_path), None) => {
+                            let license_path = pyproject_dir.join(license_path);
+                            self.license_files.push(license_path);
+                        }
+                        (None, Some(license_text)) => self.license = Some(license_text.clone()),
+                        (None, None) => {}
+                    },
                 }
             }
 
             // Until PEP 639 is approved with metadata 2.3, we can assume a
             // dynamic license-files (also awaiting full 2.2 metadata support)
             // We're already emitting the License-Files metadata without issue.
             // license-files.globs = ["LICEN[CS]E*", "COPYING*", "NOTICE*", "AUTHORS*"]
```

### Comparing `maturin-1.0.0b7/src/module_writer.rs` & `maturin-1.0.0b8/src/module_writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1145,15 +1145,15 @@
     // Include additional files
     if let Some(pyproject) = pyproject_toml {
         // FIXME: in src-layout pyproject.toml isn't located directly in python dir
         let pyproject_dir = python_dir;
         if let Some(glob_patterns) = pyproject.include() {
             for pattern in glob_patterns
                 .iter()
-                .filter_map(|glob_pattern| glob_pattern.targets(Format::Sdist))
+                .filter_map(|glob_pattern| glob_pattern.targets(Format::Wheel))
             {
                 eprintln!("📦 Including files matching \"{pattern}\"");
                 for source in glob::glob(&pyproject_dir.join(pattern).to_string_lossy())
                     .expect("No files found for pattern")
                     .filter_map(Result::ok)
                 {
                     let target = source.strip_prefix(pyproject_dir)?.to_path_buf();
```

### Comparing `maturin-1.0.0b7/src/new_project.rs` & `maturin-1.0.0b8/src/new_project.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/project_layout.rs` & `maturin-1.0.0b8/src/project_layout.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/pyproject_toml.rs` & `maturin-1.0.0b8/src/pyproject_toml.rs`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 use fs_err as fs;
 use pyproject_toml::PyProjectToml as ProjectToml;
 use serde::{Deserialize, Serialize};
 use std::collections::HashMap;
 use std::path::{Path, PathBuf};
 
 /// The `[tool]` section of a pyproject.toml
-#[derive(Serialize, Deserialize, Debug, Clone)]
+#[derive(Serialize, Deserialize, Debug, Clone, Default)]
 #[serde(rename_all = "kebab-case")]
 pub struct Tool {
-    maturin: Option<ToolMaturin>,
+    /// maturin options
+    pub maturin: Option<ToolMaturin>,
 }
 
 #[derive(Copy, Clone, Debug, Deserialize, Serialize, PartialEq, Eq)]
 #[serde(rename_all = "lowercase")]
 /// The target format for the include or exclude [GlobPattern].
 ///
 /// See [Formats].
@@ -100,36 +101,56 @@
 #[serde(rename_all = "kebab-case")]
 pub struct TargetConfig {
     /// macOS deployment target version
     #[serde(alias = "macosx-deployment-target")]
     pub macos_deployment_target: Option<String>,
 }
 
+/// Source distribution generator
+#[derive(Serialize, Deserialize, Debug, Clone, Copy, Default)]
+#[serde(rename_all = "kebab-case")]
+pub enum SdistGenerator {
+    /// Use `cargo package --list`
+    #[default]
+    Cargo,
+    /// Use `git ls-files`
+    Git,
+}
+
 /// The `[tool.maturin]` section of a pyproject.toml
-#[derive(Serialize, Deserialize, Debug, Clone)]
+#[derive(Serialize, Deserialize, Debug, Clone, Default)]
 #[serde(rename_all = "kebab-case")]
 pub struct ToolMaturin {
     // maturin specific options
-    // extension module name, accepts setuptools style import name like `foo.bar`
-    module_name: Option<String>,
-    include: Option<Vec<GlobPattern>>,
-    exclude: Option<Vec<GlobPattern>>,
-    bindings: Option<String>,
+    /// Module name, accepts setuptools style import name like `foo.bar`
+    pub module_name: Option<String>,
+    /// Include files matching the given glob pattern(s)
+    pub include: Option<Vec<GlobPattern>>,
+    /// Exclude files matching the given glob pattern(s)
+    pub exclude: Option<Vec<GlobPattern>>,
+    /// Bindings type
+    pub bindings: Option<String>,
+    /// Platform compatibility
     #[serde(alias = "manylinux")]
-    compatibility: Option<PlatformTag>,
+    pub compatibility: Option<PlatformTag>,
+    /// Skip audit wheel
+    #[serde(default)]
+    pub skip_auditwheel: bool,
+    /// Strip the final binary
     #[serde(default)]
-    skip_auditwheel: bool,
+    pub strip: bool,
+    /// Source distribution generator
     #[serde(default)]
-    strip: bool,
+    pub sdist_generator: SdistGenerator,
     /// The directory with python module, contains `<module_name>/__init__.py`
-    python_source: Option<PathBuf>,
+    pub python_source: Option<PathBuf>,
     /// Python packages to include
-    python_packages: Option<Vec<String>>,
+    pub python_packages: Option<Vec<String>>,
     /// Path to the wheel directory, defaults to `<module_name>.data`
-    data: Option<PathBuf>,
+    pub data: Option<PathBuf>,
     /// Cargo compile targets
     pub targets: Option<Vec<CargoTarget>>,
     /// Target configuration
     #[serde(default, rename = "target")]
     pub target_config: HashMap<String, TargetConfig>,
     // Some customizable cargo options
     /// Build artifacts with the specified Cargo profile
@@ -235,14 +256,21 @@
     /// Returns the value of `[tool.maturin.strip]` in pyproject.toml
     pub fn strip(&self) -> bool {
         self.maturin()
             .map(|maturin| maturin.strip)
             .unwrap_or_default()
     }
 
+    /// Returns the value of `[tool.maturin.sdist-generator]` in pyproject.toml
+    pub fn sdist_generator(&self) -> SdistGenerator {
+        self.maturin()
+            .map(|maturin| maturin.sdist_generator)
+            .unwrap_or_default()
+    }
+
     /// Returns the value of `[tool.maturin.python-source]` in pyproject.toml
     pub fn python_source(&self) -> Option<&Path> {
         self.maturin()
             .and_then(|maturin| maturin.python_source.as_deref())
     }
 
     /// Returns the value of `[tool.maturin.python-packages]` in pyproject.toml
```

### Comparing `maturin-1.0.0b7/src/python_interpreter/config.rs` & `maturin-1.0.0b8/src/python_interpreter/config.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/python_interpreter/get_interpreter_metadata.py` & `maturin-1.0.0b8/src/python_interpreter/get_interpreter_metadata.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/python_interpreter/mod.rs` & `maturin-1.0.0b8/src/python_interpreter/mod.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/python_interpreter/sysconfig-freebsd.json` & `maturin-1.0.0b8/src/python_interpreter/sysconfig-freebsd.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/python_interpreter/sysconfig-linux.json` & `maturin-1.0.0b8/src/python_interpreter/sysconfig-linux.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/python_interpreter/sysconfig-macos.json` & `maturin-1.0.0b8/src/python_interpreter/sysconfig-macos.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/python_interpreter/sysconfig-netbsd.json` & `maturin-1.0.0b8/src/python_interpreter/sysconfig-netbsd.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/python_interpreter/sysconfig-openbsd.json` & `maturin-1.0.0b8/src/python_interpreter/sysconfig-openbsd.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/python_interpreter/sysconfig-windows.json` & `maturin-1.0.0b8/src/python_interpreter/sysconfig-windows.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/source_distribution.rs` & `maturin-1.0.0b8/src/source_distribution.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use crate::module_writer::{add_data, ModuleWriter};
+use crate::pyproject_toml::SdistGenerator;
 use crate::{pyproject_toml::Format, BuildContext, PyProjectToml, SDistWriter};
 use anyhow::{bail, Context, Result};
 use cargo_metadata::{Metadata, MetadataCommand};
 use fs_err as fs;
 use ignore::overrides::Override;
 use normpath::PathExt as _;
 use std::collections::HashMap;
@@ -51,38 +52,156 @@
     root_crate: bool,
 ) -> Result<String> {
     let manifest_path = manifest_path.as_ref();
     let text = fs::read_to_string(manifest_path).context(format!(
         "Can't read Cargo.toml at {}",
         manifest_path.display(),
     ))?;
-    let mut data = text.parse::<toml_edit::Document>().context(format!(
+    let mut document = text.parse::<toml_edit::Document>().context(format!(
         "Failed to parse Cargo.toml at {}",
         manifest_path.display()
     ))?;
+
+    let workspace = workspace_manifest.get("workspace");
+    let workspace_deps = workspace
+        .and_then(|x| x.get("dependencies"))
+        .and_then(|x| x.as_table_like());
+
+    let mut rewritten = rewrite_dependencies_path(
+        document.as_table_mut(),
+        workspace_deps,
+        manifest_path,
+        known_path_deps,
+        &local_deps_folder,
+        root_crate,
+    )?;
+    if let Some(target_specs) = document
+        .get_mut("target")
+        .and_then(|x| x.as_table_like_mut())
+    {
+        for target_spec in target_specs
+            .iter_mut()
+            .filter_map(|x| x.1.as_table_like_mut())
+        {
+            rewritten |= rewrite_dependencies_path(
+                target_spec,
+                workspace_deps,
+                manifest_path,
+                known_path_deps,
+                &local_deps_folder,
+                root_crate,
+            )?;
+        }
+    }
+
+    // Update workspace inherited metadata
+    if let Some(package) = document.get_mut("package").and_then(|x| x.as_table_mut()) {
+        let workspace_package = workspace
+            .and_then(|x| x.get("package"))
+            .and_then(|x| x.as_table_like());
+        for key in WORKSPACE_INHERITABLE_FIELDS.iter().copied() {
+            let workspace_inherited = package
+                .get(key)
+                .and_then(|x| x.get("workspace"))
+                .and_then(|x| x.as_bool())
+                .unwrap_or_default();
+            if workspace_inherited {
+                if let Some(workspace_value) = workspace_package.and_then(|ws| ws.get(key)) {
+                    package[key] = workspace_value.clone();
+                    rewritten = true;
+                }
+            }
+        }
+
+        // Update resolver if workspace set one
+        if let Some(resolver) = workspace.and_then(|x| x.get("resolver")) {
+            package["resolver"] = resolver.clone();
+            rewritten = true;
+        }
+    }
+
+    if root_crate {
+        // Update workspace members
+        if let Some(workspace) = document.get_mut("workspace").and_then(|x| x.as_table_mut()) {
+            if let Some(members) = workspace.get_mut("members").and_then(|x| x.as_array_mut()) {
+                if known_path_deps.is_empty() {
+                    // Remove workspace members when there isn't any path dep
+                    workspace.remove("members");
+                    if workspace.is_empty() {
+                        // Remove workspace all together if it's empty
+                        document.remove("workspace");
+                    }
+                    rewritten = true;
+                } else {
+                    let mut new_members = toml_edit::Array::new();
+                    for member in members.iter() {
+                        if let toml_edit::Value::String(ref s) = member {
+                            let path = Path::new(s.value());
+                            if let Some(name) = path.file_name().and_then(|x| x.to_str()) {
+                                if known_path_deps.contains_key(name) {
+                                    new_members.push(format!("{LOCAL_DEPENDENCIES_FOLDER}/{name}"));
+                                }
+                            }
+                        }
+                    }
+                    if !new_members.is_empty() {
+                        workspace["members"] = toml_edit::value(new_members);
+                    } else {
+                        workspace.remove("members");
+                    }
+                    rewritten = true;
+                }
+            }
+        }
+    } else {
+        // Update package.workspace
+        // https://rust-lang.github.io/rfcs/1525-cargo-workspace.html#implicit-relations
+        // https://doc.rust-lang.org/cargo/reference/manifest.html#the-workspace-field
+        if let Some(package) = document.get_mut("package").and_then(|x| x.as_table_mut()) {
+            if let Some(workspace) = package.get("workspace").and_then(|x| x.as_str()) {
+                // This is enough to fix https://github.com/PyO3/maturin/issues/838
+                // Other cases can be fixed on demand
+                if workspace == ".." || workspace == "../" {
+                    package.remove("workspace");
+                    rewritten = true;
+                }
+            }
+        }
+    }
+    if rewritten {
+        Ok(document.to_string())
+    } else {
+        Ok(text)
+    }
+}
+
+fn rewrite_dependencies_path(
+    table: &mut dyn toml_edit::TableLike,
+    workspace_deps: Option<&dyn toml_edit::TableLike>,
+    manifest_path: &Path,
+    known_path_deps: &HashMap<String, PathBuf>,
+    local_deps_folder: &str,
+    root_crate: bool,
+) -> Result<bool> {
     let mut rewritten = false;
     //  ˇˇˇˇˇˇˇˇˇˇˇˇ dep_category
     // [dependencies]
     // some_path_dep = { path = "../some_path_dep" }
     //                          ^^^^^^^^^^^^^^^^^^ table[&dep_name]["path"]
     // ^^^^^^^^^^^^^ dep_name
     for dep_category in ["dependencies", "dev-dependencies", "build-dependencies"] {
-        if let Some(table) = data.get_mut(dep_category).and_then(|x| x.as_table_mut()) {
+        if let Some(table) = table.get_mut(dep_category).and_then(|x| x.as_table_mut()) {
             if dep_category == "dev-dependencies" && !known_path_deps.is_empty() {
                 // Remove dev-dependencies since building from sdist doesn't need them,
                 // Keep it when there are no path dependencies to support building from
                 // sdist with `--locked`/`--frozen`.
-                data.remove(dep_category);
+                table.remove(dep_category);
                 rewritten = true;
                 continue;
             }
-            let workspace_deps = workspace_manifest
-                .get("workspace")
-                .and_then(|x| x.get("dependencies"))
-                .and_then(|x| x.as_table_like());
             let dep_names: Vec<_> = table.iter().map(|(key, _)| key.to_string()).collect();
             for dep_name in dep_names {
                 let workspace_inherit = table
                     .get(&dep_name)
                     .and_then(|x| x.get("workspace"))
                     .and_then(|x| x.as_bool())
                     .unwrap_or_default();
@@ -130,32 +249,32 @@
                                     .entry("features")
                                     .or_insert_with(|| {
                                         toml_edit::Item::Value(toml_edit::Array::new().into())
                                     })
                                     .as_array_mut()
                                     .with_context(|| {
                                         format!(
-                                            "In {}, {} {} has a features value that is not an array",
-                                            manifest_path.display(),
-                                            dep_category,
-                                            dep_name
-                                        )
+                                        "In {}, {} {} has a features value that is not an array",
+                                        manifest_path.display(),
+                                        dep_category,
+                                        dep_name
+                                    )
                                     })?;
                                 existing_features.extend(features);
                             }
                             table[&dep_name] = workspace_dep;
                             rewritten = true;
                         } else {
                             bail!(
-                                "In {}, {} {} is marked as `workspace = true`, but it is found neither in \
+                            "In {}, {} {} is marked as `workspace = true`, but it is found neither in \
                                 the workspace manifest nor in the known path dependencies",
-                                manifest_path.display(),
-                                dep_category,
-                                dep_name
-                            )
+                            manifest_path.display(),
+                            dep_category,
+                            dep_name
+                        )
                         }
                         continue;
                     }
                 }
                 // This is the location of the targeted crate in the source distribution
                 table[&dep_name]["path"] = if root_crate {
                     toml_edit::value(format!("{local_deps_folder}/{dep_name}"))
@@ -170,89 +289,15 @@
                         .unwrap()
                         .remove("workspace");
                 }
                 rewritten = true;
             }
         }
     }
-
-    // Update workspace inherited metadata
-    if let Some(package) = data.get_mut("package").and_then(|x| x.as_table_mut()) {
-        let workspace_package = workspace_manifest
-            .get("workspace")
-            .and_then(|x| x.get("package"))
-            .and_then(|x| x.as_table_like());
-        for key in WORKSPACE_INHERITABLE_FIELDS.iter().copied() {
-            let workspace_inherited = package
-                .get(key)
-                .and_then(|x| x.get("workspace"))
-                .and_then(|x| x.as_bool())
-                .unwrap_or_default();
-            if workspace_inherited {
-                if let Some(workspace_value) = workspace_package.and_then(|ws| ws.get(key)) {
-                    package[key] = workspace_value.clone();
-                    rewritten = true;
-                }
-            }
-        }
-    }
-
-    if root_crate {
-        // Update workspace members
-        if let Some(workspace) = data.get_mut("workspace").and_then(|x| x.as_table_mut()) {
-            if let Some(members) = workspace.get_mut("members").and_then(|x| x.as_array_mut()) {
-                if known_path_deps.is_empty() {
-                    // Remove workspace members when there isn't any path dep
-                    workspace.remove("members");
-                    if workspace.is_empty() {
-                        // Remove workspace all together if it's empty
-                        data.remove("workspace");
-                    }
-                    rewritten = true;
-                } else {
-                    let mut new_members = toml_edit::Array::new();
-                    for member in members.iter() {
-                        if let toml_edit::Value::String(ref s) = member {
-                            let path = Path::new(s.value());
-                            if let Some(name) = path.file_name().and_then(|x| x.to_str()) {
-                                if known_path_deps.contains_key(name) {
-                                    new_members.push(format!("{LOCAL_DEPENDENCIES_FOLDER}/{name}"));
-                                }
-                            }
-                        }
-                    }
-                    if !new_members.is_empty() {
-                        workspace["members"] = toml_edit::value(new_members);
-                    } else {
-                        workspace.remove("members");
-                    }
-                    rewritten = true;
-                }
-            }
-        }
-    } else {
-        // Update package.workspace
-        // https://rust-lang.github.io/rfcs/1525-cargo-workspace.html#implicit-relations
-        // https://doc.rust-lang.org/cargo/reference/manifest.html#the-workspace-field
-        if let Some(package) = data.get_mut("package").and_then(|x| x.as_table_mut()) {
-            if let Some(workspace) = package.get("workspace").and_then(|x| x.as_str()) {
-                // This is enough to fix https://github.com/PyO3/maturin/issues/838
-                // Other cases can be fixed on demand
-                if workspace == ".." || workspace == "../" {
-                    package.remove("workspace");
-                    rewritten = true;
-                }
-            }
-        }
-    }
-    if rewritten {
-        Ok(data.to_string())
-    } else {
-        Ok(text)
-    }
+    Ok(rewritten)
 }
 
 /// Make sure that the dep entry is an inline table
 /// e.g. in the form of `{ version = "..." }`
 /// so that we can add entries for `optional` and `features`
 fn ensure_dep_is_inline_table(dep: &mut toml_edit::Item) {
     if let Some(v) = dep.as_value_mut() {
@@ -391,15 +436,21 @@
 
     if root_crate
         && !target_source
             .iter()
             .any(|(target, _)| target == Path::new("pyproject.toml"))
     {
         // Add pyproject.toml to the source distribution
-        if cargo_toml_in_subdir {
+        // `pyproject.toml` may not be included in `cargo package --list`
+        // (e.g. it's not specified in `include` or is specified in `exclude` by mistake)
+        // we check if it's the same pyproject.toml file in Cargo.toml directory
+        let pyproject_toml_in_manifest_dir =
+            same_file::is_same_file(pyproject_toml_path, abs_manifest_dir.join("pyproject.toml"))
+                .unwrap_or(false);
+        if cargo_toml_in_subdir || pyproject_toml_in_manifest_dir {
             // if Cargo.toml is in subdirectory of pyproject.toml directory
             target_source.push((
                 PathBuf::from("pyproject.toml"),
                 pyproject_toml_path.to_path_buf(),
             ));
         } else {
             // if pyproject.toml was not included by `cargo package --list`
@@ -510,53 +561,70 @@
                 }
             }
         }
     }
     Ok(path_deps)
 }
 
-/// Creates a source distribution, packing the root crate and all local dependencies
+/// Copies the files of git to a source distribution
 ///
-/// The source distribution format is specified in
-/// [PEP 517 under "build_sdist"](https://www.python.org/dev/peps/pep-0517/#build-sdist)
-/// and in
-/// https://packaging.python.org/specifications/source-distribution-format/#source-distribution-file-format
-pub fn source_distribution(
+/// Runs `git ls-files -z` to obtain a list of files to package.
+fn add_git_tracked_files_to_sdist(
+    pyproject_toml_path: &Path,
+    writer: &mut SDistWriter,
+    prefix: impl AsRef<Path>,
+) -> Result<()> {
+    let pyproject_dir = pyproject_toml_path.parent().unwrap();
+    let output = Command::new("git")
+        .args(["ls-files", "-z"])
+        .current_dir(pyproject_dir)
+        .output()
+        .context("Failed to run `git ls-files -z`")?;
+    if !output.status.success() {
+        bail!(
+            "Failed to query file list from git: {}\n--- Project Path: {}\n--- Stdout:\n{}\n--- Stderr:\n{}",
+            output.status,
+            pyproject_dir.display(),
+            String::from_utf8_lossy(&output.stdout),
+            String::from_utf8_lossy(&output.stderr),
+        );
+    }
+
+    let prefix = prefix.as_ref();
+    writer.add_directory(prefix)?;
+
+    let file_paths = str::from_utf8(&output.stdout)
+        .context("git printed invalid utf-8 ಠ_ಠ")?
+        .split('\0')
+        .filter(|s| !s.is_empty())
+        .map(Path::new);
+    for source in file_paths {
+        writer.add_file(prefix.join(source), pyproject_dir.join(source))?;
+    }
+    Ok(())
+}
+
+/// Copies the files of a crate to a source distribution, recursively adding path dependencies
+/// and rewriting path entries in Cargo.toml
+fn add_cargo_package_files_to_sdist(
     build_context: &BuildContext,
-    pyproject: &PyProjectToml,
-    excludes: Option<Override>,
-) -> Result<PathBuf> {
-    let metadata21 = &build_context.metadata21;
+    pyproject_toml_path: &Path,
+    writer: &mut SDistWriter,
+    root_dir: &Path,
+) -> Result<()> {
     let manifest_path = &build_context.manifest_path;
-    let pyproject_toml_path = build_context
-        .pyproject_toml_path
-        .normalize()
-        .with_context(|| {
-            format!(
-                "failed to normalize path `{}`",
-                build_context.pyproject_toml_path.display()
-            )
-        })?
-        .into_path_buf();
     let workspace_manifest_path = build_context
         .cargo_metadata
         .workspace_root
         .join("Cargo.toml");
     let workspace_manifest: toml_edit::Document =
         fs::read_to_string(workspace_manifest_path)?.parse()?;
 
     let known_path_deps = find_path_deps(&build_context.cargo_metadata)?;
 
-    let mut writer = SDistWriter::new(&build_context.out, metadata21, excludes)?;
-    let root_dir = PathBuf::from(format!(
-        "{}-{}",
-        &metadata21.get_distribution_escaped(),
-        &metadata21.get_version_escaped()
-    ));
-
     // Add local path dependencies
     let mut path_dep_workspace_manifests = HashMap::new();
     for (name, path_dep) in known_path_deps.iter() {
         // Path dependencies may not be in the same workspace as the root crate,
         // thus we need to find out its workspace root from `cargo metadata`
         let path_dep_metadata = MetadataCommand::new()
             .manifest_path(path_dep)
@@ -581,16 +649,16 @@
                             .parse()?;
                     path_dep_workspace_manifests
                         .insert(path_dep_metadata.workspace_root.clone(), manifest);
                 }
                 &path_dep_workspace_manifests[&path_dep_metadata.workspace_root]
             };
         add_crate_to_source_distribution(
-            &mut writer,
-            &pyproject_toml_path,
+            writer,
+            pyproject_toml_path,
             path_dep,
             path_dep_workspace_manifest,
             &root_dir.join(LOCAL_DEPENDENCIES_FOLDER).join(name),
             &known_path_deps,
             false,
         )
         .context(format!(
@@ -598,19 +666,19 @@
             name,
             path_dep.display()
         ))?;
     }
 
     // Add the main crate
     add_crate_to_source_distribution(
-        &mut writer,
-        &pyproject_toml_path,
+        writer,
+        pyproject_toml_path,
         manifest_path,
         &workspace_manifest,
-        &root_dir,
+        root_dir,
         &known_path_deps,
         true,
     )?;
 
     let abs_manifest_path = manifest_path
         .normalize()
         .with_context(|| format!("failed to normalize path `{}`", manifest_path.display()))?
@@ -679,20 +747,75 @@
                 writer.add_directory(target)?;
             } else {
                 writer.add_file(target, &source)?;
             }
         }
     }
 
+    Ok(())
+}
+
+/// Creates a source distribution, packing the root crate and all local dependencies
+///
+/// The source distribution format is specified in
+/// [PEP 517 under "build_sdist"](https://www.python.org/dev/peps/pep-0517/#build-sdist)
+/// and in
+/// https://packaging.python.org/specifications/source-distribution-format/#source-distribution-file-format
+pub fn source_distribution(
+    build_context: &BuildContext,
+    pyproject: &PyProjectToml,
+    excludes: Option<Override>,
+) -> Result<PathBuf> {
+    let pyproject_toml_path = build_context
+        .pyproject_toml_path
+        .normalize()
+        .with_context(|| {
+            format!(
+                "failed to normalize path `{}`",
+                build_context.pyproject_toml_path.display()
+            )
+        })?
+        .into_path_buf();
+    let metadata21 = &build_context.metadata21;
+    let mut writer = SDistWriter::new(&build_context.out, metadata21, excludes)?;
+    let root_dir = PathBuf::from(format!(
+        "{}-{}",
+        &metadata21.get_distribution_escaped(),
+        &metadata21.get_version_escaped()
+    ));
+
+    match pyproject.sdist_generator() {
+        SdistGenerator::Cargo => add_cargo_package_files_to_sdist(
+            build_context,
+            &pyproject_toml_path,
+            &mut writer,
+            &root_dir,
+        )?,
+        SdistGenerator::Git => {
+            add_git_tracked_files_to_sdist(&pyproject_toml_path, &mut writer, &root_dir)?
+        }
+    }
+
+    let pyproject_toml_path = build_context
+        .pyproject_toml_path
+        .normalize()
+        .with_context(|| {
+            format!(
+                "failed to normalize path `{}`",
+                build_context.pyproject_toml_path.display()
+            )
+        })?
+        .into_path_buf();
+    let pyproject_dir = pyproject_toml_path.parent().unwrap();
     // Add readme, license
     if let Some(project) = pyproject.project.as_ref() {
         if let Some(pyproject_toml::ReadMe::RelativePath(readme)) = project.readme.as_ref() {
             writer.add_file(root_dir.join(readme), pyproject_dir.join(readme))?;
         }
-        if let Some(pyproject_toml::License {
+        if let Some(pyproject_toml::License::Table {
             file: Some(license),
             text: None,
         }) = project.license.as_ref()
         {
             writer.add_file(root_dir.join(license), pyproject_dir.join(license))?;
         }
     }
```

### Comparing `maturin-1.0.0b7/src/target.rs` & `maturin-1.0.0b8/src/target.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/templates/.gitignore.j2` & `maturin-1.0.0b8/src/templates/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/templates/Cargo.toml.j2` & `maturin-1.0.0b8/src/templates/Cargo.toml.j2`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/templates/lib.rs.j2` & `maturin-1.0.0b8/src/templates/lib.rs.j2`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/templates/pyproject.toml.j2` & `maturin-1.0.0b8/src/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/src/upload.rs` & `maturin-1.0.0b8/src/upload.rs`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 use anyhow::{bail, Context, Result};
 use bytesize::ByteSize;
 use configparser::ini::Ini;
 use fs_err as fs;
 use fs_err::File;
 use multipart::client::lazy::Multipart;
 use regex::Regex;
+use serde::Deserialize;
+use std::collections::HashMap;
 use std::env;
 #[cfg(any(feature = "native-tls", feature = "rustls"))]
 use std::ffi::OsString;
 use std::io;
 use std::path::{Path, PathBuf};
+use std::time::Duration;
 use thiserror::Error;
 use tracing::debug;
 
 /// An account with a registry, possibly incomplete
 #[derive(Debug, clap::Parser)]
 pub struct PublishOpt {
     /// The repository (package index) to upload the package to. Should be a section in the config file.
@@ -192,20 +195,31 @@
 /// 4. `MATURIN_USERNAME` and `MATURIN_PASSWORD` environment variables
 /// 5. the password keyring
 /// 6. interactive prompt
 fn resolve_pypi_cred(
     opt: &PublishOpt,
     config: &Ini,
     registry_name: Option<&str>,
+    registry_url: &str,
 ) -> (String, String) {
     // API token from environment variable takes priority
     if let Ok(token) = env::var("MATURIN_PYPI_TOKEN") {
         return ("__token__".to_string(), token);
     }
 
+    // Try to get a token via OIDC exchange
+    match resolve_pypi_token_via_oidc(registry_url) {
+        Ok(Some(token)) => {
+            eprintln!("🔐 Using trusted publisher for upload");
+            return ("__token__".to_string(), token);
+        }
+        Ok(None) => {}
+        Err(e) => eprintln!("⚠️ Warning: Failed to resolve PyPI token via OIDC: {}", e),
+    }
+
     if let Some((username, password)) =
         registry_name.and_then(|name| load_pypi_cred_from_config(config, name))
     {
         eprintln!("🔐 Using credential in pypirc for upload");
         return (username, password);
     }
 
@@ -215,14 +229,78 @@
         .password
         .clone()
         .or_else(|| env::var("MATURIN_PASSWORD").ok())
         .unwrap_or_else(|| get_password(&username));
     (username, password)
 }
 
+#[derive(Debug, Deserialize)]
+struct OidcAudienceResponse {
+    audience: String,
+}
+
+#[derive(Debug, Deserialize)]
+struct OidcTokenResponse {
+    value: String,
+}
+
+#[derive(Debug, Deserialize)]
+struct MintTokenResponse {
+    token: String,
+}
+
+/// Trusted Publisher support for GitHub Actions
+fn resolve_pypi_token_via_oidc(registry_url: &str) -> Result<Option<String>> {
+    if env::var_os("GITHUB_ACTIONS").is_none() {
+        return Ok(None);
+    }
+    if let (Ok(req_token), Ok(req_url)) = (
+        env::var("ACTIONS_ID_TOKEN_REQUEST_TOKEN"),
+        env::var("ACTIONS_ID_TOKEN_REQUEST_URL"),
+    ) {
+        let registry_url = url::Url::parse(registry_url)?;
+        let mut audience_url = registry_url.clone();
+        audience_url.set_path("_/oidc/audience");
+        debug!("Requesting OIDC audience from {}", audience_url);
+        let agent = http_agent()?;
+        let audience_res = agent
+            .get(audience_url.as_str())
+            .timeout(Duration::from_secs(30))
+            .call()?;
+        if audience_res.status() == 404 {
+            // OIDC is not enabled/supported on this registry
+            return Ok(None);
+        }
+        let audience = audience_res.into_json::<OidcAudienceResponse>()?.audience;
+
+        debug!("Requesting OIDC token for {} from {}", audience, req_url);
+        let request_token_res: OidcTokenResponse = agent
+            .get(&req_url)
+            .query("audience", &audience)
+            .set("Authorization", &format!("bearer {req_token}"))
+            .timeout(Duration::from_secs(30))
+            .call()?
+            .into_json()?;
+        let oidc_token = request_token_res.value;
+
+        let mut mint_token_url = registry_url;
+        mint_token_url.set_path("_/oidc/github/mint-token");
+        debug!("Requesting API token from {}", mint_token_url);
+        let mut mint_token_req = HashMap::new();
+        mint_token_req.insert("token", oidc_token);
+        let mint_token_res = agent
+            .post(mint_token_url.as_str())
+            .timeout(Duration::from_secs(30))
+            .send_json(mint_token_req)?
+            .into_json::<MintTokenResponse>()?;
+        return Ok(Some(mint_token_res.token));
+    }
+    Ok(None)
+}
+
 /// Asks for username and password for a registry account where missing.
 fn complete_registry(opt: &PublishOpt) -> Result<Registry> {
     // load creds from pypirc if found
     let pypirc = load_pypirc();
     let (registry_name, registry_url) = if let Some(repository_url) = opt.repository_url.as_deref()
     {
         let name = match repository_url {
@@ -244,15 +322,15 @@
         bail!(
             "Failed to get registry {} in .pypirc. \
                 Note: Your index didn't start with http:// or https://, \
                 which is required for non-pypirc indices.",
             opt.repository
         );
     };
-    let (username, password) = resolve_pypi_cred(opt, &pypirc, registry_name);
+    let (username, password) = resolve_pypi_cred(opt, &pypirc, registry_name, &registry_url);
     let registry = Registry::new(username, password, registry_url);
 
     Ok(registry)
 }
 
 /// Port of pip's `canonicalize_name`
 /// https://github.com/pypa/pip/blob/b33e791742570215f15663410c3ed987d2253d5b/src/pip/_vendor/packaging/utils.py#L18-L25
```

### Comparing `maturin-1.0.0b7/test-dockerfile.sh` & `maturin-1.0.0b8/test-dockerfile.sh`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b7/PKG-INFO` & `maturin-1.0.0b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: maturin
-Version: 1.0.0b7
+Version: 1.0.0b8
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: tomli >= 1.1.0 ; python_version < '3.11'
-Requires-Dist: ziglang ~= 0.10.0 ; extra == 'zig'
+Requires-Dist: tomli >=1.1.0 ; python_version < '3.11'
+Requires-Dist: ziglang ~=0.10.0 ; extra == 'zig'
 Requires-Dist: patchelf ; extra == 'patchelf'
 Provides-Extra: zig
 Provides-Extra: patchelf
 Summary: Build and publish crates with pyo3, rust-cpython and cffi bindings as well as rust binaries as python packages
 Keywords: python,cffi,packaging,pypi,pyo3
 Home-Page: https://github.com/pyo3/maturin
 Author: konstin <konstin@mailbox.org>, messense <messense@icloud.com>
 Author-email: konstin <konstin@mailbox.org>, messense <messense@icloud.com>
 License: MIT OR Apache-2.0
-Requires-Python: >= 3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/PyO3/maturin
 Project-URL: Issues, https://github.com/PyO3/maturin/issues
 Project-URL: Documentation, https://maturin.rs
 Project-URL: Changelog, https://maturin.rs/changelog.html
 
 # Maturin
```

