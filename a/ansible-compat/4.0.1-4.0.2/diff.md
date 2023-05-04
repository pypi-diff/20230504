# Comparing `tmp/ansible-compat-4.0.1.tar.gz` & `tmp/ansible-compat-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-compat-4.0.1.tar", last modified: Mon May  1 16:29:20 2023, max compression
+gzip compressed data, was "ansible-compat-4.0.2.tar", last modified: Thu May  4 15:13:15 2023, max compression
```

## Comparing `ansible-compat-4.0.1.tar` & `ansible-compat-4.0.2.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.477434 ansible-compat-4.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.461434 ansible-compat-4.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.461434 ansible-compat-4.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.461434 ansible-compat-4.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-01 16:29:20.477434 ansible-compat-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.461434 ansible-compat-4.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.461434 ansible-compat-4.0.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.449434 ansible-compat-4.0.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.461434 ansible-compat-4.0.1/examples/reqs_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/examples/reqs_v1/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.465434 ansible-compat-4.0.1/examples/reqs_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/examples/reqs_v2/community-molecule-0.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/examples/reqs_v2/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:29:20.477434 ansible-compat-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.449434 ansible-compat-4.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.465434 ansible-compat-4.0.1/src/ansible_compat/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/src/ansible_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15946 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/src/ansible_compat/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/src/ansible_compat/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/src/ansible_compat/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/src/ansible_compat/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/src/ansible_compat/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/src/ansible_compat/prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/src/ansible_compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28537 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/src/ansible_compat/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/src/ansible_compat/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/src/ansible_compat/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.469434 ansible-compat-4.0.1/src/ansible_compat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-01 16:29:20.000000 ansible-compat-4.0.1/src/ansible_compat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-01 16:29:20.000000 ansible-compat-4.0.1/src/ansible_compat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:29:20.000000 ansible-compat-4.0.1/src/ansible_compat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-01 16:29:20.000000 ansible-compat-4.0.1/src/ansible_compat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 16:29:20.000000 ansible-compat-4.0.1/src/ansible_compat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.469434 ansible-compat-4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.473434 ansible-compat-4.0.1/test/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/assets/requirements-invalid-collection.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/assets/requirements-invalid-role.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/assets/validate0_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/assets/validate0_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/assets/validate0_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.449434 ansible-compat-4.0.1/test/collections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.473434 ansible-compat-4.0.1/test/collections/acme.broken/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/collections/acme.broken/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.473434 ansible-compat-4.0.1/test/collections/acme.goodies/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/collections/acme.goodies/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.453434 ansible-compat-4.0.1/test/collections/acme.goodies/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.473434 ansible-compat-4.0.1/test/collections/acme.goodies/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/collections/acme.goodies/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/collections/acme.goodies/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.453434 ansible-compat-4.0.1/test/collections/acme.goodies/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.453434 ansible-compat-4.0.1/test/collections/acme.goodies/roles/baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.453434 ansible-compat-4.0.1/test/collections/acme.goodies/roles/baz/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.473434 ansible-compat-4.0.1/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.473434 ansible-compat-4.0.1/test/collections/acme.goodies/roles/baz/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/collections/acme.goodies/roles/baz/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.453434 ansible-compat-4.0.1/test/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.473434 ansible-compat-4.0.1/test/roles/acme.missing_deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.473434 ansible-compat-4.0.1/test/roles/acme.missing_deps/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/roles/acme.missing_deps/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/roles/acme.missing_deps/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.453434 ansible-compat-4.0.1/test/roles/acme.sample2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.473434 ansible-compat-4.0.1/test/roles/acme.sample2/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/roles/acme.sample2/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.453434 ansible-compat-4.0.1/test/roles/ansible-role-sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.477434 ansible-compat-4.0.1/test/roles/ansible-role-sample/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/roles/ansible-role-sample/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.453434 ansible-compat-4.0.1/test/roles/sample3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.477434 ansible-compat-4.0.1/test/roles/sample3/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/roles/sample3/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.453434 ansible-compat-4.0.1/test/roles/sample4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:29:20.477434 ansible-compat-4.0.1/test/roles/sample4/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/roles/sample4/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/test_configuration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/test_prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    24524 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/test_runtime_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/test/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-01 16:29:01.000000 ansible-compat-4.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.606701 ansible-compat-4.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.610701 ansible-compat-4.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.610701 ansible-compat-4.0.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.610701 ansible-compat-4.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.610701 ansible-compat-4.0.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.598701 ansible-compat-4.0.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.610701 ansible-compat-4.0.2/examples/reqs_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/examples/reqs_v1/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.610701 ansible-compat-4.0.2/examples/reqs_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/examples/reqs_v2/community-molecule-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/examples/reqs_v2/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.598701 ansible-compat-4.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.614701 ansible-compat-4.0.2/src/ansible_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28537 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.614701 ansible-compat-4.0.2/src/ansible_compat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-04 15:13:15.000000 ansible-compat-4.0.2/src/ansible_compat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-04 15:13:15.000000 ansible-compat-4.0.2/src/ansible_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:13:15.000000 ansible-compat-4.0.2/src/ansible_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 15:13:15.000000 ansible-compat-4.0.2/src/ansible_compat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 15:13:15.000000 ansible-compat-4.0.2/src/ansible_compat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.618701 ansible-compat-4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.618701 ansible-compat-4.0.2/test/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/assets/requirements-invalid-collection.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/assets/requirements-invalid-role.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/assets/validate0_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/assets/validate0_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/assets/validate0_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/collections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.618701 ansible-compat-4.0.2/test/collections/acme.broken/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/collections/acme.broken/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.618701 ansible-compat-4.0.2/test/collections/acme.goodies/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/collections/acme.goodies/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/collections/acme.goodies/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.618701 ansible-compat-4.0.2/test/collections/acme.goodies/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/collections/acme.goodies/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/collections/acme.goodies/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/collections/acme.goodies/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/collections/acme.goodies/roles/baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/collections/acme.goodies/roles/baz/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/collections/acme.goodies/roles/baz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/collections/acme.goodies/roles/baz/tasks/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/roles/acme.missing_deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/roles/acme.missing_deps/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/roles/acme.missing_deps/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/roles/acme.missing_deps/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/roles/acme.sample2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/roles/acme.sample2/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/roles/acme.sample2/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/roles/ansible-role-sample/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/roles/ansible-role-sample/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/roles/ansible-role-sample/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/roles/sample3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/roles/sample3/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/roles/sample3/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/roles/sample4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/roles/sample4/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/roles/sample4/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_configuration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24524 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_runtime_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/tox.ini
```

### Comparing `ansible-compat-4.0.1/.github/dependabot.yml` & `ansible-compat-4.0.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/.github/workflows/release.yml` & `ansible-compat-4.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/.github/workflows/tox.yml` & `ansible-compat-4.0.2/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/.gitignore` & `ansible-compat-4.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/.pre-commit-config.yaml` & `ansible-compat-4.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/.readthedocs.yml` & `ansible-compat-4.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/.vscode/settings.json` & `ansible-compat-4.0.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/LICENSE` & `ansible-compat-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/PKG-INFO` & `ansible-compat-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.0.1
+Version: 4.0.2
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.0.1/README.md` & `ansible-compat-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/docs/images/favicon.ico` & `ansible-compat-4.0.2/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/docs/images/logo.png` & `ansible-compat-4.0.2/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/docs/images/logo.svg` & `ansible-compat-4.0.2/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/examples/reqs_v2/community-molecule-0.1.0.tar.gz` & `ansible-compat-4.0.2/examples/reqs_v2/community-molecule-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/mkdocs.yml` & `ansible-compat-4.0.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/pyproject.toml` & `ansible-compat-4.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/requirements.txt` & `ansible-compat-4.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/src/ansible_compat/config.py` & `ansible-compat-4.0.2/src/ansible_compat/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 from ansible_compat.errors import InvalidPrerequisiteError, MissingAnsibleError
 from ansible_compat.ports import cache
 
 
 # do not use lru_cache here, as environment can change between calls
 def ansible_collections_path() -> str:
     """Return collection path variable for current version of Ansible."""
+    for env_var in [
+        "ANSIBLE_COLLECTIONS_PATH",
+        "ANSIBLE_COLLECTIONS_PATHS",
+    ]:
+        if env_var in os.environ:
+            return env_var
     return "ANSIBLE_COLLECTIONS_PATH"
 
 
 def parse_ansible_version(stdout: str) -> Version:
     """Parse output of 'ansible --version'."""
     # Ansible can produce extra output before displaying version in debug mode.
```

### Comparing `ansible-compat-4.0.1/src/ansible_compat/constants.py` & `ansible-compat-4.0.2/src/ansible_compat/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/src/ansible_compat/errors.py` & `ansible-compat-4.0.2/src/ansible_compat/errors.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/src/ansible_compat/loaders.py` & `ansible-compat-4.0.2/src/ansible_compat/loaders.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/src/ansible_compat/prerun.py` & `ansible-compat-4.0.2/src/ansible_compat/prerun.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/src/ansible_compat/runtime.py` & `ansible-compat-4.0.2/src/ansible_compat/runtime.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/src/ansible_compat/schema.py` & `ansible-compat-4.0.2/src/ansible_compat/schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/src/ansible_compat/types.py` & `ansible-compat-4.0.2/src/ansible_compat/types.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/src/ansible_compat.egg-info/PKG-INFO` & `ansible-compat-4.0.2/src/ansible_compat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.0.1
+Version: 4.0.2
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.0.1/src/ansible_compat.egg-info/SOURCES.txt` & `ansible-compat-4.0.2/src/ansible_compat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/test/assets/validate0_expected.json` & `ansible-compat-4.0.2/test/assets/validate0_expected.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/test/conftest.py` & `ansible-compat-4.0.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/test/test_config.py` & `ansible-compat-4.0.2/test/test_config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/test/test_runtime.py` & `ansible-compat-4.0.2/test/test_runtime.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/test/test_runtime_example.py` & `ansible-compat-4.0.2/test/test_runtime_example.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/test/test_schema.py` & `ansible-compat-4.0.2/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.1/tox.ini` & `ansible-compat-4.0.2/tox.ini`

 * *Files identical despite different names*

