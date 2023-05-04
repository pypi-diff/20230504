# Comparing `tmp/deadnews_template_python-1.0.2a4.tar.gz` & `tmp/deadnews_template_python-1.0.2a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadnews_template_python-1.0.2a4.tar", max compression
+gzip compressed data, was "deadnews_template_python-1.0.2a5.tar", max compression
```

## Comparing `deadnews_template_python-1.0.2a4.tar` & `deadnews_template_python-1.0.2a5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-05-03 16:06:03.874501 deadnews_template_python-1.0.2a4/LICENSE
--rw-r--r--   0        0        0      845 2023-05-03 16:06:03.874501 deadnews_template_python-1.0.2a4/README.md
--rw-r--r--   0        0        0     2111 2023-05-03 16:06:20.978578 deadnews_template_python-1.0.2a4/pyproject.toml
--rw-r--r--   0        0        0      195 2023-05-03 16:06:03.874501 deadnews_template_python-1.0.2a4/src/deadnews_template_python/__init__.py
--rw-r--r--   0        0        0     1557 1970-01-01 00:00:00.000000 deadnews_template_python-1.0.2a4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-04 01:29:42.068787 deadnews_template_python-1.0.2a5/LICENSE
+-rw-r--r--   0        0        0      845 2023-05-04 01:29:42.068787 deadnews_template_python-1.0.2a5/README.md
+-rw-r--r--   0        0        0     2363 2023-05-04 01:30:04.224918 deadnews_template_python-1.0.2a5/pyproject.toml
+-rw-r--r--   0        0        0      160 2023-05-04 01:29:42.068787 deadnews_template_python-1.0.2a5/src/deadnews_template_python/__init__.py
+-rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 deadnews_template_python-1.0.2a5/PKG-INFO
```

### Comparing `deadnews_template_python-1.0.2a4/LICENSE` & `deadnews_template_python-1.0.2a5/LICENSE`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-1.0.2a4/README.md` & `deadnews_template_python-1.0.2a5/README.md`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-1.0.2a4/pyproject.toml` & `deadnews_template_python-1.0.2a5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "deadnews-template-python"
-version = "1.0.2-alpha.4"
+version = "1.0.2-alpha.5"
 description = "Python Project Template"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/deadnews-template-python"
 repository = "https://github.com/DeadNews/deadnews-template-python"
 keywords = ["python", "template", "layout"]
 classifiers = ["Operating System :: OS Independent"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 
 [tool.poetry.group.ci.dependencies]
 black = "^23.3.0"
 mypy = "^1.2.0"
-poethepoet = "^0.19.0"
+poethepoet = "^0.20.0"
 ruff = "^0.0.264"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 
 [tool.poe.tasks]
@@ -61,14 +61,16 @@
 [tool.coverage.report]
 exclude_lines = ["if __name__ == .__main__.:"]
 
 [tool.ruff]
 line-length = 99
 select = ["ALL"]
 ignore = [
+  "D203",    # 1 blank line required before class docstring
+  "D212",    # Multi-line docstring summary should start at the first line
   "E501",    # Line too long
   "EXE001",  # Shebang is present but file is not executable
   "FBT001",  # Boolean positional arg in function definition
   "PLR2004", # Magic value used in comparison
   "S113",    # Missing requests timeout
   "S603",    # Calling subprocess.Popen with shell=False
 ]
@@ -81,7 +83,14 @@
 allow-dict-calls-with-keyword-arguments = false
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.mccabe]
 max-complexity = 10
+
+[tool.ruff.pylint]
+max-args = 5
+
+# [tool.ruff.pydocstyle]
+# # Use Google-style docstrings.
+# convention = "pep257"
```

### Comparing `deadnews_template_python-1.0.2a4/PKG-INFO` & `deadnews_template_python-1.0.2a5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: deadnews-template-python
-Version: 1.0.2a4
+Version: 1.0.2a5
 Summary: Python Project Template
 Home-page: https://github.com/DeadNews/deadnews-template-python
 License: MIT
 Keywords: python,template,layout
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/DeadNews/deadnews-template-python
 Description-Content-Type: text/markdown
 
 # deadnews-template-python
```

