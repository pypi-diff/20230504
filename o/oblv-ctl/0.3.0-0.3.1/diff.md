# Comparing `tmp/oblv-ctl-0.3.0.tar.gz` & `tmp/oblv_ctl-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oblv-ctl-0.3.0.tar", last modified: Tue May  2 04:57:35 2023, max compression
+gzip compressed data, was "oblv_ctl-0.3.1.tar", max compression
```

## Comparing `oblv-ctl-0.3.0.tar` & `oblv_ctl-0.3.1.tar`

### file list

```diff
@@ -1,157 +1,99 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 04:57:35.349425 oblv-ctl-0.3.0/
--rw-rw-rw-   0        0        0    11558 2023-01-05 11:33:47.000000 oblv-ctl-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     7309 2023-05-02 04:57:35.349425 oblv-ctl-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6653 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 04:57:35.207996 oblv-ctl-0.3.0/oblv_ctl/
--rw-rw-rw-   0        0        0       94 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:57:35.233924 oblv-ctl-0.3.0/oblv_ctl/api/
--rw-rw-rw-   0        0        0       48 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:57:35.235924 oblv-ctl-0.3.0/oblv_ctl/api/account/
--rw-rw-rw-   0        0        0        0 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/account/__init__.py
--rw-rw-rw-   0        0        0     5146 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/account/get_user_accounts_account_get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:57:35.237927 oblv-ctl-0.3.0/oblv_ctl/api/auth/
--rw-rw-rw-   0        0        0        0 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/auth/__init__.py
--rw-rw-rw-   0        0        0     5029 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/auth/authenticate_key_login_apikey_post.py
--rw-rw-rw-   0        0        0     5004 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/auth/logout_session_logout_delete.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:57:35.247801 oblv-ctl-0.3.0/oblv_ctl/api/deployment/
--rw-rw-rw-   0        0        0        0 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/deployment/__init__.py
--rw-rw-rw-   0        0        0     5735 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/deployment/create_new_deployment_deployment_post.py
--rw-rw-rw-   0        0        0     5233 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/deployment/delete_deployment_deployment_delete.py
--rw-rw-rw-   0        0        0     8308 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/deployment/generate_build_args_deployment_arguments_get.py
--rw-rw-rw-   0        0        0     6874 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/deployment/get_available_deployments_deployment_available_get.py
--rw-rw-rw-   0        0        0     5302 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/deployment/get_deployment_info_deployment_get.py
--rw-rw-rw-   0        0        0     5623 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/deployment/get_deployment_roles_deployment_roles_get.py
--rw-rw-rw-   0        0        0     3227 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/deployment/get_supported_regions_deployment_supported_regions_get.py
--rw-rw-rw-   0        0        0     6724 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/deployment/get_user_owned_deployments_deployment_owned_get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:57:35.252425 oblv-ctl-0.3.0/oblv_ctl/api/notification/
--rw-rw-rw-   0        0        0        0 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/notification/__init__.py
--rw-rw-rw-   0        0        0     5145 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/notification/get_all_notifications_notification_get.py
--rw-rw-rw-   0        0        0     5110 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/notification/get_notification_details_notification_notification_id_get.py
--rw-rw-rw-   0        0        0     4484 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/notification/mark_all_notification_read_notification_delete.py
--rw-rw-rw-   0        0        0     4954 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/notification/mark_notification_read_notification_notification_id_delete.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:57:35.259434 oblv-ctl-0.3.0/oblv_ctl/api/repo/
--rw-rw-rw-   0        0        0        0 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/repo/__init__.py
--rw-rw-rw-   0        0        0     5202 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/repo/get_all_repos_repo_linked_get.py
--rw-rw-rw-   0        0        0     6198 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/repo/get_repo_from_vcs_repo_get.py
--rw-rw-rw-   0        0        0     7756 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/repo/get_repo_refs_repo_refs_get.py
--rw-rw-rw-   0        0        0     6065 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/repo/get_repo_repo_repo_id_get.py
--rw-rw-rw-   0        0        0     6245 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/repo/get_repo_repo_repo_owner_repo_name_get.py
--rw-rw-rw-   0        0        0     5907 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/repo/search_repo_from_vcs_repo_search_get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:57:35.267433 oblv-ctl-0.3.0/oblv_ctl/api/service/
--rw-rw-rw-   0        0        0        0 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/service/__init__.py
--rw-rw-rw-   0        0        0     8037 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/service/add_repo_service_repo_service_post.py
--rw-rw-rw-   0        0        0     7266 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/service/delete_repo_services_repo_service_delete.py
--rw-rw-rw-   0        0        0     7513 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/service/get_repo_service_yaml_form_content_repo_service_yaml_get.py
--rw-rw-rw-   0        0        0     8367 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/service/get_repo_services_repo_service_get.py
--rw-rw-rw-   0        0        0     7166 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/service/get_user_services_service_get.py
--rw-rw-rw-   0        0        0     8539 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/service/update_repo_service_repo_service_put.py
--rw-rw-rw-   0        0        0     8369 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/service/validate_repo_service_repo_service_validate_get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:57:35.273086 oblv-ctl-0.3.0/oblv_ctl/api/user/
--rw-rw-rw-   0        0        0        0 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/user/__init__.py
--rw-rw-rw-   0        0        0     4991 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/user/add_user_public_shared_key_user_psk_put.py
--rw-rw-rw-   0        0        0     4913 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/user/get_user_deployment_credit_usage_user_credit_usage_get.py
--rw-rw-rw-   0        0        0     4874 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/user/get_user_profile_view_user_profile_get.py
--rw-rw-rw-   0        0        0     4888 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/user/get_user_public_shared_key_user_psk_get.py
--rw-rw-rw-   0        0        0     5013 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/user/update_user_name_user_name_put.py
--rw-rw-rw-   0        0        0     5150 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/api/user/update_user_password_user_password_put.py
--rw-rw-rw-   0        0        0      389 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/auth.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:57:35.277903 oblv-ctl-0.3.0/oblv_ctl/cli/
--rw-rw-rw-   0        0        0        0 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/cli/__init__.py
--rw-rw-rw-   0        0        0     4173 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/cli/deployment.py
--rw-rw-rw-   0        0        0     2755 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/cli/main.py
--rw-rw-rw-   0        0        0     3427 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/cli/service.py
--rw-rw-rw-   0        0        0      662 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/cli/utils.py
--rw-rw-rw-   0        0        0     1885 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/client.py
--rw-rw-rw-   0        0        0       30 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/config.py
--rw-rw-rw-   0        0        0     4062 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:57:35.314845 oblv-ctl-0.3.0/oblv_ctl/models/
--rw-rw-rw-   0        0        0     1573 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/__init__.py
--rw-rw-rw-   0        0        0     2611 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/access_history.py
--rw-rw-rw-   0        0        0     2326 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/account.py
--rw-rw-rw-   0        0        0     1533 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/api_key.py
--rw-rw-rw-   0        0        0     1979 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/available_deployment.py
--rw-rw-rw-   0        0        0     2395 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/available_deployment_list.py
--rw-rw-rw-   0        0        0     1975 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/build_args_schema.py
--rw-rw-rw-   0        0        0     4051 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/create_deployment_input.py
--rw-rw-rw-   0        0        0     2108 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/create_deployment_response.py
--rw-rw-rw-   0        0        0    10161 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/deployment_complete.py
--rw-rw-rw-   0        0        0     2342 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/deployment_list.py
--rw-rw-rw-   0        0        0     8783 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/deployment_response.py
--rw-rw-rw-   0        0        0     2251 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/http_validation_error.py
--rw-rw-rw-   0        0        0     3419 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/instance.py
--rw-rw-rw-   0        0        0     1704 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/message_model.py
--rw-rw-rw-   0        0        0     1656 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/name_input.py
--rw-rw-rw-   0        0        0     3066 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/notification_response.py
--rw-rw-rw-   0        0        0     1980 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/oblv_auth_response.py
--rw-rw-rw-   0        0        0     1585 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/psk.py
--rw-rw-rw-   0        0        0     2172 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/ref_response.py
--rw-rw-rw-   0        0        0     4997 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/repo.py
--rw-rw-rw-   0        0        0     2338 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/repo_all_response.py
--rw-rw-rw-   0        0        0     2319 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/repo_service_list.py
--rw-rw-rw-   0        0        0     5571 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/repo_services.py
--rw-rw-rw-   0        0        0     2100 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/role_response.py
--rw-rw-rw-   0        0        0     1407 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/service_content_response.py
--rw-rw-rw-   0        0        0     2432 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/service_validation_response.py
--rw-rw-rw-   0        0        0     1395 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/service_yaml_add_input.py
--rw-rw-rw-   0        0        0     1410 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/service_yaml_update_input.py
--rw-rw-rw-   0        0        0     2682 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/shared_users.py
--rw-rw-rw-   0        0        0     1374 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/supported_regions.py
--rw-rw-rw-   0        0        0     3177 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/user_credit_utilization.py
--rw-rw-rw-   0        0        0     1870 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/user_password_input.py
--rw-rw-rw-   0        0        0     2688 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/user_profile_response.py
--rw-rw-rw-   0        0        0     2291 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/user_service_list.py
--rw-rw-rw-   0        0        0     3444 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/user_services.py
--rw-rw-rw-   0        0        0     2544 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/validated_service.py
--rw-rw-rw-   0        0        0     1903 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/validation_error.py
--rw-rw-rw-   0        0        0     2731 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/models/vcs_repo_response.py
--rw-rw-rw-   0        0        0    21755 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/oblv_client.py
--rw-rw-rw-   0        0        0       25 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/py.typed
--rw-rw-rw-   0        0        0      982 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/types.py
--rw-rw-rw-   0        0        0     1283 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/oblv_ctl/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:57:35.232923 oblv-ctl-0.3.0/oblv_ctl.egg-info/
--rw-rw-rw-   0        0        0     7309 2023-05-02 04:57:35.000000 oblv-ctl-0.3.0/oblv_ctl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5536 2023-05-02 04:57:35.000000 oblv-ctl-0.3.0/oblv_ctl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 04:57:35.000000 oblv-ctl-0.3.0/oblv_ctl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-02 04:57:35.000000 oblv-ctl-0.3.0/oblv_ctl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2023-05-02 04:57:35.000000 oblv-ctl-0.3.0/oblv_ctl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-02 04:57:35.000000 oblv-ctl-0.3.0/oblv_ctl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      751 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 04:57:35.349425 oblv-ctl-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1330 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:57:35.316844 oblv-ctl-0.3.0/tests/
--rw-rw-rw-   0        0        0        0 2022-09-08 17:43:31.000000 oblv-ctl-0.3.0/tests/__init__.py
--rw-rw-rw-   0        0        0       88 2023-05-02 04:50:12.000000 oblv-ctl-0.3.0/tests/test_oblv.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:57:35.348412 oblv-ctl-0.3.0/tests/unit/
--rw-rw-rw-   0        0        0        0 2022-11-22 05:48:14.000000 oblv-ctl-0.3.0/tests/unit/__init__.py
--rw-rw-rw-   0        0        0     7238 2023-05-02 04:52:35.000000 oblv-ctl-0.3.0/tests/unit/constants.py
--rw-rw-rw-   0        0        0     4052 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_add_service.py
--rw-rw-rw-   0        0        0     3703 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_auth.py
--rw-rw-rw-   0        0        0     3275 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_available_deployments.py
--rw-rw-rw-   0        0        0     3626 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_create_deployment.py
--rw-rw-rw-   0        0        0     3205 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_deployment_info.py
--rw-rw-rw-   0        0        0     3288 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_deployment_roles.py
--rw-rw-rw-   0        0        0     3430 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_generate_deployment_build_args.py
--rw-rw-rw-   0        0        0     3293 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_link_repo.py
--rw-rw-rw-   0        0        0     2926 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_logout.py
--rw-rw-rw-   0        0        0     3261 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_remove_deployment.py
--rw-rw-rw-   0        0        0     3940 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_remove_service.py
--rw-rw-rw-   0        0        0     3087 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_repo_refs.py
--rw-rw-rw-   0        0        0     3243 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_repo_services.py
--rw-rw-rw-   0        0        0     3054 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_repo_vcs.py
--rw-rw-rw-   0        0        0     3116 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_repo_with_services.py
--rw-rw-rw-   0        0        0     3429 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_revalidate_service.py
--rw-rw-rw-   0        0        0     3156 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_search_repo.py
--rw-rw-rw-   0        0        0     3309 2023-05-02 04:48:50.000000 oblv-ctl-0.3.0/tests/unit/test_service_yaml_content.py
--rw-rw-rw-   0        0        0     1874 2023-05-02 04:48:51.000000 oblv-ctl-0.3.0/tests/unit/test_supported_aws_regions.py
--rw-rw-rw-   0        0        0     3160 2023-05-02 04:48:51.000000 oblv-ctl-0.3.0/tests/unit/test_unlink_repo.py
--rw-rw-rw-   0        0        0     3821 2023-05-02 04:48:51.000000 oblv-ctl-0.3.0/tests/unit/test_update_service.py
--rw-rw-rw-   0        0        0     3225 2023-05-02 04:48:51.000000 oblv-ctl-0.3.0/tests/unit/test_update_user_password.py
--rw-rw-rw-   0        0        0     3215 2023-05-02 04:48:51.000000 oblv-ctl-0.3.0/tests/unit/test_user_accounts.py
--rw-rw-rw-   0        0        0     3353 2023-05-02 04:48:51.000000 oblv-ctl-0.3.0/tests/unit/test_user_credit_usage.py
--rw-rw-rw-   0        0        0     3152 2023-05-02 04:48:51.000000 oblv-ctl-0.3.0/tests/unit/test_user_deployments.py
--rw-rw-rw-   0        0        0     3072 2023-05-02 04:48:51.000000 oblv-ctl-0.3.0/tests/unit/test_user_linked_repos.py
--rw-rw-rw-   0        0        0     3131 2023-05-02 04:48:51.000000 oblv-ctl-0.3.0/tests/unit/test_user_name_update.py
--rw-rw-rw-   0        0        0     3359 2023-05-02 04:48:51.000000 oblv-ctl-0.3.0/tests/unit/test_user_profile.py
--rw-rw-rw-   0        0        0     3087 2023-05-02 04:48:51.000000 oblv-ctl-0.3.0/tests/unit/test_user_psk.py
--rw-rw-rw-   0        0        0     3125 2023-05-02 04:48:51.000000 oblv-ctl-0.3.0/tests/unit/test_user_services.py
--rw-rw-rw-   0        0        0     3064 2023-05-02 04:48:51.000000 oblv-ctl-0.3.0/tests/unit/test_user_set_psk.py
+-rw-r--r--   0        0        0    11558 2023-01-05 11:33:47.193634 oblv_ctl-0.3.1/LICENSE
+-rw-r--r--   0        0        0       94 2023-05-04 07:16:41.170094 oblv_ctl-0.3.1/oblv_ctl/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-02 04:48:50.842284 oblv_ctl-0.3.1/oblv_ctl/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 04:48:50.843282 oblv_ctl-0.3.1/oblv_ctl/api/account/__init__.py
+-rw-r--r--   0        0        0     5146 2023-05-02 04:48:50.843282 oblv_ctl-0.3.1/oblv_ctl/api/account/get_user_accounts_account_get.py
+-rw-r--r--   0        0        0        0 2023-05-02 04:48:50.843282 oblv_ctl-0.3.1/oblv_ctl/api/auth/__init__.py
+-rw-r--r--   0        0        0     5029 2023-05-02 04:48:50.844282 oblv_ctl-0.3.1/oblv_ctl/api/auth/authenticate_key_login_apikey_post.py
+-rw-r--r--   0        0        0     5004 2023-05-02 04:48:50.844282 oblv_ctl-0.3.1/oblv_ctl/api/auth/logout_session_logout_delete.py
+-rw-r--r--   0        0        0        0 2023-05-02 04:48:50.844282 oblv_ctl-0.3.1/oblv_ctl/api/deployment/__init__.py
+-rw-r--r--   0        0        0     5735 2023-05-02 04:48:50.845281 oblv_ctl-0.3.1/oblv_ctl/api/deployment/create_new_deployment_deployment_post.py
+-rw-r--r--   0        0        0     5233 2023-05-02 04:48:50.846280 oblv_ctl-0.3.1/oblv_ctl/api/deployment/delete_deployment_deployment_delete.py
+-rw-r--r--   0        0        0     8308 2023-05-02 04:48:50.846280 oblv_ctl-0.3.1/oblv_ctl/api/deployment/generate_build_args_deployment_arguments_get.py
+-rw-r--r--   0        0        0     6874 2023-05-02 04:48:50.846280 oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_available_deployments_deployment_available_get.py
+-rw-r--r--   0        0        0     5302 2023-05-02 04:48:50.847281 oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_deployment_info_deployment_get.py
+-rw-r--r--   0        0        0     5623 2023-05-02 04:48:50.847281 oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_deployment_roles_deployment_roles_get.py
+-rw-r--r--   0        0        0     3227 2023-05-02 04:48:50.848284 oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_supported_regions_deployment_supported_regions_get.py
+-rw-r--r--   0        0        0     6724 2023-05-02 04:48:50.848284 oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_user_owned_deployments_deployment_owned_get.py
+-rw-r--r--   0        0        0        0 2023-05-02 04:48:50.849283 oblv_ctl-0.3.1/oblv_ctl/api/notification/__init__.py
+-rw-r--r--   0        0        0     5145 2023-05-02 04:48:50.849283 oblv_ctl-0.3.1/oblv_ctl/api/notification/get_all_notifications_notification_get.py
+-rw-r--r--   0        0        0     5110 2023-05-02 04:48:50.850283 oblv_ctl-0.3.1/oblv_ctl/api/notification/get_notification_details_notification_notification_id_get.py
+-rw-r--r--   0        0        0     4484 2023-05-02 04:48:50.850283 oblv_ctl-0.3.1/oblv_ctl/api/notification/mark_all_notification_read_notification_delete.py
+-rw-r--r--   0        0        0     4954 2023-05-02 04:48:50.851281 oblv_ctl-0.3.1/oblv_ctl/api/notification/mark_notification_read_notification_notification_id_delete.py
+-rw-r--r--   0        0        0        0 2023-05-02 04:48:50.851281 oblv_ctl-0.3.1/oblv_ctl/api/repo/__init__.py
+-rw-r--r--   0        0        0     5202 2023-05-02 04:48:50.852280 oblv_ctl-0.3.1/oblv_ctl/api/repo/get_all_repos_repo_linked_get.py
+-rw-r--r--   0        0        0     6198 2023-05-02 04:48:50.852280 oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_from_vcs_repo_get.py
+-rw-r--r--   0        0        0     7756 2023-05-02 04:48:50.852280 oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_refs_repo_refs_get.py
+-rw-r--r--   0        0        0     6065 2023-05-02 04:48:50.853281 oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_repo_repo_id_get.py
+-rw-r--r--   0        0        0     6245 2023-05-02 04:48:50.853281 oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_repo_repo_owner_repo_name_get.py
+-rw-r--r--   0        0        0     5907 2023-05-02 04:48:50.854282 oblv_ctl-0.3.1/oblv_ctl/api/repo/search_repo_from_vcs_repo_search_get.py
+-rw-r--r--   0        0        0        0 2023-05-02 04:48:50.854282 oblv_ctl-0.3.1/oblv_ctl/api/service/__init__.py
+-rw-r--r--   0        0        0     8037 2023-05-02 04:48:50.854282 oblv_ctl-0.3.1/oblv_ctl/api/service/add_repo_service_repo_service_post.py
+-rw-r--r--   0        0        0     7266 2023-05-02 04:48:50.855280 oblv_ctl-0.3.1/oblv_ctl/api/service/delete_repo_services_repo_service_delete.py
+-rw-r--r--   0        0        0     7513 2023-05-02 04:48:50.855280 oblv_ctl-0.3.1/oblv_ctl/api/service/get_repo_service_yaml_form_content_repo_service_yaml_get.py
+-rw-r--r--   0        0        0     8367 2023-05-02 04:48:50.856281 oblv_ctl-0.3.1/oblv_ctl/api/service/get_repo_services_repo_service_get.py
+-rw-r--r--   0        0        0     7166 2023-05-02 04:48:50.856281 oblv_ctl-0.3.1/oblv_ctl/api/service/get_user_services_service_get.py
+-rw-r--r--   0        0        0     8539 2023-05-02 04:48:50.857280 oblv_ctl-0.3.1/oblv_ctl/api/service/update_repo_service_repo_service_put.py
+-rw-r--r--   0        0        0     8369 2023-05-02 04:48:50.857280 oblv_ctl-0.3.1/oblv_ctl/api/service/validate_repo_service_repo_service_validate_get.py
+-rw-r--r--   0        0        0        0 2023-05-02 04:48:50.857280 oblv_ctl-0.3.1/oblv_ctl/api/user/__init__.py
+-rw-r--r--   0        0        0     4991 2023-05-02 04:48:50.858280 oblv_ctl-0.3.1/oblv_ctl/api/user/add_user_public_shared_key_user_psk_put.py
+-rw-r--r--   0        0        0     4913 2023-05-02 04:48:50.858280 oblv_ctl-0.3.1/oblv_ctl/api/user/get_user_deployment_credit_usage_user_credit_usage_get.py
+-rw-r--r--   0        0        0     4874 2023-05-02 04:48:50.859281 oblv_ctl-0.3.1/oblv_ctl/api/user/get_user_profile_view_user_profile_get.py
+-rw-r--r--   0        0        0     4888 2023-05-02 04:48:50.859281 oblv_ctl-0.3.1/oblv_ctl/api/user/get_user_public_shared_key_user_psk_get.py
+-rw-r--r--   0        0        0     5013 2023-05-02 04:48:50.859281 oblv_ctl-0.3.1/oblv_ctl/api/user/update_user_name_user_name_put.py
+-rw-r--r--   0        0        0     5150 2023-05-02 04:48:50.860280 oblv_ctl-0.3.1/oblv_ctl/api/user/update_user_password_user_password_put.py
+-rw-r--r--   0        0        0      389 2023-05-02 05:12:33.359116 oblv_ctl-0.3.1/oblv_ctl/auth.py
+-rw-r--r--   0        0        0        0 2023-05-02 04:48:50.864283 oblv_ctl-0.3.1/oblv_ctl/cli/__init__.py
+-rw-r--r--   0        0        0     4910 2023-05-04 10:47:47.198954 oblv_ctl-0.3.1/oblv_ctl/cli/deployment.py
+-rw-r--r--   0        0        0     2873 2023-05-04 10:47:47.198954 oblv_ctl-0.3.1/oblv_ctl/cli/main.py
+-rw-r--r--   0        0        0     4079 2023-05-04 10:47:47.194954 oblv_ctl-0.3.1/oblv_ctl/cli/service.py
+-rw-r--r--   0        0        0     1775 2023-05-04 10:47:47.198954 oblv_ctl-0.3.1/oblv_ctl/cli/utils.py
+-rw-r--r--   0        0        0     1885 2023-05-02 04:48:50.878886 oblv_ctl-0.3.1/oblv_ctl/client.py
+-rw-r--r--   0        0        0       30 2023-05-02 04:48:50.879888 oblv_ctl-0.3.1/oblv_ctl/config.py
+-rw-r--r--   0        0        0     4219 2023-05-04 09:07:09.223713 oblv_ctl-0.3.1/oblv_ctl/exceptions.py
+-rw-r--r--   0        0        0     1573 2023-05-02 04:48:50.880884 oblv_ctl-0.3.1/oblv_ctl/models/__init__.py
+-rw-r--r--   0        0        0     2611 2023-05-02 04:48:50.881916 oblv_ctl-0.3.1/oblv_ctl/models/access_history.py
+-rw-r--r--   0        0        0     2326 2023-05-02 04:48:50.881916 oblv_ctl-0.3.1/oblv_ctl/models/account.py
+-rw-r--r--   0        0        0     1533 2023-05-02 04:48:50.881916 oblv_ctl-0.3.1/oblv_ctl/models/api_key.py
+-rw-r--r--   0        0        0     1979 2023-05-02 04:48:50.882919 oblv_ctl-0.3.1/oblv_ctl/models/available_deployment.py
+-rw-r--r--   0        0        0     2395 2023-05-02 04:48:50.883916 oblv_ctl-0.3.1/oblv_ctl/models/available_deployment_list.py
+-rw-r--r--   0        0        0     1975 2023-05-02 04:48:50.883916 oblv_ctl-0.3.1/oblv_ctl/models/build_args_schema.py
+-rw-r--r--   0        0        0     4051 2023-05-02 04:48:50.883916 oblv_ctl-0.3.1/oblv_ctl/models/create_deployment_input.py
+-rw-r--r--   0        0        0     2108 2023-05-02 04:48:50.884917 oblv_ctl-0.3.1/oblv_ctl/models/create_deployment_response.py
+-rw-r--r--   0        0        0    10161 2023-05-02 04:48:50.884917 oblv_ctl-0.3.1/oblv_ctl/models/deployment_complete.py
+-rw-r--r--   0        0        0     2342 2023-05-02 04:48:50.885915 oblv_ctl-0.3.1/oblv_ctl/models/deployment_list.py
+-rw-r--r--   0        0        0     8783 2023-05-02 04:48:50.885915 oblv_ctl-0.3.1/oblv_ctl/models/deployment_response.py
+-rw-r--r--   0        0        0     2251 2023-05-02 04:48:50.885915 oblv_ctl-0.3.1/oblv_ctl/models/http_validation_error.py
+-rw-r--r--   0        0        0     3419 2023-05-02 04:48:50.886916 oblv_ctl-0.3.1/oblv_ctl/models/instance.py
+-rw-r--r--   0        0        0     1704 2023-05-02 04:48:50.886916 oblv_ctl-0.3.1/oblv_ctl/models/message_model.py
+-rw-r--r--   0        0        0     1656 2023-05-02 04:48:50.886916 oblv_ctl-0.3.1/oblv_ctl/models/name_input.py
+-rw-r--r--   0        0        0     3066 2023-05-02 04:48:50.886916 oblv_ctl-0.3.1/oblv_ctl/models/notification_response.py
+-rw-r--r--   0        0        0     1980 2023-05-02 04:48:50.887915 oblv_ctl-0.3.1/oblv_ctl/models/oblv_auth_response.py
+-rw-r--r--   0        0        0     1585 2023-05-02 04:48:50.887915 oblv_ctl-0.3.1/oblv_ctl/models/psk.py
+-rw-r--r--   0        0        0     2172 2023-05-02 04:48:50.887915 oblv_ctl-0.3.1/oblv_ctl/models/ref_response.py
+-rw-r--r--   0        0        0     4997 2023-05-02 04:48:50.888915 oblv_ctl-0.3.1/oblv_ctl/models/repo.py
+-rw-r--r--   0        0        0     2338 2023-05-02 04:48:50.888915 oblv_ctl-0.3.1/oblv_ctl/models/repo_all_response.py
+-rw-r--r--   0        0        0     2319 2023-05-02 04:48:50.889915 oblv_ctl-0.3.1/oblv_ctl/models/repo_service_list.py
+-rw-r--r--   0        0        0     5571 2023-05-02 04:48:50.889915 oblv_ctl-0.3.1/oblv_ctl/models/repo_services.py
+-rw-r--r--   0        0        0     2100 2023-05-02 04:48:50.890916 oblv_ctl-0.3.1/oblv_ctl/models/role_response.py
+-rw-r--r--   0        0        0     1407 2023-05-02 04:48:50.890916 oblv_ctl-0.3.1/oblv_ctl/models/service_content_response.py
+-rw-r--r--   0        0        0     2432 2023-05-02 04:48:50.890916 oblv_ctl-0.3.1/oblv_ctl/models/service_validation_response.py
+-rw-r--r--   0        0        0     1395 2023-05-02 04:48:50.891916 oblv_ctl-0.3.1/oblv_ctl/models/service_yaml_add_input.py
+-rw-r--r--   0        0        0     1410 2023-05-02 04:48:50.891916 oblv_ctl-0.3.1/oblv_ctl/models/service_yaml_update_input.py
+-rw-r--r--   0        0        0     2682 2023-05-02 04:48:50.892915 oblv_ctl-0.3.1/oblv_ctl/models/shared_users.py
+-rw-r--r--   0        0        0     1374 2023-05-02 04:48:50.892915 oblv_ctl-0.3.1/oblv_ctl/models/supported_regions.py
+-rw-r--r--   0        0        0     3177 2023-05-02 04:48:50.892915 oblv_ctl-0.3.1/oblv_ctl/models/user_credit_utilization.py
+-rw-r--r--   0        0        0     1870 2023-05-02 04:48:50.893915 oblv_ctl-0.3.1/oblv_ctl/models/user_password_input.py
+-rw-r--r--   0        0        0     2688 2023-05-02 04:48:50.893915 oblv_ctl-0.3.1/oblv_ctl/models/user_profile_response.py
+-rw-r--r--   0        0        0     2291 2023-05-02 04:48:50.893915 oblv_ctl-0.3.1/oblv_ctl/models/user_service_list.py
+-rw-r--r--   0        0        0     3444 2023-05-02 04:48:50.894916 oblv_ctl-0.3.1/oblv_ctl/models/user_services.py
+-rw-r--r--   0        0        0     2544 2023-05-02 04:48:50.894916 oblv_ctl-0.3.1/oblv_ctl/models/validated_service.py
+-rw-r--r--   0        0        0     1903 2023-05-02 04:48:50.895916 oblv_ctl-0.3.1/oblv_ctl/models/validation_error.py
+-rw-r--r--   0        0        0     2731 2023-05-02 04:48:50.895916 oblv_ctl-0.3.1/oblv_ctl/models/vcs_repo_response.py
+-rw-r--r--   0        0        0    21623 2023-05-04 10:26:44.709977 oblv_ctl-0.3.1/oblv_ctl/oblv_client.py
+-rw-r--r--   0        0        0       25 2023-05-02 04:48:50.900915 oblv_ctl-0.3.1/oblv_ctl/py.typed
+-rw-r--r--   0        0        0      982 2023-05-02 04:48:50.901917 oblv_ctl-0.3.1/oblv_ctl/types.py
+-rw-r--r--   0        0        0     1283 2023-05-02 04:48:50.901917 oblv_ctl-0.3.1/oblv_ctl/utils.py
+-rw-r--r--   0        0        0      750 2023-05-04 10:15:25.127725 oblv_ctl-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6661 2023-05-02 05:12:37.943952 oblv_ctl-0.3.1/README.md
+-rw-r--r--   0        0        0     7459 1970-01-01 00:00:00.000000 oblv_ctl-0.3.1/PKG-INFO
```

### Comparing `oblv-ctl-0.3.0/LICENSE` & `oblv_ctl-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/PKG-INFO` & `oblv_ctl-0.3.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,20 @@
-Metadata-Version: 2.1
-Name: oblv-ctl
-Version: 0.3.0
-Summary: A client library for accessing Oblivious APIs
-Home-page: https://github.com/ObliviousAI/oblv-ctl
-Author: Oblivious Support
-Author-email: support@oblivious.ai
-License: Apache-2.0
-Keywords: Oblivious,python,package
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # oblv-ctl
 
 A Python library to access Oblivious APIs.
 
 ## Usage
 
 First, create a client, with your API key. This key can be created in the
 [Oblivious Console UI](https://console.oblivious.ai/). Go to the
 settings page, and create your ApiKey. Once done, the client can be
 created as follows
 
 ``` {.python}
-from oblv import authenticate
+from oblv_ctl import authenticate
 client = authenticate(apikey=*your_key_here*)
 ```
 
 
 Using this client, all the Oblivious actions can be performed, including the deployment of enclaves. Below is a step-by-step guide, to creating your first deployment.
 
 
@@ -166,15 +148,15 @@
 > file
 >
 > The service used,
 > does not have requirements for any runtime or build arguments, so not
 > needed here.
 
 ``` {.python}
-from oblv.models import CreateDeploymentInput
+from oblv_ctl.models import CreateDeploymentInput
 input = CreateDeploymentInput(
     owner="ObliviousAI",
     repo="FastAPI-Enclave-Services",
     account_type="github",
     ref="master",
     ref_type="branch",
     region_name="us-east-1",
```

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/account/get_user_accounts_account_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/account/get_user_accounts_account_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/auth/authenticate_key_login_apikey_post.py` & `oblv_ctl-0.3.1/oblv_ctl/api/auth/authenticate_key_login_apikey_post.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/auth/logout_session_logout_delete.py` & `oblv_ctl-0.3.1/oblv_ctl/api/auth/logout_session_logout_delete.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/deployment/create_new_deployment_deployment_post.py` & `oblv_ctl-0.3.1/oblv_ctl/api/deployment/create_new_deployment_deployment_post.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/deployment/delete_deployment_deployment_delete.py` & `oblv_ctl-0.3.1/oblv_ctl/api/deployment/delete_deployment_deployment_delete.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/deployment/generate_build_args_deployment_arguments_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/deployment/generate_build_args_deployment_arguments_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/deployment/get_available_deployments_deployment_available_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_available_deployments_deployment_available_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/deployment/get_deployment_info_deployment_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_deployment_info_deployment_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/deployment/get_deployment_roles_deployment_roles_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_deployment_roles_deployment_roles_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/deployment/get_supported_regions_deployment_supported_regions_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_supported_regions_deployment_supported_regions_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/deployment/get_user_owned_deployments_deployment_owned_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_user_owned_deployments_deployment_owned_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/notification/get_all_notifications_notification_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/notification/get_all_notifications_notification_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/notification/get_notification_details_notification_notification_id_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/notification/get_notification_details_notification_notification_id_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/notification/mark_all_notification_read_notification_delete.py` & `oblv_ctl-0.3.1/oblv_ctl/api/notification/mark_all_notification_read_notification_delete.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/notification/mark_notification_read_notification_notification_id_delete.py` & `oblv_ctl-0.3.1/oblv_ctl/api/notification/mark_notification_read_notification_notification_id_delete.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/repo/get_all_repos_repo_linked_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/repo/get_all_repos_repo_linked_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/repo/get_repo_from_vcs_repo_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_from_vcs_repo_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/repo/get_repo_refs_repo_refs_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_refs_repo_refs_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/repo/get_repo_repo_repo_id_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_repo_repo_id_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/repo/get_repo_repo_repo_owner_repo_name_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_repo_repo_owner_repo_name_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/repo/search_repo_from_vcs_repo_search_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/repo/search_repo_from_vcs_repo_search_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/service/add_repo_service_repo_service_post.py` & `oblv_ctl-0.3.1/oblv_ctl/api/service/add_repo_service_repo_service_post.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/service/delete_repo_services_repo_service_delete.py` & `oblv_ctl-0.3.1/oblv_ctl/api/service/delete_repo_services_repo_service_delete.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/service/get_repo_service_yaml_form_content_repo_service_yaml_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/service/get_repo_service_yaml_form_content_repo_service_yaml_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/service/get_repo_services_repo_service_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/service/get_repo_services_repo_service_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/service/get_user_services_service_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/service/get_user_services_service_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/service/update_repo_service_repo_service_put.py` & `oblv_ctl-0.3.1/oblv_ctl/api/service/update_repo_service_repo_service_put.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/service/validate_repo_service_repo_service_validate_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/service/validate_repo_service_repo_service_validate_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/user/add_user_public_shared_key_user_psk_put.py` & `oblv_ctl-0.3.1/oblv_ctl/api/user/add_user_public_shared_key_user_psk_put.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/user/get_user_deployment_credit_usage_user_credit_usage_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/user/get_user_deployment_credit_usage_user_credit_usage_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/user/get_user_profile_view_user_profile_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/user/get_user_profile_view_user_profile_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/user/get_user_public_shared_key_user_psk_get.py` & `oblv_ctl-0.3.1/oblv_ctl/api/user/get_user_public_shared_key_user_psk_get.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/user/update_user_name_user_name_put.py` & `oblv_ctl-0.3.1/oblv_ctl/api/user/update_user_name_user_name_put.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/api/user/update_user_password_user_password_put.py` & `oblv_ctl-0.3.1/oblv_ctl/api/user/update_user_password_user_password_put.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/cli/main.py` & `oblv_ctl-0.3.1/oblv_ctl/cli/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,57 +26,56 @@
     try:
         client = authenticate(apikey)
         credentials = "oblivious_user_id = {}\ntoken = {}".format(client.oblivious_user_id,client.token)
         os.makedirs(os.path.dirname(utils.cred_file_path), exist_ok=True)
         with open(utils.cred_file_path,'w') as f:
             f.write(credentials)
     except Exception as e:
-        print(e)
+        utils.render_error_message(str(e))
     else:
-        print("Successfully logged in")
+        utils.render_success_message("Logged in")
         
 @app.command(help="Command to clear and invalidate the token")
 def logout():
     try:
         if os.path.exists(utils.cred_file_path):
             with open(utils.cred_file_path,'w') as f:
-                #Just overwriting the file, whether login exists or not
                 f.write("")
     except FileNotFoundError as e:
-        #Case where .oblv folder was never generated
-        #With the check of path exists makes no sense
-        print(".oblv folder not found")
+        #If path not found, then the use is by default logged out
+        pass
     except Exception as e:
-        print(e)
+        utils.render_error_message(str(e))
     else:
-        print("Successfully logged out")
+        utils.render_success_message("Logged out")
     
 @app.command(help="Command to fetch the VCS accounts")
 def accounts():
     try:
         client = utils.read_credentials()
-        # console.print("["+",\n".join([x.__repr__() for x in client.accounts()])+"]")
         utils.render_output(client.accounts())
     except FileNotFoundError as e:
-        print("Kindly login before performing this action")
+        utils.render_warning_message("Kindly login before performing this action")
     except Exception as e:
-        print(e)
+        if e.args[0]==utils.NO_CREDS_FOUND:
+            utils.render_warning_message("Kindly login before performing this action")
     
 @app.command(help="Command to fetch/set the Public Key")
 def psk(set_key : str = typer.Option(None, help="Public key to be set")):
     try:
         client = utils.read_credentials()
         if set_key!=None:
             client.set_psk(set_key)
         else:
             utils.render_output(client.psk())
     except FileNotFoundError as e:
-        print("Kindly login before performing this action")
+        utils.render_warning_message("Kindly login before performing this action")
     except Exception as e:
-        print(e)
+        if e.args[0]==utils.NO_CREDS_FOUND:
+            utils.render_warning_message("Kindly login before performing this action")
     
 app.add_typer(service.app, name="service", help="Commands to interact with the services")
 app.add_typer(deployment.app, name="deployment", help="Commands to interact with the deployments")
 
 
 
 if __name__ == "__main__":
```

### Comparing `oblv-ctl-0.3.0/oblv_ctl/cli/service.py` & `oblv_ctl-0.3.1/oblv_ctl/cli/service.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,56 +16,64 @@
         else:
             args = {}
             if service_file!=None:
                 with open(service_file,"r") as f:
                     args = json.load(f)
             client.add_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref, data=args)
     except FileNotFoundError as e:
-        print("Kindly login before performing this action")
+        utils.render_warning_message("Kindly login before performing this action")
     except Exception as e:
-        print(e)
+        if e.args[0]==utils.NO_CREDS_FOUND:
+            utils.render_warning_message("Kindly login before performing this action")
+        pass
     else:
-        print("Successfully added the service")
+        utils.render_success_message("Added the service")
 
 @app.command(help="To remove an existing service")
 def remove(repo_owner: str = typer.Argument(..., help=("Repository Owner")), repo_name: str = typer.Argument(...,help=("Repository Name")), ref: str = typer.Argument(..., help=("Service ref name")), tag : bool = typer.Option(False, "--tag", help="If provided, the ref is considered to be a tag on repository")):
     try:
         client = utils.read_credentials()
         if tag:
             client.remove_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref,ref_type="tag")
         else:
             client.remove_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref)
     except FileNotFoundError as e:
-        print("Kindly login before performing this action")
+        utils.render_warning_message("Kindly login before performing this action")
     except Exception as e:
-        print(e)
+        if e.args[0]==utils.NO_CREDS_FOUND:
+            utils.render_warning_message("Kindly login before performing this action")
+        pass
     else:
-        print("Successfully removed the service")
+        utils.render_success_message("Removed the service")
 
 @app.command(help="To fetch user's services list")
 def fetch():
     try:
         client = utils.read_credentials()
-        print(client.user_services())
+        utils.render_output(client.user_services())
     except FileNotFoundError as e:
-        print("Kindly login before performing this action")
+        utils.render_warning_message("Kindly login before performing this action")
     except Exception as e:
-        print(e)
+        if e.args[0]==utils.NO_CREDS_FOUND:
+            utils.render_warning_message("Kindly login before performing this action")
+        pass
 
 @app.command(help="To updates user's service")
 def update(repo_owner: str = typer.Argument(..., help=("Repository Owner")), repo_name: str = typer.Argument(...,help=("Repository Name")), ref: str = typer.Argument(..., help=("Service ref name")), tag : bool = typer.Option(False, "--tag", help="If provided, the ref is considered to be a tag on repository"), service_file : str = typer.Option(None,help="Service yaml file in json format. Not allowed with --tag")):
     try:
         client = utils.read_credentials()
         if tag:
             client.update_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref,ref_type="tag")
         else:
             args = {}
             if service_file!=None:
                 with open(service_file,"r") as f:
                     args = json.load(f)
             client.update_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref, data=args)
     except FileNotFoundError as e:
-        print("Kindly login before performing this action")
+        utils.render_warning_message("Kindly login before performing this action")
     except Exception as e:
-        print(e)
+        if e.args[0]==utils.NO_CREDS_FOUND:
+            utils.render_warning_message("Kindly login before performing this action")
+        pass
     else:
-        print("Successfully updated the service")
+        utils.render_success_message("Updated the service")
```

### Comparing `oblv-ctl-0.3.0/oblv_ctl/client.py` & `oblv_ctl-0.3.1/oblv_ctl/client.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/exceptions.py` & `oblv_ctl-0.3.1/oblv_ctl/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 
+HTTP_CLIENT_ERROR_MESSAGE = 'An HTTP Client raised an unhandled exception. Kindly raise a request to the support team, along with the {} for resolution.'
+
 def _exception_from_packed_args(exception_cls, args=None, kwargs=None):
     # This is helpful for reducing Exceptions that only accept kwargs as
     # only positional arguments can be provided for __reduce__
     # Ideally, this would also be a class method on the OblvError
     # but instance methods cannot be pickled.
     if args is None:
         args = ()
```

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/__init__.py` & `oblv_ctl-0.3.1/oblv_ctl/models/__init__.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/access_history.py` & `oblv_ctl-0.3.1/oblv_ctl/models/access_history.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/account.py` & `oblv_ctl-0.3.1/oblv_ctl/models/account.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/api_key.py` & `oblv_ctl-0.3.1/oblv_ctl/models/api_key.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/available_deployment.py` & `oblv_ctl-0.3.1/oblv_ctl/models/available_deployment.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/available_deployment_list.py` & `oblv_ctl-0.3.1/oblv_ctl/models/available_deployment_list.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/build_args_schema.py` & `oblv_ctl-0.3.1/oblv_ctl/models/build_args_schema.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/create_deployment_input.py` & `oblv_ctl-0.3.1/oblv_ctl/models/create_deployment_input.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/create_deployment_response.py` & `oblv_ctl-0.3.1/oblv_ctl/models/create_deployment_response.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/deployment_complete.py` & `oblv_ctl-0.3.1/oblv_ctl/models/deployment_complete.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/deployment_list.py` & `oblv_ctl-0.3.1/oblv_ctl/models/deployment_list.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/deployment_response.py` & `oblv_ctl-0.3.1/oblv_ctl/models/deployment_response.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/http_validation_error.py` & `oblv_ctl-0.3.1/oblv_ctl/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/instance.py` & `oblv_ctl-0.3.1/oblv_ctl/models/instance.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/message_model.py` & `oblv_ctl-0.3.1/oblv_ctl/models/message_model.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/name_input.py` & `oblv_ctl-0.3.1/oblv_ctl/models/name_input.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/notification_response.py` & `oblv_ctl-0.3.1/oblv_ctl/models/notification_response.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/oblv_auth_response.py` & `oblv_ctl-0.3.1/oblv_ctl/models/oblv_auth_response.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/psk.py` & `oblv_ctl-0.3.1/oblv_ctl/models/psk.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/ref_response.py` & `oblv_ctl-0.3.1/oblv_ctl/models/ref_response.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/repo.py` & `oblv_ctl-0.3.1/oblv_ctl/models/repo.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/repo_all_response.py` & `oblv_ctl-0.3.1/oblv_ctl/models/repo_all_response.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/repo_service_list.py` & `oblv_ctl-0.3.1/oblv_ctl/models/repo_service_list.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/repo_services.py` & `oblv_ctl-0.3.1/oblv_ctl/models/repo_services.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/role_response.py` & `oblv_ctl-0.3.1/oblv_ctl/models/role_response.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/service_content_response.py` & `oblv_ctl-0.3.1/oblv_ctl/models/service_content_response.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/service_validation_response.py` & `oblv_ctl-0.3.1/oblv_ctl/models/service_validation_response.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/service_yaml_add_input.py` & `oblv_ctl-0.3.1/oblv_ctl/models/service_yaml_add_input.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/service_yaml_update_input.py` & `oblv_ctl-0.3.1/oblv_ctl/models/service_yaml_update_input.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/shared_users.py` & `oblv_ctl-0.3.1/oblv_ctl/models/shared_users.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/supported_regions.py` & `oblv_ctl-0.3.1/oblv_ctl/models/supported_regions.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/user_credit_utilization.py` & `oblv_ctl-0.3.1/oblv_ctl/models/user_credit_utilization.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/user_password_input.py` & `oblv_ctl-0.3.1/oblv_ctl/models/user_password_input.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/user_profile_response.py` & `oblv_ctl-0.3.1/oblv_ctl/models/user_profile_response.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/user_service_list.py` & `oblv_ctl-0.3.1/oblv_ctl/models/user_service_list.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/user_services.py` & `oblv_ctl-0.3.1/oblv_ctl/models/user_services.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/validated_service.py` & `oblv_ctl-0.3.1/oblv_ctl/models/validated_service.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/validation_error.py` & `oblv_ctl-0.3.1/oblv_ctl/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/models/vcs_repo_response.py` & `oblv_ctl-0.3.1/oblv_ctl/models/vcs_repo_response.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/oblv_client.py` & `oblv_ctl-0.3.1/oblv_ctl/oblv_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,14 @@
             Response[Union[Any, HTTPValidationError, MessageModel]]
         """
         update_user_name_user_name_put.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             json_body=NameInput(name),
         )
-        print("Name updated successfully")
 
     @_method_wrapper
     def update_password(self, old_pass, new_pass):
         """Update User's Password
          API to update user's password
         Args:
             old_pass (str): Old Password
@@ -175,15 +174,14 @@
             Response[Union[None, HTTPValidationError, MessageModel]]
                 None is returned if successful
         """
         input = UserPasswordInput(old_password=old_pass, password=new_pass)
         update_user_password_user_password_put.sync(
             client=self, oblivious_user_id=self.oblivious_user_id, json_body=input
         )
-        print("Password updated successfully")
 
     @_method_wrapper
     def user_profile(self):
         """Get User Profile
          API to fetch user's profile details
         Returns:
             Response[Union[Any, HTTPValidationError, MessageModel, UserProfileResponse]]
@@ -326,23 +324,22 @@
             repo_owner (str): Repo's Owner Name
             repo_name (str): Repo Name
             ref (str): Service Ref
             ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
         Returns:
             Response[Union[Any, HTTPValidationError, MessageModel]]
         """
-        delete_repo_services_repo_service_delete.sync(
+        return delete_repo_services_repo_service_delete.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             ref=ref,
             ref_type=ref_type,
             repo_name=repo_name,
             repo_owner=repo_owner,
         )
-        print("Successfully removed service")
 
     @_method_wrapper
     def service_content(
         self, repo_owner: str, repo_name: str, ref: str, ref_type: str = "branch"
     ):
         """Get Repo Service Yaml
          API to fetch the service.yaml content as object for the given service.
```

### Comparing `oblv-ctl-0.3.0/oblv_ctl/types.py` & `oblv_ctl-0.3.1/oblv_ctl/types.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl/utils.py` & `oblv_ctl-0.3.1/oblv_ctl/utils.py`

 * *Files identical despite different names*

### Comparing `oblv-ctl-0.3.0/oblv_ctl.egg-info/PKG-INFO` & `oblv_ctl-0.3.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,231 +1,240 @@
-Metadata-Version: 2.1
-Name: oblv-ctl
-Version: 0.3.0
-Summary: A client library for accessing Oblivious APIs
-Home-page: https://github.com/ObliviousAI/oblv-ctl
-Author: Oblivious Support
-Author-email: support@oblivious.ai
-License: Apache-2.0
-Keywords: Oblivious,python,package
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# oblv-ctl
-
-A Python library to access Oblivious APIs.
-
-## Usage
-
-First, create a client, with your API key. This key can be created in the
-[Oblivious Console UI](https://console.oblivious.ai/). Go to the
-settings page, and create your ApiKey. Once done, the client can be
-created as follows
-
-``` {.python}
-from oblv import authenticate
-client = authenticate(apikey=*your_key_here*)
-```
-
-
-Using this client, all the Oblivious actions can be performed, including the deployment of enclaves. Below is a step-by-step guide, to creating your first deployment.
-
-
-
-### 1 Create a service
-
-A service refers to a branch/tag of your repository that needs to be
-deployed. For your first service. you can use the repository
-[ObliviousAI/FastAPI-Enclave-Services](https://github.com/ObliviousAI/FastAPI-Enclave-Services).
-Execute the below command to create the service.
-
-``` {.python}
-client.add_service(repo_owner="ObliviousAI",repo_name="FastAPI-Enclave-Services", ref="master", data = {
-    "auth": [
-        {
-            "auth_name": "auth_name",
-            "auth_type": "signed_headers"
-        }
-    ],
-    "base_image": "oblv_ubuntu_18_04_proxy_nsm_api_python_3_8",
-    "build_args": [],
-    "meta": {
-        "author": "Team Oblivious",
-        "author_email": "hello@oblivious.ai",
-        "git": "https://github.com/ObliviousAI/FastAPI-Enclave-Services.git",
-        "version": "0.1.0"
-    },
-    "paths": [
-        {
-            "access": "user",
-            "path": "/hello/",
-            "short_description": "Hello world example"
-        }
-    ],
-    "roles": [
-        {
-            "role_auth": "auth_name",
-            "role_cardinality": 1,
-            "role_description": "Role for the data scientist",
-            "role_name": "user"
-        }
-    ],
-    "traffic": {
-        "inbound": [
-            {
-                "name": "main_io",
-                "port": 80,
-                "type": "tcp"
-            }
-        ],
-        "outbound": [
-            {
-                "domain": "example.com",
-                "name": "example",
-                "port": 443,
-                "type": "tcp"
-            }
-        ]
-    }
-})
-```
-
-The data provided here is sample service data. You can update the data as per your requirements, adhering to the schema.
-The response for the call above gives results as follows - 
-
-
->{ \
->&nbsp;&nbsp;&nbsp;&nbsp;"message": "Success", \
->&nbsp;&nbsp;&nbsp;&nbsp;"service":&nbsp;&nbsp;&nbsp;&nbsp;{ \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"ref": "master", \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"service_validated": true, \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"sha": "6b1b3e9cf6b0cb7264aad2fc80d91a009ccf0fc1", \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"type": "branch" \
->&nbsp;&nbsp;&nbsp;&nbsp;} \
->} 
-
-
-You have now successfully created your first service, and it can be now deployed to an enclave.
-
-### 2 Enclave Creation
-
-To create an enclave, you need to decide on a few of the parameters -
-
--   **deployment_name** - A unique deployment name. You cannot have two
-    running deployments with the same name.
--   **region_name** - could be one of the AWS regions from
-    - ***us-east-1*** (N. Virginia) 
-    - ***us-west-2*** (Oregon)
-    - ***eu-central-1*** (Frankfurt)
-    - ***eu-west-2*** (London)
--   **visibility** - ***private*** or ***public***
--   **is_dev_env** - ***True*** or ***False***.
--   **tags** - A list of tags for your deployment
--   **account_type** - This is the VCS type, and only GitHub*** is
-    supported for now.
--   **build_args** - Arguments specific to your deployment. It includes adding users to their roles with their public keys, runtime arguments and
-    any additional arguments for your build. It also includes the infra
-    size needed for the deployment. The options are -
-    -   ***c5.xlarge*** - CPU:4 RAM:8 GB \-- Credit Utilization: 68.0/hr
-    -   ***m5.xlarge*** - CPU:4 RAM:16 GB \-- Credit Utilization:
-        76.8/hr
-    -   ***r5.xlarge*** - CPU:4 RAM:32 GB \-- Credit Utilization:
-        100.8/hr
-    -   ***c5.2xlarge*** - CPU:8 RAM:16 GB \-- Credit Utilization:
-        136.0/hr
-    -   ***m5.2xlarge*** - CPU:8 RAM:32 GB \-- Credit Utilization:
-        153.6/hr
-
-A valid example for *build_args* for the service you created -
-
-
-```
-args = {
-    "users": {
-      "admin": [
-        {
-          "user_name": "<your name>",
-          "public key": "<your public key>"
-        }
-      ]
-    },
-    "infra_reqs": "m5.xlarge",  
-}
-
-```
-
-> 📝 **Note:**
->
-> <b>admin</b> here
-> is the role defined for the deployment in service.yaml
-> file
->
-> The service used,
-> does not have requirements for any runtime or build arguments, so not
-> needed here.
-
-``` {.python}
-from oblv.models import CreateDeploymentInput
-input = CreateDeploymentInput(
-    owner="ObliviousAI",
-    repo="FastAPI-Enclave-Services",
-    account_type="github",
-    ref="master",
-    ref_type="branch",
-    region_name="us-east-1",
-    deployment_name="Depl",
-    visibility="private",
-    is_dev_env=True,
-    tags=[],
-    build_args=args
-)
-response = client.create_deployment(input)
-```
-
-
-On successful request, enclave creation is initiated, and it returns an
-id for the deployment, which can be later used to track the status and
-connection details for the enclave.
-
-To check the state of the deployment, run
-
-``` {.python}
-client.deployment_info(response.deployment_id).current_state
-```
-
-> 'CFT Initiated'
-
-
-When the deployment state becomes ***Running***, it indicates that the
-enclave is now available for connection.
-
-To connect to the enclave, you need **Oblv CLI** installed in your
-system. The commands to use the CLI can be found in this
-[documentation](https://docs.oblivious.ai/cli/usage_examples).
-
-Cli binaries can be found [here](https://docs.oblivious.ai/cli/binaries)
-
-The URL to connect to the enclave using CLI can be accessed using
-
-``` {.python}
-client.deployment_info(response.deployment_id).instance.service_url
-```
-
->
->'https://conso-appli-15aiaxip9pcxk-94364694.enclave.oblivious.ai'
->
-
-
-The PCR codes can be found using
-
-``` {.python}
-client.deployment_info(response.deployment_id).pcr_codes
-```
-
->['d8dd856bacf4a8f0840ab530579b906091803e818e01dc4b8f51c247a7adfcfe55b4ef5f17be6d53bb952d92d87a376c',
-'bcdf05fefccaa8e55bf2c8d6dee9e79bbff31e34bf28a99aa19e6b29c37ee80b214a414b7607236edf26fcb78654e63f','79477bad9504a347afb557a8ccd6f62ea61243311dff39f66944f5150242128da0cd070f0ce629c6beb6bb4f0b52f5ed' ]
+Metadata-Version: 2.1
+Name: oblv-ctl
+Version: 0.3.1
+Summary: A client library for accessing Oblivious APIs
+Home-page: https://github.com/ObliviousAI/oblv-ctl/tree/master/README.md
+License: Apache-2.0
+Keywords: Oblivious,python,package
+Author: Oblivious Support
+Author-email: support@oblivious.ai
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: check-jsonschema (==0.22.0)
+Requires-Dist: httpx (==0.15.0)
+Requires-Dist: python-dateutil (==2.8.2)
+Requires-Dist: requests (==2.29.0)
+Requires-Dist: rich (>=11.1,<11.2)
+Requires-Dist: typer (==0.7.0)
+Project-URL: Repository, https://github.com/ObliviousAI/oblv-ctl
+Description-Content-Type: text/markdown
+
+# oblv-ctl
+
+A Python library to access Oblivious APIs.
+
+## Usage
+
+First, create a client, with your API key. This key can be created in the
+[Oblivious Console UI](https://console.oblivious.ai/). Go to the
+settings page, and create your ApiKey. Once done, the client can be
+created as follows
+
+``` {.python}
+from oblv_ctl import authenticate
+client = authenticate(apikey=*your_key_here*)
+```
+
+
+Using this client, all the Oblivious actions can be performed, including the deployment of enclaves. Below is a step-by-step guide, to creating your first deployment.
+
+
+
+### 1 Create a service
+
+A service refers to a branch/tag of your repository that needs to be
+deployed. For your first service. you can use the repository
+[ObliviousAI/FastAPI-Enclave-Services](https://github.com/ObliviousAI/FastAPI-Enclave-Services).
+Execute the below command to create the service.
+
+``` {.python}
+client.add_service(repo_owner="ObliviousAI",repo_name="FastAPI-Enclave-Services", ref="master", data = {
+    "auth": [
+        {
+            "auth_name": "auth_name",
+            "auth_type": "signed_headers"
+        }
+    ],
+    "base_image": "oblv_ubuntu_18_04_proxy_nsm_api_python_3_8",
+    "build_args": [],
+    "meta": {
+        "author": "Team Oblivious",
+        "author_email": "hello@oblivious.ai",
+        "git": "https://github.com/ObliviousAI/FastAPI-Enclave-Services.git",
+        "version": "0.1.0"
+    },
+    "paths": [
+        {
+            "access": "user",
+            "path": "/hello/",
+            "short_description": "Hello world example"
+        }
+    ],
+    "roles": [
+        {
+            "role_auth": "auth_name",
+            "role_cardinality": 1,
+            "role_description": "Role for the data scientist",
+            "role_name": "user"
+        }
+    ],
+    "traffic": {
+        "inbound": [
+            {
+                "name": "main_io",
+                "port": 80,
+                "type": "tcp"
+            }
+        ],
+        "outbound": [
+            {
+                "domain": "example.com",
+                "name": "example",
+                "port": 443,
+                "type": "tcp"
+            }
+        ]
+    }
+})
+```
+
+The data provided here is sample service data. You can update the data as per your requirements, adhering to the schema.
+The response for the call above gives results as follows - 
+
+
+>{ \
+>&nbsp;&nbsp;&nbsp;&nbsp;"message": "Success", \
+>&nbsp;&nbsp;&nbsp;&nbsp;"service":&nbsp;&nbsp;&nbsp;&nbsp;{ \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"ref": "master", \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"service_validated": true, \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"sha": "6b1b3e9cf6b0cb7264aad2fc80d91a009ccf0fc1", \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"type": "branch" \
+>&nbsp;&nbsp;&nbsp;&nbsp;} \
+>} 
+
+
+You have now successfully created your first service, and it can be now deployed to an enclave.
+
+### 2 Enclave Creation
+
+To create an enclave, you need to decide on a few of the parameters -
+
+-   **deployment_name** - A unique deployment name. You cannot have two
+    running deployments with the same name.
+-   **region_name** - could be one of the AWS regions from
+    - ***us-east-1*** (N. Virginia) 
+    - ***us-west-2*** (Oregon)
+    - ***eu-central-1*** (Frankfurt)
+    - ***eu-west-2*** (London)
+-   **visibility** - ***private*** or ***public***
+-   **is_dev_env** - ***True*** or ***False***.
+-   **tags** - A list of tags for your deployment
+-   **account_type** - This is the VCS type, and only GitHub*** is
+    supported for now.
+-   **build_args** - Arguments specific to your deployment. It includes adding users to their roles with their public keys, runtime arguments and
+    any additional arguments for your build. It also includes the infra
+    size needed for the deployment. The options are -
+    -   ***c5.xlarge*** - CPU:4 RAM:8 GB \-- Credit Utilization: 68.0/hr
+    -   ***m5.xlarge*** - CPU:4 RAM:16 GB \-- Credit Utilization:
+        76.8/hr
+    -   ***r5.xlarge*** - CPU:4 RAM:32 GB \-- Credit Utilization:
+        100.8/hr
+    -   ***c5.2xlarge*** - CPU:8 RAM:16 GB \-- Credit Utilization:
+        136.0/hr
+    -   ***m5.2xlarge*** - CPU:8 RAM:32 GB \-- Credit Utilization:
+        153.6/hr
+
+A valid example for *build_args* for the service you created -
+
+
+```
+args = {
+    "users": {
+      "admin": [
+        {
+          "user_name": "<your name>",
+          "public key": "<your public key>"
+        }
+      ]
+    },
+    "infra_reqs": "m5.xlarge",  
+}
+
+```
+
+> 📝 **Note:**
+>
+> <b>admin</b> here
+> is the role defined for the deployment in service.yaml
+> file
+>
+> The service used,
+> does not have requirements for any runtime or build arguments, so not
+> needed here.
+
+``` {.python}
+from oblv_ctl.models import CreateDeploymentInput
+input = CreateDeploymentInput(
+    owner="ObliviousAI",
+    repo="FastAPI-Enclave-Services",
+    account_type="github",
+    ref="master",
+    ref_type="branch",
+    region_name="us-east-1",
+    deployment_name="Depl",
+    visibility="private",
+    is_dev_env=True,
+    tags=[],
+    build_args=args
+)
+response = client.create_deployment(input)
+```
+
+
+On successful request, enclave creation is initiated, and it returns an
+id for the deployment, which can be later used to track the status and
+connection details for the enclave.
+
+To check the state of the deployment, run
+
+``` {.python}
+client.deployment_info(response.deployment_id).current_state
+```
+
+> 'CFT Initiated'
+
+
+When the deployment state becomes ***Running***, it indicates that the
+enclave is now available for connection.
+
+To connect to the enclave, you need **Oblv CLI** installed in your
+system. The commands to use the CLI can be found in this
+[documentation](https://docs.oblivious.ai/cli/usage_examples).
+
+Cli binaries can be found [here](https://docs.oblivious.ai/cli/binaries)
+
+The URL to connect to the enclave using CLI can be accessed using
+
+``` {.python}
+client.deployment_info(response.deployment_id).instance.service_url
+```
+
+>
+>'https://conso-appli-15aiaxip9pcxk-94364694.enclave.oblivious.ai'
+>
+
+
+The PCR codes can be found using
+
+``` {.python}
+client.deployment_info(response.deployment_id).pcr_codes
+```
+
+>['d8dd856bacf4a8f0840ab530579b906091803e818e01dc4b8f51c247a7adfcfe55b4ef5f17be6d53bb952d92d87a376c',
+'bcdf05fefccaa8e55bf2c8d6dee9e79bbff31e34bf28a99aa19e6b29c37ee80b214a414b7607236edf26fcb78654e63f','79477bad9504a347afb557a8ccd6f62ea61243311dff39f66944f5150242128da0cd070f0ce629c6beb6bb4f0b52f5ed' ]
+
```

### Comparing `oblv-ctl-0.3.0/pyproject.toml` & `oblv_ctl-0.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools >= 58.0.4", "wheel >= 0.37.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "oblv-ctl"
-version = "0.3.0"
+version = "0.3.1"
 description = "A client library for accessing Oblivious APIs"
 authors = ["Oblivious Support <support@oblivious.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/ObliviousAI/oblv-ctl"
 homepage = "https://github.com/ObliviousAI/oblv-ctl/tree/master/README.md"
 keywords = ["Oblivious", "python", "package"]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 httpx = "0.15.0"
-python-dateutil = "2.8.0"
+python-dateutil = "2.8.2"
 typer = "0.7.0"
-rich = "13.3.4"
+rich = "~11.1"
 requests = "2.29.0"
 check-jsonschema = "0.22.0"
 
 [tool.poetry.scripts]
 oblv-ctl = "oblv_ctl.cli.main:app"
```

