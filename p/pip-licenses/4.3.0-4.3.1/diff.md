# Comparing `tmp/pip-licenses-4.3.0.tar.gz` & `tmp/pip-licenses-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pip-licenses-4.3.0.tar", last modified: Tue Apr 25 08:14:50 2023, max compression
+gzip compressed data, was "dist/pip-licenses-4.3.1.tar", last modified: Thu May  4 02:33:00 2023, max compression
```

## Comparing `pip-licenses-4.3.0.tar` & `pip-licenses-4.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-25 08:14:50.275305 pip-licenses-4.3.0/
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     5344 2023-04-25 08:08:23.000000 pip-licenses-4.3.0/CHANGELOG.md
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1063 2020-12-06 15:11:59.000000 pip-licenses-4.3.0/LICENSE
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)      129 2022-12-04 03:57:54.000000 pip-licenses-4.3.0/MANIFEST.in
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    30934 2023-04-25 08:14:50.275305 pip-licenses-4.3.0/PKG-INFO
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    21661 2023-04-25 08:07:16.000000 pip-licenses-4.3.0/README.md
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-25 08:14:50.275305 pip-licenses-4.3.0/pip_licenses.egg-info/
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    30934 2023-04-25 08:14:50.000000 pip-licenses-4.3.0/pip_licenses.egg-info/PKG-INFO
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)      361 2023-04-25 08:14:50.000000 pip-licenses-4.3.0/pip_licenses.egg-info/SOURCES.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)        1 2023-04-25 08:14:50.000000 pip-licenses-4.3.0/pip_licenses.egg-info/dependency_links.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       51 2023-04-25 08:14:50.000000 pip-licenses-4.3.0/pip_licenses.egg-info/entry_points.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       85 2023-04-25 08:14:50.000000 pip-licenses-4.3.0/pip_licenses.egg-info/requires.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       12 2023-04-25 08:14:50.000000 pip-licenses-4.3.0/pip_licenses.egg-info/top_level.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    32669 2023-04-25 08:07:52.000000 pip-licenses-4.3.0/piplicenses.py
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)        0 2022-12-04 03:57:54.000000 pip-licenses-4.3.0/py.typed
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1367 2023-04-25 08:14:50.275305 pip-licenses-4.3.0/setup.cfg
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     2347 2022-12-04 03:57:54.000000 pip-licenses-4.3.0/setup.py
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    34555 2023-04-25 08:07:16.000000 pip-licenses-4.3.0/test_piplicenses.py
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-25 08:14:50.265305 pip-licenses-4.3.0/tests/
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-25 08:14:50.275305 pip-licenses-4.3.0/tests/fixtures/
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       16 2020-12-06 15:11:59.000000 pip-licenses-4.3.0/tests/fixtures/unicode_characters.txt
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-05-04 02:33:00.846429 pip-licenses-4.3.1/
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     5499 2023-05-04 02:29:28.000000 pip-licenses-4.3.1/CHANGELOG.md
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1063 2020-12-06 15:11:59.000000 pip-licenses-4.3.1/LICENSE
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)      129 2022-12-04 03:57:54.000000 pip-licenses-4.3.1/MANIFEST.in
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    31115 2023-05-04 02:33:00.846429 pip-licenses-4.3.1/PKG-INFO
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    21661 2023-04-25 08:07:16.000000 pip-licenses-4.3.1/README.md
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-05-04 02:33:00.846429 pip-licenses-4.3.1/pip_licenses.egg-info/
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    31115 2023-05-04 02:33:00.000000 pip-licenses-4.3.1/pip_licenses.egg-info/PKG-INFO
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)      361 2023-05-04 02:33:00.000000 pip-licenses-4.3.1/pip_licenses.egg-info/SOURCES.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)        1 2023-05-04 02:33:00.000000 pip-licenses-4.3.1/pip_licenses.egg-info/dependency_links.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       51 2023-05-04 02:33:00.000000 pip-licenses-4.3.1/pip_licenses.egg-info/entry_points.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       85 2023-05-04 02:33:00.000000 pip-licenses-4.3.1/pip_licenses.egg-info/requires.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       12 2023-05-04 02:33:00.000000 pip-licenses-4.3.1/pip_licenses.egg-info/top_level.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    33206 2023-05-04 02:26:34.000000 pip-licenses-4.3.1/piplicenses.py
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)        0 2022-12-04 03:57:54.000000 pip-licenses-4.3.1/py.typed
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1367 2023-05-04 02:33:00.846429 pip-licenses-4.3.1/setup.cfg
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     2347 2022-12-04 03:57:54.000000 pip-licenses-4.3.1/setup.py
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    35764 2023-05-04 02:22:44.000000 pip-licenses-4.3.1/test_piplicenses.py
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-05-04 02:33:00.846429 pip-licenses-4.3.1/tests/
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-05-04 02:33:00.846429 pip-licenses-4.3.1/tests/fixtures/
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       16 2020-12-06 15:11:59.000000 pip-licenses-4.3.1/tests/fixtures/unicode_characters.txt
```

### Comparing `pip-licenses-4.3.0/CHANGELOG.md` & `pip-licenses-4.3.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 ## CHANGELOG
 
+### 4.3.1
+
+* Fix to treat package names as normalized as in [PEP 503](https://peps.python.org/pep-0503/) with `--packages` and `--ignore-packages` option
+
 ### 4.3.0
 
 * Implement new option `--no-version`
 
 ### 4.2.0
 
 * Implement new option `--with-maintainers`
```

### Comparing `pip-licenses-4.3.0/LICENSE` & `pip-licenses-4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-licenses-4.3.0/PKG-INFO` & `pip-licenses-4.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-licenses
-Version: 4.3.0
+Version: 4.3.1
 Summary: Dump the software license list of Python packages installed with pip.
 Home-page: https://github.com/raimon49/pip-licenses
 Author: raimon
 Author-email: raimon49@hotmail.com
 License: MIT
 Project-URL: Releases, https://github.com/raimon49/pip-licenses/releases
 Project-URL: Issues, https://github.com/raimon49/pip-licenses/issues
@@ -825,14 +825,23 @@
 .. |PyPI - Downloads| image:: https://img.shields.io/pypi/dm/pip-licenses
    :target: https://pypistats.org/packages/pip-licenses
 
 
 CHANGELOG
 ---------
 
+.. _431:
+
+4.3.1
+~~~~~
+
+-  Fix to treat package names as normalized as in `PEP
+   503 <https://peps.python.org/pep-0503/>`__ with ``--packages`` and
+   ``--ignore-packages`` option
+
 .. _430:
 
 4.3.0
 ~~~~~
 
 -  Implement new option ``--no-version``
```

### Comparing `pip-licenses-4.3.0/README.md` & `pip-licenses-4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pip-licenses-4.3.0/pip_licenses.egg-info/PKG-INFO` & `pip-licenses-4.3.1/pip_licenses.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-licenses
-Version: 4.3.0
+Version: 4.3.1
 Summary: Dump the software license list of Python packages installed with pip.
 Home-page: https://github.com/raimon49/pip-licenses
 Author: raimon
 Author-email: raimon49@hotmail.com
 License: MIT
 Project-URL: Releases, https://github.com/raimon49/pip-licenses/releases
 Project-URL: Issues, https://github.com/raimon49/pip-licenses/issues
@@ -825,14 +825,23 @@
 .. |PyPI - Downloads| image:: https://img.shields.io/pypi/dm/pip-licenses
    :target: https://pypistats.org/packages/pip-licenses
 
 
 CHANGELOG
 ---------
 
+.. _431:
+
+4.3.1
+~~~~~
+
+-  Fix to treat package names as normalized as in `PEP
+   503 <https://peps.python.org/pep-0503/>`__ with ``--packages`` and
+   ``--ignore-packages`` option
+
 .. _430:
 
 4.3.0
 ~~~~~
 
 -  Implement new option ``--no-version``
```

### Comparing `pip-licenses-4.3.0/piplicenses.py` & `pip-licenses-4.3.1/piplicenses.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     from email.message import Message
     from typing import Callable, Dict, Iterator, Optional, Sequence
 
 
 open = open  # allow monkey patching
 
 __pkgname__ = "pip-licenses"
-__version__ = "4.3.0"
+__version__ = "4.3.1"
 __author__ = "raimon"
 __license__ = "MIT"
 __summary__ = (
     "Dump the software license list of Python packages installed with pip."
 )
 __url__ = "https://github.com/raimon49/pip-licenses"
 
@@ -125,14 +125,32 @@
     for priority_key in ["Homepage", "Source", "Changelog", "Bug Tracker"]:
         if priority_key in candidates:
             return candidates[priority_key]
 
     return None
 
 
+PATTERN_DELIMITER = re.compile(r"[-_.]+")
+
+
+def normalize_pkg_name(pkg_name: str) -> str:
+    """Return normalized name according to PEP specification
+
+    See here: https://peps.python.org/pep-0503/#normalized-names
+
+    Args:
+        pkg_name: Package name it is extracted from the package metadata
+                  or specified in the CLI
+
+    Returns:
+        normalized packege name
+    """
+    return PATTERN_DELIMITER.sub("-", pkg_name).lower()
+
+
 METADATA_KEYS: Dict[str, List[Callable[[Message], Optional[str]]]] = {
     "home-page": [extract_homepage],
     "author": [
         lambda metadata: metadata.get("author"),
         lambda metadata: metadata.get("author-email"),
     ],
     "maintainer": [
@@ -250,36 +268,38 @@
 
     if args.python == sys.executable:
         search_paths = sys.path
     else:
         search_paths = get_python_sys_path(args.python)
 
     pkgs = importlib_metadata.distributions(path=search_paths)
-    ignore_pkgs_as_lower = [pkg.lower() for pkg in args.ignore_packages]
-    pkgs_as_lower = [pkg.lower() for pkg in args.packages]
+    ignore_pkgs_as_normalize = [
+        normalize_pkg_name(pkg) for pkg in args.ignore_packages
+    ]
+    pkgs_as_normalize = [normalize_pkg_name(pkg) for pkg in args.packages]
 
     fail_on_licenses = set()
     if args.fail_on:
         fail_on_licenses = set(map(str.strip, args.fail_on.split(";")))
 
     allow_only_licenses = set()
     if args.allow_only:
         allow_only_licenses = set(map(str.strip, args.allow_only.split(";")))
 
     for pkg in pkgs:
-        pkg_name = pkg.metadata["name"]
+        pkg_name = normalize_pkg_name(pkg.metadata["name"])
         pkg_name_and_version = pkg_name + ":" + pkg.metadata["version"]
 
         if (
-            pkg_name.lower() in ignore_pkgs_as_lower
-            or pkg_name_and_version.lower() in ignore_pkgs_as_lower
+            pkg_name.lower() in ignore_pkgs_as_normalize
+            or pkg_name_and_version.lower() in ignore_pkgs_as_normalize
         ):
             continue
 
-        if pkgs_as_lower and pkg_name.lower() not in pkgs_as_lower:
+        if pkgs_as_normalize and pkg_name.lower() not in pkgs_as_normalize:
             continue
 
         if not args.with_system and pkg_name in SYSTEM_PACKAGES:
             continue
 
         pkg_info = get_pkg_info(pkg)
```

### Comparing `pip-licenses-4.3.0/setup.cfg` & `pip-licenses-4.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pip-licenses-4.3.0/setup.py` & `pip-licenses-4.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `pip-licenses-4.3.0/test_piplicenses.py` & `pip-licenses-4.3.1/test_piplicenses.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     enum_key_to_value,
     extract_homepage,
     factory_styled_table_with_args,
     find_license_from_classifier,
     get_output_fields,
     get_packages,
     get_sortby,
+    normalize_pkg_name,
     output_colored,
     save_if_needs,
     select_license_by_source,
     value_to_enum_key,
 )
 
 if TYPE_CHECKING:
@@ -425,14 +426,26 @@
         ]
         args = self.parser.parse_args(ignore_packages_args)
         table = create_licenses_table(args)
 
         pkg_name_columns = self._create_pkg_name_columns(table)
         self.assertNotIn(ignore_pkg_name, pkg_name_columns)
 
+    def test_ignore_normalized_packages(self) -> None:
+        ignore_pkg_name = "pip-licenses"
+        ignore_packages_args = [
+            "--ignore-package=pip_licenses",
+            "--with-system",
+        ]
+        args = self.parser.parse_args(ignore_packages_args)
+        table = create_licenses_table(args)
+
+        pkg_name_columns = self._create_pkg_name_columns(table)
+        self.assertNotIn(ignore_pkg_name, pkg_name_columns)
+
     def test_ignore_packages_and_version(self) -> None:
         # Fictitious version that does not exist
         ignore_pkg_name = "prettytable"
         ignore_pkg_spec = ignore_pkg_name + ":1.99.99"
         ignore_packages_args = [
             "--ignore-package=" + ignore_pkg_spec,
             "--with-system",
@@ -449,14 +462,26 @@
         only_packages_args = ["--packages=" + pkg_name]
         args = self.parser.parse_args(only_packages_args)
         table = create_licenses_table(args)
 
         pkg_name_columns = self._create_pkg_name_columns(table)
         self.assertListEqual([pkg_name], pkg_name_columns)
 
+    def test_with_normalized_packages(self) -> None:
+        pkg_name = "typing_extensions"
+        only_packages_args = [
+            "--package=typing-extensions",
+            "--with-system",
+        ]
+        args = self.parser.parse_args(only_packages_args)
+        table = create_licenses_table(args)
+
+        pkg_name_columns = self._create_pkg_name_columns(table)
+        self.assertListEqual([pkg_name], pkg_name_columns)
+
     def test_with_packages_with_system(self) -> None:
         pkg_name = "prettytable"
         only_packages_args = ["--packages=" + pkg_name, "--with-system"]
         args = self.parser.parse_args(only_packages_args)
         table = create_licenses_table(args)
 
         pkg_name_columns = self._create_pkg_name_columns(table)
@@ -916,14 +941,22 @@
     with pytest.raises(SystemExit) as ex:
         parser.parse_args(["--filter-strings", "--filter-code-page=XX"])
     capture = capsys.readouterr().err
     for arg in ("invalid code", "--filter-code-page"):
         assert arg in capture
 
 
+def test_normalize_pkg_name() -> None:
+    expected_normalized_name = "pip-licenses"
+
+    assert normalize_pkg_name("pip_licenses") == expected_normalized_name
+    assert normalize_pkg_name("pip.licenses") == expected_normalized_name
+    assert normalize_pkg_name("Pip-Licenses") == expected_normalized_name
+
+
 def test_extract_homepage_home_page_set() -> None:
     metadata = MagicMock()
     metadata.get.return_value = "Foobar"
 
     assert "Foobar" == extract_homepage(metadata=metadata)  # type: ignore
 
     metadata.get.assert_called_once_with("home-page", None)
```

