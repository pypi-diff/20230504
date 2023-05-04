# Comparing `tmp/kittycad-0.3.8.tar.gz` & `tmp/kittycad-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kittycad-0.3.8.tar", max compression
+gzip compressed data, was "kittycad-0.3.9.tar", max compression
```

## Comparing `kittycad-0.3.8.tar` & `kittycad-0.3.9.tar`

### file list

```diff
@@ -1,272 +1,271 @@
--rw-r--r--   0        0        0     1065 2023-05-04 07:58:53.116393 kittycad-0.3.8/LICENSE
--rw-r--r--   0        0        0      875 2023-05-04 07:58:53.116393 kittycad-0.3.8/README.md
--rw-r--r--   0        0        0       48 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/__init__.py
--rw-r--r--   0        0        0       47 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/__init__.py
--rw-r--r--   0        0        0      119 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/ai/__init__.py
--rw-r--r--   0        0        0     3747 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/ai/create_image_to_3d.py
--rw-r--r--   0        0        0     3525 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/ai/create_text_to_3d.py
--rw-r--r--   0        0        0      199 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/__init__.py
--rw-r--r--   0        0        0     3082 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/get_api_call.py
--rw-r--r--   0        0        0     2771 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/get_api_call_for_user.py
--rw-r--r--   0        0        0     3215 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/get_api_call_metrics.py
--rw-r--r--   0        0        0     6031 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/get_async_operation.py
--rw-r--r--   0        0        0     4208 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/list_api_calls.py
--rw-r--r--   0        0        0     4977 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/list_api_calls_for_user.py
--rw-r--r--   0        0        0     4787 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/list_async_operations.py
--rw-r--r--   0        0        0     4323 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/user_list_api_calls.py
--rw-r--r--   0        0        0      352 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_tokens/__init__.py
--rw-r--r--   0        0        0     2551 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_tokens/create_api_token_for_user.py
--rw-r--r--   0        0        0     2976 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_tokens/delete_api_token_for_user.py
--rw-r--r--   0        0        0     2762 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_tokens/get_api_token_for_user.py
--rw-r--r--   0        0        0     4256 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_tokens/list_api_tokens_for_user.py
--rw-r--r--   0        0        0      116 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/apps/__init__.py
--rw-r--r--   0        0        0     2694 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/apps/apps_github_callback.py
--rw-r--r--   0        0        0     2883 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/apps/apps_github_consent.py
--rw-r--r--   0        0        0     2435 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/apps/apps_github_webhook.py
--rw-r--r--   0        0        0      156 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/beta/__init__.py
--rw-r--r--   0        0        0      118 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/constant/__init__.py
--rw-r--r--   0        0        0     2730 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/constant/get_physics_constant.py
--rw-r--r--   0        0        0      142 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/drawing/__init__.py
--rw-r--r--   0        0        0     2752 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/drawing/cmd.py
--rw-r--r--   0        0        0     2656 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/drawing/cmd_batch.py
--rw-r--r--   0        0        0      161 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/executor/__init__.py
--rw-r--r--   0        0        0     1930 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/executor/create_executor_term.py
--rw-r--r--   0        0        0     3173 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/executor/create_file_execution.py
--rw-r--r--   0        0        0      233 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/__init__.py
--rw-r--r--   0        0        0     3843 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/create_file_center_of_mass.py
--rw-r--r--   0        0        0     4433 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/create_file_conversion.py
--rw-r--r--   0        0        0     1962 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/create_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0     4254 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/create_file_density.py
--rw-r--r--   0        0        0     4272 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/create_file_mass.py
--rw-r--r--   0        0        0     3827 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/create_file_surface_area.py
--rw-r--r--   0        0        0     3763 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/create_file_volume.py
--rw-r--r--   0        0        0     1341 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/get_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0      133 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/hidden/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/hidden/auth_email.py
--rw-r--r--   0        0        0     3317 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/hidden/auth_email_callback.py
--rw-r--r--   0        0        0     2236 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/hidden/logout.py
--rw-r--r--   0        0        0      105 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/meta/__init__.py
--rw-r--r--   0        0        0     2355 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/meta/get_ai_plugin_manifest.py
--rw-r--r--   0        0        0     2607 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/meta/get_metadata.py
--rw-r--r--   0        0        0     1913 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/meta/get_metrics.py
--rw-r--r--   0        0        0     2530 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/meta/get_openai_schema.py
--rw-r--r--   0        0        0     2159 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/meta/get_schema.py
--rw-r--r--   0        0        0     2211 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/meta/ping.py
--rw-r--r--   0        0        0      123 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/oauth2/__init__.py
--rw-r--r--   0        0        0      117 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/__init__.py
--rw-r--r--   0        0        0     2934 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/create_payment_information_for_user.py
--rw-r--r--   0        0        0     2610 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/create_payment_intent_for_user.py
--rw-r--r--   0        0        0     2528 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/delete_payment_information_for_user.py
--rw-r--r--   0        0        0     2583 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/delete_payment_method_for_user.py
--rw-r--r--   0        0        0     2627 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/get_payment_balance_for_user.py
--rw-r--r--   0        0        0     2659 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/get_payment_information_for_user.py
--rw-r--r--   0        0        0     2588 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/list_invoices_for_user.py
--rw-r--r--   0        0        0     2656 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/list_payment_methods_for_user.py
--rw-r--r--   0        0        0     2932 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/update_payment_information_for_user.py
--rw-r--r--   0        0        0     2580 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/validate_customer_tax_information_for_user.py
--rw-r--r--   0        0        0      101 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/unit/__init__.py
--rw-r--r--   0        0        0     3938 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/unit/get_acceleration_unit_conversion.py
--rw-r--r--   0        0        0     3756 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/unit/get_angle_unit_conversion.py
--rw-r--r--   0        0        0     4023 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_angular_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3730 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_area_unit_conversion.py
--rw-r--r--   0        0        0     3780 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_charge_unit_conversion.py
--rw-r--r--   0        0        0     3962 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_concentration_unit_conversion.py
--rw-r--r--   0        0        0     4054 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py
--rw-r--r--   0        0        0     3728 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_data_unit_conversion.py
--rw-r--r--   0        0        0     3806 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_density_unit_conversion.py
--rw-r--r--   0        0        0     3780 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_energy_unit_conversion.py
--rw-r--r--   0        0        0     3754 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_force_unit_conversion.py
--rw-r--r--   0        0        0     3910 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_illuminance_unit_conversion.py
--rw-r--r--   0        0        0     3780 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_length_unit_conversion.py
--rw-r--r--   0        0        0     4202 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py
--rw-r--r--   0        0        0     3943 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_magnetic_flux_unit_conversion.py
--rw-r--r--   0        0        0     3728 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_mass_unit_conversion.py
--rw-r--r--   0        0        0     3890 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py
--rw-r--r--   0        0        0     3927 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_metric_power_squared_unit_conversion.py
--rw-r--r--   0        0        0     3820 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_metric_power_unit_conversion.py
--rw-r--r--   0        0        0     3754 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_power_unit_conversion.py
--rw-r--r--   0        0        0     3832 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_pressure_unit_conversion.py
--rw-r--r--   0        0        0     3858 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_radiation_unit_conversion.py
--rw-r--r--   0        0        0     3962 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_radioactivity_unit_conversion.py
--rw-r--r--   0        0        0     3891 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_solid_angle_unit_conversion.py
--rw-r--r--   0        0        0     3910 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_temperature_unit_conversion.py
--rw-r--r--   0        0        0     3728 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_time_unit_conversion.py
--rw-r--r--   0        0        0     3832 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3806 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_voltage_unit_conversion.py
--rw-r--r--   0        0        0     3780 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_volume_unit_conversion.py
--rw-r--r--   0        0        0      297 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/__init__.py
--rw-r--r--   0        0        0     2676 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/delete_user_self.py
--rw-r--r--   0        0        0     2735 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/get_session_for_user.py
--rw-r--r--   0        0        0     3027 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/get_user.py
--rw-r--r--   0        0        0     3157 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/get_user_extended.py
--rw-r--r--   0        0        0     2446 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/get_user_front_hash_self.py
--rw-r--r--   0        0        0     2484 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/get_user_onboarding_self.py
--rw-r--r--   0        0        0     2489 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/get_user_self.py
--rw-r--r--   0        0        0     2601 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/get_user_self_extended.py
--rw-r--r--   0        0        0     4077 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/list_users.py
--rw-r--r--   0        0        0     4159 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/list_users_extended.py
--rw-r--r--   0        0        0     2745 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/update_user_self.py
--rw-r--r--   0        0        0     2297 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/client.py
--rw-r--r--   0        0        0     4725 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/client_test.py
--rw-r--r--   0        0        0    87053 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/examples_test.py
--rw-r--r--   0        0        0     7838 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/__init__.py
--rw-r--r--   0        0        0      322 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/account_provider.py
--rw-r--r--   0        0        0     2249 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/ai_plugin_api.py
--rw-r--r--   0        0        0      242 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/ai_plugin_api_type.py
--rw-r--r--   0        0        0     2440 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/ai_plugin_auth.py
--rw-r--r--   0        0        0      413 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/ai_plugin_auth_type.py
--rw-r--r--   0        0        0      287 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/ai_plugin_http_auth_type.py
--rw-r--r--   0        0        0     4685 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/ai_plugin_manifest.py
--rw-r--r--   0        0        0     1720 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/api_call_query_group.py
--rw-r--r--   0        0        0      777 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/api_call_query_group_by.py
--rw-r--r--   0        0        0      620 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/api_call_status.py
--rw-r--r--   0        0        0     8266 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/api_call_with_price.py
--rw-r--r--   0        0        0     2128 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/api_call_with_price_results_page.py
--rw-r--r--   0        0        0     3278 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/api_token.py
--rw-r--r--   0        0        0     2004 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/api_token_results_page.py
--rw-r--r--   0        0        0     1447 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/app_client_info.py
--rw-r--r--   0        0        0     5747 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/async_api_call.py
--rw-r--r--   0        0        0    34040 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/async_api_call_output.py
--rw-r--r--   0        0        0     2066 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/async_api_call_results_page.py
--rw-r--r--   0        0        0      648 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/async_api_call_type.py
--rw-r--r--   0        0        0     2127 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/billing_info.py
--rw-r--r--   0        0        0     1479 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/cache_metadata.py
--rw-r--r--   0        0        0     3353 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/card_details.py
--rw-r--r--   0        0        0     2697 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/cluster.py
--rw-r--r--   0        0        0      229 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/code_language.py
--rw-r--r--   0        0        0     2244 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/code_output.py
--rw-r--r--   0        0        0     1732 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/commit.py
--rw-r--r--   0        0        0    14343 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/connection.py
--rw-r--r--   0        0        0    13513 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/country_code.py
--rw-r--r--   0        0        0      507 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/created_at_sort_mode.py
--rw-r--r--   0        0        0     8623 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/currency.py
--rw-r--r--   0        0        0     4298 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/customer.py
--rw-r--r--   0        0        0     4306 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/customer_balance.py
--rw-r--r--   0        0        0     2412 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/device_access_token_request_form.py
--rw-r--r--   0        0        0     1580 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/device_auth_request_form.py
--rw-r--r--   0        0        0     1606 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/device_auth_verify_params.py
--rw-r--r--   0        0        0    21264 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/docker_system_info.py
--rw-r--r--   0        0        0     3553 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/drawing_cmd.py
--rw-r--r--   0        0        0       75 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/drawing_cmd_id.py
--rw-r--r--   0        0        0     2441 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/drawing_cmd_req.py
--rw-r--r--   0        0        0     1746 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/drawing_cmd_req_batch.py
--rw-r--r--   0        0        0     2393 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/drawing_error.py
--rw-r--r--   0        0        0     1869 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/drawing_outcome.py
--rw-r--r--   0        0        0     1505 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/drawing_outcomes.py
--rw-r--r--   0        0        0     1789 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/email_authentication_form.py
--rw-r--r--   0        0        0     3847 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/engine_metadata.py
--rw-r--r--   0        0        0      269 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/environment.py
--rw-r--r--   0        0        0     1930 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/error.py
--rw-r--r--   0        0        0     2715 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/executor_metadata.py
--rw-r--r--   0        0        0     6069 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/extended_user.py
--rw-r--r--   0        0        0     2060 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/extended_user_results_page.py
--rw-r--r--   0        0        0     5700 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_center_of_mass.py
--rw-r--r--   0        0        0     6060 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_conversion.py
--rw-r--r--   0        0        0     5725 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_density.py
--rw-r--r--   0        0        0     1369 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_export_format.py
--rw-r--r--   0        0        0     1306 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_import_format.py
--rw-r--r--   0        0        0     5707 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_mass.py
--rw-r--r--   0        0        0     5522 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_surface_area.py
--rw-r--r--   0        0        0     1513 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_system_metadata.py
--rw-r--r--   0        0        0     5428 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_volume.py
--rw-r--r--   0        0        0     2304 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/gateway.py
--rw-r--r--   0        0        0      187 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/image_type.py
--rw-r--r--   0        0        0     2228 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/index_info.py
--rw-r--r--   0        0        0     8273 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/invoice.py
--rw-r--r--   0        0        0     2888 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/invoice_line_item.py
--rw-r--r--   0        0        0      563 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/invoice_status.py
--rw-r--r--   0        0        0     2666 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/jetstream.py
--rw-r--r--   0        0        0     1907 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/jetstream_api_stats.py
--rw-r--r--   0        0        0     2212 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/jetstream_config.py
--rw-r--r--   0        0        0     3174 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/jetstream_stats.py
--rw-r--r--   0        0        0     2125 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/leaf_node.py
--rw-r--r--   0        0        0     1337 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/mesh.py
--rw-r--r--   0        0        0     1923 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/meta_cluster_info.py
--rw-r--r--   0        0        0     5025 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/metadata.py
--rw-r--r--   0        0        0     1788 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/method.py
--rw-r--r--   0        0        0     3081 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/new_address.py
--rw-r--r--   0        0        0     2038 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/o_auth2_client_info.py
--rw-r--r--   0        0        0      415 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/o_auth2_grant_type.py
--rw-r--r--   0        0        0     2501 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/onboarding.py
--rw-r--r--   0        0        0     1646 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/output_file.py
--rw-r--r--   0        0        0     1527 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/payment_intent.py
--rw-r--r--   0        0        0     3753 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/payment_method.py
--rw-r--r--   0        0        0     2267 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/payment_method_card_checks.py
--rw-r--r--   0        0        0      294 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/payment_method_type.py
--rw-r--r--   0        0        0     5424 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/physics_constant.py
--rw-r--r--   0        0        0     4448 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/physics_constant_name.py
--rw-r--r--   0        0        0     2809 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/plugins_info.py
--rw-r--r--   0        0        0     1498 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/point_e_metadata.py
--rw-r--r--   0        0        0     1432 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/pong.py
--rw-r--r--   0        0        0     4187 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/registry_service_config.py
--rw-r--r--   0        0        0     2034 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/runtime.py
--rw-r--r--   0        0        0     3638 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/session.py
--rw-r--r--   0        0        0      214 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/system_info_cgroup_driver_enum.py
--rw-r--r--   0        0        0      175 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/system_info_cgroup_version_enum.py
--rw-r--r--   0        0        0     1663 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/system_info_default_address_pools.py
--rw-r--r--   0        0        0      213 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/system_info_isolation_enum.py
--rw-r--r--   0        0        0     6317 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_acceleration_conversion.py
--rw-r--r--   0        0        0      642 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_acceleration_format.py
--rw-r--r--   0        0        0     6226 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_angle_conversion.py
--rw-r--r--   0        0        0      916 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_angle_format.py
--rw-r--r--   0        0        0     6360 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_angular_velocity_conversion.py
--rw-r--r--   0        0        0      754 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_angular_velocity_format.py
--rw-r--r--   0        0        0     6213 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_area_conversion.py
--rw-r--r--   0        0        0      888 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_area_format.py
--rw-r--r--   0        0        0     6239 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_charge_conversion.py
--rw-r--r--   0        0        0      380 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_charge_format.py
--rw-r--r--   0        0        0     6330 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_concentration_conversion.py
--rw-r--r--   0        0        0      752 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_concentration_format.py
--rw-r--r--   0        0        0     6213 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_data_conversion.py
--rw-r--r--   0        0        0      539 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_data_format.py
--rw-r--r--   0        0        0     6377 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_data_transfer_rate_conversion.py
--rw-r--r--   0        0        0      656 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_data_transfer_rate_format.py
--rw-r--r--   0        0        0     6252 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_density_conversion.py
--rw-r--r--   0        0        0     1488 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_density_format.py
--rw-r--r--   0        0        0     6239 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_energy_conversion.py
--rw-r--r--   0        0        0     1162 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_energy_format.py
--rw-r--r--   0        0        0     6226 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_force_conversion.py
--rw-r--r--   0        0        0      645 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_force_format.py
--rw-r--r--   0        0        0     6304 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_illuminance_conversion.py
--rw-r--r--   0        0        0      584 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_illuminance_format.py
--rw-r--r--   0        0        0     6239 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_length_conversion.py
--rw-r--r--   0        0        0     2187 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_length_format.py
--rw-r--r--   0        0        0     6442 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_magnetic_field_strength_conversion.py
--rw-r--r--   0        0        0      402 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_magnetic_field_strength_format.py
--rw-r--r--   0        0        0     6321 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_magnetic_flux_conversion.py
--rw-r--r--   0        0        0      389 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_magnetic_flux_format.py
--rw-r--r--   0        0        0     6213 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_mass_conversion.py
--rw-r--r--   0        0        0     1094 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_mass_format.py
--rw-r--r--   0        0        0     3438 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_metric_power.py
--rw-r--r--   0        0        0     6259 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_metric_power_conversion.py
--rw-r--r--   0        0        0     6287 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_metric_power_cubed_conversion.py
--rw-r--r--   0        0        0     6297 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_metric_power_squared_conversion.py
--rw-r--r--   0        0        0     6226 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_power_conversion.py
--rw-r--r--   0        0        0      468 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_power_format.py
--rw-r--r--   0        0        0     6265 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_pressure_conversion.py
--rw-r--r--   0        0        0      725 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_pressure_format.py
--rw-r--r--   0        0        0     6278 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_radiation_conversion.py
--rw-r--r--   0        0        0      586 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_radiation_format.py
--rw-r--r--   0        0        0     6330 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_radioactivity_conversion.py
--rw-r--r--   0        0        0      570 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_radioactivity_format.py
--rw-r--r--   0        0        0     6295 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_solid_angle_conversion.py
--rw-r--r--   0        0        0      500 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_solid_angle_format.py
--rw-r--r--   0        0        0     6304 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_temperature_conversion.py
--rw-r--r--   0        0        0      674 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_temperature_format.py
--rw-r--r--   0        0        0     6213 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_time_conversion.py
--rw-r--r--   0        0        0      902 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_time_format.py
--rw-r--r--   0        0        0     6265 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_velocity_conversion.py
--rw-r--r--   0        0        0      753 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_velocity_format.py
--rw-r--r--   0        0        0     6252 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_voltage_conversion.py
--rw-r--r--   0        0        0      452 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_voltage_format.py
--rw-r--r--   0        0        0     6239 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_volume_conversion.py
--rw-r--r--   0        0        0     3286 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_volume_format.py
--rw-r--r--   0        0        0     2577 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/update_user.py
--rw-r--r--   0        0        0     5084 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/user.py
--rw-r--r--   0        0        0     1942 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/user_results_page.py
--rw-r--r--   0        0        0       67 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/uuid.py
--rw-r--r--   0        0        0     3448 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/verification_token.py
--rw-r--r--   0        0        0       26 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/py.typed
--rw-r--r--   0        0        0     1049 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/types.py
--rw-r--r--   0        0        0     2416 2023-05-04 07:58:53.412392 kittycad-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 kittycad-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-04 08:24:50.530608 kittycad-0.3.9/LICENSE
+-rw-r--r--   0        0        0      875 2023-05-04 08:24:50.530608 kittycad-0.3.9/README.md
+-rw-r--r--   0        0        0       48 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/ai/__init__.py
+-rw-r--r--   0        0        0     3747 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/ai/create_image_to_3d.py
+-rw-r--r--   0        0        0     3525 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/ai/create_text_to_3d.py
+-rw-r--r--   0        0        0      199 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/__init__.py
+-rw-r--r--   0        0        0     3082 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/get_api_call.py
+-rw-r--r--   0        0        0     2771 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/get_api_call_for_user.py
+-rw-r--r--   0        0        0     3215 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/get_api_call_metrics.py
+-rw-r--r--   0        0        0     6031 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/get_async_operation.py
+-rw-r--r--   0        0        0     4208 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/list_api_calls.py
+-rw-r--r--   0        0        0     4977 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/list_api_calls_for_user.py
+-rw-r--r--   0        0        0     4787 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/list_async_operations.py
+-rw-r--r--   0        0        0     4323 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_calls/user_list_api_calls.py
+-rw-r--r--   0        0        0      352 2023-05-04 08:24:50.946632 kittycad-0.3.9/kittycad/api/api_tokens/__init__.py
+-rw-r--r--   0        0        0     2551 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/api_tokens/create_api_token_for_user.py
+-rw-r--r--   0        0        0     2976 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/api_tokens/delete_api_token_for_user.py
+-rw-r--r--   0        0        0     2762 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/api_tokens/get_api_token_for_user.py
+-rw-r--r--   0        0        0     4256 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/api_tokens/list_api_tokens_for_user.py
+-rw-r--r--   0        0        0      116 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/apps/__init__.py
+-rw-r--r--   0        0        0     2694 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/apps/apps_github_callback.py
+-rw-r--r--   0        0        0     2883 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/apps/apps_github_consent.py
+-rw-r--r--   0        0        0     2435 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/apps/apps_github_webhook.py
+-rw-r--r--   0        0        0      156 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/beta/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/constant/__init__.py
+-rw-r--r--   0        0        0     2730 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/constant/get_physics_constant.py
+-rw-r--r--   0        0        0      142 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/drawing/__init__.py
+-rw-r--r--   0        0        0     2752 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/drawing/cmd.py
+-rw-r--r--   0        0        0     2656 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/drawing/cmd_batch.py
+-rw-r--r--   0        0        0      161 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/executor/__init__.py
+-rw-r--r--   0        0        0     1930 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/executor/create_executor_term.py
+-rw-r--r--   0        0        0     3173 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/executor/create_file_execution.py
+-rw-r--r--   0        0        0      233 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/__init__.py
+-rw-r--r--   0        0        0     3843 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/create_file_center_of_mass.py
+-rw-r--r--   0        0        0     4433 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/create_file_conversion.py
+-rw-r--r--   0        0        0     1962 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/create_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0     4254 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/create_file_density.py
+-rw-r--r--   0        0        0     4272 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/create_file_mass.py
+-rw-r--r--   0        0        0     3827 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/create_file_surface_area.py
+-rw-r--r--   0        0        0     3763 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/create_file_volume.py
+-rw-r--r--   0        0        0     1341 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/file/get_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0      133 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/hidden/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/hidden/auth_email.py
+-rw-r--r--   0        0        0     3317 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/hidden/auth_email_callback.py
+-rw-r--r--   0        0        0     2236 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/hidden/logout.py
+-rw-r--r--   0        0        0      105 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/meta/__init__.py
+-rw-r--r--   0        0        0     2355 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/meta/get_ai_plugin_manifest.py
+-rw-r--r--   0        0        0     2607 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/meta/get_metadata.py
+-rw-r--r--   0        0        0     2530 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/meta/get_openai_schema.py
+-rw-r--r--   0        0        0     2159 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/meta/get_schema.py
+-rw-r--r--   0        0        0     2211 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/meta/ping.py
+-rw-r--r--   0        0        0      123 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/oauth2/__init__.py
+-rw-r--r--   0        0        0      117 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/__init__.py
+-rw-r--r--   0        0        0     2934 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/create_payment_information_for_user.py
+-rw-r--r--   0        0        0     2610 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/create_payment_intent_for_user.py
+-rw-r--r--   0        0        0     2528 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/delete_payment_information_for_user.py
+-rw-r--r--   0        0        0     2583 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/delete_payment_method_for_user.py
+-rw-r--r--   0        0        0     2627 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/get_payment_balance_for_user.py
+-rw-r--r--   0        0        0     2659 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/get_payment_information_for_user.py
+-rw-r--r--   0        0        0     2588 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/list_invoices_for_user.py
+-rw-r--r--   0        0        0     2656 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/list_payment_methods_for_user.py
+-rw-r--r--   0        0        0     2932 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/update_payment_information_for_user.py
+-rw-r--r--   0        0        0     2580 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/payments/validate_customer_tax_information_for_user.py
+-rw-r--r--   0        0        0      101 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/__init__.py
+-rw-r--r--   0        0        0     3938 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_acceleration_unit_conversion.py
+-rw-r--r--   0        0        0     3756 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_angle_unit_conversion.py
+-rw-r--r--   0        0        0     4023 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_angular_velocity_unit_conversion.py
+-rw-r--r--   0        0        0     3730 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_area_unit_conversion.py
+-rw-r--r--   0        0        0     3780 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_charge_unit_conversion.py
+-rw-r--r--   0        0        0     3962 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_concentration_unit_conversion.py
+-rw-r--r--   0        0        0     4054 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py
+-rw-r--r--   0        0        0     3728 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_data_unit_conversion.py
+-rw-r--r--   0        0        0     3806 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_density_unit_conversion.py
+-rw-r--r--   0        0        0     3780 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_energy_unit_conversion.py
+-rw-r--r--   0        0        0     3754 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_force_unit_conversion.py
+-rw-r--r--   0        0        0     3910 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_illuminance_unit_conversion.py
+-rw-r--r--   0        0        0     3780 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_length_unit_conversion.py
+-rw-r--r--   0        0        0     4202 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py
+-rw-r--r--   0        0        0     3943 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_magnetic_flux_unit_conversion.py
+-rw-r--r--   0        0        0     3728 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_mass_unit_conversion.py
+-rw-r--r--   0        0        0     3890 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py
+-rw-r--r--   0        0        0     3927 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_metric_power_squared_unit_conversion.py
+-rw-r--r--   0        0        0     3820 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_metric_power_unit_conversion.py
+-rw-r--r--   0        0        0     3754 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_power_unit_conversion.py
+-rw-r--r--   0        0        0     3832 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_pressure_unit_conversion.py
+-rw-r--r--   0        0        0     3858 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_radiation_unit_conversion.py
+-rw-r--r--   0        0        0     3962 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_radioactivity_unit_conversion.py
+-rw-r--r--   0        0        0     3891 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_solid_angle_unit_conversion.py
+-rw-r--r--   0        0        0     3910 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_temperature_unit_conversion.py
+-rw-r--r--   0        0        0     3728 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_time_unit_conversion.py
+-rw-r--r--   0        0        0     3832 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_velocity_unit_conversion.py
+-rw-r--r--   0        0        0     3806 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_voltage_unit_conversion.py
+-rw-r--r--   0        0        0     3780 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/unit/get_volume_unit_conversion.py
+-rw-r--r--   0        0        0      297 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/__init__.py
+-rw-r--r--   0        0        0     2676 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/delete_user_self.py
+-rw-r--r--   0        0        0     2735 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/get_session_for_user.py
+-rw-r--r--   0        0        0     3027 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/get_user.py
+-rw-r--r--   0        0        0     3157 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/get_user_extended.py
+-rw-r--r--   0        0        0     2446 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/get_user_front_hash_self.py
+-rw-r--r--   0        0        0     2484 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/get_user_onboarding_self.py
+-rw-r--r--   0        0        0     2489 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/get_user_self.py
+-rw-r--r--   0        0        0     2601 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/get_user_self_extended.py
+-rw-r--r--   0        0        0     4077 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/list_users.py
+-rw-r--r--   0        0        0     4159 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/list_users_extended.py
+-rw-r--r--   0        0        0     2745 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/api/users/update_user_self.py
+-rw-r--r--   0        0        0     2297 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/client.py
+-rw-r--r--   0        0        0     4725 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/client_test.py
+-rw-r--r--   0        0        0    86464 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/examples_test.py
+-rw-r--r--   0        0        0     7838 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/__init__.py
+-rw-r--r--   0        0        0      322 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/account_provider.py
+-rw-r--r--   0        0        0     2249 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/ai_plugin_api.py
+-rw-r--r--   0        0        0      242 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/ai_plugin_api_type.py
+-rw-r--r--   0        0        0     2440 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/ai_plugin_auth.py
+-rw-r--r--   0        0        0      413 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/ai_plugin_auth_type.py
+-rw-r--r--   0        0        0      287 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/ai_plugin_http_auth_type.py
+-rw-r--r--   0        0        0     4685 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/ai_plugin_manifest.py
+-rw-r--r--   0        0        0     1720 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/api_call_query_group.py
+-rw-r--r--   0        0        0      777 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/api_call_query_group_by.py
+-rw-r--r--   0        0        0      620 2023-05-04 08:24:50.950633 kittycad-0.3.9/kittycad/models/api_call_status.py
+-rw-r--r--   0        0        0     8266 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/api_call_with_price.py
+-rw-r--r--   0        0        0     2128 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/api_call_with_price_results_page.py
+-rw-r--r--   0        0        0     3278 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/api_token.py
+-rw-r--r--   0        0        0     2004 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/api_token_results_page.py
+-rw-r--r--   0        0        0     1447 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/app_client_info.py
+-rw-r--r--   0        0        0     5747 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/async_api_call.py
+-rw-r--r--   0        0        0    34040 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/async_api_call_output.py
+-rw-r--r--   0        0        0     2066 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/async_api_call_results_page.py
+-rw-r--r--   0        0        0      648 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/async_api_call_type.py
+-rw-r--r--   0        0        0     2127 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/billing_info.py
+-rw-r--r--   0        0        0     1479 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/cache_metadata.py
+-rw-r--r--   0        0        0     3353 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/card_details.py
+-rw-r--r--   0        0        0     2697 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/cluster.py
+-rw-r--r--   0        0        0      229 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/code_language.py
+-rw-r--r--   0        0        0     2244 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/code_output.py
+-rw-r--r--   0        0        0     1732 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/commit.py
+-rw-r--r--   0        0        0    14343 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/connection.py
+-rw-r--r--   0        0        0    13513 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/country_code.py
+-rw-r--r--   0        0        0      507 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/created_at_sort_mode.py
+-rw-r--r--   0        0        0     8623 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/currency.py
+-rw-r--r--   0        0        0     4298 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/customer.py
+-rw-r--r--   0        0        0     4306 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/customer_balance.py
+-rw-r--r--   0        0        0     2412 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/device_access_token_request_form.py
+-rw-r--r--   0        0        0     1580 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/device_auth_request_form.py
+-rw-r--r--   0        0        0     1606 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/device_auth_verify_params.py
+-rw-r--r--   0        0        0    21264 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/docker_system_info.py
+-rw-r--r--   0        0        0     3553 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/drawing_cmd.py
+-rw-r--r--   0        0        0       75 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/drawing_cmd_id.py
+-rw-r--r--   0        0        0     2441 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/drawing_cmd_req.py
+-rw-r--r--   0        0        0     1746 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/drawing_cmd_req_batch.py
+-rw-r--r--   0        0        0     2393 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/drawing_error.py
+-rw-r--r--   0        0        0     1869 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/drawing_outcome.py
+-rw-r--r--   0        0        0     1505 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/drawing_outcomes.py
+-rw-r--r--   0        0        0     1789 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/email_authentication_form.py
+-rw-r--r--   0        0        0     3847 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/engine_metadata.py
+-rw-r--r--   0        0        0      269 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/environment.py
+-rw-r--r--   0        0        0     1930 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/error.py
+-rw-r--r--   0        0        0     2715 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/executor_metadata.py
+-rw-r--r--   0        0        0     6069 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/extended_user.py
+-rw-r--r--   0        0        0     2060 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/extended_user_results_page.py
+-rw-r--r--   0        0        0     5700 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_center_of_mass.py
+-rw-r--r--   0        0        0     6060 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_conversion.py
+-rw-r--r--   0        0        0     5725 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_density.py
+-rw-r--r--   0        0        0     1369 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_export_format.py
+-rw-r--r--   0        0        0     1306 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_import_format.py
+-rw-r--r--   0        0        0     5707 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_mass.py
+-rw-r--r--   0        0        0     5522 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_surface_area.py
+-rw-r--r--   0        0        0     1513 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_system_metadata.py
+-rw-r--r--   0        0        0     5428 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/file_volume.py
+-rw-r--r--   0        0        0     2304 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/gateway.py
+-rw-r--r--   0        0        0      187 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/image_type.py
+-rw-r--r--   0        0        0     2228 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/index_info.py
+-rw-r--r--   0        0        0     8273 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/invoice.py
+-rw-r--r--   0        0        0     2888 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/invoice_line_item.py
+-rw-r--r--   0        0        0      563 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/invoice_status.py
+-rw-r--r--   0        0        0     2666 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/jetstream.py
+-rw-r--r--   0        0        0     1907 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/jetstream_api_stats.py
+-rw-r--r--   0        0        0     2212 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/jetstream_config.py
+-rw-r--r--   0        0        0     3174 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/jetstream_stats.py
+-rw-r--r--   0        0        0     2125 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/leaf_node.py
+-rw-r--r--   0        0        0     1337 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/mesh.py
+-rw-r--r--   0        0        0     1923 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/meta_cluster_info.py
+-rw-r--r--   0        0        0     5025 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/metadata.py
+-rw-r--r--   0        0        0     1788 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/method.py
+-rw-r--r--   0        0        0     3081 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/new_address.py
+-rw-r--r--   0        0        0     2038 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/o_auth2_client_info.py
+-rw-r--r--   0        0        0      415 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/o_auth2_grant_type.py
+-rw-r--r--   0        0        0     2501 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/onboarding.py
+-rw-r--r--   0        0        0     1646 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/output_file.py
+-rw-r--r--   0        0        0     1527 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/payment_intent.py
+-rw-r--r--   0        0        0     3753 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/payment_method.py
+-rw-r--r--   0        0        0     2267 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/payment_method_card_checks.py
+-rw-r--r--   0        0        0      294 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/payment_method_type.py
+-rw-r--r--   0        0        0     5424 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/physics_constant.py
+-rw-r--r--   0        0        0     4448 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/physics_constant_name.py
+-rw-r--r--   0        0        0     2809 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/plugins_info.py
+-rw-r--r--   0        0        0     1498 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/point_e_metadata.py
+-rw-r--r--   0        0        0     1432 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/pong.py
+-rw-r--r--   0        0        0     4187 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/registry_service_config.py
+-rw-r--r--   0        0        0     2034 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/runtime.py
+-rw-r--r--   0        0        0     3638 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/session.py
+-rw-r--r--   0        0        0      214 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/system_info_cgroup_driver_enum.py
+-rw-r--r--   0        0        0      175 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/system_info_cgroup_version_enum.py
+-rw-r--r--   0        0        0     1663 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/system_info_default_address_pools.py
+-rw-r--r--   0        0        0      213 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/system_info_isolation_enum.py
+-rw-r--r--   0        0        0     6317 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_acceleration_conversion.py
+-rw-r--r--   0        0        0      642 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_acceleration_format.py
+-rw-r--r--   0        0        0     6226 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_angle_conversion.py
+-rw-r--r--   0        0        0      916 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_angle_format.py
+-rw-r--r--   0        0        0     6360 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_angular_velocity_conversion.py
+-rw-r--r--   0        0        0      754 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_angular_velocity_format.py
+-rw-r--r--   0        0        0     6213 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_area_conversion.py
+-rw-r--r--   0        0        0      888 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_area_format.py
+-rw-r--r--   0        0        0     6239 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_charge_conversion.py
+-rw-r--r--   0        0        0      380 2023-05-04 08:24:50.954633 kittycad-0.3.9/kittycad/models/unit_charge_format.py
+-rw-r--r--   0        0        0     6330 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_concentration_conversion.py
+-rw-r--r--   0        0        0      752 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_concentration_format.py
+-rw-r--r--   0        0        0     6213 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_data_conversion.py
+-rw-r--r--   0        0        0      539 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_data_format.py
+-rw-r--r--   0        0        0     6377 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_data_transfer_rate_conversion.py
+-rw-r--r--   0        0        0      656 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_data_transfer_rate_format.py
+-rw-r--r--   0        0        0     6252 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_density_conversion.py
+-rw-r--r--   0        0        0     1488 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_density_format.py
+-rw-r--r--   0        0        0     6239 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_energy_conversion.py
+-rw-r--r--   0        0        0     1162 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_energy_format.py
+-rw-r--r--   0        0        0     6226 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_force_conversion.py
+-rw-r--r--   0        0        0      645 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_force_format.py
+-rw-r--r--   0        0        0     6304 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_illuminance_conversion.py
+-rw-r--r--   0        0        0      584 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_illuminance_format.py
+-rw-r--r--   0        0        0     6239 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_length_conversion.py
+-rw-r--r--   0        0        0     2187 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_length_format.py
+-rw-r--r--   0        0        0     6442 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_magnetic_field_strength_conversion.py
+-rw-r--r--   0        0        0      402 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_magnetic_field_strength_format.py
+-rw-r--r--   0        0        0     6321 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_magnetic_flux_conversion.py
+-rw-r--r--   0        0        0      389 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_magnetic_flux_format.py
+-rw-r--r--   0        0        0     6213 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_mass_conversion.py
+-rw-r--r--   0        0        0     1094 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_mass_format.py
+-rw-r--r--   0        0        0     3438 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_metric_power.py
+-rw-r--r--   0        0        0     6259 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_metric_power_conversion.py
+-rw-r--r--   0        0        0     6287 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_metric_power_cubed_conversion.py
+-rw-r--r--   0        0        0     6297 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_metric_power_squared_conversion.py
+-rw-r--r--   0        0        0     6226 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_power_conversion.py
+-rw-r--r--   0        0        0      468 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_power_format.py
+-rw-r--r--   0        0        0     6265 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_pressure_conversion.py
+-rw-r--r--   0        0        0      725 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_pressure_format.py
+-rw-r--r--   0        0        0     6278 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_radiation_conversion.py
+-rw-r--r--   0        0        0      586 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_radiation_format.py
+-rw-r--r--   0        0        0     6330 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_radioactivity_conversion.py
+-rw-r--r--   0        0        0      570 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_radioactivity_format.py
+-rw-r--r--   0        0        0     6295 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_solid_angle_conversion.py
+-rw-r--r--   0        0        0      500 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_solid_angle_format.py
+-rw-r--r--   0        0        0     6304 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_temperature_conversion.py
+-rw-r--r--   0        0        0      674 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_temperature_format.py
+-rw-r--r--   0        0        0     6213 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_time_conversion.py
+-rw-r--r--   0        0        0      902 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_time_format.py
+-rw-r--r--   0        0        0     6265 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_velocity_conversion.py
+-rw-r--r--   0        0        0      753 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_velocity_format.py
+-rw-r--r--   0        0        0     6252 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_voltage_conversion.py
+-rw-r--r--   0        0        0      452 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_voltage_format.py
+-rw-r--r--   0        0        0     6239 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_volume_conversion.py
+-rw-r--r--   0        0        0     3286 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/unit_volume_format.py
+-rw-r--r--   0        0        0     2577 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/update_user.py
+-rw-r--r--   0        0        0     5084 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/user.py
+-rw-r--r--   0        0        0     1942 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/user_results_page.py
+-rw-r--r--   0        0        0       67 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/uuid.py
+-rw-r--r--   0        0        0     3448 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/models/verification_token.py
+-rw-r--r--   0        0        0       26 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/py.typed
+-rw-r--r--   0        0        0     1049 2023-05-04 08:24:50.958633 kittycad-0.3.9/kittycad/types.py
+-rw-r--r--   0        0        0     2416 2023-05-04 08:24:50.958633 kittycad-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 kittycad-0.3.9/PKG-INFO
```

### Comparing `kittycad-0.3.8/LICENSE` & `kittycad-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/README.md` & `kittycad-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/ai/create_image_to_3d.py` & `kittycad-0.3.9/kittycad/api/ai/create_image_to_3d.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/ai/create_text_to_3d.py` & `kittycad-0.3.9/kittycad/api/ai/create_text_to_3d.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/api_calls/get_api_call.py` & `kittycad-0.3.9/kittycad/api/api_calls/get_api_call.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/api_calls/get_api_call_for_user.py` & `kittycad-0.3.9/kittycad/api/api_calls/get_api_call_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/api_calls/get_api_call_metrics.py` & `kittycad-0.3.9/kittycad/api/api_calls/get_api_call_metrics.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/api_calls/get_async_operation.py` & `kittycad-0.3.9/kittycad/api/api_calls/get_async_operation.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/api_calls/list_api_calls.py` & `kittycad-0.3.9/kittycad/api/api_calls/list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/api_calls/list_api_calls_for_user.py` & `kittycad-0.3.9/kittycad/api/api_calls/list_api_calls_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/api_calls/list_async_operations.py` & `kittycad-0.3.9/kittycad/api/api_calls/list_async_operations.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/api_calls/user_list_api_calls.py` & `kittycad-0.3.9/kittycad/api/api_calls/user_list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/api_tokens/create_api_token_for_user.py` & `kittycad-0.3.9/kittycad/api/api_tokens/create_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/api_tokens/delete_api_token_for_user.py` & `kittycad-0.3.9/kittycad/api/api_tokens/delete_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/api_tokens/get_api_token_for_user.py` & `kittycad-0.3.9/kittycad/api/api_tokens/get_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/api_tokens/list_api_tokens_for_user.py` & `kittycad-0.3.9/kittycad/api/api_tokens/list_api_tokens_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/apps/apps_github_callback.py` & `kittycad-0.3.9/kittycad/api/apps/apps_github_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/apps/apps_github_consent.py` & `kittycad-0.3.9/kittycad/api/apps/apps_github_consent.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/apps/apps_github_webhook.py` & `kittycad-0.3.9/kittycad/api/apps/apps_github_webhook.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/constant/get_physics_constant.py` & `kittycad-0.3.9/kittycad/api/constant/get_physics_constant.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/drawing/cmd.py` & `kittycad-0.3.9/kittycad/api/drawing/cmd.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/drawing/cmd_batch.py` & `kittycad-0.3.9/kittycad/api/drawing/cmd_batch.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/executor/create_executor_term.py` & `kittycad-0.3.9/kittycad/api/executor/create_executor_term.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/executor/create_file_execution.py` & `kittycad-0.3.9/kittycad/api/executor/create_file_execution.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/file/create_file_center_of_mass.py` & `kittycad-0.3.9/kittycad/api/file/create_file_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/file/create_file_conversion.py` & `kittycad-0.3.9/kittycad/api/file/create_file_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/file/create_file_conversion_with_base64_helper.py` & `kittycad-0.3.9/kittycad/api/file/create_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/file/create_file_density.py` & `kittycad-0.3.9/kittycad/api/file/create_file_density.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/file/create_file_mass.py` & `kittycad-0.3.9/kittycad/api/file/create_file_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/file/create_file_surface_area.py` & `kittycad-0.3.9/kittycad/api/file/create_file_surface_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/file/create_file_volume.py` & `kittycad-0.3.9/kittycad/api/file/create_file_volume.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/file/get_file_conversion_with_base64_helper.py` & `kittycad-0.3.9/kittycad/api/file/get_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/hidden/auth_email.py` & `kittycad-0.3.9/kittycad/api/hidden/auth_email.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/hidden/auth_email_callback.py` & `kittycad-0.3.9/kittycad/api/hidden/auth_email_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/hidden/logout.py` & `kittycad-0.3.9/kittycad/api/hidden/logout.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/meta/get_ai_plugin_manifest.py` & `kittycad-0.3.9/kittycad/api/meta/get_ai_plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/meta/get_metadata.py` & `kittycad-0.3.9/kittycad/api/meta/get_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/meta/get_metrics.py` & `kittycad-0.3.9/kittycad/api/payments/get_payment_information_for_user.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,64 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.customer import Customer
+from ...models.error import Error
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/_meta/metrics".format(client.base_url)  # noqa: E501
+    url = "{}/user/payment".format(client.base_url)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any,]]:
-    return None
+) -> Optional[Union[Any, Customer, Error]]:
+    if response.status_code == 200:
+        response_200 = Customer.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
     return None
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any,]]:
+) -> Response[Union[Any, Customer, Error]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Union[Any,]]:
+) -> Response[Union[Any, Customer, Error]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -56,40 +66,42 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[Any,]]:
-    """You must be a KittyCAD employee to perform this request."""  # noqa: E501
+) -> Optional[Union[Any, Customer, Error]]:
+    """This includes billing address, phone, and name.
+    This endpoint requires authentication by any KittyCAD user. It gets the payment information for the authenticated user."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Union[Any,]]:
+) -> Response[Union[Any, Customer, Error]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[Any,]]:
-    """You must be a KittyCAD employee to perform this request."""  # noqa: E501
+) -> Optional[Union[Any, Customer, Error]]:
+    """This includes billing address, phone, and name.
+    This endpoint requires authentication by any KittyCAD user. It gets the payment information for the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.8/kittycad/api/meta/get_openai_schema.py` & `kittycad-0.3.9/kittycad/api/meta/get_openai_schema.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/meta/get_schema.py` & `kittycad-0.3.9/kittycad/api/meta/get_schema.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/meta/ping.py` & `kittycad-0.3.9/kittycad/api/meta/ping.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/payments/create_payment_information_for_user.py` & `kittycad-0.3.9/kittycad/api/payments/create_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/payments/create_payment_intent_for_user.py` & `kittycad-0.3.9/kittycad/api/payments/create_payment_intent_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/payments/delete_payment_information_for_user.py` & `kittycad-0.3.9/kittycad/api/payments/delete_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/payments/delete_payment_method_for_user.py` & `kittycad-0.3.9/kittycad/api/payments/delete_payment_method_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/payments/get_payment_balance_for_user.py` & `kittycad-0.3.9/kittycad/api/payments/get_payment_balance_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/payments/get_payment_information_for_user.py` & `kittycad-0.3.9/kittycad/api/users/get_session_for_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,107 +1,114 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.customer import Customer
 from ...models.error import Error
+from ...models.session import Session
 from ...types import Response
 
 
 def _get_kwargs(
+    token: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/payment".format(client.base_url)  # noqa: E501
+    url = "{}/user/session/{token}".format(client.base_url, token=token)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, Customer, Error]]:
+) -> Optional[Union[Any, Session, Error]]:
     if response.status_code == 200:
-        response_200 = Customer.from_dict(response.json())
+        response_200 = Session.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return None
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, Customer, Error]]:
+) -> Response[Union[Any, Session, Error]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    token: str,
     *,
     client: Client,
-) -> Response[Union[Any, Customer, Error]]:
+) -> Response[Union[Any, Session, Error]]:
     kwargs = _get_kwargs(
+        token=token,
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
+    token: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Customer, Error]]:
-    """This includes billing address, phone, and name.
-    This endpoint requires authentication by any KittyCAD user. It gets the payment information for the authenticated user."""  # noqa: E501
+) -> Optional[Union[Any, Session, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It returns details of the requested API token for the user."""  # noqa: E501
 
     return sync_detailed(
+        token=token,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    token: str,
     *,
     client: Client,
-) -> Response[Union[Any, Customer, Error]]:
+) -> Response[Union[Any, Session, Error]]:
     kwargs = _get_kwargs(
+        token=token,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
+    token: str,
     *,
     client: Client,
-) -> Optional[Union[Any, Customer, Error]]:
-    """This includes billing address, phone, and name.
-    This endpoint requires authentication by any KittyCAD user. It gets the payment information for the authenticated user."""  # noqa: E501
+) -> Optional[Union[Any, Session, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It returns details of the requested API token for the user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
+            token=token,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.8/kittycad/api/payments/list_invoices_for_user.py` & `kittycad-0.3.9/kittycad/api/payments/list_invoices_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/payments/list_payment_methods_for_user.py` & `kittycad-0.3.9/kittycad/api/payments/list_payment_methods_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/payments/update_payment_information_for_user.py` & `kittycad-0.3.9/kittycad/api/payments/update_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/payments/validate_customer_tax_information_for_user.py` & `kittycad-0.3.9/kittycad/api/payments/validate_customer_tax_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_acceleration_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_acceleration_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_angle_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_angle_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_angular_velocity_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_angular_velocity_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_area_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_area_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_charge_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_charge_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_concentration_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_concentration_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_data_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_data_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_density_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_density_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_energy_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_energy_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_force_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_force_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_illuminance_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_illuminance_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_length_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_length_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_magnetic_flux_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_magnetic_flux_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_mass_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_mass_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_metric_power_squared_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_metric_power_squared_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_metric_power_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_metric_power_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_power_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_power_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_pressure_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_pressure_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_radiation_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_radiation_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_radioactivity_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_radioactivity_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_solid_angle_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_solid_angle_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_temperature_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_temperature_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_time_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_time_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_velocity_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_velocity_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_voltage_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_voltage_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/unit/get_volume_unit_conversion.py` & `kittycad-0.3.9/kittycad/api/unit/get_volume_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/users/delete_user_self.py` & `kittycad-0.3.9/kittycad/api/users/delete_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/users/get_session_for_user.py` & `kittycad-0.3.9/kittycad/api/users/update_user_self.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,112 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.session import Session
+from ...models.update_user import UpdateUser
+from ...models.user import User
 from ...types import Response
 
 
 def _get_kwargs(
-    token: str,
+    body: UpdateUser,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/session/{token}".format(client.base_url, token=token)  # noqa: E501
+    url = "{}/user".format(client.base_url)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "content": body,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, Session, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, User, Error]]:
     if response.status_code == 200:
-        response_200 = Session.from_dict(response.json())
+        response_200 = User.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return None
 
 
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[Any, Session, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, User, Error]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    token: str,
+    body: UpdateUser,
     *,
     client: Client,
-) -> Response[Union[Any, Session, Error]]:
+) -> Response[Union[Any, User, Error]]:
     kwargs = _get_kwargs(
-        token=token,
+        body=body,
         client=client,
     )
 
-    response = httpx.get(
+    response = httpx.put(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    token: str,
+    body: UpdateUser,
     *,
     client: Client,
-) -> Optional[Union[Any, Session, Error]]:
-    """This endpoint requires authentication by any KittyCAD user. It returns details of the requested API token for the user."""  # noqa: E501
+) -> Optional[Union[Any, User, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user."""  # noqa: E501
 
     return sync_detailed(
-        token=token,
+        body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    token: str,
+    body: UpdateUser,
     *,
     client: Client,
-) -> Response[Union[Any, Session, Error]]:
+) -> Response[Union[Any, User, Error]]:
     kwargs = _get_kwargs(
-        token=token,
+        body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.get(**kwargs)
+        response = await _client.put(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    token: str,
+    body: UpdateUser,
     *,
     client: Client,
-) -> Optional[Union[Any, Session, Error]]:
-    """This endpoint requires authentication by any KittyCAD user. It returns details of the requested API token for the user."""  # noqa: E501
+) -> Optional[Union[Any, User, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            token=token,
+            body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.3.8/kittycad/api/users/get_user.py` & `kittycad-0.3.9/kittycad/api/users/get_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/users/get_user_extended.py` & `kittycad-0.3.9/kittycad/api/users/get_user_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/users/get_user_front_hash_self.py` & `kittycad-0.3.9/kittycad/api/users/get_user_front_hash_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/users/get_user_onboarding_self.py` & `kittycad-0.3.9/kittycad/api/users/get_user_onboarding_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/users/get_user_self.py` & `kittycad-0.3.9/kittycad/api/users/get_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/users/get_user_self_extended.py` & `kittycad-0.3.9/kittycad/api/users/get_user_self_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/users/list_users.py` & `kittycad-0.3.9/kittycad/api/users/list_users.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/api/users/list_users_extended.py` & `kittycad-0.3.9/kittycad/api/users/list_users_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/client.py` & `kittycad-0.3.9/kittycad/client.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/client_test.py` & `kittycad-0.3.9/kittycad/client_test.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/examples_test.py` & `kittycad-0.3.9/kittycad/examples_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     create_file_surface_area,
     create_file_volume,
 )
 from kittycad.api.hidden import auth_email, auth_email_callback, logout
 from kittycad.api.meta import (
     get_ai_plugin_manifest,
     get_metadata,
-    get_metrics,
     get_openai_schema,
     get_schema,
     ping,
 )
 from kittycad.api.payments import (
     create_payment_information_for_user,
     create_payment_intent_for_user,
@@ -236,46 +235,14 @@
     # OR run async with more info
     await get_metadata.asyncio_detailed(
         client=client,
     )
 
 
 @pytest.mark.skip
-def test_get_metrics():
-    # Create our client.
-    client = ClientFromEnv()
-
-    get_metrics.sync(
-        client=client,
-    )
-
-    # OR if you need more info (e.g. status_code)
-    get_metrics.sync_detailed(
-        client=client,
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_get_metrics_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    await get_metrics.asyncio(
-        client=client,
-    )
-
-    # OR run async with more info
-    await get_metrics.asyncio_detailed(
-        client=client,
-    )
-
-
-@pytest.mark.skip
 def test_create_image_to_3d():
     # Create our client.
     client = ClientFromEnv()
 
     create_image_to_3d.sync(
         client=client,
         input_format=ImageType.PNG,
```

### Comparing `kittycad-0.3.8/kittycad/models/__init__.py` & `kittycad-0.3.9/kittycad/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/ai_plugin_api.py` & `kittycad-0.3.9/kittycad/models/ai_plugin_api.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/ai_plugin_auth.py` & `kittycad-0.3.9/kittycad/models/ai_plugin_auth.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/ai_plugin_manifest.py` & `kittycad-0.3.9/kittycad/models/ai_plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/api_call_query_group.py` & `kittycad-0.3.9/kittycad/models/api_call_query_group.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/api_call_query_group_by.py` & `kittycad-0.3.9/kittycad/models/api_call_query_group_by.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/api_call_status.py` & `kittycad-0.3.9/kittycad/models/api_call_status.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/api_call_with_price.py` & `kittycad-0.3.9/kittycad/models/api_call_with_price.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/api_call_with_price_results_page.py` & `kittycad-0.3.9/kittycad/models/api_call_with_price_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/api_token.py` & `kittycad-0.3.9/kittycad/models/api_token.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/api_token_results_page.py` & `kittycad-0.3.9/kittycad/models/api_token_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/app_client_info.py` & `kittycad-0.3.9/kittycad/models/app_client_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/async_api_call.py` & `kittycad-0.3.9/kittycad/models/async_api_call.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/async_api_call_output.py` & `kittycad-0.3.9/kittycad/models/async_api_call_output.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/async_api_call_results_page.py` & `kittycad-0.3.9/kittycad/models/async_api_call_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/async_api_call_type.py` & `kittycad-0.3.9/kittycad/models/async_api_call_type.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/billing_info.py` & `kittycad-0.3.9/kittycad/models/billing_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/cache_metadata.py` & `kittycad-0.3.9/kittycad/models/cache_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/card_details.py` & `kittycad-0.3.9/kittycad/models/card_details.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/cluster.py` & `kittycad-0.3.9/kittycad/models/cluster.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/code_output.py` & `kittycad-0.3.9/kittycad/models/code_output.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/commit.py` & `kittycad-0.3.9/kittycad/models/commit.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/connection.py` & `kittycad-0.3.9/kittycad/models/connection.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/country_code.py` & `kittycad-0.3.9/kittycad/models/country_code.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/currency.py` & `kittycad-0.3.9/kittycad/models/currency.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/customer.py` & `kittycad-0.3.9/kittycad/models/customer.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/customer_balance.py` & `kittycad-0.3.9/kittycad/models/customer_balance.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/device_access_token_request_form.py` & `kittycad-0.3.9/kittycad/models/device_access_token_request_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/device_auth_request_form.py` & `kittycad-0.3.9/kittycad/models/device_auth_request_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/device_auth_verify_params.py` & `kittycad-0.3.9/kittycad/models/device_auth_verify_params.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/docker_system_info.py` & `kittycad-0.3.9/kittycad/models/docker_system_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/drawing_cmd.py` & `kittycad-0.3.9/kittycad/models/drawing_cmd.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/drawing_cmd_req.py` & `kittycad-0.3.9/kittycad/models/drawing_cmd_req.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/drawing_cmd_req_batch.py` & `kittycad-0.3.9/kittycad/models/drawing_cmd_req_batch.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/drawing_error.py` & `kittycad-0.3.9/kittycad/models/drawing_error.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/drawing_outcome.py` & `kittycad-0.3.9/kittycad/models/drawing_outcome.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/drawing_outcomes.py` & `kittycad-0.3.9/kittycad/models/drawing_outcomes.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/email_authentication_form.py` & `kittycad-0.3.9/kittycad/models/email_authentication_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/engine_metadata.py` & `kittycad-0.3.9/kittycad/models/engine_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/error.py` & `kittycad-0.3.9/kittycad/models/error.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/executor_metadata.py` & `kittycad-0.3.9/kittycad/models/executor_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/extended_user.py` & `kittycad-0.3.9/kittycad/models/extended_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/extended_user_results_page.py` & `kittycad-0.3.9/kittycad/models/extended_user_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/file_center_of_mass.py` & `kittycad-0.3.9/kittycad/models/file_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/file_conversion.py` & `kittycad-0.3.9/kittycad/models/file_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/file_density.py` & `kittycad-0.3.9/kittycad/models/file_density.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/file_export_format.py` & `kittycad-0.3.9/kittycad/models/file_export_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/file_import_format.py` & `kittycad-0.3.9/kittycad/models/file_import_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/file_mass.py` & `kittycad-0.3.9/kittycad/models/file_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/file_surface_area.py` & `kittycad-0.3.9/kittycad/models/file_surface_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/file_system_metadata.py` & `kittycad-0.3.9/kittycad/models/file_system_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/file_volume.py` & `kittycad-0.3.9/kittycad/models/file_volume.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/gateway.py` & `kittycad-0.3.9/kittycad/models/gateway.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/index_info.py` & `kittycad-0.3.9/kittycad/models/index_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/invoice.py` & `kittycad-0.3.9/kittycad/models/invoice.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/invoice_line_item.py` & `kittycad-0.3.9/kittycad/models/invoice_line_item.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/invoice_status.py` & `kittycad-0.3.9/kittycad/models/invoice_status.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/jetstream.py` & `kittycad-0.3.9/kittycad/models/jetstream.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/jetstream_api_stats.py` & `kittycad-0.3.9/kittycad/models/jetstream_api_stats.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/jetstream_config.py` & `kittycad-0.3.9/kittycad/models/jetstream_config.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/jetstream_stats.py` & `kittycad-0.3.9/kittycad/models/jetstream_stats.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/leaf_node.py` & `kittycad-0.3.9/kittycad/models/leaf_node.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/mesh.py` & `kittycad-0.3.9/kittycad/models/mesh.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/meta_cluster_info.py` & `kittycad-0.3.9/kittycad/models/meta_cluster_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/metadata.py` & `kittycad-0.3.9/kittycad/models/metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/method.py` & `kittycad-0.3.9/kittycad/models/method.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/new_address.py` & `kittycad-0.3.9/kittycad/models/new_address.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/o_auth2_client_info.py` & `kittycad-0.3.9/kittycad/models/o_auth2_client_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/onboarding.py` & `kittycad-0.3.9/kittycad/models/onboarding.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/output_file.py` & `kittycad-0.3.9/kittycad/models/output_file.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/payment_intent.py` & `kittycad-0.3.9/kittycad/models/payment_intent.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/payment_method.py` & `kittycad-0.3.9/kittycad/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/payment_method_card_checks.py` & `kittycad-0.3.9/kittycad/models/payment_method_card_checks.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/physics_constant.py` & `kittycad-0.3.9/kittycad/models/physics_constant.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/physics_constant_name.py` & `kittycad-0.3.9/kittycad/models/physics_constant_name.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/plugins_info.py` & `kittycad-0.3.9/kittycad/models/plugins_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/point_e_metadata.py` & `kittycad-0.3.9/kittycad/models/point_e_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/pong.py` & `kittycad-0.3.9/kittycad/models/pong.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/registry_service_config.py` & `kittycad-0.3.9/kittycad/models/registry_service_config.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/runtime.py` & `kittycad-0.3.9/kittycad/models/runtime.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/session.py` & `kittycad-0.3.9/kittycad/models/session.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/system_info_default_address_pools.py` & `kittycad-0.3.9/kittycad/models/system_info_default_address_pools.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_acceleration_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_acceleration_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_acceleration_format.py` & `kittycad-0.3.9/kittycad/models/unit_acceleration_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_angle_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_angle_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_angle_format.py` & `kittycad-0.3.9/kittycad/models/unit_angle_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_angular_velocity_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_angular_velocity_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_angular_velocity_format.py` & `kittycad-0.3.9/kittycad/models/unit_angular_velocity_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_area_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_area_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_area_format.py` & `kittycad-0.3.9/kittycad/models/unit_area_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_charge_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_charge_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_concentration_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_concentration_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_concentration_format.py` & `kittycad-0.3.9/kittycad/models/unit_concentration_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_data_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_data_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_data_format.py` & `kittycad-0.3.9/kittycad/models/unit_data_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_data_transfer_rate_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_data_transfer_rate_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_data_transfer_rate_format.py` & `kittycad-0.3.9/kittycad/models/unit_data_transfer_rate_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_density_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_density_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_density_format.py` & `kittycad-0.3.9/kittycad/models/unit_density_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_energy_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_energy_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_energy_format.py` & `kittycad-0.3.9/kittycad/models/unit_energy_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_force_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_force_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_force_format.py` & `kittycad-0.3.9/kittycad/models/unit_force_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_illuminance_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_illuminance_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_illuminance_format.py` & `kittycad-0.3.9/kittycad/models/unit_illuminance_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_length_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_length_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_length_format.py` & `kittycad-0.3.9/kittycad/models/unit_length_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_magnetic_field_strength_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_magnetic_field_strength_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_magnetic_flux_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_magnetic_flux_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_mass_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_mass_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_mass_format.py` & `kittycad-0.3.9/kittycad/models/unit_mass_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_metric_power.py` & `kittycad-0.3.9/kittycad/models/unit_metric_power.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_metric_power_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_metric_power_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_metric_power_cubed_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_metric_power_cubed_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_metric_power_squared_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_metric_power_squared_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_power_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_power_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_pressure_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_pressure_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_pressure_format.py` & `kittycad-0.3.9/kittycad/models/unit_pressure_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_radiation_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_radiation_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_radiation_format.py` & `kittycad-0.3.9/kittycad/models/unit_radiation_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_radioactivity_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_radioactivity_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_radioactivity_format.py` & `kittycad-0.3.9/kittycad/models/unit_radioactivity_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_solid_angle_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_solid_angle_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_temperature_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_temperature_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_temperature_format.py` & `kittycad-0.3.9/kittycad/models/unit_temperature_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_time_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_time_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_time_format.py` & `kittycad-0.3.9/kittycad/models/unit_time_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_velocity_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_velocity_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_velocity_format.py` & `kittycad-0.3.9/kittycad/models/unit_velocity_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_voltage_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_voltage_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_volume_conversion.py` & `kittycad-0.3.9/kittycad/models/unit_volume_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/unit_volume_format.py` & `kittycad-0.3.9/kittycad/models/unit_volume_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/update_user.py` & `kittycad-0.3.9/kittycad/models/update_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/user.py` & `kittycad-0.3.9/kittycad/models/user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/user_results_page.py` & `kittycad-0.3.9/kittycad/models/user_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/models/verification_token.py` & `kittycad-0.3.9/kittycad/models/verification_token.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/kittycad/types.py` & `kittycad-0.3.9/kittycad/types.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.8/pyproject.toml` & `kittycad-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kittycad"
-version = "0.3.8"
+version = "0.3.9"
 description = "A client library for accessing KittyCAD"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "kittycad"},
```

### Comparing `kittycad-0.3.8/PKG-INFO` & `kittycad-0.3.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kittycad
-Version: 0.3.8
+Version: 0.3.9
 Summary: A client library for accessing KittyCAD
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

