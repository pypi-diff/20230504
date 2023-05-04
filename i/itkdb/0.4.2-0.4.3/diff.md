# Comparing `tmp/itkdb-0.4.2.tar.gz` & `tmp/itkdb-0.4.3.tar.gz`

## Comparing `itkdb-0.4.2.tar` & `itkdb-0.4.3.tar`

### file list

```diff
@@ -1,121 +1,122 @@
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 itkdb-0.4.2/.gitlab-ci.yml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 itkdb-0.4.2/.linkcheckerrc
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 itkdb-0.4.2/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 itkdb-0.4.2/add_attachment.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 itkdb-0.4.2/add_comment.py
--rwxr-xr-x   0        0        0    36494 2020-02-02 00:00:00.000000 itkdb-0.4.2/generatePlots.py
--rwxr-xr-x   0        0        0    27894 2020-02-02 00:00:00.000000 itkdb-0.4.2/getContentSummary.py
--rwxr-xr-x   0        0        0    20487 2020-02-02 00:00:00.000000 itkdb-0.4.2/getInventory.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 itkdb-0.4.2/mkdocs.yml
--rwxr-xr-x   0        0        0    27949 2020-02-02 00:00:00.000000 itkdb-0.4.2/registerComponent.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 itkdb-0.4.2/tbump.toml
--rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 itkdb-0.4.2/ci/pre-commit-update.sh
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 itkdb-0.4.2/docs/config.md
--rw-r--r--   0        0        0    18833 2020-02-02 00:00:00.000000 itkdb-0.4.2/docs/examples.md
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 itkdb-0.4.2/docs/history.md
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 itkdb-0.4.2/docs/index.md
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 itkdb-0.4.2/docs/install.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 itkdb-0.4.2/docs/macros.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 itkdb-0.4.2/docs/.overrides/main.html
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itkdb-0.4.2/docs/.snippets/abbrs.txt
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 itkdb-0.4.2/docs/.snippets/links.txt
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 itkdb-0.4.2/docs/assets/css/custom.css
--rw-r--r--   0        0        0    23475 2020-02-02 00:00:00.000000 itkdb-0.4.2/docs/assets/images/logo.svg
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 itkdb-0.4.2/docs/meta/authors.md
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 itkdb-0.4.2/docs/meta/faq.md
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 itkdb-0.4.2/docs/reference/gen_ref_nav.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 itkdb-0.4.2/docs/reference/cli/itkdb.md
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/_version.py
--rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/client.py
--rw-r--r--   0        0        0     8034 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/commandline.py
--rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/core.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/py.typed
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/responses.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/typing.py
--rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/utils.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/caching/__init__.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/caching/adapter.py
--rw-r--r--   0        0        0    11031 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/caching/controller.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/caching/utils.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/data/1x1.jpg
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/data/1x1.sh
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/data/CERN_chain.pem
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/data/README.md
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/data/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/data/tiny.root
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/models/__init__.py
--rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/models/file.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/models/institution.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/settings/__init__.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 itkdb-0.4.2/src/itkdb/settings/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/conftest.py
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/test_cli.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/test_client.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/test_image.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/test_response.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/test_scripts.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/test_session.py
--rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/test_user.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/test_utils.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/test_attachments.py
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/test_binaryData.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/test_cache.py
--rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/test_components.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/test_institution.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/test_projects.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/test_session.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/test_shipments.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/test_stats.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/test_summary.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/test_testproperties.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/test_tests.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/test_user.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/test_warning.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_attachments.test_add_attachment.json
--rw-r--r--   0        0        0    94089 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_attachments.test_list_all_attachments.json
--rw-r--r--   0        0        0     7917 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_binaryData.test_get_image.json
--rw-r--r--   0        0        0    11021 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_binaryData.test_get_plainText.json
--rw-r--r--   0        0        0   304955 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_binaryData.test_get_zipfile.json
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_binaryData.test_issue4.json
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_components.test_add_comment.json
--rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0    32318 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_components.test_get.json
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_components.test_get_component_bulk.json
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_components.test_get_component_info_code.json
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_components.test_get_component_info_serial.json
--rw-r--r--   0        0        0   112349 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json
--rw-r--r--   0        0        0   108642 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json
--rw-r--r--   0        0        0   245837 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_components.test_list_componentsv1.json
--rw-r--r--   0        0        0   245811 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_components.test_list_componentsv2.json
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_institution.test_get.json
--rw-r--r--   0        0        0   101372 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_institution.test_pagination.json
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_projects.test_list_projects.json
--rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_scripts.test_getInventory.trashUnassembled.json
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_session.test_fake_route.json
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_session.test_invalid_project.json
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_session.test_missing_required.json
--rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_session.test_no_bearer.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_session.test_unauthorized.json
--rw-r--r--   0        0        0    19435 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_stats.test_get.json
--rw-r--r--   0        0        0   509788 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_summary.test_get_summary.json
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_testproperties.test_delete_test_property.json
--rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_tests.test_list_test_types.json
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_user.test_user_anonymous_login.json
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_user.test_user_bad_login.json
--rw-r--r--   0        0        0    17319 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_user.test_user_good_login.json
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 itkdb-0.4.2/tests/integration/cassettes/test_warnings.test_get_component.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 itkdb-0.4.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 itkdb-0.4.2/COPYING
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 itkdb-0.4.2/LICENSE
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 itkdb-0.4.2/README.md
--rw-r--r--   0        0        0     7722 2020-02-02 00:00:00.000000 itkdb-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 itkdb-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 itkdb-0.4.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 itkdb-0.4.3/.linkcheckerrc
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 itkdb-0.4.3/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 itkdb-0.4.3/add_attachment.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 itkdb-0.4.3/add_comment.py
+-rwxr-xr-x   0        0        0    36494 2020-02-02 00:00:00.000000 itkdb-0.4.3/generatePlots.py
+-rwxr-xr-x   0        0        0    27894 2020-02-02 00:00:00.000000 itkdb-0.4.3/getContentSummary.py
+-rwxr-xr-x   0        0        0    20487 2020-02-02 00:00:00.000000 itkdb-0.4.3/getInventory.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 itkdb-0.4.3/mkdocs.yml
+-rwxr-xr-x   0        0        0    27949 2020-02-02 00:00:00.000000 itkdb-0.4.3/registerComponent.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 itkdb-0.4.3/tbump.toml
+-rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 itkdb-0.4.3/ci/pre-commit-update.sh
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 itkdb-0.4.3/docs/config.md
+-rw-r--r--   0        0        0    18833 2020-02-02 00:00:00.000000 itkdb-0.4.3/docs/examples.md
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 itkdb-0.4.3/docs/history.md
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 itkdb-0.4.3/docs/index.md
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 itkdb-0.4.3/docs/install.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 itkdb-0.4.3/docs/macros.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 itkdb-0.4.3/docs/.overrides/main.html
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itkdb-0.4.3/docs/.snippets/abbrs.txt
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 itkdb-0.4.3/docs/.snippets/links.txt
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 itkdb-0.4.3/docs/assets/css/custom.css
+-rw-r--r--   0        0        0    23475 2020-02-02 00:00:00.000000 itkdb-0.4.3/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 itkdb-0.4.3/docs/meta/authors.md
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 itkdb-0.4.3/docs/meta/faq.md
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 itkdb-0.4.3/docs/reference/gen_ref_nav.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 itkdb-0.4.3/docs/reference/cli/itkdb.md
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/_version.py
+-rw-r--r--   0        0        0    14195 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/client.py
+-rw-r--r--   0        0        0     8034 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/commandline.py
+-rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/core.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/py.typed
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/responses.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/typing.py
+-rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/utils.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/caching/__init__.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/caching/adapter.py
+-rw-r--r--   0        0        0    10896 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/caching/controller.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/caching/utils.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/data/1x1.jpg
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/data/1x1.sh
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/data/CERN_chain.pem
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/data/README.md
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/data/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/data/tiny.root
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/models/__init__.py
+-rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/models/file.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/models/institution.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/settings/__init__.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 itkdb-0.4.3/src/itkdb/settings/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/__init__.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/conftest.py
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/test_cli.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/test_client.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/test_image.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/test_response.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/test_scripts.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/test_session.py
+-rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/test_user.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/test_utils.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/test_attachments.py
+-rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/test_binaryData.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/test_cache.py
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/test_components.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/test_institution.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/test_projects.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/test_session.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/test_shipments.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/test_stats.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/test_summary.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/test_testproperties.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/test_tests.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/test_user.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/test_warning.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_attachments.test_add_attachment.json
+-rw-r--r--   0        0        0    94089 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_attachments.test_list_all_attachments.json
+-rw-r--r--   0        0        0     7917 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_binaryData.test_get_image.json
+-rw-r--r--   0        0        0    11021 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_binaryData.test_get_json.json
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_binaryData.test_get_plainText.json
+-rw-r--r--   0        0        0   304955 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_binaryData.test_get_zipfile.json
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_binaryData.test_issue4.json
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_components.test_add_comment.json
+-rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json
+-rw-r--r--   0        0        0    32318 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_components.test_get.json
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_components.test_get_component_bulk.json
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_components.test_get_component_info_code.json
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_components.test_get_component_info_serial.json
+-rw-r--r--   0        0        0   112349 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json
+-rw-r--r--   0        0        0   108642 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json
+-rw-r--r--   0        0        0   245837 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_components.test_list_componentsv1.json
+-rw-r--r--   0        0        0   245811 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_components.test_list_componentsv2.json
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_institution.test_get.json
+-rw-r--r--   0        0        0   101372 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_institution.test_pagination.json
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_projects.test_list_projects.json
+-rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_scripts.test_getInventory.trashUnassembled.json
+-rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_session.test_fake_route.json
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_session.test_invalid_project.json
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_session.test_missing_required.json
+-rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_session.test_no_bearer.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_session.test_unauthorized.json
+-rw-r--r--   0        0        0    19435 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_stats.test_get.json
+-rw-r--r--   0        0        0   509788 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_summary.test_get_summary.json
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_testproperties.test_delete_test_property.json
+-rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json
+-rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_tests.test_list_test_types.json
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_user.test_user_anonymous_login.json
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_user.test_user_bad_login.json
+-rw-r--r--   0        0        0    17319 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_user.test_user_good_login.json
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 itkdb-0.4.3/tests/integration/cassettes/test_warnings.test_get_component.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 itkdb-0.4.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 itkdb-0.4.3/COPYING
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 itkdb-0.4.3/LICENSE
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 itkdb-0.4.3/README.md
+-rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 itkdb-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 itkdb-0.4.3/PKG-INFO
```

### Comparing `itkdb-0.4.2/.gitlab-ci.yml` & `itkdb-0.4.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/.pre-commit-config.yaml` & `itkdb-0.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/generatePlots.py` & `itkdb-0.4.3/generatePlots.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/getContentSummary.py` & `itkdb-0.4.3/getContentSummary.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/getInventory.py` & `itkdb-0.4.3/getInventory.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/mkdocs.yml` & `itkdb-0.4.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/registerComponent.py` & `itkdb-0.4.3/registerComponent.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tbump.toml` & `itkdb-0.4.3/tbump.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2230 2e34 2e32 220a 0a23 2045  t = "0.4.2"..# E
+00000010: 7420 3d20 2230 2e34 2e33 220a 0a23 2045  t = "0.4.3"..# E
 00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
 00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
 00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
 00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
 00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
 00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
 00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
@@ -15,15 +15,15 @@
 000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
 000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
 00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
 00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
 00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
 00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
 00000140: 6d70 2076 6572 7369 6f6e 3a20 302e 342e  mp version: 0.4.
-00000150: 3220 e286 9220 7b6e 6577 5f76 6572 7369  2 ... {new_versi
+00000150: 3320 e286 9220 7b6e 6577 5f76 6572 7369  3 ... {new_versi
 00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
 00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
 00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
 00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
 000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
 000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
 000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
```

### Comparing `itkdb-0.4.2/ci/pre-commit-update.sh` & `itkdb-0.4.3/ci/pre-commit-update.sh`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/docs/config.md` & `itkdb-0.4.3/docs/config.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/docs/examples.md` & `itkdb-0.4.3/docs/examples.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/docs/history.md` & `itkdb-0.4.3/docs/history.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/docs/index.md` & `itkdb-0.4.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/docs/install.md` & `itkdb-0.4.3/docs/install.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/docs/assets/css/custom.css` & `itkdb-0.4.3/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/docs/assets/images/logo.svg` & `itkdb-0.4.3/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/docs/meta/faq.md` & `itkdb-0.4.3/docs/meta/faq.md`

 * *Files 2% similar despite different names*

```diff
@@ -125,13 +125,16 @@
 --no-use-pep517 --global-option="--with..."
 ```
 
 instead of using `--install-option` which is deprecated in favor of
 `--global-option`, and disabling the use of PEP517 to allow the use of
 `--global-option`.
 
+Also be sure that you have the curl headers installed (e.g. via `libcurl-devel`)
+on your machine.
+
 ## Potpourri
 
 **_Q_**: I'm still stuck and I don't see my question here.
 
 **_A_**: I'm still working on fleshing out the FAQs. Check back soon. In the
 meantime, file an [issue][].
```

### Comparing `itkdb-0.4.2/docs/reference/gen_ref_nav.py` & `itkdb-0.4.3/docs/reference/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/src/itkdb/client.py` & `itkdb-0.4.3/src/itkdb/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,15 +304,17 @@
 
     def _response_handler(self, response):
         # sometimes we don't get content-type, so make sure it's a string at least
         content_type = response.headers.get("content-type")
         if content_type is None:
             return response
 
-        if content_type.startswith("application/json"):
+        if content_type.startswith("application/json") and not response.url.endswith(
+            "uu-app-binarystore/getBinaryData"
+        ):
             if response.headers.get("content-length") == "0":
                 return {}
 
             try:
                 data = response.json()
                 self._handle_warnings(data)
             except ValueError as err:
@@ -356,17 +358,19 @@
             binary_file._mimetype = (  # pylint: disable=protected-access
                 binary_file.content_type
             )
             response.headers["content-type"] = binary_file.mimetype
 
         if binary_file.mimetype.startswith("image/"):
             binary_file.__class__ = models.ImageFile
-        elif binary_file.mimetype.startswith(
-            "text/"
-        ) or binary_file.mimetype.startswith("text"):
+        elif (
+            binary_file.mimetype.startswith("text/")
+            or binary_file.mimetype.startswith("text")
+            or binary_file.mimetype == "application/json"
+        ):
             binary_file.__class__ = models.TextFile
         elif binary_file.mimetype == "application/zip":
             binary_file = models.ZipFile(binary_file)
         else:
             log.warning(
                 "No model available for Content-Type: '%s'. Defaulting to BinaryFile.",
                 binary_file.mimetype,
```

### Comparing `itkdb-0.4.2/src/itkdb/commandline.py` & `itkdb-0.4.3/src/itkdb/commandline.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/src/itkdb/core.py` & `itkdb-0.4.3/src/itkdb/core.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/src/itkdb/exceptions.py` & `itkdb-0.4.3/src/itkdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/src/itkdb/responses.py` & `itkdb-0.4.3/src/itkdb/responses.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/src/itkdb/utils.py` & `itkdb-0.4.3/src/itkdb/utils.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/src/itkdb/caching/adapter.py` & `itkdb-0.4.3/src/itkdb/caching/adapter.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/src/itkdb/caching/controller.py` & `itkdb-0.4.3/src/itkdb/caching/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,17 +198,14 @@
         # Storing such a response leads to a deserialization warning
         # during cache lookup and is not allowed to ever be served,
         # so storing it can be avoided.
         if "*" in response_headers.get("vary", ""):
             logger.debug('Response header has "Vary: *"')
             return
 
-        # https://gitlab.cern.ch/scipp/strips/itkdataflow/-/jobs/29230451
-        response.strict = getattr(response, "strict", True)
-
         # If we've been given an etag, then keep the response
         if self.cache_etags and "etag" in response_headers:
             logger.debug("Caching due to etag")
             self.cache.set(
                 cache_url, self.serializer.dumps(request, response, body=body)
             )
```

### Comparing `itkdb-0.4.2/src/itkdb/caching/utils.py` & `itkdb-0.4.3/src/itkdb/caching/utils.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/src/itkdb/data/1x1.sh` & `itkdb-0.4.3/src/itkdb/data/1x1.sh`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/src/itkdb/data/CERN_chain.pem` & `itkdb-0.4.3/src/itkdb/data/CERN_chain.pem`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/src/itkdb/data/README.md` & `itkdb-0.4.3/src/itkdb/data/README.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/src/itkdb/models/file.py` & `itkdb-0.4.3/src/itkdb/models/file.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/src/itkdb/models/institution.py` & `itkdb-0.4.3/src/itkdb/models/institution.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/conftest.py` & `itkdb-0.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/test_cli.py` & `itkdb-0.4.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/test_client.py` & `itkdb-0.4.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/test_image.py` & `itkdb-0.4.3/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/test_response.py` & `itkdb-0.4.3/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/test_scripts.py` & `itkdb-0.4.3/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/test_session.py` & `itkdb-0.4.3/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/test_user.py` & `itkdb-0.4.3/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/test_utils.py` & `itkdb-0.4.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/test_attachments.py` & `itkdb-0.4.3/tests/integration/test_attachments.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/test_binaryData.py` & `itkdb-0.4.3/tests/integration/test_binaryData.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,14 +65,39 @@
         assert text.suggested_filename == "for_gui test3.txt"
         assert text.extension == "txt"
         temp = tmpdir.join("saved_text.txt")
         nbytes = text.save(filename=temp.strpath)
         assert nbytes == 23
 
 
+def test_get_json(auth_session):
+    with betamax.Betamax(auth_session).use_cassette("test_binaryData.test_get_json"):
+        response = auth_session.get(
+            "uu-app-binarystore/getBinaryData",
+            json={"code": "54fc652d3e2f745ea15bc612b4f2b16d"},
+        )
+        assert response
+        assert response.status_code == 200
+        assert response.headers.get("content-type") == "application/json"
+
+
+def test_get_json_model(auth_client, tmpdir):
+    with betamax.Betamax(auth_client).use_cassette("test_binaryData.test_get_json"):
+        text = auth_client.get(
+            "uu-app-binarystore/getBinaryData",
+            json={"code": "54fc652d3e2f745ea15bc612b4f2b16d"},
+        )
+        assert isinstance(text, itkdb.models.TextFile)
+        assert text.suggested_filename == "644ecb882d292775dfcf0ec3.json"
+        assert text.extension == "json"
+        temp = tmpdir.join("saved_json.json")
+        nbytes = text.save(filename=temp.strpath)
+        assert nbytes == 896
+
+
 def test_issue4(auth_session):
     with betamax.Betamax(auth_session).use_cassette("test_binaryData.test_issue4"):
         response = auth_session.get(
             "uu-app-binarystore/getBinaryData",
             json={
                 "code": "fe4f85dd3740c53956c22bb4324065b8",
                 "contentDisposition": "attachment",
```

### Comparing `itkdb-0.4.2/tests/integration/test_cache.py` & `itkdb-0.4.3/tests/integration/test_cache.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/test_components.py` & `itkdb-0.4.3/tests/integration/test_components.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/test_institution.py` & `itkdb-0.4.3/tests/integration/test_institution.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/test_session.py` & `itkdb-0.4.3/tests/integration/test_session.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/test_shipments.py` & `itkdb-0.4.3/tests/integration/test_shipments.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/test_summary.py` & `itkdb-0.4.3/tests/integration/test_summary.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/test_testproperties.py` & `itkdb-0.4.3/tests/integration/test_testproperties.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/test_tests.py` & `itkdb-0.4.3/tests/integration/test_tests.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/test_user.py` & `itkdb-0.4.3/tests/integration/test_user.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/test_warning.py` & `itkdb-0.4.3/tests/integration/test_warning.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_attachments.test_add_attachment.json` & `itkdb-0.4.3/tests/integration/cassettes/test_attachments.test_add_attachment.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_attachments.test_list_all_attachments.json` & `itkdb-0.4.3/tests/integration/cassettes/test_attachments.test_list_all_attachments.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_binaryData.test_get_image.json` & `itkdb-0.4.3/tests/integration/cassettes/test_binaryData.test_get_image.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json` & `itkdb-0.4.3/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_binaryData.test_get_plainText.json` & `itkdb-0.4.3/tests/integration/cassettes/test_binaryData.test_get_plainText.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_binaryData.test_get_zipfile.json` & `itkdb-0.4.3/tests/integration/cassettes/test_binaryData.test_get_zipfile.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_binaryData.test_issue4.json` & `itkdb-0.4.3/tests/integration/cassettes/test_binaryData.test_issue4.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_components.test_add_comment.json` & `itkdb-0.4.3/tests/integration/cassettes/test_components.test_add_comment.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json` & `itkdb-0.4.3/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_components.test_get.json` & `itkdb-0.4.3/tests/integration/cassettes/test_components.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_components.test_get_component_bulk.json` & `itkdb-0.4.3/tests/integration/cassettes/test_components.test_get_component_bulk.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_components.test_get_component_info_code.json` & `itkdb-0.4.3/tests/integration/cassettes/test_components.test_get_component_info_code.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_components.test_get_component_info_serial.json` & `itkdb-0.4.3/tests/integration/cassettes/test_components.test_get_component_info_serial.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json` & `itkdb-0.4.3/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json` & `itkdb-0.4.3/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_components.test_list_componentsv1.json` & `itkdb-0.4.3/tests/integration/cassettes/test_components.test_list_componentsv1.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_components.test_list_componentsv2.json` & `itkdb-0.4.3/tests/integration/cassettes/test_components.test_list_componentsv2.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_institution.test_get.json` & `itkdb-0.4.3/tests/integration/cassettes/test_institution.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_institution.test_pagination.json` & `itkdb-0.4.3/tests/integration/cassettes/test_institution.test_pagination.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_projects.test_list_projects.json` & `itkdb-0.4.3/tests/integration/cassettes/test_projects.test_list_projects.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json` & `itkdb-0.4.3/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json` & `itkdb-0.4.3/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json` & `itkdb-0.4.3/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_session.test_fake_route.json` & `itkdb-0.4.3/tests/integration/cassettes/test_session.test_fake_route.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_session.test_invalid_project.json` & `itkdb-0.4.3/tests/integration/cassettes/test_session.test_invalid_project.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_session.test_missing_required.json` & `itkdb-0.4.3/tests/integration/cassettes/test_session.test_missing_required.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_session.test_no_bearer.json` & `itkdb-0.4.3/tests/integration/cassettes/test_session.test_no_bearer.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json` & `itkdb-0.4.3/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_stats.test_get.json` & `itkdb-0.4.3/tests/integration/cassettes/test_stats.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_summary.test_get_summary.json` & `itkdb-0.4.3/tests/integration/cassettes/test_summary.test_get_summary.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_testproperties.test_delete_test_property.json` & `itkdb-0.4.3/tests/integration/cassettes/test_testproperties.test_delete_test_property.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json` & `itkdb-0.4.3/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_tests.test_list_test_types.json` & `itkdb-0.4.3/tests/integration/cassettes/test_tests.test_list_test_types.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_user.test_user_anonymous_login.json` & `itkdb-0.4.3/tests/integration/cassettes/test_user.test_user_anonymous_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_user.test_user_bad_login.json` & `itkdb-0.4.3/tests/integration/cassettes/test_user.test_user_bad_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_user.test_user_good_login.json` & `itkdb-0.4.3/tests/integration/cassettes/test_user.test_user_good_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/tests/integration/cassettes/test_warnings.test_get_component.json` & `itkdb-0.4.3/tests/integration/cassettes/test_warnings.test_get_component.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/.gitignore` & `itkdb-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/COPYING` & `itkdb-0.4.3/COPYING`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/LICENSE` & `itkdb-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.2/README.md` & `itkdb-0.4.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ITk DB v0.4.2
+# ITk DB v0.4.3
 
 Python wrapper around the ITk Production Database API.
 
 ---
 
 <!-- sync the following div with docs/index.md -->
 <div align="center">
```

### Comparing `itkdb-0.4.2/pyproject.toml` & `itkdb-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Development Status :: 1 - Planning",
 ]
 
 dependencies = [
     "requests>=2.0",  # for all HTTP calls to the API
-    "urllib3>=1.26.11", # for EOS uploading, need a correct urllib
+    "urllib3>=1.26.11,<2", # for EOS uploading, need a correct urllib
     "certifi",  # SSL
     "cachecontrol[filecache]",  # for caching HTTP requests according to spec to local file
     "click>=6.0",  # for console scripts,
     "python-jose",  # for id token decoding
     "attrs",  # for model inflation/deflation
     "python-dotenv",  # for loading env variables
     "simple-settings",  # for handling settings more easily
```

### Comparing `itkdb-0.4.2/PKG-INFO` & `itkdb-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkdb
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python wrapper to interface with ITk DB.
 Project-URL: Documentation, https://itkdb.docs.cern.ch/0.4/
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itkdb
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itkdb/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/sw/db/itkdb
 Author-email: Giordon Stark <kratsg@gmail.com>
 Maintainer-email: Giordon Stark <kratsg@gmail.com>
@@ -34,22 +34,22 @@
 Requires-Dist: pylibmagic
 Requires-Dist: python-dotenv
 Requires-Dist: python-jose
 Requires-Dist: python-magic
 Requires-Dist: requests>=2.0
 Requires-Dist: simple-settings
 Requires-Dist: typing-extensions>=4.0; python_version < '3.11'
-Requires-Dist: urllib3>=1.26.11
+Requires-Dist: urllib3<2,>=1.26.11
 Provides-Extra: contrib
 Requires-Dist: html2text; extra == 'contrib'
 Provides-Extra: eos
 Requires-Dist: pycurl; extra == 'eos'
 Description-Content-Type: text/markdown
 
-# ITk DB v0.4.2
+# ITk DB v0.4.3
 
 Python wrapper around the ITk Production Database API.
 
 ---
 
 <!-- sync the following div with docs/index.md -->
 <div align="center">
```

