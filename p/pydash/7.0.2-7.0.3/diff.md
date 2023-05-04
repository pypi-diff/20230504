# Comparing `tmp/pydash-7.0.2.tar.gz` & `tmp/pydash-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydash-7.0.2.tar", last modified: Thu Apr 27 16:26:18 2023, max compression
+gzip compressed data, was "pydash-7.0.3.tar", last modified: Thu May  4 14:18:50 2023, max compression
```

## Comparing `pydash-7.0.2.tar` & `pydash-7.0.3.tar`

### file list

```diff
@@ -1,633 +1,633 @@
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.466705 pydash-7.0.2/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.414261 pydash-7.0.2/.tox/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400546 pydash-7.0.2/.tox/.package/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400608 pydash-7.0.2/.tox/.package/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400655 pydash-7.0.2/.tox/.package/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400705 pydash-7.0.2/.tox/.package/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.421087 pydash-7.0.2/.tox/.package/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:46.000000 pydash-7.0.2/.tox/.package/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400826 pydash-7.0.2/.tox/.pkg/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400864 pydash-7.0.2/.tox/.pkg/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400903 pydash-7.0.2/.tox/.pkg/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400940 pydash-7.0.2/.tox/.pkg/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.421374 pydash-7.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:04.000000 pydash-7.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.401048 pydash-7.0.2/.tox/3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.401085 pydash-7.0.2/.tox/3.11/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.401129 pydash-7.0.2/.tox/3.11/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.403638 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.421610 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.421699 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.421784 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.421870 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.422164 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.422256 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.422353 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.422467 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.422568 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.422662 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.422765 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423048 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423148 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423239 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423330 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423422 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.402244 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423514 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423799 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423904 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.424005 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:23.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.424264 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.424365 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.424573 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.424651 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.424884 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.424977 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.425197 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:03.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.425405 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.425485 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.425567 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:35:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.425663 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.425752 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.425850 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:23:24.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426100 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426185 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426277 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426365 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426448 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:21.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426538 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426621 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.403741 pydash-7.0.2/.tox/py310/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.403779 pydash-7.0.2/.tox/py310/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.403816 pydash-7.0.2/.tox/py310/lib/python3.10/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.406074 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426709 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426800 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426889 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426977 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427242 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427318 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427399 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427474 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427550 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427635 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427729 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427979 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428064 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428148 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428229 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428318 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428409 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.404791 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428493 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428776 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428866 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428947 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.429170 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.429250 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.429494 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.429588 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.429806 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.429893 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.430123 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:53:26.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.430318 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.430402 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.430494 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.430582 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.430678 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.430770 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:53:43.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431018 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431097 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431178 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431264 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431352 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:40.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431679 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:40.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431782 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431883 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.406167 pydash-7.0.2/.tox/py311/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.406203 pydash-7.0.2/.tox/py311/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.406241 pydash-7.0.2/.tox/py311/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.408814 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431985 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432068 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432157 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432252 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432517 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432599 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432678 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432764 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432847 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432940 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433028 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433273 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433354 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433446 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433528 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433615 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.407209 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433709 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433966 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.434044 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.434128 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:37.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.434404 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.434516 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.434807 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.434910 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.435156 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.435254 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.435501 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 02:01:09.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.435731 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.435825 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.435916 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 02:06:00.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.435996 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436079 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436173 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:54:38.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436408 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436497 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436586 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436669 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436751 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:35.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436833 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436924 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.408936 pydash-7.0.2/.tox/py37/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.408979 pydash-7.0.2/.tox/py37/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.409018 pydash-7.0.2/.tox/py37/lib/python3.7/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.411424 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437013 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437096 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437173 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437250 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437473 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437553 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437639 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437719 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437797 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437878 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438152 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438246 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438340 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438433 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438512 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438603 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.409998 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438690 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438920 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.439001 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.439091 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:32.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.439371 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.439461 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.439689 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.439773 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:50:32.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.439972 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440053 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440248 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:52.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440446 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440529 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440607 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/py/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.410863 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440688 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/py/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440774 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440857 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440937 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441155 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441235 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441315 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441394 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441479 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:30.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441715 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:30.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441800 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.411550 pydash-7.0.2/.tox/py38/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.411585 pydash-7.0.2/.tox/py38/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.411622 pydash-7.0.2/.tox/py38/lib/python3.8/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.414204 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441883 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441971 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442077 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442176 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442456 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442560 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442645 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442740 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442840 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442942 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443050 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443335 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443431 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443518 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443616 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443715 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/importlib_resources/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/importlib_resources/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443823 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443951 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.412680 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.444068 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.444349 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.444458 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.444558 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.444824 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.444930 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.445201 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.445322 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.445542 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.445651 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.445919 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:51:24.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.446176 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.446291 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.446408 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.446523 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.446634 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.446740 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.447048 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.447174 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.447301 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.447423 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.447540 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:35.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.447803 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:35.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.447919 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448038 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.414298 pydash-7.0.2/.tox/py39/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.414337 pydash-7.0.2/.tox/py39/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.414387 pydash-7.0.2/.tox/py39/lib/python3.9/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.417498 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448159 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448271 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448374 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448476 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448757 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448868 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448970 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449059 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449157 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449263 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449375 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449649 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449755 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449865 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449979 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.450089 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.450201 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.415679 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.450315 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.450583 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.450701 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.450811 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.451060 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.451170 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.451395 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.451521 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.451739 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.451841 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.452127 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:52:27.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.452335 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.452417 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.452499 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.452588 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.452685 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.452789 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453034 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453126 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453223 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453328 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453432 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:38.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453664 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:38.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453769 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453872 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/twine/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)     1257 2021-06-27 18:15:07.000000 pydash-7.0.2/AUTHORS.rst
--rw-r--r--   0 dgilland   (501) staff       (20)    40342 2023-04-27 16:17:02.000000 pydash-7.0.2/CHANGELOG.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2581 2020-10-29 15:03:50.000000 pydash-7.0.2/CONTRIBUTING.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     1072 2021-01-05 22:53:19.000000 pydash-7.0.2/LICENSE.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      283 2023-03-18 22:34:56.000000 pydash-7.0.2/MANIFEST.in
--rw-r--r--   0 dgilland   (501) staff       (20)    43817 2023-04-27 16:26:18.466780 pydash-7.0.2/PKG-INFO
--rw-r--r--   0 dgilland   (501) staff       (20)     1243 2020-10-29 02:16:13.000000 pydash-7.0.2/README.rst
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.456801 pydash-7.0.2/docs/
--rw-r--r--   0 dgilland   (501) staff       (20)     3937 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/Makefile
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.457028 pydash-7.0.2/docs/_static/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.2/docs/_static/.gitignore
--rw-r--r--   0 dgilland   (501) staff       (20)      137 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/_static/theme_override.css
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.457168 pydash-7.0.2/docs/_templates/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.2/docs/_templates/.gitignore
--rw-r--r--   0 dgilland   (501) staff       (20)     2885 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/api.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       28 2014-07-29 03:38:06.000000 pydash-7.0.2/docs/authors.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     4065 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/callbacks.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2927 2021-09-28 21:40:18.000000 pydash-7.0.2/docs/chaining.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       30 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/changelog.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     5733 2022-09-23 13:07:13.000000 pydash-7.0.2/docs/conf.py
--rw-r--r--   0 dgilland   (501) staff       (20)       33 2014-07-29 03:34:57.000000 pydash-7.0.2/docs/contributing.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      760 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/deeppath.rst
--rw-rw-r--   0 dgilland   (501) staff       (20)       29 2020-10-28 20:30:40.000000 pydash-7.0.2/docs/devguide.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2045 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/differences.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      605 2020-10-29 19:54:30.000000 pydash-7.0.2/docs/index.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      187 2021-06-27 18:15:05.000000 pydash-7.0.2/docs/installation.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      100 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/kudos.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       45 2021-01-05 22:53:19.000000 pydash-7.0.2/docs/license.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     1499 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/quickstart.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      562 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/templating.rst
--rw-r--r--   0 dgilland   (501) staff       (20)    10538 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/upgrading.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      497 2014-08-20 02:16:49.000000 pydash-7.0.2/docs/versioning.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     4371 2021-07-15 23:20:06.000000 pydash-7.0.2/pylintrc
--rw-r--r--   0 dgilland   (501) staff       (20)      274 2022-09-23 12:58:40.000000 pydash-7.0.2/pyproject.toml
--rw-r--r--   0 dgilland   (501) staff       (20)       10 2020-10-28 20:38:46.000000 pydash-7.0.2/requirements.txt
--rw-r--r--   0 dgilland   (501) staff       (20)     2528 2023-04-27 16:26:18.467153 pydash-7.0.2/setup.cfg
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.417917 pydash-7.0.2/src/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.460127 pydash-7.0.2/src/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)    11148 2023-04-27 16:17:18.000000 pydash-7.0.2/src/pydash/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)    69680 2023-04-12 02:13:49.000000 pydash-7.0.2/src/pydash/arrays.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.461728 pydash-7.0.2/src/pydash/chaining/
--rw-r--r--   0 dgilland   (501) staff       (20)      111 2023-03-18 22:34:56.000000 pydash-7.0.2/src/pydash/chaining/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1364 2023-03-20 14:30:38.000000 pydash-7.0.2/src/pydash/chaining/all_funcs.py
--rw-r--r--   0 dgilland   (501) staff       (20)   123183 2023-04-12 02:15:39.000000 pydash-7.0.2/src/pydash/chaining/all_funcs.pyi
--rw-r--r--   0 dgilland   (501) staff       (20)     8218 2023-03-20 14:30:38.000000 pydash-7.0.2/src/pydash/chaining/chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)    54698 2023-04-12 02:03:04.000000 pydash-7.0.2/src/pydash/collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)      431 2023-03-18 22:34:56.000000 pydash-7.0.2/src/pydash/exceptions.py
--rw-r--r--   0 dgilland   (501) staff       (20)    39876 2023-04-12 02:03:04.000000 pydash-7.0.2/src/pydash/functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8901 2023-04-12 02:03:04.000000 pydash-7.0.2/src/pydash/helpers.py
--rw-r--r--   0 dgilland   (501) staff       (20)    27145 2023-04-12 02:03:04.000000 pydash-7.0.2/src/pydash/numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    62990 2023-04-12 02:03:04.000000 pydash-7.0.2/src/pydash/objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    26652 2023-03-20 14:30:38.000000 pydash-7.0.2/src/pydash/predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.2/src/pydash/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)    57917 2023-04-12 02:03:04.000000 pydash-7.0.2/src/pydash/strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)      690 2023-04-27 16:14:56.000000 pydash-7.0.2/src/pydash/types.py
--rw-r--r--   0 dgilland   (501) staff       (20)    38320 2023-04-12 02:03:04.000000 pydash-7.0.2/src/pydash/utilities.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.460739 pydash-7.0.2/src/pydash.egg-info/
--rw-r--r--   0 dgilland   (501) staff       (20)    43817 2023-04-27 16:26:16.000000 pydash-7.0.2/src/pydash.egg-info/PKG-INFO
--rw-r--r--   0 dgilland   (501) staff       (20)    16310 2023-04-27 16:26:18.000000 pydash-7.0.2/src/pydash.egg-info/SOURCES.txt
--rw-r--r--   0 dgilland   (501) staff       (20)        1 2023-04-27 16:26:16.000000 pydash-7.0.2/src/pydash.egg-info/dependency_links.txt
--rw-r--r--   0 dgilland   (501) staff       (20)      293 2023-04-27 16:26:16.000000 pydash-7.0.2/src/pydash.egg-info/requires.txt
--rw-r--r--   0 dgilland   (501) staff       (20)        7 2023-04-27 16:26:16.000000 pydash-7.0.2/src/pydash.egg-info/top_level.txt
--rw-r--r--   0 dgilland   (501) staff       (20)     6510 2023-04-06 20:16:10.000000 pydash-7.0.2/tasks.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.464327 pydash-7.0.2/tests/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-23 03:21:55.000000 pydash-7.0.2/tests/__init__.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.418208 pydash-7.0.2/tests/build/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.464479 pydash-7.0.2/tests/build/testresults/
--rw-r--r--   0 dgilland   (501) staff       (20)      925 2023-04-06 01:12:00.000000 pydash-7.0.2/tests/build/testresults/junit.xml
--rw-r--r--   0 dgilland   (501) staff       (20)      143 2022-09-23 13:25:56.000000 pydash-7.0.2/tests/conftest.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1870 2022-09-23 13:11:57.000000 pydash-7.0.2/tests/helpers.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.466591 pydash-7.0.2/tests/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.2/tests/pytest_mypy_testing/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)    16142 2023-04-12 02:13:49.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_arrays.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1234 2023-04-12 02:10:33.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8643 2023-04-12 02:10:41.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)     9870 2023-04-12 02:15:39.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     5582 2023-04-12 02:10:58.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    13212 2023-04-12 02:11:04.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    10786 2023-04-12 02:15:39.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)    13294 2023-04-12 02:15:39.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8532 2023-04-12 02:15:39.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_utilities.py
--rw-r--r--   0 dgilland   (501) staff       (20)      178 2021-06-27 18:15:05.000000 pydash-7.0.2/tests/test_annotations.py
--rw-r--r--   0 dgilland   (501) staff       (20)    24160 2021-09-28 21:40:18.000000 pydash-7.0.2/tests/test_arrays.py
--rw-r--r--   0 dgilland   (501) staff       (20)     4229 2023-03-18 22:34:56.000000 pydash-7.0.2/tests/test_chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)    29669 2022-09-23 13:19:05.000000 pydash-7.0.2/tests/test_collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)     9935 2022-09-23 13:25:56.000000 pydash-7.0.2/tests/test_functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     7640 2021-06-27 18:15:05.000000 pydash-7.0.2/tests/test_numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    28249 2023-03-18 22:34:56.000000 pydash-7.0.2/tests/test_objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    12617 2022-09-23 13:19:37.000000 pydash-7.0.2/tests/test_predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)    33926 2023-04-06 01:12:00.000000 pydash-7.0.2/tests/test_strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)    18221 2023-03-18 22:34:56.000000 pydash-7.0.2/tests/test_utilities.py
--rw-r--r--   0 dgilland   (501) staff       (20)      296 2023-01-28 17:36:13.000000 pydash-7.0.2/tox.ini
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.327670 pydash-7.0.3/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.275059 pydash-7.0.3/.tox/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261449 pydash-7.0.3/.tox/.package/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261507 pydash-7.0.3/.tox/.package/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261558 pydash-7.0.3/.tox/.package/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261598 pydash-7.0.3/.tox/.package/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.281661 pydash-7.0.3/.tox/.package/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:46.000000 pydash-7.0.3/.tox/.package/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261706 pydash-7.0.3/.tox/.pkg/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261748 pydash-7.0.3/.tox/.pkg/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261795 pydash-7.0.3/.tox/.pkg/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261844 pydash-7.0.3/.tox/.pkg/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.281909 pydash-7.0.3/.tox/.pkg/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:04.000000 pydash-7.0.3/.tox/.pkg/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261952 pydash-7.0.3/.tox/3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.261999 pydash-7.0.3/.tox/3.11/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.262051 pydash-7.0.3/.tox/3.11/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.264530 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282129 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282233 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282329 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282427 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282694 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282808 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282902 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.282998 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283109 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283206 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283292 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283543 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283633 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283720 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283804 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283901 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.263151 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.283986 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.284333 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.284456 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.284546 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:23.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.284798 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.284888 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.285106 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.285202 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.285431 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.285512 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.285705 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:03.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.285906 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.285999 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286094 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:35:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286227 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286332 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286425 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:23:24.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286692 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286785 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286873 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.286958 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287045 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:21.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287139 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287223 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.3/.tox/3.11/lib/python3.11/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.264646 pydash-7.0.3/.tox/py310/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.264687 pydash-7.0.3/.tox/py310/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.264726 pydash-7.0.3/.tox/py310/lib/python3.10/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.267143 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287322 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287412 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287498 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287584 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287834 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.287932 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288031 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288125 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288220 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288317 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288404 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288625 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288727 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288816 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288895 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.288978 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.289070 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.265843 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.289168 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.289415 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.289502 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.289579 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.289756 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.289835 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.290068 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.290161 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.290363 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.290438 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.290647 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:53:26.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.290850 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.290943 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291041 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291133 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291229 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291329 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:53:43.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291577 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291658 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291737 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291819 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.291903 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:40.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.292219 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:40.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.292320 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.292429 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.3/.tox/py310/lib/python3.10/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.267244 pydash-7.0.3/.tox/py311/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.267286 pydash-7.0.3/.tox/py311/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.267326 pydash-7.0.3/.tox/py311/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.269736 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.292534 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.292621 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.292709 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.292788 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293041 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293132 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293229 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293328 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293433 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293522 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293606 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293861 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.293959 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294047 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294135 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294215 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.268465 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294309 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294550 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294630 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294714 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:37.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.294918 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.295000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.295229 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.295316 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.295568 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.295664 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.295902 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 02:01:09.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.296176 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.296283 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.296377 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 02:06:00.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.296461 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.296547 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.296645 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:54:38.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.296903 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297024 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297136 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297240 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297335 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:35.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297429 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297524 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.3/.tox/py311/lib/python3.11/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.269839 pydash-7.0.3/.tox/py37/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.269879 pydash-7.0.3/.tox/py37/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.269919 pydash-7.0.3/.tox/py37/lib/python3.7/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.272326 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297626 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297722 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297832 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.297943 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.298197 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.298301 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.298393 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.298482 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.298578 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.298663 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.298919 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299007 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299102 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299199 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299295 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299395 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.270870 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299493 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299766 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299873 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.299980 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:32.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.300245 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.300340 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.300575 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.300660 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:50:32.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.300873 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.300953 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301177 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:52.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301395 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301487 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301582 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/py/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.271765 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301666 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/py/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301749 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301845 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.301946 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.302173 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.302270 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.302373 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.302475 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.302576 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:30.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.302902 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:30.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303021 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.3/.tox/py37/lib/python3.7/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.272423 pydash-7.0.3/.tox/py38/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.272459 pydash-7.0.3/.tox/py38/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.272494 pydash-7.0.3/.tox/py38/lib/python3.8/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.274981 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303133 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303245 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303351 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303436 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303711 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303819 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.303927 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304042 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304157 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304264 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304373 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304653 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304771 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304884 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.304998 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.305122 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/importlib_resources/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/importlib_resources/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.305233 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.305344 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.273504 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.305462 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.305738 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.305858 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.305973 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.306241 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.306355 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.306623 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.306778 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.307019 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.307132 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.307396 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:51:24.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.307668 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.307789 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.307900 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308008 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308122 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308235 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308515 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308630 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308741 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308858 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.308972 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:35.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.309214 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:35.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.309321 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.309424 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.3/.tox/py38/lib/python3.8/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.275111 pydash-7.0.3/.tox/py39/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.275161 pydash-7.0.3/.tox/py39/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.275213 pydash-7.0.3/.tox/py39/lib/python3.9/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.278550 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.309536 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.309641 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.309749 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.309848 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310119 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310232 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310326 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310430 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310536 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310629 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310723 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.310989 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311102 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311206 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311302 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311395 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311491 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.276652 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311595 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311848 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.311954 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.312061 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.312292 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.312388 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.312590 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.312673 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.312872 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.312954 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.313182 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:52:27.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.313383 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.313477 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.313572 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.313659 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.313743 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.313835 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314043 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314125 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314210 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314287 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314370 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:38.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314581 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:38.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314669 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.314759 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.3/.tox/py39/lib/python3.9/site-packages/twine/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)     1257 2021-06-27 18:15:07.000000 pydash-7.0.3/AUTHORS.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)    40554 2023-05-04 14:14:49.000000 pydash-7.0.3/CHANGELOG.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2581 2020-10-29 15:03:50.000000 pydash-7.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     1072 2021-01-05 22:53:19.000000 pydash-7.0.3/LICENSE.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      283 2023-03-18 22:34:56.000000 pydash-7.0.3/MANIFEST.in
+-rw-r--r--   0 dgilland   (501) staff       (20)    44029 2023-05-04 14:18:50.327762 pydash-7.0.3/PKG-INFO
+-rw-r--r--   0 dgilland   (501) staff       (20)     1243 2020-10-29 02:16:13.000000 pydash-7.0.3/README.rst
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.317511 pydash-7.0.3/docs/
+-rw-r--r--   0 dgilland   (501) staff       (20)     3937 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/Makefile
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.317729 pydash-7.0.3/docs/_static/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.3/docs/_static/.gitignore
+-rw-r--r--   0 dgilland   (501) staff       (20)      137 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/_static/theme_override.css
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.317934 pydash-7.0.3/docs/_templates/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.3/docs/_templates/.gitignore
+-rw-r--r--   0 dgilland   (501) staff       (20)     2885 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/api.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       28 2014-07-29 03:38:06.000000 pydash-7.0.3/docs/authors.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     4065 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/callbacks.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2927 2021-09-28 21:40:18.000000 pydash-7.0.3/docs/chaining.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       30 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/changelog.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     5733 2022-09-23 13:07:13.000000 pydash-7.0.3/docs/conf.py
+-rw-r--r--   0 dgilland   (501) staff       (20)       33 2014-07-29 03:34:57.000000 pydash-7.0.3/docs/contributing.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      760 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/deeppath.rst
+-rw-rw-r--   0 dgilland   (501) staff       (20)       29 2020-10-28 20:30:40.000000 pydash-7.0.3/docs/devguide.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2045 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/differences.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      605 2020-10-29 19:54:30.000000 pydash-7.0.3/docs/index.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      187 2021-06-27 18:15:05.000000 pydash-7.0.3/docs/installation.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      100 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/kudos.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       45 2021-01-05 22:53:19.000000 pydash-7.0.3/docs/license.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     1499 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/quickstart.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      562 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/templating.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)    10538 2019-02-04 01:30:20.000000 pydash-7.0.3/docs/upgrading.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      497 2014-08-20 02:16:49.000000 pydash-7.0.3/docs/versioning.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     4371 2021-07-15 23:20:06.000000 pydash-7.0.3/pylintrc
+-rw-r--r--   0 dgilland   (501) staff       (20)      274 2022-09-23 12:58:40.000000 pydash-7.0.3/pyproject.toml
+-rw-r--r--   0 dgilland   (501) staff       (20)       10 2020-10-28 20:38:46.000000 pydash-7.0.3/requirements.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)     2528 2023-05-04 14:18:50.328144 pydash-7.0.3/setup.cfg
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.278985 pydash-7.0.3/src/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.321462 pydash-7.0.3/src/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)    11148 2023-05-04 14:14:07.000000 pydash-7.0.3/src/pydash/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    69733 2023-05-04 14:12:08.000000 pydash-7.0.3/src/pydash/arrays.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.322716 pydash-7.0.3/src/pydash/chaining/
+-rw-r--r--   0 dgilland   (501) staff       (20)      111 2023-03-18 22:34:56.000000 pydash-7.0.3/src/pydash/chaining/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1364 2023-03-20 14:30:38.000000 pydash-7.0.3/src/pydash/chaining/all_funcs.py
+-rw-r--r--   0 dgilland   (501) staff       (20)   123215 2023-05-04 14:12:08.000000 pydash-7.0.3/src/pydash/chaining/all_funcs.pyi
+-rw-r--r--   0 dgilland   (501) staff       (20)     8218 2023-03-20 14:30:38.000000 pydash-7.0.3/src/pydash/chaining/chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    54698 2023-04-12 02:03:04.000000 pydash-7.0.3/src/pydash/collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      431 2023-03-18 22:34:56.000000 pydash-7.0.3/src/pydash/exceptions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    39876 2023-04-12 02:03:04.000000 pydash-7.0.3/src/pydash/functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8901 2023-04-12 02:03:04.000000 pydash-7.0.3/src/pydash/helpers.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    27145 2023-04-12 02:03:04.000000 pydash-7.0.3/src/pydash/numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    62990 2023-04-12 02:03:04.000000 pydash-7.0.3/src/pydash/objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    26652 2023-03-20 14:30:38.000000 pydash-7.0.3/src/pydash/predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.3/src/pydash/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)    57917 2023-04-12 02:03:04.000000 pydash-7.0.3/src/pydash/strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      690 2023-04-27 16:14:56.000000 pydash-7.0.3/src/pydash/types.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    38320 2023-04-12 02:03:04.000000 pydash-7.0.3/src/pydash/utilities.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.322059 pydash-7.0.3/src/pydash.egg-info/
+-rw-r--r--   0 dgilland   (501) staff       (20)    44029 2023-05-04 14:18:48.000000 pydash-7.0.3/src/pydash.egg-info/PKG-INFO
+-rw-r--r--   0 dgilland   (501) staff       (20)    16310 2023-05-04 14:18:50.000000 pydash-7.0.3/src/pydash.egg-info/SOURCES.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)        1 2023-05-04 14:18:48.000000 pydash-7.0.3/src/pydash.egg-info/dependency_links.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)      293 2023-05-04 14:18:48.000000 pydash-7.0.3/src/pydash.egg-info/requires.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)        7 2023-05-04 14:18:48.000000 pydash-7.0.3/src/pydash.egg-info/top_level.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)     6510 2023-04-06 20:16:10.000000 pydash-7.0.3/tasks.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.325235 pydash-7.0.3/tests/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-23 03:21:55.000000 pydash-7.0.3/tests/__init__.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.279251 pydash-7.0.3/tests/build/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.325386 pydash-7.0.3/tests/build/testresults/
+-rw-r--r--   0 dgilland   (501) staff       (20)      925 2023-04-06 01:12:00.000000 pydash-7.0.3/tests/build/testresults/junit.xml
+-rw-r--r--   0 dgilland   (501) staff       (20)      143 2022-09-23 13:25:56.000000 pydash-7.0.3/tests/conftest.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1870 2022-09-23 13:11:57.000000 pydash-7.0.3/tests/helpers.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-05-04 14:18:50.327555 pydash-7.0.3/tests/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.3/tests/pytest_mypy_testing/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    16882 2023-05-04 14:12:08.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_arrays.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1234 2023-04-12 02:10:33.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8643 2023-04-12 02:10:41.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     9870 2023-04-12 02:15:39.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     5582 2023-04-12 02:10:58.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    13212 2023-04-12 02:11:04.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    10786 2023-04-12 02:15:39.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    13294 2023-04-12 02:15:39.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8532 2023-04-12 02:15:39.000000 pydash-7.0.3/tests/pytest_mypy_testing/test_utilities.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      178 2021-06-27 18:15:05.000000 pydash-7.0.3/tests/test_annotations.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    24160 2021-09-28 21:40:18.000000 pydash-7.0.3/tests/test_arrays.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     4229 2023-03-18 22:34:56.000000 pydash-7.0.3/tests/test_chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    29669 2022-09-23 13:19:05.000000 pydash-7.0.3/tests/test_collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     9935 2022-09-23 13:25:56.000000 pydash-7.0.3/tests/test_functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     7640 2021-06-27 18:15:05.000000 pydash-7.0.3/tests/test_numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    28249 2023-03-18 22:34:56.000000 pydash-7.0.3/tests/test_objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    12617 2022-09-23 13:19:37.000000 pydash-7.0.3/tests/test_predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    33926 2023-04-06 01:12:00.000000 pydash-7.0.3/tests/test_strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    18221 2023-03-18 22:34:56.000000 pydash-7.0.3/tests/test_utilities.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      296 2023-01-28 17:36:13.000000 pydash-7.0.3/tox.ini
```

### Comparing `pydash-7.0.2/AUTHORS.rst` & `pydash-7.0.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/CHANGELOG.rst` & `pydash-7.0.3/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.3 (2023-05-04)
+-------------------
+
+- Fix typing for ``difference_by``, ``intersection_by``, ``union_by``, ``uniq_by``, and ``xor_by`` by allowing ``iteratee`` argument to be `Any`.  Thanks DeviousStoat_!
+
+
 v7.0.2 (2023-04-27)
 -------------------
 
 - Fix issue where using ``pyright`` as a type checker with ``reportPrivateUsage=true`` would report errors that objects are not exported from ``pydash``. Thanks DeviousStoat_!
 
 
 v7.0.1 (2023-04-13)
```

### Comparing `pydash-7.0.2/CONTRIBUTING.rst` & `pydash-7.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/LICENSE.rst` & `pydash-7.0.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/PKG-INFO` & `pydash-7.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash
-Version: 7.0.2
+Version: 7.0.3
 Summary: The kitchen sink of Python utility libraries for doing "stuff" in a functional way. Based on the Lo-Dash Javascript library.
 Home-page: https://github.com/dgilland/pydash
 Author: Derrick Gilland
 Author-email: dgilland@gmail.com
 License: MIT License
 Keywords: pydash utility functional lodash underscore
 Classifier: Development Status :: 5 - Production/Stable
@@ -61,14 +61,20 @@
     :target: https://pypi.python.org/pypi/pydash/
 
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.3 (2023-05-04)
+-------------------
+
+- Fix typing for ``difference_by``, ``intersection_by``, ``union_by``, ``uniq_by``, and ``xor_by`` by allowing ``iteratee`` argument to be `Any`.  Thanks DeviousStoat_!
+
+
 v7.0.2 (2023-04-27)
 -------------------
 
 - Fix issue where using ``pyright`` as a type checker with ``reportPrivateUsage=true`` would report errors that objects are not exported from ``pydash``. Thanks DeviousStoat_!
 
 
 v7.0.1 (2023-04-13)
```

### Comparing `pydash-7.0.2/README.rst` & `pydash-7.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/docs/Makefile` & `pydash-7.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/docs/api.rst` & `pydash-7.0.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/docs/callbacks.rst` & `pydash-7.0.3/docs/callbacks.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/docs/chaining.rst` & `pydash-7.0.3/docs/chaining.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/docs/conf.py` & `pydash-7.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/docs/deeppath.rst` & `pydash-7.0.3/docs/deeppath.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/docs/differences.rst` & `pydash-7.0.3/docs/differences.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/docs/index.rst` & `pydash-7.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/docs/quickstart.rst` & `pydash-7.0.3/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/docs/templating.rst` & `pydash-7.0.3/docs/templating.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/docs/upgrading.rst` & `pydash-7.0.3/docs/upgrading.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/pylintrc` & `pydash-7.0.3/pylintrc`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/setup.cfg` & `pydash-7.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/src/pydash/__init__.py` & `pydash-7.0.3/src/pydash/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Python port of Lo-Dash."""
 
-__version__ = "7.0.2"
+__version__ = "7.0.3"
 
 from .arrays import (
     chunk,
     compact,
     concat,
     difference,
     difference_by,
```

### Comparing `pydash-7.0.2/src/pydash/arrays.py` & `pydash-7.0.3/src/pydash/arrays.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,22 +189,22 @@
     return difference_with(array, *others)
 
 
 @t.overload
 def difference_by(
     array: t.Iterable[T],
     *others: t.Iterable[T],
-    iteratee: t.Union[IterateeObjT, t.Callable[[T], T], None],
+    iteratee: t.Union[IterateeObjT, t.Callable[[T], t.Any], None],
 ) -> t.List[T]:
     ...
 
 
 @t.overload
 def difference_by(
-    array: t.Iterable[T], *others: t.Union[IterateeObjT, t.Iterable[T], t.Callable[[T], T]]
+    array: t.Iterable[T], *others: t.Union[IterateeObjT, t.Iterable[T], t.Callable[[T], t.Any]]
 ) -> t.List[T]:
     ...
 
 
 def difference_by(array, *others, **kwargs):
     """
     This method is like :func:`difference` except that it accepts an iteratee which is invoked for
@@ -898,22 +898,22 @@
     return intersection_with(array, *others)
 
 
 @t.overload
 def intersection_by(
     array: t.Sequence[T],
     *others: t.Iterable[t.Any],
-    iteratee: t.Union[t.Callable[[T], T], IterateeObjT],
+    iteratee: t.Union[t.Callable[[T], t.Any], IterateeObjT],
 ) -> t.List[T]:
     ...
 
 
 @t.overload
 def intersection_by(
-    array: t.Sequence[T], *others: t.Union[t.Iterable[t.Any], t.Callable[[T], T], IterateeObjT]
+    array: t.Sequence[T], *others: t.Union[t.Iterable[t.Any], t.Callable[[T], t.Any], IterateeObjT]
 ) -> t.List[T]:
     ...
 
 
 def intersection_by(array, *others, **kwargs):
     """
     This method is like :func:`intersection` except that it accepts an iteratee which is invoked for
@@ -2175,15 +2175,15 @@
     array: t.Sequence[T], *others: t.Iterable[T], iteratee: t.Callable[[T], t.Any]
 ) -> t.List[T]:
     ...
 
 
 @t.overload
 def union_by(
-    array: t.Sequence[T], *others: t.Union[t.Iterable[T], t.Callable[[T], T]]
+    array: t.Sequence[T], *others: t.Union[t.Iterable[T], t.Callable[[T], t.Any]]
 ) -> t.List[T]:
     ...
 
 
 def union_by(array, *others, **kwargs):
     """
     This method is similar to :func:`union` except that it accepts iteratee which is invoked for
@@ -2290,15 +2290,17 @@
 
         - Moved `iteratee` argument to :func:`uniq_by`.
         - Removed alias ``unique``.
     """
     return uniq_by(array)
 
 
-def uniq_by(array: t.Iterable[T], iteratee: t.Union[t.Callable[[T], T], None] = None) -> t.List[T]:
+def uniq_by(
+    array: t.Iterable[T], iteratee: t.Union[t.Callable[[T], t.Any], None] = None
+) -> t.List[T]:
     """
     This method is like :func:`uniq` except that it accepts iteratee which is invoked for each
     element in array to generate the criterion by which uniqueness is computed. The order of result
     values is determined by the order they occur in the array. The iteratee is invoked with one
     argument: ``(value)``.
 
     Args:
@@ -2492,21 +2494,25 @@
     .. versionadded:: 1.0.0
     """
     return xor_by(array, *lists)
 
 
 @t.overload
 def xor_by(
-    array: t.Iterable[T], *lists: t.Iterable[T], iteratee: t.Union[t.Callable[[T], T], IterateeObjT]
+    array: t.Iterable[T],
+    *lists: t.Iterable[T],
+    iteratee: t.Union[t.Callable[[T], t.Any], IterateeObjT],
 ) -> t.List[T]:
     ...
 
 
 @t.overload
-def xor_by(array: t.Iterable[T], *lists: t.Union[t.Iterable[T], t.Callable[[T], T]]) -> t.List[T]:
+def xor_by(
+    array: t.Iterable[T], *lists: t.Union[t.Iterable[T], t.Callable[[T], t.Any]]
+) -> t.List[T]:
     ...
 
 
 def xor_by(array, *lists, **kwargs):
     """
     This method is like :func:`xor` except that it accepts iteratee which is invoked for each
     element of each arras to generate the criterion by which they're compared. The order of result
```

### Comparing `pydash-7.0.2/src/pydash/chaining/all_funcs.py` & `pydash-7.0.3/src/pydash/chaining/all_funcs.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/src/pydash/chaining/all_funcs.pyi` & `pydash-7.0.3/src/pydash/chaining/all_funcs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -68,20 +68,20 @@
         return self._wrap(pyd.compact)()
     def difference(self: "Chain[t.Iterable[T]]", *others: t.Iterable[T]) -> "Chain[t.List[T]]":
         return self._wrap(pyd.difference)(*others)
     @t.overload
     def difference_by(
         self: "Chain[t.Iterable[T]]",
         *others: t.Iterable[T],
-        iteratee: t.Union[IterateeObjT, t.Callable[[T], T], None]
+        iteratee: t.Union[IterateeObjT, t.Callable[[T], t.Any], None]
     ) -> "Chain[t.List[T]]": ...
     @t.overload
     def difference_by(
         self: "Chain[t.Iterable[T]]",
-        *others: t.Union[IterateeObjT, t.Iterable[T], t.Callable[[T], T]]
+        *others: t.Union[IterateeObjT, t.Iterable[T], t.Callable[[T], t.Any]]
     ) -> "Chain[t.List[T]]": ...
     def difference_by(self, *others, **kwargs):
         return self._wrap(pyd.difference_by)(*others, **kwargs)
     @t.overload
     def difference_with(
         self: "Chain[t.Iterable[T]]",
         *others: t.Iterable[T2],
@@ -212,20 +212,20 @@
         self: "Chain[t.Sequence[T]]", *others: t.Iterable[t.Any]
     ) -> "Chain[t.List[T]]":
         return self._wrap(pyd.intersection)(*others)
     @t.overload
     def intersection_by(
         self: "Chain[t.Sequence[T]]",
         *others: t.Iterable[t.Any],
-        iteratee: t.Union[t.Callable[[T], T], IterateeObjT]
+        iteratee: t.Union[t.Callable[[T], t.Any], IterateeObjT]
     ) -> "Chain[t.List[T]]": ...
     @t.overload
     def intersection_by(
         self: "Chain[t.Sequence[T]]",
-        *others: t.Union[t.Iterable[t.Any], t.Callable[[T], T], IterateeObjT]
+        *others: t.Union[t.Iterable[t.Any], t.Callable[[T], t.Any], IterateeObjT]
     ) -> "Chain[t.List[T]]": ...
     def intersection_by(self, *others, **kwargs):
         return self._wrap(pyd.intersection_by)(*others, **kwargs)
     @t.overload
     def intersection_with(
         self: "Chain[t.Sequence[T]]",
         *others: t.Iterable[T2],
@@ -453,15 +453,15 @@
         return self._wrap(pyd.union)(*others)
     @t.overload
     def union_by(
         self: "Chain[t.Sequence[T]]", *others: t.Iterable[T], iteratee: t.Callable[[T], t.Any]
     ) -> "Chain[t.List[T]]": ...
     @t.overload
     def union_by(
-        self: "Chain[t.Sequence[T]]", *others: t.Union[t.Iterable[T], t.Callable[[T], T]]
+        self: "Chain[t.Sequence[T]]", *others: t.Union[t.Iterable[T], t.Callable[[T], t.Any]]
     ) -> "Chain[t.List[T]]": ...
     def union_by(self, *others, **kwargs):
         return self._wrap(pyd.union_by)(*others, **kwargs)
     @t.overload
     def union_with(
         self: "Chain[t.Sequence[T]]",
         *others: t.Iterable[T2],
@@ -472,15 +472,15 @@
         self: "Chain[t.Sequence[T]]", *others: t.Union[t.Iterable[T2], t.Callable[[T, T2], t.Any]]
     ) -> "Chain[t.List[T]]": ...
     def union_with(self, *others, **kwargs):
         return self._wrap(pyd.union_with)(*others, **kwargs)
     def uniq(self: "Chain[t.Iterable[T]]") -> "Chain[t.List[T]]":
         return self._wrap(pyd.uniq)()
     def uniq_by(
-        self: "Chain[t.Iterable[T]]", iteratee: t.Union[t.Callable[[T], T], None] = None
+        self: "Chain[t.Iterable[T]]", iteratee: t.Union[t.Callable[[T], t.Any], None] = None
     ) -> "Chain[t.List[T]]":
         return self._wrap(pyd.uniq_by)(iteratee)
     def uniq_with(
         self: "Chain[t.Sequence[T]]", comparator: t.Union[t.Callable[[T, T], t.Any], None] = None
     ) -> "Chain[t.List[T]]":
         return self._wrap(pyd.uniq_with)(comparator)
     def unshift(self: "Chain[t.List[T]]", *items: T2) -> "Chain[t.List[t.Union[T, T2]]]":
@@ -507,19 +507,19 @@
         return self._wrap(pyd.without)(*values)
     def xor(self: "Chain[t.Iterable[T]]", *lists: t.Iterable[T]) -> "Chain[t.List[T]]":
         return self._wrap(pyd.xor)(*lists)
     @t.overload
     def xor_by(
         self: "Chain[t.Iterable[T]]",
         *lists: t.Iterable[T],
-        iteratee: t.Union[t.Callable[[T], T], IterateeObjT]
+        iteratee: t.Union[t.Callable[[T], t.Any], IterateeObjT]
     ) -> "Chain[t.List[T]]": ...
     @t.overload
     def xor_by(
-        self: "Chain[t.Iterable[T]]", *lists: t.Union[t.Iterable[T], t.Callable[[T], T]]
+        self: "Chain[t.Iterable[T]]", *lists: t.Union[t.Iterable[T], t.Callable[[T], t.Any]]
     ) -> "Chain[t.List[T]]": ...
     def xor_by(self, *lists, **kwargs):
         return self._wrap(pyd.xor_by)(*lists, **kwargs)
     @t.overload
     def xor_with(
         self: "Chain[t.Sequence[T]]", *lists: t.Iterable[T2], comparator: t.Callable[[T, T2], t.Any]
     ) -> "Chain[t.List[T]]": ...
```

### Comparing `pydash-7.0.2/src/pydash/chaining/chaining.py` & `pydash-7.0.3/src/pydash/chaining/chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/src/pydash/collections.py` & `pydash-7.0.3/src/pydash/collections.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/src/pydash/functions.py` & `pydash-7.0.3/src/pydash/functions.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/src/pydash/helpers.py` & `pydash-7.0.3/src/pydash/helpers.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/src/pydash/numerical.py` & `pydash-7.0.3/src/pydash/numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/src/pydash/objects.py` & `pydash-7.0.3/src/pydash/objects.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/src/pydash/predicates.py` & `pydash-7.0.3/src/pydash/predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/src/pydash/strings.py` & `pydash-7.0.3/src/pydash/strings.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/src/pydash/types.py` & `pydash-7.0.3/src/pydash/types.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/src/pydash/utilities.py` & `pydash-7.0.3/src/pydash/utilities.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/src/pydash.egg-info/PKG-INFO` & `pydash-7.0.3/src/pydash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash
-Version: 7.0.2
+Version: 7.0.3
 Summary: The kitchen sink of Python utility libraries for doing "stuff" in a functional way. Based on the Lo-Dash Javascript library.
 Home-page: https://github.com/dgilland/pydash
 Author: Derrick Gilland
 Author-email: dgilland@gmail.com
 License: MIT License
 Keywords: pydash utility functional lodash underscore
 Classifier: Development Status :: 5 - Production/Stable
@@ -61,14 +61,20 @@
     :target: https://pypi.python.org/pypi/pydash/
 
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.3 (2023-05-04)
+-------------------
+
+- Fix typing for ``difference_by``, ``intersection_by``, ``union_by``, ``uniq_by``, and ``xor_by`` by allowing ``iteratee`` argument to be `Any`.  Thanks DeviousStoat_!
+
+
 v7.0.2 (2023-04-27)
 -------------------
 
 - Fix issue where using ``pyright`` as a type checker with ``reportPrivateUsage=true`` would report errors that objects are not exported from ``pydash``. Thanks DeviousStoat_!
 
 
 v7.0.1 (2023-04-13)
```

### Comparing `pydash-7.0.2/src/pydash.egg-info/SOURCES.txt` & `pydash-7.0.3/src/pydash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tasks.py` & `pydash-7.0.3/tasks.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/build/testresults/junit.xml` & `pydash-7.0.3/tests/build/testresults/junit.xml`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/helpers.py` & `pydash-7.0.3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/pytest_mypy_testing/test_arrays.py` & `pydash-7.0.3/tests/pytest_mypy_testing/test_arrays.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     reveal_type(_.difference([1, 2, 3], [1], [2]))  # R: builtins.list[builtins.int]
 
 
 @pytest.mark.mypy_testing
 def test_mypy_difference_by() -> None:
     reveal_type(_.difference_by([1.2, 1.5, 1.7, 2.8], [0.9, 3.2], round))  # R: builtins.list[builtins.float]
 
+    reveal_type(_.difference_by([{"hello": 1}], [{"hello": 2}], lambda d: d["hello"]))  # R: builtins.list[builtins.dict[builtins.str, builtins.int]]
+
 
 @pytest.mark.mypy_testing
 def test_mypy_difference_with() -> None:
     array = ['apple', 'banana', 'pear']
     others = (['avocado', 'pumpkin'], ['peach'])
     def comparator(a: str, b: str) -> bool:
         return a[0] == b[0]
@@ -145,14 +147,16 @@
     reveal_type(_.intersection([1, 2, 3]))  # R: builtins.list[builtins.int]
 
 
 @pytest.mark.mypy_testing
 def test_mypy_intersection_by() -> None:
     reveal_type(_.intersection_by([1.2, 1.5, 1.7, 2.8], [0.9, 3.2], round))  # R: builtins.list[builtins.float]
 
+    reveal_type(_.intersection_by([{"hello": 1}], [{"hello": 2}], lambda d: d["hello"]))  # R: builtins.list[builtins.dict[builtins.str, builtins.int]]
+
 
 @pytest.mark.mypy_testing
 def test_mypy_intersection_with() -> None:
     array = ['apple', 'banana', 'pear']
     others = (['avocado', 'pumpkin'], ['peach'])
     def comparator(a: str, b:str) -> bool:
         return a[0] == b[0]
@@ -363,14 +367,16 @@
     reveal_type(_.union([1, 2, 3], ["hello"]))  # R: builtins.list[Union[builtins.int, builtins.str]]
 
 
 @pytest.mark.mypy_testing
 def test_mypy_union_by() -> None:
     reveal_type(_.union_by([1, 2, 3], [2, 3, 4], iteratee=lambda x: x % 2))  # R: builtins.list[builtins.int]
 
+    reveal_type(_.union_by([{"hello": 1}], [{"hello": 2}], lambda d: d["hello"]))  # R: builtins.list[builtins.dict[builtins.str, builtins.int]]
+
 
 @pytest.mark.mypy_testing
 def test_mypy_union_with() -> None:
     comparator = lambda a, b: (a % 2) == (b % 2)
     reveal_type(_.union_with([1, 2, 3], [2, 3, 4], comparator=comparator))  # R: builtins.list[builtins.int]
     reveal_type(_.union_with([1, 2, 3], [2, 3, 4]))  # R: builtins.list[builtins.int]
 
@@ -379,14 +385,15 @@
 def test_mypy_uniq() -> None:
     reveal_type(_.uniq([1, 2, 3, 1, 2, 3]))  # R: builtins.list[builtins.int]
 
 
 @pytest.mark.mypy_testing
 def test_mypy_uniq_by() -> None:
     reveal_type(_.uniq_by([1, 2, 3, 1, 2, 3], lambda val: val % 2))  # R: builtins.list[builtins.int]
+    reveal_type(_.uniq_by([{"hello": 1}, {"hello": 1}], lambda val: val["hello"]))  # R: builtins.list[builtins.dict[builtins.str, builtins.int]]
 
 
 @pytest.mark.mypy_testing
 def test_mypy_uniq_with() -> None:
     reveal_type(_.uniq_with([1, 2, 3, 4, 5], lambda a, b: (a % 2) == (b % 2)))  # R: builtins.list[builtins.int]
 
 
@@ -422,14 +429,16 @@
 
 
 @pytest.mark.mypy_testing
 def test_mypy_xor_by() -> None:
     reveal_type(_.xor_by([2.1, 1.2], [2.3, 3.4], round))  # R: builtins.list[builtins.float]
     reveal_type(_.xor_by([{'x': 1}], [{'x': 2}, {'x': 1}], iteratee='x'))  # R: builtins.list[builtins.dict[builtins.str, builtins.int]]
 
+    reveal_type(_.xor_by([{"hello": 1}], [{"hello": 2}], lambda d: d["hello"]))  # R: builtins.list[builtins.dict[builtins.str, builtins.int]]
+
 
 @pytest.mark.mypy_testing
 def test_mypy_xor_with() -> None:
     objects = [{'x': 1, 'y': 2}, {'x': 2, 'y': 1}]
     others = [{'x': 1, 'y': 1}, {'x': 1, 'y': 2}]
     reveal_type(_.xor_with(objects, others, lambda a, b: a == b))  # R: builtins.list[builtins.dict[builtins.str, builtins.int]]
```

### Comparing `pydash-7.0.2/tests/pytest_mypy_testing/test_chaining.py` & `pydash-7.0.3/tests/pytest_mypy_testing/test_chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/pytest_mypy_testing/test_collections.py` & `pydash-7.0.3/tests/pytest_mypy_testing/test_collections.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/pytest_mypy_testing/test_functions.py` & `pydash-7.0.3/tests/pytest_mypy_testing/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/pytest_mypy_testing/test_numerical.py` & `pydash-7.0.3/tests/pytest_mypy_testing/test_numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/pytest_mypy_testing/test_objects.py` & `pydash-7.0.3/tests/pytest_mypy_testing/test_objects.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/pytest_mypy_testing/test_predicates.py` & `pydash-7.0.3/tests/pytest_mypy_testing/test_predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/pytest_mypy_testing/test_strings.py` & `pydash-7.0.3/tests/pytest_mypy_testing/test_strings.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/pytest_mypy_testing/test_utilities.py` & `pydash-7.0.3/tests/pytest_mypy_testing/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/test_arrays.py` & `pydash-7.0.3/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/test_chaining.py` & `pydash-7.0.3/tests/test_chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/test_collections.py` & `pydash-7.0.3/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/test_functions.py` & `pydash-7.0.3/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/test_numerical.py` & `pydash-7.0.3/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/test_objects.py` & `pydash-7.0.3/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/test_predicates.py` & `pydash-7.0.3/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/test_strings.py` & `pydash-7.0.3/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.2/tests/test_utilities.py` & `pydash-7.0.3/tests/test_utilities.py`

 * *Files identical despite different names*

