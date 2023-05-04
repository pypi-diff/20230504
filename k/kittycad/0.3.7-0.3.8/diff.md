# Comparing `tmp/kittycad-0.3.7.tar.gz` & `tmp/kittycad-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kittycad-0.3.7.tar", max compression
+gzip compressed data, was "kittycad-0.3.8.tar", max compression
```

## Comparing `kittycad-0.3.7.tar` & `kittycad-0.3.8.tar`

### file list

```diff
@@ -1,263 +1,272 @@
--rw-r--r--   0        0        0     1065 2023-04-17 21:11:22.955786 kittycad-0.3.7/LICENSE
--rw-r--r--   0        0        0      875 2023-04-17 21:11:22.955786 kittycad-0.3.7/README.md
--rw-r--r--   0        0        0       90 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/__init__.py
--rw-r--r--   0        0        0       47 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/__init__.py
--rw-r--r--   0        0        0      105 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/ai/__init__.py
--rw-r--r--   0        0        0     3316 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/ai/create_image_to_3d.py
--rw-r--r--   0        0        0     3012 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/ai/create_text_to_3d.py
--rw-r--r--   0        0        0      185 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/__init__.py
--rw-r--r--   0        0        0     2729 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/get_api_call.py
--rw-r--r--   0        0        0     2434 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/get_api_call_for_user.py
--rw-r--r--   0        0        0     2725 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/get_api_call_metrics.py
--rw-r--r--   0        0        0     4715 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/get_async_operation.py
--rw-r--r--   0        0        0     3388 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/list_api_calls.py
--rw-r--r--   0        0        0     4090 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/list_api_calls_for_user.py
--rw-r--r--   0        0        0     3785 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/list_async_operations.py
--rw-r--r--   0        0        0     3495 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/user_list_api_calls.py
--rw-r--r--   0        0        0      338 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_tokens/__init__.py
--rw-r--r--   0        0        0     2257 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_tokens/create_api_token_for_user.py
--rw-r--r--   0        0        0     2629 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_tokens/delete_api_token_for_user.py
--rw-r--r--   0        0        0     2411 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_tokens/get_api_token_for_user.py
--rw-r--r--   0        0        0     3428 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_tokens/list_api_tokens_for_user.py
--rw-r--r--   0        0        0      102 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/apps/__init__.py
--rw-r--r--   0        0        0     2404 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/apps/apps_github_callback.py
--rw-r--r--   0        0        0     2581 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/apps/apps_github_consent.py
--rw-r--r--   0        0        0     2104 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/apps/apps_github_webhook.py
--rw-r--r--   0        0        0      142 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/beta/__init__.py
--rw-r--r--   0        0        0      104 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/constant/__init__.py
--rw-r--r--   0        0        0     2409 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/constant/get_physics_constant.py
--rw-r--r--   0        0        0      219 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/__init__.py
--rw-r--r--   0        0        0     4186 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_2d_vector_conversion.py
--rw-r--r--   0        0        0     3329 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_center_of_mass.py
--rw-r--r--   0        0        0     3974 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_conversion.py
--rw-r--r--   0        0        0     1854 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0     3559 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_density.py
--rw-r--r--   0        0        0     2643 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_execution.py
--rw-r--r--   0        0        0     3574 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_mass.py
--rw-r--r--   0        0        0     3313 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_surface_area.py
--rw-r--r--   0        0        0     3249 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_volume.py
--rw-r--r--   0        0        0     1158 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/get_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0      119 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/hidden/__init__.py
--rw-r--r--   0        0        0     2388 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/hidden/auth_email.py
--rw-r--r--   0        0        0     2539 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/hidden/auth_email_callback.py
--rw-r--r--   0        0        0     1954 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/hidden/logout.py
--rw-r--r--   0        0        0       91 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/meta/__init__.py
--rw-r--r--   0        0        0     2091 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/meta/get_ai_plugin_manifest.py
--rw-r--r--   0        0        0     2305 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/meta/get_metadata.py
--rw-r--r--   0        0        0     2280 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/meta/get_openai_schema.py
--rw-r--r--   0        0        0     1939 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/meta/get_schema.py
--rw-r--r--   0        0        0     1959 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/meta/ping.py
--rw-r--r--   0        0        0      109 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/oauth2/__init__.py
--rw-r--r--   0        0        0      103 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/__init__.py
--rw-r--r--   0        0        0     2583 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/create_payment_information_for_user.py
--rw-r--r--   0        0        0     2316 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/create_payment_intent_for_user.py
--rw-r--r--   0        0        0     2238 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/delete_payment_information_for_user.py
--rw-r--r--   0        0        0     2258 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/delete_payment_method_for_user.py
--rw-r--r--   0        0        0     2333 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/get_payment_balance_for_user.py
--rw-r--r--   0        0        0     2357 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/get_payment_information_for_user.py
--rw-r--r--   0        0        0     2274 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/list_invoices_for_user.py
--rw-r--r--   0        0        0     2342 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/list_payment_methods_for_user.py
--rw-r--r--   0        0        0     2581 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/update_payment_information_for_user.py
--rw-r--r--   0        0        0     2298 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/validate_customer_tax_information_for_user.py
--rw-r--r--   0        0        0      142 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/sessions/__init__.py
--rw-r--r--   0        0        0     2398 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/sessions/get_session_for_user.py
--rw-r--r--   0        0        0       87 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/__init__.py
--rw-r--r--   0        0        0     3441 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_acceleration_unit_conversion.py
--rw-r--r--   0        0        0     3245 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_angle_unit_conversion.py
--rw-r--r--   0        0        0     3533 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_angular_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3217 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_area_unit_conversion.py
--rw-r--r--   0        0        0     3271 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_charge_unit_conversion.py
--rw-r--r--   0        0        0     3467 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_concentration_unit_conversion.py
--rw-r--r--   0        0        0     3567 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py
--rw-r--r--   0        0        0     3215 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_data_unit_conversion.py
--rw-r--r--   0        0        0     3299 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_density_unit_conversion.py
--rw-r--r--   0        0        0     3271 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_energy_unit_conversion.py
--rw-r--r--   0        0        0     3243 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_force_unit_conversion.py
--rw-r--r--   0        0        0     3411 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_illuminance_unit_conversion.py
--rw-r--r--   0        0        0     3271 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_length_unit_conversion.py
--rw-r--r--   0        0        0     3707 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py
--rw-r--r--   0        0        0     3447 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_magnetic_flux_unit_conversion.py
--rw-r--r--   0        0        0     3215 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_mass_unit_conversion.py
--rw-r--r--   0        0        0     3379 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py
--rw-r--r--   0        0        0     3407 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_metric_power_squared_unit_conversion.py
--rw-r--r--   0        0        0     3309 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_metric_power_unit_conversion.py
--rw-r--r--   0        0        0     3243 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_power_unit_conversion.py
--rw-r--r--   0        0        0     3327 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_pressure_unit_conversion.py
--rw-r--r--   0        0        0     3355 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_radiation_unit_conversion.py
--rw-r--r--   0        0        0     3467 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_radioactivity_unit_conversion.py
--rw-r--r--   0        0        0     3391 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_solid_angle_unit_conversion.py
--rw-r--r--   0        0        0     3411 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_temperature_unit_conversion.py
--rw-r--r--   0        0        0     3215 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_time_unit_conversion.py
--rw-r--r--   0        0        0     3327 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3299 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_voltage_unit_conversion.py
--rw-r--r--   0        0        0     3271 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_volume_unit_conversion.py
--rw-r--r--   0        0        0      283 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/__init__.py
--rw-r--r--   0        0        0     2386 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/delete_user_self.py
--rw-r--r--   0        0        0     2686 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/get_user.py
--rw-r--r--   0        0        0     2804 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/get_user_extended.py
--rw-r--r--   0        0        0     2194 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/get_user_front_hash_self.py
--rw-r--r--   0        0        0     2190 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/get_user_onboarding_self.py
--rw-r--r--   0        0        0     2199 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/get_user_self.py
--rw-r--r--   0        0        0     2299 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/get_user_self_extended.py
--rw-r--r--   0        0        0     3257 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/list_users.py
--rw-r--r--   0        0        0     3339 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/list_users_extended.py
--rw-r--r--   0        0        0     2414 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/update_user_self.py
--rw-r--r--   0        0        0     1960 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/client.py
--rw-r--r--   0        0        0     4227 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/client_test.py
--rw-r--r--   0        0        0     7730 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/models/__init__.py
--rw-r--r--   0        0        0      164 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/account_provider.py
--rw-r--r--   0        0        0     2261 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/ai_plugin_api.py
--rw-r--r--   0        0        0      144 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/ai_plugin_api_type.py
--rw-r--r--   0        0        0     2511 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/ai_plugin_auth.py
--rw-r--r--   0        0        0      221 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/ai_plugin_auth_type.py
--rw-r--r--   0        0        0      167 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/ai_plugin_http_auth_type.py
--rw-r--r--   0        0        0     4590 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/ai_plugin_manifest.py
--rw-r--r--   0        0        0     1638 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/api_call_query_group.py
--rw-r--r--   0        0        0      268 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/api_call_query_group_by.py
--rw-r--r--   0        0        0      248 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/api_call_status.py
--rw-r--r--   0        0        0     8246 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/api_call_with_price.py
--rw-r--r--   0        0        0     2087 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/api_call_with_price_results_page.py
--rw-r--r--   0        0        0     3218 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/api_token.py
--rw-r--r--   0        0        0     1963 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/api_token_results_page.py
--rw-r--r--   0        0        0     1396 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/app_client_info.py
--rw-r--r--   0        0        0     5846 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/async_api_call.py
--rw-r--r--   0        0        0     2025 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/async_api_call_results_page.py
--rw-r--r--   0        0        0      395 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/async_api_call_type.py
--rw-r--r--   0        0        0     2131 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/billing_info.py
--rw-r--r--   0        0        0     1384 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/cache_metadata.py
--rw-r--r--   0        0        0     3356 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/card_details.py
--rw-r--r--   0        0        0     2663 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/cluster.py
--rw-r--r--   0        0        0      171 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/code_language.py
--rw-r--r--   0        0        0     2193 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/code_output.py
--rw-r--r--   0        0        0     1574 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/commit.py
--rw-r--r--   0        0        0    14432 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/connection.py
--rw-r--r--   0        0        0     3602 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/country_code.py
--rw-r--r--   0        0        0      224 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/created_at_sort_mode.py
--rw-r--r--   0        0        0     2337 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/currency.py
--rw-r--r--   0        0        0     4342 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/customer.py
--rw-r--r--   0        0        0     4238 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/customer_balance.py
--rw-r--r--   0        0        0     2413 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/device_access_token_request_form.py
--rw-r--r--   0        0        0     1499 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/device_auth_request_form.py
--rw-r--r--   0        0        0     1504 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/device_auth_verify_params.py
--rw-r--r--   0        0        0    21726 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/docker_system_info.py
--rw-r--r--   0        0        0     1735 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/email_authentication_form.py
--rw-r--r--   0        0        0     3925 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/engine_metadata.py
--rw-r--r--   0        0        0      202 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/environment.py
--rw-r--r--   0        0        0     1888 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/error.py
--rw-r--r--   0        0        0     2707 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/executor_metadata.py
--rw-r--r--   0        0        0     5849 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/extended_user.py
--rw-r--r--   0        0        0     2019 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/extended_user_results_page.py
--rw-r--r--   0        0        0     6350 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file2_d_vector_conversion.py
--rw-r--r--   0        0        0      191 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file2_d_vector_export_format.py
--rw-r--r--   0        0        0      161 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file2_d_vector_import_format.py
--rw-r--r--   0        0        0      261 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file3_d_import_format.py
--rw-r--r--   0        0        0     5799 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_center_of_mass.py
--rw-r--r--   0        0        0     6220 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_conversion.py
--rw-r--r--   0        0        0     5837 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_density.py
--rw-r--r--   0        0        0      269 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_export_format.py
--rw-r--r--   0        0        0      275 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_import_format.py
--rw-r--r--   0        0        0     5822 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_mass.py
--rw-r--r--   0        0        0     5629 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_surface_area.py
--rw-r--r--   0        0        0     1412 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_system_metadata.py
--rw-r--r--   0        0        0     5541 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_volume.py
--rw-r--r--   0        0        0     2276 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/gateway.py
--rw-r--r--   0        0        0      146 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/image_type.py
--rw-r--r--   0        0        0     2166 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/index_info.py
--rw-r--r--   0        0        0     8343 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/invoice.py
--rw-r--r--   0        0        0     2909 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/invoice_line_item.py
--rw-r--r--   0        0        0      252 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/invoice_status.py
--rw-r--r--   0        0        0     2777 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/jetstream.py
--rw-r--r--   0        0        0     1874 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/jetstream_api_stats.py
--rw-r--r--   0        0        0     2180 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/jetstream_config.py
--rw-r--r--   0        0        0     3190 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/jetstream_stats.py
--rw-r--r--   0        0        0     2095 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/leaf_node.py
--rw-r--r--   0        0        0     1355 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/mesh.py
--rw-r--r--   0        0        0     1894 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/meta_cluster_info.py
--rw-r--r--   0        0        0     5250 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/metadata.py
--rw-r--r--   0        0        0      317 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/method.py
--rw-r--r--   0        0        0     2967 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/new_address.py
--rw-r--r--   0        0        0     1992 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/o_auth2_client_info.py
--rw-r--r--   0        0        0      218 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/o_auth2_grant_type.py
--rw-r--r--   0        0        0     2449 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/onboarding.py
--rw-r--r--   0        0        0     1617 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/output_file.py
--rw-r--r--   0        0        0     1493 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/payment_intent.py
--rw-r--r--   0        0        0     3874 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/payment_method.py
--rw-r--r--   0        0        0     2247 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/payment_method_card_checks.py
--rw-r--r--   0        0        0      140 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/payment_method_type.py
--rw-r--r--   0        0        0     5526 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/physics_constant.py
--rw-r--r--   0        0        0     1024 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/physics_constant_name.py
--rw-r--r--   0        0        0     2588 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/plugins_info.py
--rw-r--r--   0        0        0     1392 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/point_e_metadata.py
--rw-r--r--   0        0        0     1385 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/pong.py
--rw-r--r--   0        0        0     4159 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/registry_service_config.py
--rw-r--r--   0        0        0     1773 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/runtime.py
--rw-r--r--   0        0        0     3573 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/session.py
--rw-r--r--   0        0        0      214 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/system_info_cgroup_driver_enum.py
--rw-r--r--   0        0        0      175 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/system_info_cgroup_version_enum.py
--rw-r--r--   0        0        0     1681 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/system_info_default_address_pools.py
--rw-r--r--   0        0        0      213 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/system_info_isolation_enum.py
--rw-r--r--   0        0        0     6477 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_acceleration_conversion.py
--rw-r--r--   0        0        0      285 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_acceleration_format.py
--rw-r--r--   0        0        0     6386 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_angle_conversion.py
--rw-r--r--   0        0        0      300 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_angle_format.py
--rw-r--r--   0        0        0     6520 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_angular_velocity_conversion.py
--rw-r--r--   0        0        0      334 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_angular_velocity_format.py
--rw-r--r--   0        0        0     6373 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_area_conversion.py
--rw-r--r--   0        0        0      333 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_area_format.py
--rw-r--r--   0        0        0     6399 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_charge_conversion.py
--rw-r--r--   0        0        0      177 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_charge_format.py
--rw-r--r--   0        0        0     6490 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_concentration_conversion.py
--rw-r--r--   0        0        0      286 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_concentration_format.py
--rw-r--r--   0        0        0     6373 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_data_conversion.py
--rw-r--r--   0        0        0      199 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_data_format.py
--rw-r--r--   0        0        0     6537 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_data_transfer_rate_conversion.py
--rw-r--r--   0        0        0      307 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_data_transfer_rate_format.py
--rw-r--r--   0        0        0     6412 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_density_conversion.py
--rw-r--r--   0        0        0      626 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_density_format.py
--rw-r--r--   0        0        0     6399 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_energy_conversion.py
--rw-r--r--   0        0        0      441 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_energy_format.py
--rw-r--r--   0        0        0     6386 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_force_conversion.py
--rw-r--r--   0        0        0      230 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_force_format.py
--rw-r--r--   0        0        0     6464 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_illuminance_conversion.py
--rw-r--r--   0        0        0      244 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_illuminance_format.py
--rw-r--r--   0        0        0     6399 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_length_conversion.py
--rw-r--r--   0        0        0      639 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_length_format.py
--rw-r--r--   0        0        0     6602 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_magnetic_field_strength_conversion.py
--rw-r--r--   0        0        0      176 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_magnetic_field_strength_format.py
--rw-r--r--   0        0        0     6481 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_magnetic_flux_conversion.py
--rw-r--r--   0        0        0      171 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_magnetic_flux_format.py
--rw-r--r--   0        0        0     6373 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_mass_conversion.py
--rw-r--r--   0        0        0      345 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_mass_format.py
--rw-r--r--   0        0        0      434 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_metric_power.py
--rw-r--r--   0        0        0     6419 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_metric_power_conversion.py
--rw-r--r--   0        0        0     6447 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_metric_power_cubed_conversion.py
--rw-r--r--   0        0        0     6457 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_metric_power_squared_conversion.py
--rw-r--r--   0        0        0     6386 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_power_conversion.py
--rw-r--r--   0        0        0      196 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_power_format.py
--rw-r--r--   0        0        0     6425 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_pressure_conversion.py
--rw-r--r--   0        0        0      263 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_pressure_format.py
--rw-r--r--   0        0        0     6438 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_radiation_conversion.py
--rw-r--r--   0        0        0      182 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_radiation_format.py
--rw-r--r--   0        0        0     6490 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_radioactivity_conversion.py
--rw-r--r--   0        0        0      206 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_radioactivity_format.py
--rw-r--r--   0        0        0     6455 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_solid_angle_conversion.py
--rw-r--r--   0        0        0      209 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_solid_angle_format.py
--rw-r--r--   0        0        0     6464 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_temperature_conversion.py
--rw-r--r--   0        0        0      250 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_temperature_format.py
--rw-r--r--   0        0        0     6373 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_time_conversion.py
--rw-r--r--   0        0        0      303 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_time_format.py
--rw-r--r--   0        0        0     6425 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_velocity_conversion.py
--rw-r--r--   0        0        0      311 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_velocity_format.py
--rw-r--r--   0        0        0     6412 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_voltage_conversion.py
--rw-r--r--   0        0        0      188 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_voltage_format.py
--rw-r--r--   0        0        0     6399 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_volume_conversion.py
--rw-r--r--   0        0        0      865 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_volume_format.py
--rw-r--r--   0        0        0     2533 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/update_user.py
--rw-r--r--   0        0        0     5069 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/user.py
--rw-r--r--   0        0        0     1901 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/user_results_page.py
--rw-r--r--   0        0        0       68 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/uuid.py
--rw-r--r--   0        0        0     3346 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/verification_token.py
--rw-r--r--   0        0        0       25 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/py.typed
--rw-r--r--   0        0        0      984 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/types.py
--rw-r--r--   0        0        0     1058 2023-04-17 21:11:23.031788 kittycad-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 kittycad-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-04 07:58:53.116393 kittycad-0.3.8/LICENSE
+-rw-r--r--   0        0        0      875 2023-05-04 07:58:53.116393 kittycad-0.3.8/README.md
+-rw-r--r--   0        0        0       48 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/ai/__init__.py
+-rw-r--r--   0        0        0     3747 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/ai/create_image_to_3d.py
+-rw-r--r--   0        0        0     3525 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/ai/create_text_to_3d.py
+-rw-r--r--   0        0        0      199 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/__init__.py
+-rw-r--r--   0        0        0     3082 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/get_api_call.py
+-rw-r--r--   0        0        0     2771 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/get_api_call_for_user.py
+-rw-r--r--   0        0        0     3215 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/get_api_call_metrics.py
+-rw-r--r--   0        0        0     6031 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/get_async_operation.py
+-rw-r--r--   0        0        0     4208 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/list_api_calls.py
+-rw-r--r--   0        0        0     4977 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/list_api_calls_for_user.py
+-rw-r--r--   0        0        0     4787 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/list_async_operations.py
+-rw-r--r--   0        0        0     4323 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_calls/user_list_api_calls.py
+-rw-r--r--   0        0        0      352 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_tokens/__init__.py
+-rw-r--r--   0        0        0     2551 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_tokens/create_api_token_for_user.py
+-rw-r--r--   0        0        0     2976 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_tokens/delete_api_token_for_user.py
+-rw-r--r--   0        0        0     2762 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_tokens/get_api_token_for_user.py
+-rw-r--r--   0        0        0     4256 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/api_tokens/list_api_tokens_for_user.py
+-rw-r--r--   0        0        0      116 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/apps/__init__.py
+-rw-r--r--   0        0        0     2694 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/apps/apps_github_callback.py
+-rw-r--r--   0        0        0     2883 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/apps/apps_github_consent.py
+-rw-r--r--   0        0        0     2435 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/apps/apps_github_webhook.py
+-rw-r--r--   0        0        0      156 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/beta/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/constant/__init__.py
+-rw-r--r--   0        0        0     2730 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/constant/get_physics_constant.py
+-rw-r--r--   0        0        0      142 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/drawing/__init__.py
+-rw-r--r--   0        0        0     2752 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/drawing/cmd.py
+-rw-r--r--   0        0        0     2656 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/drawing/cmd_batch.py
+-rw-r--r--   0        0        0      161 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/executor/__init__.py
+-rw-r--r--   0        0        0     1930 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/executor/create_executor_term.py
+-rw-r--r--   0        0        0     3173 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/executor/create_file_execution.py
+-rw-r--r--   0        0        0      233 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/__init__.py
+-rw-r--r--   0        0        0     3843 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/create_file_center_of_mass.py
+-rw-r--r--   0        0        0     4433 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/create_file_conversion.py
+-rw-r--r--   0        0        0     1962 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/create_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0     4254 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/create_file_density.py
+-rw-r--r--   0        0        0     4272 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/create_file_mass.py
+-rw-r--r--   0        0        0     3827 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/create_file_surface_area.py
+-rw-r--r--   0        0        0     3763 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/create_file_volume.py
+-rw-r--r--   0        0        0     1341 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/file/get_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0      133 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/hidden/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/hidden/auth_email.py
+-rw-r--r--   0        0        0     3317 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/hidden/auth_email_callback.py
+-rw-r--r--   0        0        0     2236 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/hidden/logout.py
+-rw-r--r--   0        0        0      105 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/meta/__init__.py
+-rw-r--r--   0        0        0     2355 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/meta/get_ai_plugin_manifest.py
+-rw-r--r--   0        0        0     2607 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/meta/get_metadata.py
+-rw-r--r--   0        0        0     1913 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/meta/get_metrics.py
+-rw-r--r--   0        0        0     2530 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/meta/get_openai_schema.py
+-rw-r--r--   0        0        0     2159 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/meta/get_schema.py
+-rw-r--r--   0        0        0     2211 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/meta/ping.py
+-rw-r--r--   0        0        0      123 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/oauth2/__init__.py
+-rw-r--r--   0        0        0      117 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/__init__.py
+-rw-r--r--   0        0        0     2934 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/create_payment_information_for_user.py
+-rw-r--r--   0        0        0     2610 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/create_payment_intent_for_user.py
+-rw-r--r--   0        0        0     2528 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/delete_payment_information_for_user.py
+-rw-r--r--   0        0        0     2583 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/delete_payment_method_for_user.py
+-rw-r--r--   0        0        0     2627 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/get_payment_balance_for_user.py
+-rw-r--r--   0        0        0     2659 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/get_payment_information_for_user.py
+-rw-r--r--   0        0        0     2588 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/list_invoices_for_user.py
+-rw-r--r--   0        0        0     2656 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/list_payment_methods_for_user.py
+-rw-r--r--   0        0        0     2932 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/update_payment_information_for_user.py
+-rw-r--r--   0        0        0     2580 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/payments/validate_customer_tax_information_for_user.py
+-rw-r--r--   0        0        0      101 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/unit/__init__.py
+-rw-r--r--   0        0        0     3938 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/unit/get_acceleration_unit_conversion.py
+-rw-r--r--   0        0        0     3756 2023-05-04 07:58:53.404393 kittycad-0.3.8/kittycad/api/unit/get_angle_unit_conversion.py
+-rw-r--r--   0        0        0     4023 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_angular_velocity_unit_conversion.py
+-rw-r--r--   0        0        0     3730 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_area_unit_conversion.py
+-rw-r--r--   0        0        0     3780 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_charge_unit_conversion.py
+-rw-r--r--   0        0        0     3962 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_concentration_unit_conversion.py
+-rw-r--r--   0        0        0     4054 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py
+-rw-r--r--   0        0        0     3728 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_data_unit_conversion.py
+-rw-r--r--   0        0        0     3806 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_density_unit_conversion.py
+-rw-r--r--   0        0        0     3780 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_energy_unit_conversion.py
+-rw-r--r--   0        0        0     3754 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_force_unit_conversion.py
+-rw-r--r--   0        0        0     3910 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_illuminance_unit_conversion.py
+-rw-r--r--   0        0        0     3780 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_length_unit_conversion.py
+-rw-r--r--   0        0        0     4202 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py
+-rw-r--r--   0        0        0     3943 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_magnetic_flux_unit_conversion.py
+-rw-r--r--   0        0        0     3728 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_mass_unit_conversion.py
+-rw-r--r--   0        0        0     3890 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py
+-rw-r--r--   0        0        0     3927 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_metric_power_squared_unit_conversion.py
+-rw-r--r--   0        0        0     3820 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_metric_power_unit_conversion.py
+-rw-r--r--   0        0        0     3754 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_power_unit_conversion.py
+-rw-r--r--   0        0        0     3832 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_pressure_unit_conversion.py
+-rw-r--r--   0        0        0     3858 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_radiation_unit_conversion.py
+-rw-r--r--   0        0        0     3962 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_radioactivity_unit_conversion.py
+-rw-r--r--   0        0        0     3891 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_solid_angle_unit_conversion.py
+-rw-r--r--   0        0        0     3910 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_temperature_unit_conversion.py
+-rw-r--r--   0        0        0     3728 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_time_unit_conversion.py
+-rw-r--r--   0        0        0     3832 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_velocity_unit_conversion.py
+-rw-r--r--   0        0        0     3806 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_voltage_unit_conversion.py
+-rw-r--r--   0        0        0     3780 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/unit/get_volume_unit_conversion.py
+-rw-r--r--   0        0        0      297 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/__init__.py
+-rw-r--r--   0        0        0     2676 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/delete_user_self.py
+-rw-r--r--   0        0        0     2735 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/get_session_for_user.py
+-rw-r--r--   0        0        0     3027 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/get_user.py
+-rw-r--r--   0        0        0     3157 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/get_user_extended.py
+-rw-r--r--   0        0        0     2446 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/get_user_front_hash_self.py
+-rw-r--r--   0        0        0     2484 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/get_user_onboarding_self.py
+-rw-r--r--   0        0        0     2489 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/get_user_self.py
+-rw-r--r--   0        0        0     2601 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/get_user_self_extended.py
+-rw-r--r--   0        0        0     4077 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/list_users.py
+-rw-r--r--   0        0        0     4159 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/list_users_extended.py
+-rw-r--r--   0        0        0     2745 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/api/users/update_user_self.py
+-rw-r--r--   0        0        0     2297 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/client.py
+-rw-r--r--   0        0        0     4725 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/client_test.py
+-rw-r--r--   0        0        0    87053 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/examples_test.py
+-rw-r--r--   0        0        0     7838 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/__init__.py
+-rw-r--r--   0        0        0      322 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/account_provider.py
+-rw-r--r--   0        0        0     2249 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/ai_plugin_api.py
+-rw-r--r--   0        0        0      242 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/ai_plugin_api_type.py
+-rw-r--r--   0        0        0     2440 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/ai_plugin_auth.py
+-rw-r--r--   0        0        0      413 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/ai_plugin_auth_type.py
+-rw-r--r--   0        0        0      287 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/ai_plugin_http_auth_type.py
+-rw-r--r--   0        0        0     4685 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/ai_plugin_manifest.py
+-rw-r--r--   0        0        0     1720 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/api_call_query_group.py
+-rw-r--r--   0        0        0      777 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/api_call_query_group_by.py
+-rw-r--r--   0        0        0      620 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/api_call_status.py
+-rw-r--r--   0        0        0     8266 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/api_call_with_price.py
+-rw-r--r--   0        0        0     2128 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/api_call_with_price_results_page.py
+-rw-r--r--   0        0        0     3278 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/api_token.py
+-rw-r--r--   0        0        0     2004 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/api_token_results_page.py
+-rw-r--r--   0        0        0     1447 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/app_client_info.py
+-rw-r--r--   0        0        0     5747 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/async_api_call.py
+-rw-r--r--   0        0        0    34040 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/async_api_call_output.py
+-rw-r--r--   0        0        0     2066 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/async_api_call_results_page.py
+-rw-r--r--   0        0        0      648 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/async_api_call_type.py
+-rw-r--r--   0        0        0     2127 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/billing_info.py
+-rw-r--r--   0        0        0     1479 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/cache_metadata.py
+-rw-r--r--   0        0        0     3353 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/card_details.py
+-rw-r--r--   0        0        0     2697 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/cluster.py
+-rw-r--r--   0        0        0      229 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/code_language.py
+-rw-r--r--   0        0        0     2244 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/code_output.py
+-rw-r--r--   0        0        0     1732 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/commit.py
+-rw-r--r--   0        0        0    14343 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/connection.py
+-rw-r--r--   0        0        0    13513 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/country_code.py
+-rw-r--r--   0        0        0      507 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/created_at_sort_mode.py
+-rw-r--r--   0        0        0     8623 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/currency.py
+-rw-r--r--   0        0        0     4298 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/customer.py
+-rw-r--r--   0        0        0     4306 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/customer_balance.py
+-rw-r--r--   0        0        0     2412 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/device_access_token_request_form.py
+-rw-r--r--   0        0        0     1580 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/device_auth_request_form.py
+-rw-r--r--   0        0        0     1606 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/device_auth_verify_params.py
+-rw-r--r--   0        0        0    21264 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/docker_system_info.py
+-rw-r--r--   0        0        0     3553 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/drawing_cmd.py
+-rw-r--r--   0        0        0       75 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/drawing_cmd_id.py
+-rw-r--r--   0        0        0     2441 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/drawing_cmd_req.py
+-rw-r--r--   0        0        0     1746 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/drawing_cmd_req_batch.py
+-rw-r--r--   0        0        0     2393 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/drawing_error.py
+-rw-r--r--   0        0        0     1869 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/drawing_outcome.py
+-rw-r--r--   0        0        0     1505 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/drawing_outcomes.py
+-rw-r--r--   0        0        0     1789 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/email_authentication_form.py
+-rw-r--r--   0        0        0     3847 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/engine_metadata.py
+-rw-r--r--   0        0        0      269 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/environment.py
+-rw-r--r--   0        0        0     1930 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/error.py
+-rw-r--r--   0        0        0     2715 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/executor_metadata.py
+-rw-r--r--   0        0        0     6069 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/extended_user.py
+-rw-r--r--   0        0        0     2060 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/extended_user_results_page.py
+-rw-r--r--   0        0        0     5700 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_center_of_mass.py
+-rw-r--r--   0        0        0     6060 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_conversion.py
+-rw-r--r--   0        0        0     5725 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_density.py
+-rw-r--r--   0        0        0     1369 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_export_format.py
+-rw-r--r--   0        0        0     1306 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_import_format.py
+-rw-r--r--   0        0        0     5707 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_mass.py
+-rw-r--r--   0        0        0     5522 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_surface_area.py
+-rw-r--r--   0        0        0     1513 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_system_metadata.py
+-rw-r--r--   0        0        0     5428 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/file_volume.py
+-rw-r--r--   0        0        0     2304 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/gateway.py
+-rw-r--r--   0        0        0      187 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/image_type.py
+-rw-r--r--   0        0        0     2228 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/index_info.py
+-rw-r--r--   0        0        0     8273 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/invoice.py
+-rw-r--r--   0        0        0     2888 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/invoice_line_item.py
+-rw-r--r--   0        0        0      563 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/invoice_status.py
+-rw-r--r--   0        0        0     2666 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/jetstream.py
+-rw-r--r--   0        0        0     1907 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/jetstream_api_stats.py
+-rw-r--r--   0        0        0     2212 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/jetstream_config.py
+-rw-r--r--   0        0        0     3174 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/jetstream_stats.py
+-rw-r--r--   0        0        0     2125 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/leaf_node.py
+-rw-r--r--   0        0        0     1337 2023-05-04 07:58:53.408393 kittycad-0.3.8/kittycad/models/mesh.py
+-rw-r--r--   0        0        0     1923 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/meta_cluster_info.py
+-rw-r--r--   0        0        0     5025 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/metadata.py
+-rw-r--r--   0        0        0     1788 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/method.py
+-rw-r--r--   0        0        0     3081 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/new_address.py
+-rw-r--r--   0        0        0     2038 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/o_auth2_client_info.py
+-rw-r--r--   0        0        0      415 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/o_auth2_grant_type.py
+-rw-r--r--   0        0        0     2501 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/onboarding.py
+-rw-r--r--   0        0        0     1646 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/output_file.py
+-rw-r--r--   0        0        0     1527 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/payment_intent.py
+-rw-r--r--   0        0        0     3753 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/payment_method.py
+-rw-r--r--   0        0        0     2267 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/payment_method_card_checks.py
+-rw-r--r--   0        0        0      294 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/payment_method_type.py
+-rw-r--r--   0        0        0     5424 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/physics_constant.py
+-rw-r--r--   0        0        0     4448 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/physics_constant_name.py
+-rw-r--r--   0        0        0     2809 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/plugins_info.py
+-rw-r--r--   0        0        0     1498 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/point_e_metadata.py
+-rw-r--r--   0        0        0     1432 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/pong.py
+-rw-r--r--   0        0        0     4187 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/registry_service_config.py
+-rw-r--r--   0        0        0     2034 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/runtime.py
+-rw-r--r--   0        0        0     3638 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/session.py
+-rw-r--r--   0        0        0      214 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/system_info_cgroup_driver_enum.py
+-rw-r--r--   0        0        0      175 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/system_info_cgroup_version_enum.py
+-rw-r--r--   0        0        0     1663 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/system_info_default_address_pools.py
+-rw-r--r--   0        0        0      213 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/system_info_isolation_enum.py
+-rw-r--r--   0        0        0     6317 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_acceleration_conversion.py
+-rw-r--r--   0        0        0      642 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_acceleration_format.py
+-rw-r--r--   0        0        0     6226 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_angle_conversion.py
+-rw-r--r--   0        0        0      916 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_angle_format.py
+-rw-r--r--   0        0        0     6360 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_angular_velocity_conversion.py
+-rw-r--r--   0        0        0      754 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_angular_velocity_format.py
+-rw-r--r--   0        0        0     6213 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_area_conversion.py
+-rw-r--r--   0        0        0      888 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_area_format.py
+-rw-r--r--   0        0        0     6239 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_charge_conversion.py
+-rw-r--r--   0        0        0      380 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_charge_format.py
+-rw-r--r--   0        0        0     6330 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_concentration_conversion.py
+-rw-r--r--   0        0        0      752 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_concentration_format.py
+-rw-r--r--   0        0        0     6213 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_data_conversion.py
+-rw-r--r--   0        0        0      539 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_data_format.py
+-rw-r--r--   0        0        0     6377 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_data_transfer_rate_conversion.py
+-rw-r--r--   0        0        0      656 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_data_transfer_rate_format.py
+-rw-r--r--   0        0        0     6252 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_density_conversion.py
+-rw-r--r--   0        0        0     1488 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_density_format.py
+-rw-r--r--   0        0        0     6239 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_energy_conversion.py
+-rw-r--r--   0        0        0     1162 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_energy_format.py
+-rw-r--r--   0        0        0     6226 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_force_conversion.py
+-rw-r--r--   0        0        0      645 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_force_format.py
+-rw-r--r--   0        0        0     6304 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_illuminance_conversion.py
+-rw-r--r--   0        0        0      584 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_illuminance_format.py
+-rw-r--r--   0        0        0     6239 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_length_conversion.py
+-rw-r--r--   0        0        0     2187 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_length_format.py
+-rw-r--r--   0        0        0     6442 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_magnetic_field_strength_conversion.py
+-rw-r--r--   0        0        0      402 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_magnetic_field_strength_format.py
+-rw-r--r--   0        0        0     6321 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_magnetic_flux_conversion.py
+-rw-r--r--   0        0        0      389 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_magnetic_flux_format.py
+-rw-r--r--   0        0        0     6213 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_mass_conversion.py
+-rw-r--r--   0        0        0     1094 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_mass_format.py
+-rw-r--r--   0        0        0     3438 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_metric_power.py
+-rw-r--r--   0        0        0     6259 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_metric_power_conversion.py
+-rw-r--r--   0        0        0     6287 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_metric_power_cubed_conversion.py
+-rw-r--r--   0        0        0     6297 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_metric_power_squared_conversion.py
+-rw-r--r--   0        0        0     6226 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_power_conversion.py
+-rw-r--r--   0        0        0      468 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_power_format.py
+-rw-r--r--   0        0        0     6265 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_pressure_conversion.py
+-rw-r--r--   0        0        0      725 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_pressure_format.py
+-rw-r--r--   0        0        0     6278 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_radiation_conversion.py
+-rw-r--r--   0        0        0      586 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_radiation_format.py
+-rw-r--r--   0        0        0     6330 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_radioactivity_conversion.py
+-rw-r--r--   0        0        0      570 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_radioactivity_format.py
+-rw-r--r--   0        0        0     6295 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_solid_angle_conversion.py
+-rw-r--r--   0        0        0      500 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_solid_angle_format.py
+-rw-r--r--   0        0        0     6304 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_temperature_conversion.py
+-rw-r--r--   0        0        0      674 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_temperature_format.py
+-rw-r--r--   0        0        0     6213 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_time_conversion.py
+-rw-r--r--   0        0        0      902 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_time_format.py
+-rw-r--r--   0        0        0     6265 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_velocity_conversion.py
+-rw-r--r--   0        0        0      753 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_velocity_format.py
+-rw-r--r--   0        0        0     6252 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_voltage_conversion.py
+-rw-r--r--   0        0        0      452 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_voltage_format.py
+-rw-r--r--   0        0        0     6239 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_volume_conversion.py
+-rw-r--r--   0        0        0     3286 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/unit_volume_format.py
+-rw-r--r--   0        0        0     2577 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/update_user.py
+-rw-r--r--   0        0        0     5084 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/user.py
+-rw-r--r--   0        0        0     1942 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/user_results_page.py
+-rw-r--r--   0        0        0       67 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/uuid.py
+-rw-r--r--   0        0        0     3448 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/models/verification_token.py
+-rw-r--r--   0        0        0       26 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/py.typed
+-rw-r--r--   0        0        0     1049 2023-05-04 07:58:53.412392 kittycad-0.3.8/kittycad/types.py
+-rw-r--r--   0        0        0     2416 2023-05-04 07:58:53.412392 kittycad-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 kittycad-0.3.8/PKG-INFO
```

### Comparing `kittycad-0.3.7/LICENSE` & `kittycad-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.7/README.md` & `kittycad-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.7/kittycad/api/ai/create_image_to_3d.py` & `kittycad-0.3.8/kittycad/api/ai/create_text_to_3d.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,130 +1,127 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.mesh import Mesh
 from ...models.error import Error
-from ...models.image_type import ImageType
 from ...models.file_export_format import FileExportFormat
+from ...models.mesh import Mesh
 from ...types import Response
 
+
 def _get_kwargs(
-	input_format: ImageType,
-	output_format: FileExportFormat,
-	body: bytes,
-	*,
-	client: Client,
+    output_format: FileExportFormat,
+    prompt: str,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/ai/image-to-3d/{input_format}/{output_format}".format(client.base_url, input_format=input_format, output_format=output_format)
-
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
-
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-		"content": body,
-	}
+    url = "{}/ai/text-to-3d/{output_format}".format(
+        client.base_url, output_format=output_format
+    )  # noqa: E501
+    if prompt is not None:
+        if "?" in url:
+            url = url + "&prompt=" + str(prompt)
+        else:
+            url = url + "?prompt=" + str(prompt)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
 
 
 def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Mesh, Error]]:
-	if response.status_code == 200:
-		response_200 = Mesh.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
+    if response.status_code == 200:
+        response_200 = Mesh.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
 
 
 def _build_response(*, response: httpx.Response) -> Response[Union[Any, Mesh, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	input_format: ImageType,
-	output_format: FileExportFormat,
-	body: bytes,
-	*,
-	client: Client,
+    output_format: FileExportFormat,
+    prompt: str,
+    *,
+    client: Client,
 ) -> Response[Union[Any, Mesh, Error]]:
-	kwargs = _get_kwargs(
-		input_format=input_format,
-		output_format=output_format,
-		body=body,
-		client=client,
-	)
-
-	response = httpx.post(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        prompt=prompt,
+        client=client,
+    )
+
+    response = httpx.post(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	input_format: ImageType,
-	output_format: FileExportFormat,
-	body: bytes,
-	*,
-	client: Client,
+    output_format: FileExportFormat,
+    prompt: str,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, Mesh, Error]]:
-	""" This is an alpha endpoint. It will change in the future. The current output is honestly pretty bad. So if you find this endpoint, you get what you pay for, which currently is nothing. But in the future will be made a lot better. """
+    """This is an alpha endpoint. It will change in the future. The current output is honestly pretty bad. So if you find this endpoint, you get what you pay for, which currently is nothing. But in the future will be made a lot better."""  # noqa: E501
 
-	return sync_detailed(
-		input_format=input_format,
-		output_format=output_format,
-		body=body,
-		client=client,
-	).parsed
+    return sync_detailed(
+        output_format=output_format,
+        prompt=prompt,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	input_format: ImageType,
-	output_format: FileExportFormat,
-	body: bytes,
-	*,
-	client: Client,
+    output_format: FileExportFormat,
+    prompt: str,
+    *,
+    client: Client,
 ) -> Response[Union[Any, Mesh, Error]]:
-	kwargs = _get_kwargs(
-		input_format=input_format,
-		output_format=output_format,
-		body=body,
-		client=client,
-	)
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        prompt=prompt,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.post(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.post(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	input_format: ImageType,
-	output_format: FileExportFormat,
-	body: bytes,
-	*,
-	client: Client,
+    output_format: FileExportFormat,
+    prompt: str,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, Mesh, Error]]:
-	""" This is an alpha endpoint. It will change in the future. The current output is honestly pretty bad. So if you find this endpoint, you get what you pay for, which currently is nothing. But in the future will be made a lot better. """
+    """This is an alpha endpoint. It will change in the future. The current output is honestly pretty bad. So if you find this endpoint, you get what you pay for, which currently is nothing. But in the future will be made a lot better."""  # noqa: E501
 
-	return (
-		await asyncio_detailed(
-		input_format=input_format,
-		output_format=output_format,
-		body=body,
-			client=client,
-		)
-	).parsed
+    return (
+        await asyncio_detailed(
+            output_format=output_format,
+            prompt=prompt,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/api_calls/get_api_call.py` & `kittycad-0.3.8/kittycad/api/payments/create_payment_information_for_user.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,113 +1,118 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.api_call_with_price import ApiCallWithPrice
+from ...models.billing_info import BillingInfo
+from ...models.customer import Customer
 from ...models.error import Error
 from ...types import Response
 
+
 def _get_kwargs(
-	id: str,
-	*,
-	client: Client,
+    body: BillingInfo,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/api-calls/{id}".format(client.base_url, id=id)
+    url = "{}/user/payment".format(client.base_url)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ApiCallWithPrice, Error]]:
-	if response.status_code == 200:
-		response_200 = ApiCallWithPrice.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ApiCallWithPrice, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "content": body,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, Customer, Error]]:
+    if response.status_code == 201:
+        response_201 = Customer.from_dict(response.json())
+        return response_201
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, Customer, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	id: str,
-	*,
-	client: Client,
-) -> Response[Union[Any, ApiCallWithPrice, Error]]:
-	kwargs = _get_kwargs(
-		id=id,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    body: BillingInfo,
+    *,
+    client: Client,
+) -> Response[Union[Any, Customer, Error]]:
+    kwargs = _get_kwargs(
+        body=body,
+        client=client,
+    )
+
+    response = httpx.post(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	id: str,
-	*,
-	client: Client,
-) -> Optional[Union[Any, ApiCallWithPrice, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It returns details of the requested API call for the user.
-If the user is not authenticated to view the specified API call, then it is not returned.
-Only KittyCAD employees can view API calls for other users. """
-
-	return sync_detailed(
-		id=id,
-		client=client,
-	).parsed
+    body: BillingInfo,
+    *,
+    client: Client,
+) -> Optional[Union[Any, Customer, Error]]:
+    """This includes billing address, phone, and name.
+    This endpoint requires authentication by any KittyCAD user. It creates the payment information for the authenticated user."""  # noqa: E501
+
+    return sync_detailed(
+        body=body,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	id: str,
-	*,
-	client: Client,
-) -> Response[Union[Any, ApiCallWithPrice, Error]]:
-	kwargs = _get_kwargs(
-		id=id,
-		client=client,
-	)
+    body: BillingInfo,
+    *,
+    client: Client,
+) -> Response[Union[Any, Customer, Error]]:
+    kwargs = _get_kwargs(
+        body=body,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.post(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	id: str,
-	*,
-	client: Client,
-) -> Optional[Union[Any, ApiCallWithPrice, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It returns details of the requested API call for the user.
-If the user is not authenticated to view the specified API call, then it is not returned.
-Only KittyCAD employees can view API calls for other users. """
-
-	return (
-		await asyncio_detailed(
-		id=id,
-			client=client,
-		)
-	).parsed
+    body: BillingInfo,
+    *,
+    client: Client,
+) -> Optional[Union[Any, Customer, Error]]:
+    """This includes billing address, phone, and name.
+    This endpoint requires authentication by any KittyCAD user. It creates the payment information for the authenticated user."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            body=body,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/api_calls/get_api_call_for_user.py` & `kittycad-0.3.8/kittycad/api/meta/get_openai_schema.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,109 +1,100 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.api_call_with_price import ApiCallWithPrice
 from ...models.error import Error
 from ...types import Response
 
+
 def _get_kwargs(
-	id: str,
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/user/api-calls/{id}".format(client.base_url, id=id)
+    url = "{}/openai/openapi.json".format(client.base_url)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ApiCallWithPrice, Error]]:
-	if response.status_code == 200:
-		response_200 = ApiCallWithPrice.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ApiCallWithPrice, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, dict, Error]]:
+    if response.status_code == 200:
+        response_200 = response.json()
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, dict, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	id: str,
-	*,
-	client: Client,
-) -> Response[Union[Any, ApiCallWithPrice, Error]]:
-	kwargs = _get_kwargs(
-		id=id,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, dict, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	id: str,
-	*,
-	client: Client,
-) -> Optional[Union[Any, ApiCallWithPrice, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It returns details of the requested API call for the user. """
-
-	return sync_detailed(
-		id=id,
-		client=client,
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, dict, Error]]:
+    """This is the same as the OpenAPI schema, BUT it has some modifications to make it compatible with OpenAI. For example, descriptions must be < 300 chars."""  # noqa: E501
+
+    return sync_detailed(
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	id: str,
-	*,
-	client: Client,
-) -> Response[Union[Any, ApiCallWithPrice, Error]]:
-	kwargs = _get_kwargs(
-		id=id,
-		client=client,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, dict, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	id: str,
-	*,
-	client: Client,
-) -> Optional[Union[Any, ApiCallWithPrice, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It returns details of the requested API call for the user. """
-
-	return (
-		await asyncio_detailed(
-		id=id,
-			client=client,
-		)
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, dict, Error]]:
+    """This is the same as the OpenAPI schema, BUT it has some modifications to make it compatible with OpenAI. For example, descriptions must be < 300 chars."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/api_calls/get_api_call_metrics.py` & `kittycad-0.3.8/kittycad/api/users/delete_user_self.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,113 +1,102 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.api_call_query_group import ApiCallQueryGroup
 from ...models.error import Error
-from ...models.api_call_query_group_by import ApiCallQueryGroupBy
 from ...types import Response
 
+
 def _get_kwargs(
-	group_by: ApiCallQueryGroupBy,
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/api-call-metrics?group_by={group_by}".format(client.base_url, group_by=group_by)
+    url = "{}/user".format(client.base_url)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, [ApiCallQueryGroup], Error]]:
-	if response.status_code == 200:
-		response_200 = [
-			ApiCallQueryGroup.from_dict(item)
-			for item in response.json()
-		]
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, [ApiCallQueryGroup], Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
+    if response.status_code == 204:
+        response_204 = None
+        return response_204
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	group_by: ApiCallQueryGroupBy,
-	*,
-	client: Client,
-) -> Response[Union[Any, [ApiCallQueryGroup], Error]]:
-	kwargs = _get_kwargs(
-		group_by=group_by,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
+
+    response = httpx.delete(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	group_by: ApiCallQueryGroupBy,
-	*,
-	client: Client,
-) -> Optional[Union[Any, [ApiCallQueryGroup], Error]]:
-	""" This endpoint requires authentication by a KittyCAD employee. The API calls are grouped by the parameter passed. """
-
-	return sync_detailed(
-		group_by=group_by,
-		client=client,
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It deletes the authenticated user from KittyCAD's database.
+    This call will only succeed if all invoices associated with the user have been paid in full and there is no outstanding balance."""  # noqa: E501
+
+    return sync_detailed(
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	group_by: ApiCallQueryGroupBy,
-	*,
-	client: Client,
-) -> Response[Union[Any, [ApiCallQueryGroup], Error]]:
-	kwargs = _get_kwargs(
-		group_by=group_by,
-		client=client,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.delete(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	group_by: ApiCallQueryGroupBy,
-	*,
-	client: Client,
-) -> Optional[Union[Any, [ApiCallQueryGroup], Error]]:
-	""" This endpoint requires authentication by a KittyCAD employee. The API calls are grouped by the parameter passed. """
-
-	return (
-		await asyncio_detailed(
-		group_by=group_by,
-			client=client,
-		)
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It deletes the authenticated user from KittyCAD's database.
+    This call will only succeed if all invoices associated with the user have been paid in full and there is no outstanding balance."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/api_calls/list_async_operations.py` & `kittycad-0.3.8/kittycad/api/users/list_users_extended.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,140 +1,148 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.async_api_call_results_page import AsyncApiCallResultsPage
-from ...models.error import Error
 from ...models.created_at_sort_mode import CreatedAtSortMode
-from ...models.api_call_status import ApiCallStatus
+from ...models.error import Error
+from ...models.extended_user_results_page import ExtendedUserResultsPage
 from ...types import Response
 
+
 def _get_kwargs(
-	sort_by: CreatedAtSortMode,
-	status: ApiCallStatus,
-	*,
-	client: Client,
-	limit: Optional[int] = None,
-	page_token: Optional[str] = None,
+    sort_by: CreatedAtSortMode,
+    *,
+    client: Client,
+    limit: Optional[int] = None,
+    page_token: Optional[str] = None,
 ) -> Dict[str, Any]:
-	url = "{}/async/operations?limit={limit}&page_token={page_token}&sort_by={sort_by}&status={status}".format(client.base_url, limit=limit, page_token=page_token, sort_by=sort_by, status=status)
-
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
-
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, AsyncApiCallResultsPage, Error]]:
-	if response.status_code == 200:
-		response_200 = AsyncApiCallResultsPage.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, AsyncApiCallResultsPage, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    url = "{}/users-extended".format(client.base_url)  # noqa: E501
+    if limit is not None:
+        if "?" in url:
+            url = url + "&limit=" + str(limit)
+        else:
+            url = url + "?limit=" + str(limit)
+    if page_token is not None:
+        if "?" in url:
+            url = url + "&page_token=" + str(page_token)
+        else:
+            url = url + "?page_token=" + str(page_token)
+    if sort_by is not None:
+        if "?" in url:
+            url = url + "&sort_by=" + str(sort_by)
+        else:
+            url = url + "?sort_by=" + str(sort_by)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, ExtendedUserResultsPage, Error]]:
+    if response.status_code == 200:
+        response_200 = ExtendedUserResultsPage.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, ExtendedUserResultsPage, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	sort_by: CreatedAtSortMode,
-	status: ApiCallStatus,
-	*,
-	client: Client,
-	limit: Optional[int] = None,
-	page_token: Optional[str] = None,
-) -> Response[Union[Any, AsyncApiCallResultsPage, Error]]:
-	kwargs = _get_kwargs(
-		limit=limit,
-		page_token=page_token,
-		sort_by=sort_by,
-		status=status,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    sort_by: CreatedAtSortMode,
+    *,
+    client: Client,
+    limit: Optional[int] = None,
+    page_token: Optional[str] = None,
+) -> Response[Union[Any, ExtendedUserResultsPage, Error]]:
+    kwargs = _get_kwargs(
+        limit=limit,
+        page_token=page_token,
+        sort_by=sort_by,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	sort_by: CreatedAtSortMode,
-	status: ApiCallStatus,
-	*,
-	client: Client,
-	limit: Optional[int] = None,
-	page_token: Optional[str] = None,
-) -> Optional[Union[Any, AsyncApiCallResultsPage, Error]]:
-	""" For async file conversion operations, this endpoint does not return the contents of converted files (`output`). To get the contents use the `/async/operations/{id}` endpoint.
-This endpoint requires authentication by a KittyCAD employee. """
-
-	return sync_detailed(
-		limit=limit,
-		page_token=page_token,
-		sort_by=sort_by,
-		status=status,
-		client=client,
-	).parsed
+    sort_by: CreatedAtSortMode,
+    *,
+    client: Client,
+    limit: Optional[int] = None,
+    page_token: Optional[str] = None,
+) -> Optional[Union[Any, ExtendedUserResultsPage, Error]]:
+    """This endpoint required authentication by a KittyCAD employee. The users are returned in order of creation, with the most recently created users first."""  # noqa: E501
+
+    return sync_detailed(
+        limit=limit,
+        page_token=page_token,
+        sort_by=sort_by,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	sort_by: CreatedAtSortMode,
-	status: ApiCallStatus,
-	*,
-	client: Client,
-	limit: Optional[int] = None,
-	page_token: Optional[str] = None,
-) -> Response[Union[Any, AsyncApiCallResultsPage, Error]]:
-	kwargs = _get_kwargs(
-		limit=limit,
-		page_token=page_token,
-		sort_by=sort_by,
-		status=status,
-		client=client,
-	)
+    sort_by: CreatedAtSortMode,
+    *,
+    client: Client,
+    limit: Optional[int] = None,
+    page_token: Optional[str] = None,
+) -> Response[Union[Any, ExtendedUserResultsPage, Error]]:
+    kwargs = _get_kwargs(
+        limit=limit,
+        page_token=page_token,
+        sort_by=sort_by,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	sort_by: CreatedAtSortMode,
-	status: ApiCallStatus,
-	*,
-	client: Client,
-	limit: Optional[int] = None,
-	page_token: Optional[str] = None,
-) -> Optional[Union[Any, AsyncApiCallResultsPage, Error]]:
-	""" For async file conversion operations, this endpoint does not return the contents of converted files (`output`). To get the contents use the `/async/operations/{id}` endpoint.
-This endpoint requires authentication by a KittyCAD employee. """
-
-	return (
-		await asyncio_detailed(
-		limit=limit,
-		page_token=page_token,
-		sort_by=sort_by,
-		status=status,
-			client=client,
-		)
-	).parsed
+    sort_by: CreatedAtSortMode,
+    *,
+    client: Client,
+    limit: Optional[int] = None,
+    page_token: Optional[str] = None,
+) -> Optional[Union[Any, ExtendedUserResultsPage, Error]]:
+    """This endpoint required authentication by a KittyCAD employee. The users are returned in order of creation, with the most recently created users first."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            limit=limit,
+            page_token=page_token,
+            sort_by=sort_by,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/api_tokens/delete_api_token_for_user.py` & `kittycad-0.3.8/kittycad/api/users/get_user_extended.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,118 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
+from ...models.extended_user import ExtendedUser
 from ...types import Response
 
+
 def _get_kwargs(
-	token: str,
-	*,
-	client: Client,
+    id: str,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/user/api-tokens/{token}".format(client.base_url, token=token)
+    url = "{}/users-extended/{id}".format(client.base_url, id=id)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
-	if response.status_code == 204:
-		response_204 = None
-		return response_204
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, ExtendedUser, Error]]:
+    if response.status_code == 200:
+        response_200 = ExtendedUser.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, ExtendedUser, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	token: str,
-	*,
-	client: Client,
-) -> Response[Union[Any, Error]]:
-	kwargs = _get_kwargs(
-		token=token,
-		client=client,
-	)
-
-	response = httpx.delete(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    id: str,
+    *,
+    client: Client,
+) -> Response[Union[Any, ExtendedUser, Error]]:
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	token: str,
-	*,
-	client: Client,
-) -> Optional[Union[Any, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It deletes the requested API token for the user.
-This endpoint does not actually delete the API token from the database. It merely marks the token as invalid. We still want to keep the token in the database for historical purposes. """
-
-	return sync_detailed(
-		token=token,
-		client=client,
-	).parsed
+    id: str,
+    *,
+    client: Client,
+) -> Optional[Union[Any, ExtendedUser, Error]]:
+    """To get information about yourself, use `/users-extended/me` as the endpoint. By doing so you will get the user information for the authenticated user.
+    Alternatively, to get information about the authenticated user, use `/user/extended` endpoint.
+    To get information about any KittyCAD user, you must be a KittyCAD employee."""  # noqa: E501
+
+    return sync_detailed(
+        id=id,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	token: str,
-	*,
-	client: Client,
-) -> Response[Union[Any, Error]]:
-	kwargs = _get_kwargs(
-		token=token,
-		client=client,
-	)
+    id: str,
+    *,
+    client: Client,
+) -> Response[Union[Any, ExtendedUser, Error]]:
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.delete(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	token: str,
-	*,
-	client: Client,
-) -> Optional[Union[Any, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It deletes the requested API token for the user.
-This endpoint does not actually delete the API token from the database. It merely marks the token as invalid. We still want to keep the token in the database for historical purposes. """
-
-	return (
-		await asyncio_detailed(
-		token=token,
-			client=client,
-		)
-	).parsed
+    id: str,
+    *,
+    client: Client,
+) -> Optional[Union[Any, ExtendedUser, Error]]:
+    """To get information about yourself, use `/users-extended/me` as the endpoint. By doing so you will get the user information for the authenticated user.
+    Alternatively, to get information about the authenticated user, use `/user/extended` endpoint.
+    To get information about any KittyCAD user, you must be a KittyCAD employee."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            id=id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/api_tokens/get_api_token_for_user.py` & `kittycad-0.3.8/kittycad/api/users/get_user_self.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,103 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.api_token import ApiToken
 from ...models.error import Error
+from ...models.user import User
 from ...types import Response
 
+
 def _get_kwargs(
-	token: str,
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/user/api-tokens/{token}".format(client.base_url, token=token)
+    url = "{}/user".format(client.base_url)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ApiToken, Error]]:
-	if response.status_code == 200:
-		response_200 = ApiToken.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ApiToken, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, User, Error]]:
+    if response.status_code == 200:
+        response_200 = User.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, User, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	token: str,
-	*,
-	client: Client,
-) -> Response[Union[Any, ApiToken, Error]]:
-	kwargs = _get_kwargs(
-		token=token,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, User, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	token: str,
-	*,
-	client: Client,
-) -> Optional[Union[Any, ApiToken, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It returns details of the requested API token for the user. """
-
-	return sync_detailed(
-		token=token,
-		client=client,
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, User, Error]]:
+    """Get the user information for the authenticated user.
+    Alternatively, you can also use the `/users/me` endpoint."""  # noqa: E501
+
+    return sync_detailed(
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	token: str,
-	*,
-	client: Client,
-) -> Response[Union[Any, ApiToken, Error]]:
-	kwargs = _get_kwargs(
-		token=token,
-		client=client,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, User, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	token: str,
-	*,
-	client: Client,
-) -> Optional[Union[Any, ApiToken, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It returns details of the requested API token for the user. """
-
-	return (
-		await asyncio_detailed(
-		token=token,
-			client=client,
-		)
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, User, Error]]:
+    """Get the user information for the authenticated user.
+    Alternatively, you can also use the `/users/me` endpoint."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/apps/apps_github_consent.py` & `kittycad-0.3.8/kittycad/api/payments/list_invoices_for_user.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,102 +1,105 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.app_client_info import AppClientInfo
 from ...models.error import Error
+from ...models.invoice import Invoice
 from ...types import Response
 
+
 def _get_kwargs(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/apps/github/consent".format(client.base_url)
+    url = "{}/user/payment/invoices".format(client.base_url)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, AppClientInfo, Error]]:
-	if response.status_code == 200:
-		response_200 = AppClientInfo.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, AppClientInfo, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, List[Invoice], Error]]:
+    if response.status_code == 200:
+        response_200 = [Invoice.from_dict(item) for item in response.json()]
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, List[Invoice], Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, AppClientInfo, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, List[Invoice], Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	*,
-	client: Client,
-) -> Optional[Union[Any, AppClientInfo, Error]]:
-	""" This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
-The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos. """
-
-	return sync_detailed(
-		client=client,
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, List[Invoice], Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It lists invoices for the authenticated user."""  # noqa: E501
+
+    return sync_detailed(
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, AppClientInfo, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, List[Invoice], Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	*,
-	client: Client,
-) -> Optional[Union[Any, AppClientInfo, Error]]:
-	""" This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
-The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos. """
-
-	return (
-		await asyncio_detailed(
-			client=client,
-		)
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, List[Invoice], Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It lists invoices for the authenticated user."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/apps/apps_github_webhook.py` & `kittycad-0.3.8/kittycad/api/hidden/logout.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,100 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
 from ...types import Response
 
+
 def _get_kwargs(
-	body: bytes,
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/apps/github/webhook".format(client.base_url)
+    url = "{}/logout".format(client.base_url)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-		"content": body,
-	}
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
 
 
 def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
-	if response.status_code == 204:
-		response_204 = None
-		return response_204
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
+    if response.status_code == 204:
+        response_204 = None
+        return response_204
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
 
 
 def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	body: bytes,
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Response[Union[Any, Error]]:
-	kwargs = _get_kwargs(
-		body=body,
-		client=client,
-	)
-
-	response = httpx.post(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    kwargs = _get_kwargs(
+        client=client,
+    )
+
+    response = httpx.post(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	body: bytes,
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, Error]]:
-	""" These come from the GitHub app. """
+    """This is used in logout scenarios."""  # noqa: E501
 
-	return sync_detailed(
-		body=body,
-		client=client,
-	).parsed
+    return sync_detailed(
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	body: bytes,
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Response[Union[Any, Error]]:
-	kwargs = _get_kwargs(
-		body=body,
-		client=client,
-	)
+    kwargs = _get_kwargs(
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.post(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.post(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	body: bytes,
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, Error]]:
-	""" These come from the GitHub app. """
+    """This is used in logout scenarios."""  # noqa: E501
 
-	return (
-		await asyncio_detailed(
-		body=body,
-			client=client,
-		)
-	).parsed
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/constant/get_physics_constant.py` & `kittycad-0.3.8/kittycad/api/constant/get_physics_constant.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,115 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.physics_constant import PhysicsConstant
 from ...models.error import Error
+from ...models.physics_constant import PhysicsConstant
 from ...models.physics_constant_name import PhysicsConstantName
 from ...types import Response
 
+
 def _get_kwargs(
-	constant: PhysicsConstantName,
-	*,
-	client: Client,
+    constant: PhysicsConstantName,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/constant/physics/{constant}".format(client.base_url, constant=constant)
+    url = "{}/constant/physics/{constant}".format(
+        client.base_url, constant=constant
+    )  # noqa: E501
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, PhysicsConstant, Error]]:
-	if response.status_code == 200:
-		response_200 = PhysicsConstant.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, PhysicsConstant, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, PhysicsConstant, Error]]:
+    if response.status_code == 200:
+        response_200 = PhysicsConstant.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, PhysicsConstant, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	constant: PhysicsConstantName,
-	*,
-	client: Client,
+    constant: PhysicsConstantName,
+    *,
+    client: Client,
 ) -> Response[Union[Any, PhysicsConstant, Error]]:
-	kwargs = _get_kwargs(
-		constant=constant,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    kwargs = _get_kwargs(
+        constant=constant,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	constant: PhysicsConstantName,
-	*,
-	client: Client,
+    constant: PhysicsConstantName,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, PhysicsConstant, Error]]:
 
-	return sync_detailed(
-		constant=constant,
-		client=client,
-	).parsed
+    return sync_detailed(
+        constant=constant,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	constant: PhysicsConstantName,
-	*,
-	client: Client,
+    constant: PhysicsConstantName,
+    *,
+    client: Client,
 ) -> Response[Union[Any, PhysicsConstant, Error]]:
-	kwargs = _get_kwargs(
-		constant=constant,
-		client=client,
-	)
+    kwargs = _get_kwargs(
+        constant=constant,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	constant: PhysicsConstantName,
-	*,
-	client: Client,
+    constant: PhysicsConstantName,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, PhysicsConstant, Error]]:
 
-	return (
-		await asyncio_detailed(
-		constant=constant,
-			client=client,
-		)
-	).parsed
+    return (
+        await asyncio_detailed(
+            constant=constant,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/file/create_file_2d_vector_conversion.py` & `kittycad-0.3.8/kittycad/api/file/create_file_conversion.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,134 +1,141 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.file2_d_vector_conversion import File2DVectorConversion
 from ...models.error import Error
-from ...models.file2_d_vector_export_format import File2DVectorExportFormat
-from ...models.file2_d_vector_import_format import File2DVectorImportFormat
+from ...models.file_conversion import FileConversion
+from ...models.file_export_format import FileExportFormat
+from ...models.file_import_format import FileImportFormat
 from ...types import Response
 
+
 def _get_kwargs(
-	output_format: File2DVectorExportFormat,
-	src_format: File2DVectorImportFormat,
-	body: bytes,
-	*,
-	client: Client,
+    output_format: FileExportFormat,
+    src_format: FileImportFormat,
+    body: bytes,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/file/2d/vector/conversion/{src_format}/{output_format}".format(client.base_url, output_format=output_format, src_format=src_format)
-
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
-
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-		"content": body,
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, File2DVectorConversion, Error]]:
-	if response.status_code == 201:
-		response_201 = File2DVectorConversion.from_dict(response.json())
-		return response_201
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, File2DVectorConversion, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    url = "{}/file/conversion/{src_format}/{output_format}".format(
+        client.base_url, output_format=output_format, src_format=src_format
+    )  # noqa: E501
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "content": body,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, FileConversion, Error]]:
+    if response.status_code == 201:
+        response_201 = FileConversion.from_dict(response.json())
+        return response_201
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, FileConversion, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	output_format: File2DVectorExportFormat,
-	src_format: File2DVectorImportFormat,
-	body: bytes,
-	*,
-	client: Client,
-) -> Response[Union[Any, File2DVectorConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		body=body,
-		client=client,
-	)
-
-	response = httpx.post(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    output_format: FileExportFormat,
+    src_format: FileImportFormat,
+    body: bytes,
+    *,
+    client: Client,
+) -> Response[Union[Any, FileConversion, Error]]:
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        body=body,
+        client=client,
+    )
+
+    response = httpx.post(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	output_format: File2DVectorExportFormat,
-	src_format: File2DVectorImportFormat,
-	body: bytes,
-	*,
-	client: Client,
-) -> Optional[Union[Any, File2DVectorConversion, Error]]:
-	""" Convert a 2D Vector file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
-If the conversion is performed synchronously, the contents of the converted file (`output`) will be returned as a base64 encoded string.
-If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint. """
-
-	return sync_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		body=body,
-		client=client,
-	).parsed
+    output_format: FileExportFormat,
+    src_format: FileImportFormat,
+    body: bytes,
+    *,
+    client: Client,
+) -> Optional[Union[Any, FileConversion, Error]]:
+    """Convert a CAD file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
+    If the conversion is performed synchronously, the contents of the converted file (`output`) will be returned as a base64 encoded string.
+    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
+
+    return sync_detailed(
+        output_format=output_format,
+        src_format=src_format,
+        body=body,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	output_format: File2DVectorExportFormat,
-	src_format: File2DVectorImportFormat,
-	body: bytes,
-	*,
-	client: Client,
-) -> Response[Union[Any, File2DVectorConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		body=body,
-		client=client,
-	)
+    output_format: FileExportFormat,
+    src_format: FileImportFormat,
+    body: bytes,
+    *,
+    client: Client,
+) -> Response[Union[Any, FileConversion, Error]]:
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        body=body,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.post(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.post(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: File2DVectorExportFormat,
-	src_format: File2DVectorImportFormat,
-	body: bytes,
-	*,
-	client: Client,
-) -> Optional[Union[Any, File2DVectorConversion, Error]]:
-	""" Convert a 2D Vector file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
-If the conversion is performed synchronously, the contents of the converted file (`output`) will be returned as a base64 encoded string.
-If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint. """
-
-	return (
-		await asyncio_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		body=body,
-			client=client,
-		)
-	).parsed
+    output_format: FileExportFormat,
+    src_format: FileImportFormat,
+    body: bytes,
+    *,
+    client: Client,
+) -> Optional[Union[Any, FileConversion, Error]]:
+    """Convert a CAD file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
+    If the conversion is performed synchronously, the contents of the converted file (`output`) will be returned as a base64 encoded string.
+    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            output_format=output_format,
+            src_format=src_format,
+            body=body,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/file/create_file_conversion_with_base64_helper.py` & `kittycad-0.3.8/kittycad/api/file/create_file_conversion_with_base64_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,14 @@
-from typing import Any, Dict, Optional, Union
-
 import base64
-import httpx
+from typing import Any, Optional, Union
 
+from ...api.file.create_file_conversion import asyncio as fc_asyncio, sync as fc_sync
 from ...client import Client
-from ...models import Error
-from ...models import FileConversion
-from ...models import FileImportFormat
-from ...models import FileExportFormat
-from ...types import Response
-from ...api.file.create_file_conversion import sync as fc_sync, asyncio as fc_asyncio
+from ...models import Error, FileConversion, FileExportFormat, FileImportFormat
+
 
 def sync(
     src_format: FileImportFormat,
     output_format: FileExportFormat,
     body: bytes,
     *,
     client: Client,
@@ -26,15 +21,18 @@
         src_format=src_format,
         output_format=output_format,
         body=encoded,
         client=client,
     )
 
     if isinstance(fc, FileConversion) and fc.output != "":
-        fc.output = base64.b64decode(fc.output)
+        if isinstance(fc.output, str):
+            b = base64.b64decode(fc.output)
+            # decode the bytes to a string
+            fc.output = b.decode("utf-8")
 
     return fc
 
 
 async def asyncio(
     src_format: FileImportFormat,
     output_format: FileExportFormat,
@@ -43,17 +41,20 @@
     client: Client,
 ) -> Optional[Union[Any, FileConversion, Error]]:
     """Convert a CAD file from one format to another. If the file being converted is larger than a certain size it will be performed asynchronously. This function automatically base64 encodes the request body and base64 decodes the request output."""
 
     encoded = base64.b64encode(body)
 
     fc = await fc_asyncio(
-            src_format=src_format,
-            output_format=output_format,
-            body=encoded,
-            client=client,
-        )
+        src_format=src_format,
+        output_format=output_format,
+        body=encoded,
+        client=client,
+    )
 
     if isinstance(fc, FileConversion) and fc.output != "":
-        fc.output = base64.b64decode(fc.output)
+        if isinstance(fc.output, str):
+            b = base64.b64decode(fc.output)
+            # decode the bytes to a string
+            fc.output = b.decode("utf-8")
 
     return fc
```

### Comparing `kittycad-0.3.7/kittycad/api/file/create_file_density.py` & `kittycad-0.3.8/kittycad/api/file/create_file_density.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,131 +1,146 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.file_density import FileDensity
 from ...models.error import Error
-from ...models.file3_d_import_format import File3DImportFormat
+from ...models.file_density import FileDensity
+from ...models.file_import_format import FileImportFormat
 from ...types import Response
 
+
 def _get_kwargs(
-	material_mass: float,
-	src_format: File3DImportFormat,
-	body: bytes,
-	*,
-	client: Client,
+    material_mass: float,
+    src_format: FileImportFormat,
+    body: bytes,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/file/density?material_mass={material_mass}&src_format={src_format}".format(client.base_url, material_mass=material_mass, src_format=src_format)
+    url = "{}/file/density".format(client.base_url)  # noqa: E501
+    if material_mass is not None:
+        if "?" in url:
+            url = url + "&material_mass=" + str(material_mass)
+        else:
+            url = url + "?material_mass=" + str(material_mass)
+    if src_format is not None:
+        if "?" in url:
+            url = url + "&src_format=" + str(src_format)
+        else:
+            url = url + "?src_format=" + str(src_format)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "content": body,
+    }
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-		"content": body,
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, FileDensity, Error]]:
-	if response.status_code == 201:
-		response_201 = FileDensity.from_dict(response.json())
-		return response_201
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, FileDensity, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, FileDensity, Error]]:
+    if response.status_code == 201:
+        response_201 = FileDensity.from_dict(response.json())
+        return response_201
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, FileDensity, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	material_mass: float,
-	src_format: File3DImportFormat,
-	body: bytes,
-	*,
-	client: Client,
+    material_mass: float,
+    src_format: FileImportFormat,
+    body: bytes,
+    *,
+    client: Client,
 ) -> Response[Union[Any, FileDensity, Error]]:
-	kwargs = _get_kwargs(
-		material_mass=material_mass,
-		src_format=src_format,
-		body=body,
-		client=client,
-	)
-
-	response = httpx.post(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    kwargs = _get_kwargs(
+        material_mass=material_mass,
+        src_format=src_format,
+        body=body,
+        client=client,
+    )
+
+    response = httpx.post(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	material_mass: float,
-	src_format: File3DImportFormat,
-	body: bytes,
-	*,
-	client: Client,
+    material_mass: float,
+    src_format: FileImportFormat,
+    body: bytes,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, FileDensity, Error]]:
-	""" Get the density of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
-If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint. """
+    """Get the density of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
-	return sync_detailed(
-		material_mass=material_mass,
-		src_format=src_format,
-		body=body,
-		client=client,
-	).parsed
+    return sync_detailed(
+        material_mass=material_mass,
+        src_format=src_format,
+        body=body,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	material_mass: float,
-	src_format: File3DImportFormat,
-	body: bytes,
-	*,
-	client: Client,
+    material_mass: float,
+    src_format: FileImportFormat,
+    body: bytes,
+    *,
+    client: Client,
 ) -> Response[Union[Any, FileDensity, Error]]:
-	kwargs = _get_kwargs(
-		material_mass=material_mass,
-		src_format=src_format,
-		body=body,
-		client=client,
-	)
+    kwargs = _get_kwargs(
+        material_mass=material_mass,
+        src_format=src_format,
+        body=body,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.post(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.post(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	material_mass: float,
-	src_format: File3DImportFormat,
-	body: bytes,
-	*,
-	client: Client,
+    material_mass: float,
+    src_format: FileImportFormat,
+    body: bytes,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, FileDensity, Error]]:
-	""" Get the density of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
-If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint. """
+    """Get the density of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
-	return (
-		await asyncio_detailed(
-		material_mass=material_mass,
-		src_format=src_format,
-		body=body,
-			client=client,
-		)
-	).parsed
+    return (
+        await asyncio_detailed(
+            material_mass=material_mass,
+            src_format=src_format,
+            body=body,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/file/create_file_mass.py` & `kittycad-0.3.8/kittycad/api/file/create_file_surface_area.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,131 +1,132 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.file_mass import FileMass
 from ...models.error import Error
-from ...models.file3_d_import_format import File3DImportFormat
+from ...models.file_import_format import FileImportFormat
+from ...models.file_surface_area import FileSurfaceArea
 from ...types import Response
 
+
 def _get_kwargs(
-	material_density: float,
-	src_format: File3DImportFormat,
-	body: bytes,
-	*,
-	client: Client,
+    src_format: FileImportFormat,
+    body: bytes,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/file/mass?material_density={material_density}&src_format={src_format}".format(client.base_url, material_density=material_density, src_format=src_format)
-
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
-
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-		"content": body,
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, FileMass, Error]]:
-	if response.status_code == 201:
-		response_201 = FileMass.from_dict(response.json())
-		return response_201
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, FileMass, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    url = "{}/file/surface-area".format(client.base_url)  # noqa: E501
+    if src_format is not None:
+        if "?" in url:
+            url = url + "&src_format=" + str(src_format)
+        else:
+            url = url + "?src_format=" + str(src_format)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "content": body,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, FileSurfaceArea, Error]]:
+    if response.status_code == 201:
+        response_201 = FileSurfaceArea.from_dict(response.json())
+        return response_201
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, FileSurfaceArea, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	material_density: float,
-	src_format: File3DImportFormat,
-	body: bytes,
-	*,
-	client: Client,
-) -> Response[Union[Any, FileMass, Error]]:
-	kwargs = _get_kwargs(
-		material_density=material_density,
-		src_format=src_format,
-		body=body,
-		client=client,
-	)
-
-	response = httpx.post(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    src_format: FileImportFormat,
+    body: bytes,
+    *,
+    client: Client,
+) -> Response[Union[Any, FileSurfaceArea, Error]]:
+    kwargs = _get_kwargs(
+        src_format=src_format,
+        body=body,
+        client=client,
+    )
+
+    response = httpx.post(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	material_density: float,
-	src_format: File3DImportFormat,
-	body: bytes,
-	*,
-	client: Client,
-) -> Optional[Union[Any, FileMass, Error]]:
-	""" Get the mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
-If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint. """
-
-	return sync_detailed(
-		material_density=material_density,
-		src_format=src_format,
-		body=body,
-		client=client,
-	).parsed
+    src_format: FileImportFormat,
+    body: bytes,
+    *,
+    client: Client,
+) -> Optional[Union[Any, FileSurfaceArea, Error]]:
+    """Get the surface area of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
+
+    return sync_detailed(
+        src_format=src_format,
+        body=body,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	material_density: float,
-	src_format: File3DImportFormat,
-	body: bytes,
-	*,
-	client: Client,
-) -> Response[Union[Any, FileMass, Error]]:
-	kwargs = _get_kwargs(
-		material_density=material_density,
-		src_format=src_format,
-		body=body,
-		client=client,
-	)
+    src_format: FileImportFormat,
+    body: bytes,
+    *,
+    client: Client,
+) -> Response[Union[Any, FileSurfaceArea, Error]]:
+    kwargs = _get_kwargs(
+        src_format=src_format,
+        body=body,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.post(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.post(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	material_density: float,
-	src_format: File3DImportFormat,
-	body: bytes,
-	*,
-	client: Client,
-) -> Optional[Union[Any, FileMass, Error]]:
-	""" Get the mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
-If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint. """
-
-	return (
-		await asyncio_detailed(
-		material_density=material_density,
-		src_format=src_format,
-		body=body,
-			client=client,
-		)
-	).parsed
+    src_format: FileImportFormat,
+    body: bytes,
+    *,
+    client: Client,
+) -> Optional[Union[Any, FileSurfaceArea, Error]]:
+    """Get the surface area of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            src_format=src_format,
+            body=body,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/file/get_file_conversion_with_base64_helper.py` & `kittycad-0.3.8/kittycad/api/file/get_file_conversion_with_base64_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-from typing import Any, Dict, Optional, Union
-
 import base64
-import httpx
+from typing import Any, Optional, Union
 
+from ...api.api_calls.get_async_operation import asyncio as fc_asyncio, sync as fc_sync
 from ...client import Client
 from ...models import Error
 from ...models.file_conversion import FileConversion
-from ...types import Response
-from ...api.file.get_file_conversion import sync as fc_sync, asyncio as fc_asyncio
 
 
 def sync(
     id: str,
     *,
     client: Client,
 ) -> Optional[Union[Any, FileConversion, Error]]:
@@ -19,28 +16,34 @@
 
     fc = fc_sync(
         id=id,
         client=client,
     )
 
     if isinstance(fc, FileConversion) and fc.output != "":
-        fc.output = base64.b64decode(fc.output)
+        if isinstance(fc.output, str):
+            b = base64.b64decode(fc.output)
+            # decode the bytes to a string
+            fc.output = b.decode("utf-8")
 
     return fc
 
 
 async def asyncio(
     id: str,
     *,
     client: Client,
 ) -> Optional[Union[Any, FileConversion, Error]]:
     """Get the status of a file conversion. This function automatically base64 decodes the output response if there is one."""
 
     fc = await fc_asyncio(
-            id=id,
-            client=client,
-        )
+        id=id,
+        client=client,
+    )
 
     if isinstance(fc, FileConversion) and fc.output != "":
-        fc.output = base64.b64decode(fc.output)
+        if isinstance(fc.output, str):
+            b = base64.b64decode(fc.output)
+            # decode the bytes to a string
+            fc.output = b.decode("utf-8")
 
     return fc
```

### Comparing `kittycad-0.3.7/kittycad/api/hidden/auth_email.py` & `kittycad-0.3.8/kittycad/api/payments/validate_customer_tax_information_for_user.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,109 +1,100 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.verification_token import VerificationToken
 from ...models.error import Error
-from ...models.email_authentication_form import EmailAuthenticationForm
 from ...types import Response
 
+
 def _get_kwargs(
-	body: EmailAuthenticationForm,
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/auth/email".format(client.base_url)
+    url = "{}/user/payment/tax".format(client.base_url)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-		"content": body,
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, VerificationToken, Error]]:
-	if response.status_code == 201:
-		response_201 = VerificationToken.from_dict(response.json())
-		return response_201
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, VerificationToken, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
+    if response.status_code == 204:
+        response_204 = None
+        return response_204
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	body: EmailAuthenticationForm,
-	*,
-	client: Client,
-) -> Response[Union[Any, VerificationToken, Error]]:
-	kwargs = _get_kwargs(
-		body=body,
-		client=client,
-	)
-
-	response = httpx.post(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	body: EmailAuthenticationForm,
-	*,
-	client: Client,
-) -> Optional[Union[Any, VerificationToken, Error]]:
-
-	return sync_detailed(
-		body=body,
-		client=client,
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It will return an error if the customer's information is not valid for automatic tax. Otherwise, it will return an empty successful response."""  # noqa: E501
+
+    return sync_detailed(
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	body: EmailAuthenticationForm,
-	*,
-	client: Client,
-) -> Response[Union[Any, VerificationToken, Error]]:
-	kwargs = _get_kwargs(
-		body=body,
-		client=client,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.post(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	body: EmailAuthenticationForm,
-	*,
-	client: Client,
-) -> Optional[Union[Any, VerificationToken, Error]]:
-
-	return (
-		await asyncio_detailed(
-		body=body,
-			client=client,
-		)
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It will return an error if the customer's information is not valid for automatic tax. Otherwise, it will return an empty successful response."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/hidden/auth_email_callback.py` & `kittycad-0.3.8/kittycad/api/users/get_user_front_hash_self.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,124 +1,100 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
 from ...types import Response
 
+
 def _get_kwargs(
-	email: str,
-	token: str,
-	*,
-	client: Client,
-	callback_url: Optional[str] = None,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/auth/email/callback?callback_url={callback_url}&email={email}&token={token}".format(client.base_url, callback_url=callback_url, email=email, token=token)
+    url = "{}/user/front-hash".format(client.base_url)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
-	if response.status_code == 302:
-		response_302 = None
-		return response_302
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, str, Error]]:
+    if response.status_code == 200:
+        response_200 = response.text
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, str, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	email: str,
-	token: str,
-	*,
-	client: Client,
-	callback_url: Optional[str] = None,
-) -> Response[Union[Any, Error]]:
-	kwargs = _get_kwargs(
-		callback_url=callback_url,
-		email=email,
-		token=token,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, str, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	email: str,
-	token: str,
-	*,
-	client: Client,
-	callback_url: Optional[str] = None,
-) -> Optional[Union[Any, Error]]:
-
-	return sync_detailed(
-		callback_url=callback_url,
-		email=email,
-		token=token,
-		client=client,
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, str, Error]]:
+    """This info is sent to front when initialing the front chat, it prevents impersonations using js hacks in the browser"""  # noqa: E501
+
+    return sync_detailed(
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	email: str,
-	token: str,
-	*,
-	client: Client,
-	callback_url: Optional[str] = None,
-) -> Response[Union[Any, Error]]:
-	kwargs = _get_kwargs(
-		callback_url=callback_url,
-		email=email,
-		token=token,
-		client=client,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, str, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	email: str,
-	token: str,
-	*,
-	client: Client,
-	callback_url: Optional[str] = None,
-) -> Optional[Union[Any, Error]]:
-
-	return (
-		await asyncio_detailed(
-		callback_url=callback_url,
-		email=email,
-		token=token,
-			client=client,
-		)
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, str, Error]]:
+    """This info is sent to front when initialing the front chat, it prevents impersonations using js hacks in the browser"""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/hidden/logout.py` & `kittycad-0.3.8/kittycad/api/meta/get_metadata.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,107 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
+from ...models.metadata import Metadata
 from ...types import Response
 
+
 def _get_kwargs(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/logout".format(client.base_url)
+    url = "{}/_meta/info".format(client.base_url)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
-	if response.status_code == 204:
-		response_204 = None
-		return response_204
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, Metadata, Error]]:
+    if response.status_code == 200:
+        response_200 = Metadata.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, Metadata, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
-
-	response = httpx.post(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, Metadata, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	*,
-	client: Client,
-) -> Optional[Union[Any, Error]]:
-	""" This is used in logout scenarios. """
-
-	return sync_detailed(
-		client=client,
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, Metadata, Error]]:
+    """This includes information on any of our other distributed systems it is connected to.
+    You must be a KittyCAD employee to perform this request."""  # noqa: E501
+
+    return sync_detailed(
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, Metadata, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.post(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	*,
-	client: Client,
-) -> Optional[Union[Any, Error]]:
-	""" This is used in logout scenarios. """
-
-	return (
-		await asyncio_detailed(
-			client=client,
-		)
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, Metadata, Error]]:
+    """This includes information on any of our other distributed systems it is connected to.
+    You must be a KittyCAD employee to perform this request."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/meta/get_ai_plugin_manifest.py` & `kittycad-0.3.8/kittycad/api/payments/get_payment_balance_for_user.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,105 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.ai_plugin_manifest import AiPluginManifest
+from ...models.customer_balance import CustomerBalance
 from ...models.error import Error
 from ...types import Response
 
+
 def _get_kwargs(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/.well-known/ai-plugin.json".format(client.base_url)
+    url = "{}/user/payment/balance".format(client.base_url)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, AiPluginManifest, Error]]:
-	if response.status_code == 200:
-		response_200 = AiPluginManifest.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, AiPluginManifest, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, CustomerBalance, Error]]:
+    if response.status_code == 200:
+        response_200 = CustomerBalance.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, CustomerBalance, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, AiPluginManifest, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, CustomerBalance, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	*,
-	client: Client,
-) -> Optional[Union[Any, AiPluginManifest, Error]]:
-
-	return sync_detailed(
-		client=client,
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, CustomerBalance, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It gets the balance information for the authenticated user."""  # noqa: E501
+
+    return sync_detailed(
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, AiPluginManifest, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, CustomerBalance, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	*,
-	client: Client,
-) -> Optional[Union[Any, AiPluginManifest, Error]]:
-
-	return (
-		await asyncio_detailed(
-			client=client,
-		)
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, CustomerBalance, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It gets the balance information for the authenticated user."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/meta/get_schema.py` & `kittycad-0.3.8/kittycad/api/payments/get_payment_information_for_user.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,98 +1,107 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.dict import dict
+from ...models.customer import Customer
 from ...models.error import Error
 from ...types import Response
 
+
 def _get_kwargs(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/".format(client.base_url)
+    url = "{}/user/payment".format(client.base_url)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, dict, Error]]:
-	if response.status_code == 200:
-		response_200 = response.json()
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, dict, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
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
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, Customer, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, dict, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, Customer, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	*,
-	client: Client,
-) -> Optional[Union[Any, dict, Error]]:
-
-	return sync_detailed(
-		client=client,
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, Customer, Error]]:
+    """This includes billing address, phone, and name.
+    This endpoint requires authentication by any KittyCAD user. It gets the payment information for the authenticated user."""  # noqa: E501
+
+    return sync_detailed(
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, dict, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, Customer, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	*,
-	client: Client,
-) -> Optional[Union[Any, dict, Error]]:
-
-	return (
-		await asyncio_detailed(
-			client=client,
-		)
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, Customer, Error]]:
+    """This includes billing address, phone, and name.
+    This endpoint requires authentication by any KittyCAD user. It gets the payment information for the authenticated user."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/meta/ping.py` & `kittycad-0.3.8/kittycad/api/payments/update_payment_information_for_user.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,118 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.pong import Pong
+from ...models.billing_info import BillingInfo
+from ...models.customer import Customer
 from ...models.error import Error
 from ...types import Response
 
+
 def _get_kwargs(
-	*,
-	client: Client,
+    body: BillingInfo,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/ping".format(client.base_url)
+    url = "{}/user/payment".format(client.base_url)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Pong, Error]]:
-	if response.status_code == 200:
-		response_200 = Pong.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Pong, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "content": body,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
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
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, Customer, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, Pong, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    body: BillingInfo,
+    *,
+    client: Client,
+) -> Response[Union[Any, Customer, Error]]:
+    kwargs = _get_kwargs(
+        body=body,
+        client=client,
+    )
+
+    response = httpx.put(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	*,
-	client: Client,
-) -> Optional[Union[Any, Pong, Error]]:
-
-	return sync_detailed(
-		client=client,
-	).parsed
+    body: BillingInfo,
+    *,
+    client: Client,
+) -> Optional[Union[Any, Customer, Error]]:
+    """This includes billing address, phone, and name.
+    This endpoint requires authentication by any KittyCAD user. It updates the payment information for the authenticated user."""  # noqa: E501
+
+    return sync_detailed(
+        body=body,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, Pong, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
+    body: BillingInfo,
+    *,
+    client: Client,
+) -> Response[Union[Any, Customer, Error]]:
+    kwargs = _get_kwargs(
+        body=body,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.put(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	*,
-	client: Client,
-) -> Optional[Union[Any, Pong, Error]]:
-
-	return (
-		await asyncio_detailed(
-			client=client,
-		)
-	).parsed
+    body: BillingInfo,
+    *,
+    client: Client,
+) -> Optional[Union[Any, Customer, Error]]:
+    """This includes billing address, phone, and name.
+    This endpoint requires authentication by any KittyCAD user. It updates the payment information for the authenticated user."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            body=body,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/payments/create_payment_intent_for_user.py` & `kittycad-0.3.8/kittycad/api/payments/create_payment_intent_for_user.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,105 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.payment_intent import PaymentIntent
 from ...models.error import Error
+from ...models.payment_intent import PaymentIntent
 from ...types import Response
 
+
 def _get_kwargs(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/user/payment/intent".format(client.base_url)
+    url = "{}/user/payment/intent".format(client.base_url)  # noqa: E501
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, PaymentIntent, Error]]:
-	if response.status_code == 201:
-		response_201 = PaymentIntent.from_dict(response.json())
-		return response_201
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, PaymentIntent, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, PaymentIntent, Error]]:
+    if response.status_code == 201:
+        response_201 = PaymentIntent.from_dict(response.json())
+        return response_201
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, PaymentIntent, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Response[Union[Any, PaymentIntent, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
-
-	response = httpx.post(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    kwargs = _get_kwargs(
+        client=client,
+    )
+
+    response = httpx.post(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, PaymentIntent, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It creates a new payment intent for the authenticated user. """
+    """This endpoint requires authentication by any KittyCAD user. It creates a new payment intent for the authenticated user."""  # noqa: E501
 
-	return sync_detailed(
-		client=client,
-	).parsed
+    return sync_detailed(
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Response[Union[Any, PaymentIntent, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
+    kwargs = _get_kwargs(
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.post(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.post(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, PaymentIntent, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It creates a new payment intent for the authenticated user. """
+    """This endpoint requires authentication by any KittyCAD user. It creates a new payment intent for the authenticated user."""  # noqa: E501
 
-	return (
-		await asyncio_detailed(
-			client=client,
-		)
-	).parsed
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/payments/validate_customer_tax_information_for_user.py` & `kittycad-0.3.8/kittycad/api/api_tokens/create_api_token_for_user.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,99 +1,105 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.api_token import ApiToken
 from ...models.error import Error
 from ...types import Response
 
+
 def _get_kwargs(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/user/payment/tax".format(client.base_url)
+    url = "{}/user/api-tokens".format(client.base_url)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
-	if response.status_code == 204:
-		response_204 = None
-		return response_204
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, ApiToken, Error]]:
+    if response.status_code == 201:
+        response_201 = ApiToken.from_dict(response.json())
+        return response_201
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, ApiToken, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, ApiToken, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
+
+    response = httpx.post(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	*,
-	client: Client,
-) -> Optional[Union[Any, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It will return an error if the customer's information is not valid for automatic tax. Otherwise, it will return an empty successful response. """
-
-	return sync_detailed(
-		client=client,
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, ApiToken, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It creates a new API token for the authenticated user."""  # noqa: E501
+
+    return sync_detailed(
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, ApiToken, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.post(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	*,
-	client: Client,
-) -> Optional[Union[Any, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It will return an error if the customer's information is not valid for automatic tax. Otherwise, it will return an empty successful response. """
-
-	return (
-		await asyncio_detailed(
-			client=client,
-		)
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, ApiToken, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It creates a new API token for the authenticated user."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/sessions/get_session_for_user.py` & `kittycad-0.3.8/kittycad/api/users/get_user.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,114 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.session import Session
 from ...models.error import Error
+from ...models.user import User
 from ...types import Response
 
+
 def _get_kwargs(
-	token: str,
-	*,
-	client: Client,
+    id: str,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/user/session/{token}".format(client.base_url, token=token)
+    url = "{}/users/{id}".format(client.base_url, id=id)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Session, Error]]:
-	if response.status_code == 200:
-		response_200 = Session.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Session, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, User, Error]]:
+    if response.status_code == 200:
+        response_200 = User.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, User, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	token: str,
-	*,
-	client: Client,
-) -> Response[Union[Any, Session, Error]]:
-	kwargs = _get_kwargs(
-		token=token,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    id: str,
+    *,
+    client: Client,
+) -> Response[Union[Any, User, Error]]:
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	token: str,
-	*,
-	client: Client,
-) -> Optional[Union[Any, Session, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It returns details of the requested API token for the user. """
-
-	return sync_detailed(
-		token=token,
-		client=client,
-	).parsed
+    id: str,
+    *,
+    client: Client,
+) -> Optional[Union[Any, User, Error]]:
+    """To get information about yourself, use `/users/me` as the endpoint. By doing so you will get the user information for the authenticated user.
+    Alternatively, to get information about the authenticated user, use `/user` endpoint.
+    To get information about any KittyCAD user, you must be a KittyCAD employee."""  # noqa: E501
+
+    return sync_detailed(
+        id=id,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	token: str,
-	*,
-	client: Client,
-) -> Response[Union[Any, Session, Error]]:
-	kwargs = _get_kwargs(
-		token=token,
-		client=client,
-	)
+    id: str,
+    *,
+    client: Client,
+) -> Response[Union[Any, User, Error]]:
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	token: str,
-	*,
-	client: Client,
-) -> Optional[Union[Any, Session, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It returns details of the requested API token for the user. """
-
-	return (
-		await asyncio_detailed(
-		token=token,
-			client=client,
-		)
-	).parsed
+    id: str,
+    *,
+    client: Client,
+) -> Optional[Union[Any, User, Error]]:
+    """To get information about yourself, use `/users/me` as the endpoint. By doing so you will get the user information for the authenticated user.
+    Alternatively, to get information about the authenticated user, use `/user` endpoint.
+    To get information about any KittyCAD user, you must be a KittyCAD employee."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            id=id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/unit/get_angle_unit_conversion.py` & `kittycad-0.3.8/kittycad/api/unit/get_length_unit_conversion.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,129 +1,140 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.unit_angle_conversion import UnitAngleConversion
 from ...models.error import Error
-from ...models.unit_angle_format import UnitAngleFormat
-from ...models.unit_angle_format import UnitAngleFormat
+from ...models.unit_length_conversion import UnitLengthConversion
+from ...models.unit_length_format import UnitLengthFormat
 from ...types import Response
 
+
 def _get_kwargs(
-	output_format: UnitAngleFormat,
-	src_format: UnitAngleFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitLengthFormat,
+    src_format: UnitLengthFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/angle/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
-
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
-
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitAngleConversion, Error]]:
-	if response.status_code == 200:
-		response_200 = UnitAngleConversion.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitAngleConversion, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    url = "{}/unit/conversion/length/{src_format}/{output_format}".format(
+        client.base_url, output_format=output_format, src_format=src_format
+    )  # noqa: E501
+    if value is not None:
+        if "?" in url:
+            url = url + "&value=" + str(value)
+        else:
+            url = url + "?value=" + str(value)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, UnitLengthConversion, Error]]:
+    if response.status_code == 200:
+        response_200 = UnitLengthConversion.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, UnitLengthConversion, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	output_format: UnitAngleFormat,
-	src_format: UnitAngleFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Response[Union[Any, UnitAngleConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    output_format: UnitLengthFormat,
+    src_format: UnitLengthFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Response[Union[Any, UnitLengthConversion, Error]]:
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitAngleFormat,
-	src_format: UnitAngleFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Optional[Union[Any, UnitAngleConversion, Error]]:
-	""" Convert an angle unit value to another angle unit value. This is a nice endpoint to use for helper functions. """
-
-	return sync_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	).parsed
+    output_format: UnitLengthFormat,
+    src_format: UnitLengthFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Optional[Union[Any, UnitLengthConversion, Error]]:
+    """Convert a length unit value to another length unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+
+    return sync_detailed(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitAngleFormat,
-	src_format: UnitAngleFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Response[Union[Any, UnitAngleConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
+    output_format: UnitLengthFormat,
+    src_format: UnitLengthFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Response[Union[Any, UnitLengthConversion, Error]]:
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitAngleFormat,
-	src_format: UnitAngleFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Optional[Union[Any, UnitAngleConversion, Error]]:
-	""" Convert an angle unit value to another angle unit value. This is a nice endpoint to use for helper functions. """
-
-	return (
-		await asyncio_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-			client=client,
-		)
-	).parsed
+    output_format: UnitLengthFormat,
+    src_format: UnitLengthFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Optional[Union[Any, UnitLengthConversion, Error]]:
+    """Convert a length unit value to another length unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            output_format=output_format,
+            src_format=src_format,
+            value=value,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/unit/get_area_unit_conversion.py` & `kittycad-0.3.8/kittycad/api/unit/get_area_unit_conversion.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,129 +1,140 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.unit_area_conversion import UnitAreaConversion
 from ...models.error import Error
-from ...models.unit_area_format import UnitAreaFormat
+from ...models.unit_area_conversion import UnitAreaConversion
 from ...models.unit_area_format import UnitAreaFormat
 from ...types import Response
 
+
 def _get_kwargs(
-	output_format: UnitAreaFormat,
-	src_format: UnitAreaFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitAreaFormat,
+    src_format: UnitAreaFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/area/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
+    url = "{}/unit/conversion/area/{src_format}/{output_format}".format(
+        client.base_url, output_format=output_format, src_format=src_format
+    )  # noqa: E501
+    if value is not None:
+        if "?" in url:
+            url = url + "&value=" + str(value)
+        else:
+            url = url + "?value=" + str(value)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitAreaConversion, Error]]:
-	if response.status_code == 200:
-		response_200 = UnitAreaConversion.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitAreaConversion, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, UnitAreaConversion, Error]]:
+    if response.status_code == 200:
+        response_200 = UnitAreaConversion.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, UnitAreaConversion, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	output_format: UnitAreaFormat,
-	src_format: UnitAreaFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitAreaFormat,
+    src_format: UnitAreaFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Response[Union[Any, UnitAreaConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitAreaFormat,
-	src_format: UnitAreaFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitAreaFormat,
+    src_format: UnitAreaFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, UnitAreaConversion, Error]]:
-	""" Convert an area unit value to another area unit value. This is a nice endpoint to use for helper functions. """
+    """Convert an area unit value to another area unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
-	return sync_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	).parsed
+    return sync_detailed(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitAreaFormat,
-	src_format: UnitAreaFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitAreaFormat,
+    src_format: UnitAreaFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Response[Union[Any, UnitAreaConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitAreaFormat,
-	src_format: UnitAreaFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitAreaFormat,
+    src_format: UnitAreaFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, UnitAreaConversion, Error]]:
-	""" Convert an area unit value to another area unit value. This is a nice endpoint to use for helper functions. """
+    """Convert an area unit value to another area unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
-	return (
-		await asyncio_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-			client=client,
-		)
-	).parsed
+    return (
+        await asyncio_detailed(
+            output_format=output_format,
+            src_format=src_format,
+            value=value,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py` & `kittycad-0.3.8/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,129 +1,140 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.unit_data_transfer_rate_conversion import UnitDataTransferRateConversion
 from ...models.error import Error
-from ...models.unit_data_transfer_rate_format import UnitDataTransferRateFormat
+from ...models.unit_data_transfer_rate_conversion import UnitDataTransferRateConversion
 from ...models.unit_data_transfer_rate_format import UnitDataTransferRateFormat
 from ...types import Response
 
+
 def _get_kwargs(
-	output_format: UnitDataTransferRateFormat,
-	src_format: UnitDataTransferRateFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitDataTransferRateFormat,
+    src_format: UnitDataTransferRateFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/data-transfer-rate/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
+    url = "{}/unit/conversion/data-transfer-rate/{src_format}/{output_format}".format(
+        client.base_url, output_format=output_format, src_format=src_format
+    )  # noqa: E501
+    if value is not None:
+        if "?" in url:
+            url = url + "&value=" + str(value)
+        else:
+            url = url + "?value=" + str(value)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitDataTransferRateConversion, Error]]:
-	if response.status_code == 200:
-		response_200 = UnitDataTransferRateConversion.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitDataTransferRateConversion, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, UnitDataTransferRateConversion, Error]]:
+    if response.status_code == 200:
+        response_200 = UnitDataTransferRateConversion.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, UnitDataTransferRateConversion, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	output_format: UnitDataTransferRateFormat,
-	src_format: UnitDataTransferRateFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitDataTransferRateFormat,
+    src_format: UnitDataTransferRateFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Response[Union[Any, UnitDataTransferRateConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitDataTransferRateFormat,
-	src_format: UnitDataTransferRateFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitDataTransferRateFormat,
+    src_format: UnitDataTransferRateFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, UnitDataTransferRateConversion, Error]]:
-	""" Convert a data transfer rate unit value to another data transfer rate unit value. This is a nice endpoint to use for helper functions. """
+    """Convert a data transfer rate unit value to another data transfer rate unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
-	return sync_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	).parsed
+    return sync_detailed(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitDataTransferRateFormat,
-	src_format: UnitDataTransferRateFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitDataTransferRateFormat,
+    src_format: UnitDataTransferRateFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Response[Union[Any, UnitDataTransferRateConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitDataTransferRateFormat,
-	src_format: UnitDataTransferRateFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitDataTransferRateFormat,
+    src_format: UnitDataTransferRateFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, UnitDataTransferRateConversion, Error]]:
-	""" Convert a data transfer rate unit value to another data transfer rate unit value. This is a nice endpoint to use for helper functions. """
+    """Convert a data transfer rate unit value to another data transfer rate unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
-	return (
-		await asyncio_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-			client=client,
-		)
-	).parsed
+    return (
+        await asyncio_detailed(
+            output_format=output_format,
+            src_format=src_format,
+            value=value,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/unit/get_data_unit_conversion.py` & `kittycad-0.3.8/kittycad/api/unit/get_metric_power_unit_conversion.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,129 +1,140 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.unit_data_conversion import UnitDataConversion
 from ...models.error import Error
-from ...models.unit_data_format import UnitDataFormat
-from ...models.unit_data_format import UnitDataFormat
+from ...models.unit_metric_power import UnitMetricPower
+from ...models.unit_metric_power_conversion import UnitMetricPowerConversion
 from ...types import Response
 
+
 def _get_kwargs(
-	output_format: UnitDataFormat,
-	src_format: UnitDataFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMetricPower,
+    src_format: UnitMetricPower,
+    value: float,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/data/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
-
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
-
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitDataConversion, Error]]:
-	if response.status_code == 200:
-		response_200 = UnitDataConversion.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitDataConversion, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    url = "{}/unit/conversion/metric/power/{src_format}/{output_format}".format(
+        client.base_url, output_format=output_format, src_format=src_format
+    )  # noqa: E501
+    if value is not None:
+        if "?" in url:
+            url = url + "&value=" + str(value)
+        else:
+            url = url + "?value=" + str(value)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, UnitMetricPowerConversion, Error]]:
+    if response.status_code == 200:
+        response_200 = UnitMetricPowerConversion.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, UnitMetricPowerConversion, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	output_format: UnitDataFormat,
-	src_format: UnitDataFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Response[Union[Any, UnitDataConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    output_format: UnitMetricPower,
+    src_format: UnitMetricPower,
+    value: float,
+    *,
+    client: Client,
+) -> Response[Union[Any, UnitMetricPowerConversion, Error]]:
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitDataFormat,
-	src_format: UnitDataFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Optional[Union[Any, UnitDataConversion, Error]]:
-	""" Convert a data unit value to another data unit value. This is a nice endpoint to use for helper functions. """
-
-	return sync_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	).parsed
+    output_format: UnitMetricPower,
+    src_format: UnitMetricPower,
+    value: float,
+    *,
+    client: Client,
+) -> Optional[Union[Any, UnitMetricPowerConversion, Error]]:
+    """Convert a metric unit value to another metric unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+
+    return sync_detailed(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitDataFormat,
-	src_format: UnitDataFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Response[Union[Any, UnitDataConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
+    output_format: UnitMetricPower,
+    src_format: UnitMetricPower,
+    value: float,
+    *,
+    client: Client,
+) -> Response[Union[Any, UnitMetricPowerConversion, Error]]:
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitDataFormat,
-	src_format: UnitDataFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Optional[Union[Any, UnitDataConversion, Error]]:
-	""" Convert a data unit value to another data unit value. This is a nice endpoint to use for helper functions. """
-
-	return (
-		await asyncio_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-			client=client,
-		)
-	).parsed
+    output_format: UnitMetricPower,
+    src_format: UnitMetricPower,
+    value: float,
+    *,
+    client: Client,
+) -> Optional[Union[Any, UnitMetricPowerConversion, Error]]:
+    """Convert a metric unit value to another metric unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            output_format=output_format,
+            src_format=src_format,
+            value=value,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py` & `kittycad-0.3.8/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,144 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.unit_magnetic_field_strength_conversion import UnitMagneticFieldStrengthConversion
 from ...models.error import Error
-from ...models.unit_magnetic_field_strength_format import UnitMagneticFieldStrengthFormat
-from ...models.unit_magnetic_field_strength_format import UnitMagneticFieldStrengthFormat
+from ...models.unit_magnetic_field_strength_conversion import (
+    UnitMagneticFieldStrengthConversion,
+)
+from ...models.unit_magnetic_field_strength_format import (
+    UnitMagneticFieldStrengthFormat,
+)
 from ...types import Response
 
+
 def _get_kwargs(
-	output_format: UnitMagneticFieldStrengthFormat,
-	src_format: UnitMagneticFieldStrengthFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMagneticFieldStrengthFormat,
+    src_format: UnitMagneticFieldStrengthFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/magnetic-field-strength/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
+    url = "{}/unit/conversion/magnetic-field-strength/{src_format}/{output_format}".format(
+        client.base_url, output_format=output_format, src_format=src_format
+    )  # noqa: E501
+    if value is not None:
+        if "?" in url:
+            url = url + "&value=" + str(value)
+        else:
+            url = url + "?value=" + str(value)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, UnitMagneticFieldStrengthConversion, Error]]:
+    if response.status_code == 200:
+        response_200 = UnitMagneticFieldStrengthConversion.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitMagneticFieldStrengthConversion, Error]]:
-	if response.status_code == 200:
-		response_200 = UnitMagneticFieldStrengthConversion.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitMagneticFieldStrengthConversion, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, UnitMagneticFieldStrengthConversion, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	output_format: UnitMagneticFieldStrengthFormat,
-	src_format: UnitMagneticFieldStrengthFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMagneticFieldStrengthFormat,
+    src_format: UnitMagneticFieldStrengthFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Response[Union[Any, UnitMagneticFieldStrengthConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitMagneticFieldStrengthFormat,
-	src_format: UnitMagneticFieldStrengthFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMagneticFieldStrengthFormat,
+    src_format: UnitMagneticFieldStrengthFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, UnitMagneticFieldStrengthConversion, Error]]:
-	""" Convert a magnetic field strength unit value to another magnetic field strength unit value. This is a nice endpoint to use for helper functions. """
+    """Convert a magnetic field strength unit value to another magnetic field strength unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
-	return sync_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	).parsed
+    return sync_detailed(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitMagneticFieldStrengthFormat,
-	src_format: UnitMagneticFieldStrengthFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMagneticFieldStrengthFormat,
+    src_format: UnitMagneticFieldStrengthFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Response[Union[Any, UnitMagneticFieldStrengthConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitMagneticFieldStrengthFormat,
-	src_format: UnitMagneticFieldStrengthFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMagneticFieldStrengthFormat,
+    src_format: UnitMagneticFieldStrengthFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, UnitMagneticFieldStrengthConversion, Error]]:
-	""" Convert a magnetic field strength unit value to another magnetic field strength unit value. This is a nice endpoint to use for helper functions. """
+    """Convert a magnetic field strength unit value to another magnetic field strength unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
-	return (
-		await asyncio_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-			client=client,
-		)
-	).parsed
+    return (
+        await asyncio_detailed(
+            output_format=output_format,
+            src_format=src_format,
+            value=value,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py` & `kittycad-0.3.8/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,129 +1,140 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.unit_metric_power_cubed_conversion import UnitMetricPowerCubedConversion
 from ...models.error import Error
 from ...models.unit_metric_power import UnitMetricPower
-from ...models.unit_metric_power import UnitMetricPower
+from ...models.unit_metric_power_cubed_conversion import UnitMetricPowerCubedConversion
 from ...types import Response
 
+
 def _get_kwargs(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMetricPower,
+    src_format: UnitMetricPower,
+    value: float,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/metric/cubed/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
+    url = "{}/unit/conversion/metric/cubed/{src_format}/{output_format}".format(
+        client.base_url, output_format=output_format, src_format=src_format
+    )  # noqa: E501
+    if value is not None:
+        if "?" in url:
+            url = url + "&value=" + str(value)
+        else:
+            url = url + "?value=" + str(value)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitMetricPowerCubedConversion, Error]]:
-	if response.status_code == 200:
-		response_200 = UnitMetricPowerCubedConversion.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitMetricPowerCubedConversion, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, UnitMetricPowerCubedConversion, Error]]:
+    if response.status_code == 200:
+        response_200 = UnitMetricPowerCubedConversion.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, UnitMetricPowerCubedConversion, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMetricPower,
+    src_format: UnitMetricPower,
+    value: float,
+    *,
+    client: Client,
 ) -> Response[Union[Any, UnitMetricPowerCubedConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMetricPower,
+    src_format: UnitMetricPower,
+    value: float,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, UnitMetricPowerCubedConversion, Error]]:
-	""" Convert a metric cubed unit value to another metric cubed unit value. This is a nice endpoint to use for helper functions. """
+    """Convert a metric cubed unit value to another metric cubed unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
-	return sync_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	).parsed
+    return sync_detailed(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMetricPower,
+    src_format: UnitMetricPower,
+    value: float,
+    *,
+    client: Client,
 ) -> Response[Union[Any, UnitMetricPowerCubedConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMetricPower,
+    src_format: UnitMetricPower,
+    value: float,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, UnitMetricPowerCubedConversion, Error]]:
-	""" Convert a metric cubed unit value to another metric cubed unit value. This is a nice endpoint to use for helper functions. """
+    """Convert a metric cubed unit value to another metric cubed unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
-	return (
-		await asyncio_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-			client=client,
-		)
-	).parsed
+    return (
+        await asyncio_detailed(
+            output_format=output_format,
+            src_format=src_format,
+            value=value,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/unit/get_metric_power_squared_unit_conversion.py` & `kittycad-0.3.8/kittycad/api/unit/get_metric_power_squared_unit_conversion.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,129 +1,142 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.unit_metric_power_squared_conversion import UnitMetricPowerSquaredConversion
 from ...models.error import Error
 from ...models.unit_metric_power import UnitMetricPower
-from ...models.unit_metric_power import UnitMetricPower
+from ...models.unit_metric_power_squared_conversion import (
+    UnitMetricPowerSquaredConversion,
+)
 from ...types import Response
 
+
 def _get_kwargs(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMetricPower,
+    src_format: UnitMetricPower,
+    value: float,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/metric/squared/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
+    url = "{}/unit/conversion/metric/squared/{src_format}/{output_format}".format(
+        client.base_url, output_format=output_format, src_format=src_format
+    )  # noqa: E501
+    if value is not None:
+        if "?" in url:
+            url = url + "&value=" + str(value)
+        else:
+            url = url + "?value=" + str(value)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, UnitMetricPowerSquaredConversion, Error]]:
+    if response.status_code == 200:
+        response_200 = UnitMetricPowerSquaredConversion.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitMetricPowerSquaredConversion, Error]]:
-	if response.status_code == 200:
-		response_200 = UnitMetricPowerSquaredConversion.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitMetricPowerSquaredConversion, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, UnitMetricPowerSquaredConversion, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMetricPower,
+    src_format: UnitMetricPower,
+    value: float,
+    *,
+    client: Client,
 ) -> Response[Union[Any, UnitMetricPowerSquaredConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMetricPower,
+    src_format: UnitMetricPower,
+    value: float,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, UnitMetricPowerSquaredConversion, Error]]:
-	""" Convert a metric squared unit value to another metric squared unit value. This is a nice endpoint to use for helper functions. """
+    """Convert a metric squared unit value to another metric squared unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
-	return sync_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	).parsed
+    return sync_detailed(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMetricPower,
+    src_format: UnitMetricPower,
+    value: float,
+    *,
+    client: Client,
 ) -> Response[Union[Any, UnitMetricPowerSquaredConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitMetricPower,
+    src_format: UnitMetricPower,
+    value: float,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, UnitMetricPowerSquaredConversion, Error]]:
-	""" Convert a metric squared unit value to another metric squared unit value. This is a nice endpoint to use for helper functions. """
+    """Convert a metric squared unit value to another metric squared unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
-	return (
-		await asyncio_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-			client=client,
-		)
-	).parsed
+    return (
+        await asyncio_detailed(
+            output_format=output_format,
+            src_format=src_format,
+            value=value,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/unit/get_metric_power_unit_conversion.py` & `kittycad-0.3.8/kittycad/api/unit/get_charge_unit_conversion.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,129 +1,140 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.unit_metric_power_conversion import UnitMetricPowerConversion
 from ...models.error import Error
-from ...models.unit_metric_power import UnitMetricPower
-from ...models.unit_metric_power import UnitMetricPower
+from ...models.unit_charge_conversion import UnitChargeConversion
+from ...models.unit_charge_format import UnitChargeFormat
 from ...types import Response
 
+
 def _get_kwargs(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitChargeFormat,
+    src_format: UnitChargeFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/metric/power/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
-
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
-
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitMetricPowerConversion, Error]]:
-	if response.status_code == 200:
-		response_200 = UnitMetricPowerConversion.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitMetricPowerConversion, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    url = "{}/unit/conversion/charge/{src_format}/{output_format}".format(
+        client.base_url, output_format=output_format, src_format=src_format
+    )  # noqa: E501
+    if value is not None:
+        if "?" in url:
+            url = url + "&value=" + str(value)
+        else:
+            url = url + "?value=" + str(value)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, UnitChargeConversion, Error]]:
+    if response.status_code == 200:
+        response_200 = UnitChargeConversion.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, UnitChargeConversion, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
-	value: float,
-	*,
-	client: Client,
-) -> Response[Union[Any, UnitMetricPowerConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    output_format: UnitChargeFormat,
+    src_format: UnitChargeFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Response[Union[Any, UnitChargeConversion, Error]]:
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
-	value: float,
-	*,
-	client: Client,
-) -> Optional[Union[Any, UnitMetricPowerConversion, Error]]:
-	""" Convert a metric unit value to another metric unit value. This is a nice endpoint to use for helper functions. """
-
-	return sync_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	).parsed
+    output_format: UnitChargeFormat,
+    src_format: UnitChargeFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Optional[Union[Any, UnitChargeConversion, Error]]:
+    """Convert a charge unit value to another charge unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+
+    return sync_detailed(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
-	value: float,
-	*,
-	client: Client,
-) -> Response[Union[Any, UnitMetricPowerConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
+    output_format: UnitChargeFormat,
+    src_format: UnitChargeFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Response[Union[Any, UnitChargeConversion, Error]]:
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
-	value: float,
-	*,
-	client: Client,
-) -> Optional[Union[Any, UnitMetricPowerConversion, Error]]:
-	""" Convert a metric unit value to another metric unit value. This is a nice endpoint to use for helper functions. """
-
-	return (
-		await asyncio_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-			client=client,
-		)
-	).parsed
+    output_format: UnitChargeFormat,
+    src_format: UnitChargeFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Optional[Union[Any, UnitChargeConversion, Error]]:
+    """Convert a charge unit value to another charge unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            output_format=output_format,
+            src_format=src_format,
+            value=value,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/unit/get_power_unit_conversion.py` & `kittycad-0.3.8/kittycad/api/unit/get_power_unit_conversion.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,129 +1,140 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.unit_power_conversion import UnitPowerConversion
 from ...models.error import Error
-from ...models.unit_power_format import UnitPowerFormat
+from ...models.unit_power_conversion import UnitPowerConversion
 from ...models.unit_power_format import UnitPowerFormat
 from ...types import Response
 
+
 def _get_kwargs(
-	output_format: UnitPowerFormat,
-	src_format: UnitPowerFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitPowerFormat,
+    src_format: UnitPowerFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/power/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
+    url = "{}/unit/conversion/power/{src_format}/{output_format}".format(
+        client.base_url, output_format=output_format, src_format=src_format
+    )  # noqa: E501
+    if value is not None:
+        if "?" in url:
+            url = url + "&value=" + str(value)
+        else:
+            url = url + "?value=" + str(value)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitPowerConversion, Error]]:
-	if response.status_code == 200:
-		response_200 = UnitPowerConversion.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitPowerConversion, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, UnitPowerConversion, Error]]:
+    if response.status_code == 200:
+        response_200 = UnitPowerConversion.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, UnitPowerConversion, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	output_format: UnitPowerFormat,
-	src_format: UnitPowerFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitPowerFormat,
+    src_format: UnitPowerFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Response[Union[Any, UnitPowerConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitPowerFormat,
-	src_format: UnitPowerFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitPowerFormat,
+    src_format: UnitPowerFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, UnitPowerConversion, Error]]:
-	""" Convert a power unit value to another power unit value. This is a nice endpoint to use for helper functions. """
+    """Convert a power unit value to another power unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
-	return sync_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	).parsed
+    return sync_detailed(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitPowerFormat,
-	src_format: UnitPowerFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitPowerFormat,
+    src_format: UnitPowerFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Response[Union[Any, UnitPowerConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitPowerFormat,
-	src_format: UnitPowerFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitPowerFormat,
+    src_format: UnitPowerFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, UnitPowerConversion, Error]]:
-	""" Convert a power unit value to another power unit value. This is a nice endpoint to use for helper functions. """
+    """Convert a power unit value to another power unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
 
-	return (
-		await asyncio_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-			client=client,
-		)
-	).parsed
+    return (
+        await asyncio_detailed(
+            output_format=output_format,
+            src_format=src_format,
+            value=value,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/unit/get_pressure_unit_conversion.py` & `kittycad-0.3.8/kittycad/api/unit/get_force_unit_conversion.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,129 +1,140 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.unit_pressure_conversion import UnitPressureConversion
 from ...models.error import Error
-from ...models.unit_pressure_format import UnitPressureFormat
-from ...models.unit_pressure_format import UnitPressureFormat
+from ...models.unit_force_conversion import UnitForceConversion
+from ...models.unit_force_format import UnitForceFormat
 from ...types import Response
 
+
 def _get_kwargs(
-	output_format: UnitPressureFormat,
-	src_format: UnitPressureFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitForceFormat,
+    src_format: UnitForceFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/pressure/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
-
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
-
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitPressureConversion, Error]]:
-	if response.status_code == 200:
-		response_200 = UnitPressureConversion.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitPressureConversion, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    url = "{}/unit/conversion/force/{src_format}/{output_format}".format(
+        client.base_url, output_format=output_format, src_format=src_format
+    )  # noqa: E501
+    if value is not None:
+        if "?" in url:
+            url = url + "&value=" + str(value)
+        else:
+            url = url + "?value=" + str(value)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, UnitForceConversion, Error]]:
+    if response.status_code == 200:
+        response_200 = UnitForceConversion.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, UnitForceConversion, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	output_format: UnitPressureFormat,
-	src_format: UnitPressureFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Response[Union[Any, UnitPressureConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    output_format: UnitForceFormat,
+    src_format: UnitForceFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Response[Union[Any, UnitForceConversion, Error]]:
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitPressureFormat,
-	src_format: UnitPressureFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Optional[Union[Any, UnitPressureConversion, Error]]:
-	""" Convert a pressure unit value to another pressure unit value. This is a nice endpoint to use for helper functions. """
-
-	return sync_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	).parsed
+    output_format: UnitForceFormat,
+    src_format: UnitForceFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Optional[Union[Any, UnitForceConversion, Error]]:
+    """Convert a force unit value to another force unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+
+    return sync_detailed(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitPressureFormat,
-	src_format: UnitPressureFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Response[Union[Any, UnitPressureConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
+    output_format: UnitForceFormat,
+    src_format: UnitForceFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Response[Union[Any, UnitForceConversion, Error]]:
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitPressureFormat,
-	src_format: UnitPressureFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Optional[Union[Any, UnitPressureConversion, Error]]:
-	""" Convert a pressure unit value to another pressure unit value. This is a nice endpoint to use for helper functions. """
-
-	return (
-		await asyncio_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-			client=client,
-		)
-	).parsed
+    output_format: UnitForceFormat,
+    src_format: UnitForceFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Optional[Union[Any, UnitForceConversion, Error]]:
+    """Convert a force unit value to another force unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            output_format=output_format,
+            src_format=src_format,
+            value=value,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/unit/get_radioactivity_unit_conversion.py` & `kittycad-0.3.8/kittycad/api/unit/get_voltage_unit_conversion.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,129 +1,140 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.unit_radioactivity_conversion import UnitRadioactivityConversion
 from ...models.error import Error
-from ...models.unit_radioactivity_format import UnitRadioactivityFormat
-from ...models.unit_radioactivity_format import UnitRadioactivityFormat
+from ...models.unit_voltage_conversion import UnitVoltageConversion
+from ...models.unit_voltage_format import UnitVoltageFormat
 from ...types import Response
 
+
 def _get_kwargs(
-	output_format: UnitRadioactivityFormat,
-	src_format: UnitRadioactivityFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitVoltageFormat,
+    src_format: UnitVoltageFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/radioactivity/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
-
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
-
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitRadioactivityConversion, Error]]:
-	if response.status_code == 200:
-		response_200 = UnitRadioactivityConversion.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitRadioactivityConversion, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    url = "{}/unit/conversion/voltage/{src_format}/{output_format}".format(
+        client.base_url, output_format=output_format, src_format=src_format
+    )  # noqa: E501
+    if value is not None:
+        if "?" in url:
+            url = url + "&value=" + str(value)
+        else:
+            url = url + "?value=" + str(value)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, UnitVoltageConversion, Error]]:
+    if response.status_code == 200:
+        response_200 = UnitVoltageConversion.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, UnitVoltageConversion, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	output_format: UnitRadioactivityFormat,
-	src_format: UnitRadioactivityFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Response[Union[Any, UnitRadioactivityConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    output_format: UnitVoltageFormat,
+    src_format: UnitVoltageFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Response[Union[Any, UnitVoltageConversion, Error]]:
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitRadioactivityFormat,
-	src_format: UnitRadioactivityFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Optional[Union[Any, UnitRadioactivityConversion, Error]]:
-	""" Convert a radioactivity unit value to another radioactivity unit value. This is a nice endpoint to use for helper functions. """
-
-	return sync_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	).parsed
+    output_format: UnitVoltageFormat,
+    src_format: UnitVoltageFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Optional[Union[Any, UnitVoltageConversion, Error]]:
+    """Convert a voltage unit value to another voltage unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+
+    return sync_detailed(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitRadioactivityFormat,
-	src_format: UnitRadioactivityFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Response[Union[Any, UnitRadioactivityConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
+    output_format: UnitVoltageFormat,
+    src_format: UnitVoltageFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Response[Union[Any, UnitVoltageConversion, Error]]:
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitRadioactivityFormat,
-	src_format: UnitRadioactivityFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Optional[Union[Any, UnitRadioactivityConversion, Error]]:
-	""" Convert a radioactivity unit value to another radioactivity unit value. This is a nice endpoint to use for helper functions. """
-
-	return (
-		await asyncio_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-			client=client,
-		)
-	).parsed
+    output_format: UnitVoltageFormat,
+    src_format: UnitVoltageFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Optional[Union[Any, UnitVoltageConversion, Error]]:
+    """Convert a voltage unit value to another voltage unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            output_format=output_format,
+            src_format=src_format,
+            value=value,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/unit/get_temperature_unit_conversion.py` & `kittycad-0.3.8/kittycad/api/unit/get_angle_unit_conversion.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,129 +1,140 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.unit_temperature_conversion import UnitTemperatureConversion
 from ...models.error import Error
-from ...models.unit_temperature_format import UnitTemperatureFormat
-from ...models.unit_temperature_format import UnitTemperatureFormat
+from ...models.unit_angle_conversion import UnitAngleConversion
+from ...models.unit_angle_format import UnitAngleFormat
 from ...types import Response
 
+
 def _get_kwargs(
-	output_format: UnitTemperatureFormat,
-	src_format: UnitTemperatureFormat,
-	value: float,
-	*,
-	client: Client,
+    output_format: UnitAngleFormat,
+    src_format: UnitAngleFormat,
+    value: float,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/temperature/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
-
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
-
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitTemperatureConversion, Error]]:
-	if response.status_code == 200:
-		response_200 = UnitTemperatureConversion.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitTemperatureConversion, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    url = "{}/unit/conversion/angle/{src_format}/{output_format}".format(
+        client.base_url, output_format=output_format, src_format=src_format
+    )  # noqa: E501
+    if value is not None:
+        if "?" in url:
+            url = url + "&value=" + str(value)
+        else:
+            url = url + "?value=" + str(value)
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, UnitAngleConversion, Error]]:
+    if response.status_code == 200:
+        response_200 = UnitAngleConversion.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, UnitAngleConversion, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	output_format: UnitTemperatureFormat,
-	src_format: UnitTemperatureFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Response[Union[Any, UnitTemperatureConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    output_format: UnitAngleFormat,
+    src_format: UnitAngleFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Response[Union[Any, UnitAngleConversion, Error]]:
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitTemperatureFormat,
-	src_format: UnitTemperatureFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Optional[Union[Any, UnitTemperatureConversion, Error]]:
-	""" Convert a temperature unit value to another temperature unit value. This is a nice endpoint to use for helper functions. """
-
-	return sync_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	).parsed
+    output_format: UnitAngleFormat,
+    src_format: UnitAngleFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Optional[Union[Any, UnitAngleConversion, Error]]:
+    """Convert an angle unit value to another angle unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+
+    return sync_detailed(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitTemperatureFormat,
-	src_format: UnitTemperatureFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Response[Union[Any, UnitTemperatureConversion, Error]]:
-	kwargs = _get_kwargs(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-		client=client,
-	)
+    output_format: UnitAngleFormat,
+    src_format: UnitAngleFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Response[Union[Any, UnitAngleConversion, Error]]:
+    kwargs = _get_kwargs(
+        output_format=output_format,
+        src_format=src_format,
+        value=value,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitTemperatureFormat,
-	src_format: UnitTemperatureFormat,
-	value: float,
-	*,
-	client: Client,
-) -> Optional[Union[Any, UnitTemperatureConversion, Error]]:
-	""" Convert a temperature unit value to another temperature unit value. This is a nice endpoint to use for helper functions. """
-
-	return (
-		await asyncio_detailed(
-		output_format=output_format,
-		src_format=src_format,
-		value=value,
-			client=client,
-		)
-	).parsed
+    output_format: UnitAngleFormat,
+    src_format: UnitAngleFormat,
+    value: float,
+    *,
+    client: Client,
+) -> Optional[Union[Any, UnitAngleConversion, Error]]:
+    """Convert an angle unit value to another angle unit value. This is a nice endpoint to use for helper functions."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            output_format=output_format,
+            src_format=src_format,
+            value=value,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/users/get_user_front_hash_self.py` & `kittycad-0.3.8/kittycad/api/api_tokens/delete_api_token_for_user.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,113 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.str import str
 from ...models.error import Error
 from ...types import Response
 
+
 def _get_kwargs(
-	*,
-	client: Client,
+    token: str,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/user/front-hash".format(client.base_url)
-
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
-
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, str, Error]]:
-	if response.status_code == 200:
-		response_200 = response.text
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, str, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    url = "{}/user/api-tokens/{token}".format(
+        client.base_url, token=token
+    )  # noqa: E501
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
+    if response.status_code == 204:
+        response_204 = None
+        return response_204
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, str, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    token: str,
+    *,
+    client: Client,
+) -> Response[Union[Any, Error]]:
+    kwargs = _get_kwargs(
+        token=token,
+        client=client,
+    )
+
+    response = httpx.delete(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	*,
-	client: Client,
-) -> Optional[Union[Any, str, Error]]:
-	""" This info is sent to front when initialing the front chat, it prevents impersonations using js hacks in the browser """
-
-	return sync_detailed(
-		client=client,
-	).parsed
+    token: str,
+    *,
+    client: Client,
+) -> Optional[Union[Any, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It deletes the requested API token for the user.
+    This endpoint does not actually delete the API token from the database. It merely marks the token as invalid. We still want to keep the token in the database for historical purposes."""  # noqa: E501
+
+    return sync_detailed(
+        token=token,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, str, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
+    token: str,
+    *,
+    client: Client,
+) -> Response[Union[Any, Error]]:
+    kwargs = _get_kwargs(
+        token=token,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.delete(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	*,
-	client: Client,
-) -> Optional[Union[Any, str, Error]]:
-	""" This info is sent to front when initialing the front chat, it prevents impersonations using js hacks in the browser """
-
-	return (
-		await asyncio_detailed(
-			client=client,
-		)
-	).parsed
+    token: str,
+    *,
+    client: Client,
+) -> Optional[Union[Any, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It deletes the requested API token for the user.
+    This endpoint does not actually delete the API token from the database. It merely marks the token as invalid. We still want to keep the token in the database for historical purposes."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            token=token,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/users/get_user_onboarding_self.py` & `kittycad-0.3.8/kittycad/api/apps/apps_github_callback.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,102 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.onboarding import Onboarding
 from ...models.error import Error
 from ...types import Response
 
+
 def _get_kwargs(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/user/onboarding".format(client.base_url)
+    url = "{}/apps/github/callback".format(client.base_url)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Onboarding, Error]]:
-	if response.status_code == 200:
-		response_200 = Onboarding.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Onboarding, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
+    if response.status_code == 204:
+        response_204 = None
+        return response_204
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, Onboarding, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	*,
-	client: Client,
-) -> Optional[Union[Any, Onboarding, Error]]:
-	""" Checks key part of their api usage to determine their onboarding progress """
-
-	return sync_detailed(
-		client=client,
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, Error]]:
+    """This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
+    The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos."""  # noqa: E501
+
+    return sync_detailed(
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, Onboarding, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
+    *,
+    client: Client,
+) -> Response[Union[Any, Error]]:
+    kwargs = _get_kwargs(
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	*,
-	client: Client,
-) -> Optional[Union[Any, Onboarding, Error]]:
-	""" Checks key part of their api usage to determine their onboarding progress """
-
-	return (
-		await asyncio_detailed(
-			client=client,
-		)
-	).parsed
+    *,
+    client: Client,
+) -> Optional[Union[Any, Error]]:
+    """This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
+    The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/users/get_user_self.py` & `kittycad-0.3.8/kittycad/api/apps/apps_github_webhook.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,102 +1,110 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.user import User
 from ...models.error import Error
 from ...types import Response
 
+
 def _get_kwargs(
-	*,
-	client: Client,
+    body: bytes,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/user".format(client.base_url)
+    url = "{}/apps/github/webhook".format(client.base_url)  # noqa: E501
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, User, Error]]:
-	if response.status_code == 200:
-		response_200 = User.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, User, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "content": body,
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Error]]:
+    if response.status_code == 204:
+        response_204 = None
+        return response_204
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, User, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    body: bytes,
+    *,
+    client: Client,
+) -> Response[Union[Any, Error]]:
+    kwargs = _get_kwargs(
+        body=body,
+        client=client,
+    )
+
+    response = httpx.post(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	*,
-	client: Client,
-) -> Optional[Union[Any, User, Error]]:
-	""" Get the user information for the authenticated user.
-Alternatively, you can also use the `/users/me` endpoint. """
-
-	return sync_detailed(
-		client=client,
-	).parsed
+    body: bytes,
+    *,
+    client: Client,
+) -> Optional[Union[Any, Error]]:
+    """These come from the GitHub app."""  # noqa: E501
+
+    return sync_detailed(
+        body=body,
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	*,
-	client: Client,
-) -> Response[Union[Any, User, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
+    body: bytes,
+    *,
+    client: Client,
+) -> Response[Union[Any, Error]]:
+    kwargs = _get_kwargs(
+        body=body,
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.post(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	*,
-	client: Client,
-) -> Optional[Union[Any, User, Error]]:
-	""" Get the user information for the authenticated user.
-Alternatively, you can also use the `/users/me` endpoint. """
-
-	return (
-		await asyncio_detailed(
-			client=client,
-		)
-	).parsed
+    body: bytes,
+    *,
+    client: Client,
+) -> Optional[Union[Any, Error]]:
+    """These come from the GitHub app."""  # noqa: E501
+
+    return (
+        await asyncio_detailed(
+            body=body,
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/api/users/get_user_self_extended.py` & `kittycad-0.3.8/kittycad/api/users/get_user_self_extended.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,102 +1,107 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.extended_user import ExtendedUser
 from ...models.error import Error
+from ...models.extended_user import ExtendedUser
 from ...types import Response
 
+
 def _get_kwargs(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/user/extended".format(client.base_url)
+    url = "{}/user/extended".format(client.base_url)  # noqa: E501
+
+    headers: Dict[str, Any] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+    }
 
-	headers: Dict[str, Any] = client.get_headers()
-	cookies: Dict[str, Any] = client.get_cookies()
 
-	return {
-		"url": url,
-		"headers": headers,
-		"cookies": cookies,
-		"timeout": client.get_timeout(),
-	}
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ExtendedUser, Error]]:
-	if response.status_code == 200:
-		response_200 = ExtendedUser.from_dict(response.json())
-		return response_200
-	if response.status_code == 400:
-		response_4XX = Error.from_dict(response.json())
-		return response_4XX
-	if response.status_code == 500:
-		response_5XX = Error.from_dict(response.json())
-		return response_5XX
-	return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ExtendedUser, Error]]:
-	return Response(
-		status_code=response.status_code,
-		content=response.content,
-		headers=response.headers,
-		parsed=_parse_response(response=response),
-	)
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, ExtendedUser, Error]]:
+    if response.status_code == 200:
+        response_200 = ExtendedUser.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, ExtendedUser, Error]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
 
 
 def sync_detailed(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Response[Union[Any, ExtendedUser, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
-
-	response = httpx.get(
-		verify=client.verify_ssl,
-		**kwargs,
-	)
+    kwargs = _get_kwargs(
+        client=client,
+    )
+
+    response = httpx.get(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 def sync(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, ExtendedUser, Error]]:
-	""" Get the user information for the authenticated user.
-Alternatively, you can also use the `/users-extended/me` endpoint. """
+    """Get the user information for the authenticated user.
+    Alternatively, you can also use the `/users-extended/me` endpoint."""  # noqa: E501
 
-	return sync_detailed(
-		client=client,
-	).parsed
+    return sync_detailed(
+        client=client,
+    ).parsed
 
 
 async def asyncio_detailed(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Response[Union[Any, ExtendedUser, Error]]:
-	kwargs = _get_kwargs(
-		client=client,
-	)
+    kwargs = _get_kwargs(
+        client=client,
+    )
 
-	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.get(**kwargs)
 
-	return _build_response(response=response)
+    return _build_response(response=response)
 
 
 async def asyncio(
-	*,
-	client: Client,
+    *,
+    client: Client,
 ) -> Optional[Union[Any, ExtendedUser, Error]]:
-	""" Get the user information for the authenticated user.
-Alternatively, you can also use the `/users-extended/me` endpoint. """
+    """Get the user information for the authenticated user.
+    Alternatively, you can also use the `/users-extended/me` endpoint."""  # noqa: E501
 
-	return (
-		await asyncio_detailed(
-			client=client,
-		)
-	).parsed
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `kittycad-0.3.7/kittycad/client.py` & `kittycad-0.3.8/kittycad/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import ssl
-from typing import Dict, Union
+from typing import Dict, Optional, Union
 
 import attr
 
 
 @attr.s(auto_attribs=True)
 class Client:
-    """A Client which has been authenticated for use on secured endpoints of the KittyCAD API."""
+    """A Client which has been authenticated for use on secured endpoints of the KittyCAD API."""  # noqa: E501
 
     token: str = attr.ib(kw_only=True)
     base_url: str = attr.ib(default="https://api.kittycad.io")
     cookies: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
     headers: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
     timeout: float = attr.ib(50.0, kw_only=True)
     verify_ssl: Union[str, bool, ssl.SSLContext] = attr.ib(True, kw_only=True)
@@ -37,14 +37,24 @@
     def with_timeout(self, timeout: float) -> "Client":
         """Get a new client matching this one with a new timeout (in seconds)"""
         return attr.evolve(self, timeout=timeout)
 
 
 @attr.s(auto_attribs=True)
 class ClientFromEnv(Client):
-    """A Client which has been authenticated for use on secured endpoints that uses the KITTYCAD_API_TOKEN environment variable for the authentication token."""
+    """A Client which has been authenticated for use on secured endpoints that uses the KITTYCAD_API_TOKEN environment variable for the authentication token."""  # noqa: E501
 
-    token: str = attr.ib(default=os.getenv('KITTYCAD_API_TOKEN'))
+    token: str = attr.field()
+
+    @token.default
+    def set_token(self):
+        maybe_token: Optional[str] = os.getenv("KITTYCAD_API_TOKEN")
+        if maybe_token is None:
+            raise ValueError(
+                "KITTYCAD_API_TOKEN environment variable must be set to use ClientFromEnv"
+            )
+        token: str = maybe_token
+        return token
 
     def get_headers(self) -> Dict[str, str]:
         """Get headers to be used in authenticated endpoints"""
         return {"Authorization": f"Bearer {self.token}", **self.headers}
```

### Comparing `kittycad-0.3.7/kittycad/client_test.py` & `kittycad-0.3.8/kittycad/client_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 import os
+
 import pytest
-import asyncio
 
-from .client import ClientFromEnv
-from .models import FileConversion, FileExportFormat, FileImportFormat, User, Pong, ApiCallStatus, FileMass, FileVolume, ApiTokenResultsPage, CreatedAtSortMode
-from .api.file import create_file_conversion_with_base64_helper, create_file_mass, create_file_volume
-from .api.meta import ping
-from .api.users import get_user_self
 from .api.api_tokens import list_api_tokens_for_user
+from .api.file import (
+    create_file_conversion_with_base64_helper,
+    create_file_mass,
+    create_file_volume,
+)
+from .api.meta import ping
+from .api.users import get_user_self, list_users_extended
+from .client import ClientFromEnv
+from .models import (
+    ApiCallStatus,
+    ApiTokenResultsPage,
+    CreatedAtSortMode,
+    ExtendedUserResultsPage,
+    FileConversion,
+    FileExportFormat,
+    FileImportFormat,
+    FileMass,
+    FileVolume,
+    Pong,
+    User,
+)
 
 
 def test_get_session():
     # Create our client.
     client = ClientFromEnv()
 
     # Get the session.
@@ -25,15 +41,16 @@
 @pytest.mark.asyncio
 async def test_get_api_tokens_async():
     # Create our client.
     client = ClientFromEnv()
 
     # List API tokens.
     fc: ApiTokenResultsPage = list_api_tokens_for_user.sync(
-        client=client, sort_by=CreatedAtSortMode)
+        client=client, sort_by=CreatedAtSortMode
+    )
 
     assert fc is not None
 
     print(f"fc: {fc}")
 
 
 @pytest.mark.asyncio
@@ -84,15 +101,16 @@
     file.close()
 
     # Get the fc.
     fc: FileConversion = create_file_conversion_with_base64_helper.sync(
         client=client,
         body=content,
         src_format=FileImportFormat.STL,
-        output_format=FileExportFormat.OBJ)
+        output_format=FileExportFormat.OBJ,
+    )
 
     assert fc is not None
 
     print(f"FileConversion: {fc}")
 
     assert fc.id is not None
 
@@ -108,15 +126,20 @@
 
     dir_path = os.path.dirname(os.path.realpath(__file__))
     file = open(os.path.join(dir_path, "../assets/testing.stl"), "rb")
     content = file.read()
     file.close()
 
     # Get the fc.
-    fc: FileConversion = await create_file_conversion_with_base64_helper.asyncio(client=client, body=content, src_format=FileImportFormat.STL, output_format=FileExportFormat.OBJ)
+    fc: FileConversion = await create_file_conversion_with_base64_helper.asyncio(
+        client=client,
+        body=content,
+        src_format=FileImportFormat.STL,
+        output_format=FileExportFormat.OBJ,
+    )
 
     assert fc is not None
 
     print(f"FileConversion: {fc}")
 
     assert fc.id is not None
 
@@ -133,15 +156,16 @@
     file.close()
 
     # Get the fc.
     fm: FileMass = create_file_mass.sync(
         client=client,
         body=content,
         src_format=FileImportFormat.OBJ,
-        material_density=1.0)
+        material_density=1.0,
+    )
 
     assert fm is not None
 
     print(f"FileMass: {fm}")
 
     assert fm.id is not None
     assert fm.mass is not None
@@ -158,21 +182,34 @@
     dir_path = os.path.dirname(os.path.realpath(__file__))
     file = open(os.path.join(dir_path, "../assets/testing.obj"), "rb")
     content = file.read()
     file.close()
 
     # Get the fc.
     fv: FileVolume = create_file_volume.sync(
-        client=client,
-        body=content,
-        src_format=FileImportFormat.OBJ)
+        client=client, body=content, src_format=FileImportFormat.OBJ
+    )
 
     assert fv is not None
 
     print(f"FileVolume: {fv}")
 
     assert fv.id is not None
     assert fv.volume is not None
 
     assert fv.to_dict() is not None
 
     assert fv.status == ApiCallStatus.COMPLETED
+
+
+def test_list_users():
+    # Create our client.
+    client = ClientFromEnv()
+
+    response: ExtendedUserResultsPage = list_users_extended.sync(
+        sort_by=CreatedAtSortMode.CREATED_AT_DESCENDING, client=client, limit=10
+    )
+
+    print(f"ExtendedUserResultsPage: {response}")
+
+    assert response is not None
+    assert response.items is not None
```

### Comparing `kittycad-0.3.7/kittycad/models/__init__.py` & `kittycad-0.3.8/kittycad/models/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .api_call_status import ApiCallStatus
 from .api_call_with_price import ApiCallWithPrice
 from .api_call_with_price_results_page import ApiCallWithPriceResultsPage
 from .api_token import ApiToken
 from .api_token_results_page import ApiTokenResultsPage
 from .app_client_info import AppClientInfo
 from .async_api_call import AsyncApiCall
+from .async_api_call_output import AsyncApiCallOutput
 from .async_api_call_results_page import AsyncApiCallResultsPage
 from .async_api_call_type import AsyncApiCallType
 from .billing_info import BillingInfo
 from .cache_metadata import CacheMetadata
 from .card_details import CardDetails
 from .cluster import Cluster
 from .code_language import CodeLanguage
@@ -31,25 +32,28 @@
 from .currency import Currency
 from .customer import Customer
 from .customer_balance import CustomerBalance
 from .device_access_token_request_form import DeviceAccessTokenRequestForm
 from .device_auth_request_form import DeviceAuthRequestForm
 from .device_auth_verify_params import DeviceAuthVerifyParams
 from .docker_system_info import DockerSystemInfo
+from .drawing_cmd import DrawingCmd
+from .drawing_cmd_id import DrawingCmdId
+from .drawing_cmd_req import DrawingCmdReq
+from .drawing_cmd_req_batch import DrawingCmdReqBatch
+from .drawing_error import DrawingError
+from .drawing_outcome import DrawingOutcome
+from .drawing_outcomes import DrawingOutcomes
 from .email_authentication_form import EmailAuthenticationForm
 from .engine_metadata import EngineMetadata
 from .environment import Environment
 from .error import Error
 from .executor_metadata import ExecutorMetadata
 from .extended_user import ExtendedUser
 from .extended_user_results_page import ExtendedUserResultsPage
-from .file2_d_vector_conversion import File2DVectorConversion
-from .file2_d_vector_export_format import File2DVectorExportFormat
-from .file2_d_vector_import_format import File2DVectorImportFormat
-from .file3_d_import_format import File3DImportFormat
 from .file_center_of_mass import FileCenterOfMass
 from .file_conversion import FileConversion
 from .file_density import FileDensity
 from .file_export_format import FileExportFormat
 from .file_import_format import FileImportFormat
 from .file_mass import FileMass
 from .file_surface_area import FileSurfaceArea
```

### Comparing `kittycad-0.3.7/kittycad/models/ai_plugin_api.py` & `kittycad-0.3.8/kittycad/models/ai_plugin_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.ai_plugin_api_type import AiPluginApiType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="AiPluginApi")
+S = TypeVar("S", bound="AiPluginApi")
 
 
 @attr.s(auto_attribs=True)
 class AiPluginApi:
-    """ """
+    """AI plugin api information."""  # noqa: E501
+
     is_user_authenticated: Union[Unset, bool] = False
     type: Union[Unset, AiPluginApiType] = UNSET
     url: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         is_user_authenticated = self.is_user_authenticated
-        type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
-            type = self.type.value
+            type = self.type
         url = self.url
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if is_user_authenticated is not UNSET:
-            field_dict['is_user_authenticated'] = is_user_authenticated
+            field_dict["is_user_authenticated"] = is_user_authenticated
         if type is not UNSET:
-            field_dict['type'] = type
+            field_dict["type"] = type
         if url is not UNSET:
-            field_dict['url'] = url
+            field_dict["url"] = url
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
         d = src_dict.copy()
         is_user_authenticated = d.pop("is_user_authenticated", UNSET)
 
         _type = d.pop("type", UNSET)
         type: Union[Unset, AiPluginApiType]
         if isinstance(_type, Unset):
             type = UNSET
```

### Comparing `kittycad-0.3.7/kittycad/models/ai_plugin_auth.py` & `kittycad-0.3.8/kittycad/models/ai_plugin_auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.ai_plugin_http_auth_type import AiPluginHttpAuthType
 from ..models.ai_plugin_auth_type import AiPluginAuthType
+from ..models.ai_plugin_http_auth_type import AiPluginHttpAuthType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="AiPluginAuth")
+B = TypeVar("B", bound="AiPluginAuth")
 
 
 @attr.s(auto_attribs=True)
 class AiPluginAuth:
-    """ """
+    """AI plugin auth information."""  # noqa: E501
+
     authorization_type: Union[Unset, AiPluginHttpAuthType] = UNSET
     type: Union[Unset, AiPluginAuthType] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        authorization_type: Union[Unset, str] = UNSET
         if not isinstance(self.authorization_type, Unset):
-            authorization_type = self.authorization_type.value
-        type: Union[Unset, str] = UNSET
+            authorization_type = self.authorization_type
         if not isinstance(self.type, Unset):
-            type = self.type.value
+            type = self.type
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if authorization_type is not UNSET:
-            field_dict['authorization_type'] = authorization_type
+            field_dict["authorization_type"] = authorization_type
         if type is not UNSET:
-            field_dict['type'] = type
+            field_dict["type"] = type
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
         d = src_dict.copy()
         _authorization_type = d.pop("authorization_type", UNSET)
         authorization_type: Union[Unset, AiPluginHttpAuthType]
         if isinstance(_authorization_type, Unset):
             authorization_type = UNSET
         else:
             authorization_type = AiPluginHttpAuthType(_authorization_type)
```

### Comparing `kittycad-0.3.7/kittycad/models/ai_plugin_manifest.py` & `kittycad-0.3.8/kittycad/models/ai_plugin_manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,79 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.ai_plugin_api import AiPluginApi
 from ..models.ai_plugin_auth import AiPluginAuth
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="AiPluginManifest")
+N = TypeVar("N", bound="AiPluginManifest")
 
 
 @attr.s(auto_attribs=True)
 class AiPluginManifest:
-    """ """
+    """AI plugin manifest.
+
+    This is used for OpenAI's ChatGPT plugins. You can read more about them [here](https://platform.openai.com/docs/plugins/getting-started/plugin-manifest)."""  # noqa: E501
+
     api: Union[Unset, AiPluginApi] = UNSET
     auth: Union[Unset, AiPluginAuth] = UNSET
     contact_email: Union[Unset, str] = UNSET
     description_for_human: Union[Unset, str] = UNSET
     description_for_model: Union[Unset, str] = UNSET
     legal_info_url: Union[Unset, str] = UNSET
     logo_url: Union[Unset, str] = UNSET
     name_for_human: Union[Unset, str] = UNSET
     name_for_model: Union[Unset, str] = UNSET
     schema_version: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        api: Union[Unset, str] = UNSET
         if not isinstance(self.api, Unset):
-            api = self.api.value
-        auth: Union[Unset, str] = UNSET
+            api = self.api
         if not isinstance(self.auth, Unset):
-            auth = self.auth.value
+            auth = self.auth
         contact_email = self.contact_email
         description_for_human = self.description_for_human
         description_for_model = self.description_for_model
         legal_info_url = self.legal_info_url
         logo_url = self.logo_url
         name_for_human = self.name_for_human
         name_for_model = self.name_for_model
         schema_version = self.schema_version
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if api is not UNSET:
-            field_dict['api'] = api
+            field_dict["api"] = api
         if auth is not UNSET:
-            field_dict['auth'] = auth
+            field_dict["auth"] = auth
         if contact_email is not UNSET:
-            field_dict['contact_email'] = contact_email
+            field_dict["contact_email"] = contact_email
         if description_for_human is not UNSET:
-            field_dict['description_for_human'] = description_for_human
+            field_dict["description_for_human"] = description_for_human
         if description_for_model is not UNSET:
-            field_dict['description_for_model'] = description_for_model
+            field_dict["description_for_model"] = description_for_model
         if legal_info_url is not UNSET:
-            field_dict['legal_info_url'] = legal_info_url
+            field_dict["legal_info_url"] = legal_info_url
         if logo_url is not UNSET:
-            field_dict['logo_url'] = logo_url
+            field_dict["logo_url"] = logo_url
         if name_for_human is not UNSET:
-            field_dict['name_for_human'] = name_for_human
+            field_dict["name_for_human"] = name_for_human
         if name_for_model is not UNSET:
-            field_dict['name_for_model'] = name_for_model
+            field_dict["name_for_model"] = name_for_model
         if schema_version is not UNSET:
-            field_dict['schema_version'] = schema_version
+            field_dict["schema_version"] = schema_version
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         _api = d.pop("api", UNSET)
         api: Union[Unset, AiPluginApi]
         if isinstance(_api, Unset):
             api = UNSET
         else:
             api = AiPluginApi(_api)
```

### Comparing `kittycad-0.3.7/kittycad/models/api_call_query_group.py` & `kittycad-0.3.8/kittycad/models/api_call_query_group.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ApiCallQueryGroup")
+P = TypeVar("P", bound="ApiCallQueryGroup")
 
 
 @attr.s(auto_attribs=True)
 class ApiCallQueryGroup:
-    """ """
+    """A response for a query on the API call table that is grouped by something."""  # noqa: E501
+
     count: Union[Unset, int] = UNSET
     query: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
         query = self.query
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if count is not UNSET:
-            field_dict['count'] = count
+            field_dict["count"] = count
         if query is not UNSET:
-            field_dict['query'] = query
+            field_dict["query"] = query
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
         d = src_dict.copy()
         count = d.pop("count", UNSET)
 
         query = d.pop("query", UNSET)
 
         api_call_query_group = cls(
             count=count,
```

### Comparing `kittycad-0.3.7/kittycad/models/api_call_with_price.py` & `kittycad-0.3.8/kittycad/models/api_call_with_price.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
 from ..models.method import Method
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ApiCallWithPrice")
+S = TypeVar("S", bound="ApiCallWithPrice")
 
 
 @attr.s(auto_attribs=True)
 class ApiCallWithPrice:
-    """ """
+    """An API call with the price.
+
+    This is a join of the `ApiCall` and `ApiCallPrice` tables."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     duration: Union[Unset, int] = UNSET
     email: Union[Unset, str] = UNSET
     endpoint: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     ip_address: Union[Unset, str] = UNSET
@@ -48,17 +50,16 @@
             created_at = self.created_at.isoformat()
         duration = self.duration
         email = self.email
         endpoint = self.endpoint
         id = self.id
         ip_address = self.ip_address
         litterbox = self.litterbox
-        method: Union[Unset, str] = UNSET
         if not isinstance(self.method, Unset):
-            method = self.method.value
+            method = self.method
         minutes = self.minutes
         origin = self.origin
         price = self.price
         request_body = self.request_body
         request_query_params = self.request_query_params
         response_body = self.response_body
         started_at: Union[Unset, str] = UNSET
@@ -73,62 +74,62 @@
         user_agent = self.user_agent
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if duration is not UNSET:
-            field_dict['duration'] = duration
+            field_dict["duration"] = duration
         if email is not UNSET:
-            field_dict['email'] = email
+            field_dict["email"] = email
         if endpoint is not UNSET:
-            field_dict['endpoint'] = endpoint
+            field_dict["endpoint"] = endpoint
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if ip_address is not UNSET:
-            field_dict['ip_address'] = ip_address
+            field_dict["ip_address"] = ip_address
         if litterbox is not UNSET:
-            field_dict['litterbox'] = litterbox
+            field_dict["litterbox"] = litterbox
         if method is not UNSET:
-            field_dict['method'] = method
+            field_dict["method"] = method
         if minutes is not UNSET:
-            field_dict['minutes'] = minutes
+            field_dict["minutes"] = minutes
         if origin is not UNSET:
-            field_dict['origin'] = origin
+            field_dict["origin"] = origin
         if price is not UNSET:
-            field_dict['price'] = price
+            field_dict["price"] = price
         if request_body is not UNSET:
-            field_dict['request_body'] = request_body
+            field_dict["request_body"] = request_body
         if request_query_params is not UNSET:
-            field_dict['request_query_params'] = request_query_params
+            field_dict["request_query_params"] = request_query_params
         if response_body is not UNSET:
-            field_dict['response_body'] = response_body
+            field_dict["response_body"] = response_body
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status_code is not UNSET:
-            field_dict['status_code'] = status_code
+            field_dict["status_code"] = status_code
         if stripe_invoice_item_id is not UNSET:
-            field_dict['stripe_invoice_item_id'] = stripe_invoice_item_id
+            field_dict["stripe_invoice_item_id"] = stripe_invoice_item_id
         if token is not UNSET:
-            field_dict['token'] = token
+            field_dict["token"] = token
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_agent is not UNSET:
-            field_dict['user_agent'] = user_agent
+            field_dict["user_agent"] = user_agent
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/api_call_with_price_results_page.py` & `kittycad-0.3.8/kittycad/models/api_call_with_price_results_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ApiCallWithPriceResultsPage")
+A = TypeVar("A", bound="ApiCallWithPriceResultsPage")
 
 
 @attr.s(auto_attribs=True)
 class ApiCallWithPriceResultsPage:
-    """ """
+    """A single page of results"""  # noqa: E501
+
     from ..models.api_call_with_price import ApiCallWithPrice
+
     items: Union[Unset, List[ApiCallWithPrice]] = UNSET
     next_page: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         from ..models.api_call_with_price import ApiCallWithPrice
+
         items: Union[Unset, List[ApiCallWithPrice]] = UNSET
         if not isinstance(self.items, Unset):
             items = self.items
         next_page = self.next_page
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if items is not UNSET:
-            field_dict['items'] = items
+            field_dict["items"] = items
         if next_page is not UNSET:
-            field_dict['next_page'] = next_page
+            field_dict["next_page"] = next_page
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[A], src_dict: Dict[str, Any]) -> A:
         d = src_dict.copy()
         from ..models.api_call_with_price import ApiCallWithPrice
+
         items = cast(List[ApiCallWithPrice], d.pop("items", UNSET))
 
         next_page = d.pop("next_page", UNSET)
 
         api_call_with_price_results_page = cls(
             items=items,
             next_page=next_page,
```

### Comparing `kittycad-0.3.7/kittycad/models/api_token.py` & `kittycad-0.3.8/kittycad/models/api_token.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ApiToken")
+G = TypeVar("G", bound="ApiToken")
 
 
 @attr.s(auto_attribs=True)
 class ApiToken:
-    """ """
+    """An API token.
+
+    These are used to authenticate users with Bearer authentication."""  # noqa: E501
+
     created_at: Union[Unset, datetime.datetime] = UNSET
     id: Union[Unset, str] = UNSET
     is_valid: Union[Unset, bool] = False
     token: Union[Unset, str] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
@@ -34,30 +36,30 @@
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if is_valid is not UNSET:
-            field_dict['is_valid'] = is_valid
+            field_dict["is_valid"] = is_valid
         if token is not UNSET:
-            field_dict['token'] = token
+            field_dict["token"] = token
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[G], src_dict: Dict[str, Any]) -> G:
         d = src_dict.copy()
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/api_token_results_page.py` & `kittycad-0.3.8/kittycad/models/api_token_results_page.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ApiTokenResultsPage")
+P = TypeVar("P", bound="ApiTokenResultsPage")
 
 
 @attr.s(auto_attribs=True)
 class ApiTokenResultsPage:
-    """ """
+    """A single page of results"""  # noqa: E501
+
     from ..models.api_token import ApiToken
+
     items: Union[Unset, List[ApiToken]] = UNSET
     next_page: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         from ..models.api_token import ApiToken
+
         items: Union[Unset, List[ApiToken]] = UNSET
         if not isinstance(self.items, Unset):
             items = self.items
         next_page = self.next_page
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if items is not UNSET:
-            field_dict['items'] = items
+            field_dict["items"] = items
         if next_page is not UNSET:
-            field_dict['next_page'] = next_page
+            field_dict["next_page"] = next_page
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
         d = src_dict.copy()
         from ..models.api_token import ApiToken
+
         items = cast(List[ApiToken], d.pop("items", UNSET))
 
         next_page = d.pop("next_page", UNSET)
 
         api_token_results_page = cls(
             items=items,
             next_page=next_page,
```

### Comparing `kittycad-0.3.7/kittycad/models/app_client_info.py` & `kittycad-0.3.8/kittycad/models/cache_metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,48 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="AppClientInfo")
+L = TypeVar("L", bound="CacheMetadata")
 
 
 @attr.s(auto_attribs=True)
-class AppClientInfo:
-    """ """
-    url: Union[Unset, str] = UNSET
+class CacheMetadata:
+    """Metadata about our cache.
+
+    This is mostly used for internal purposes and debugging."""  # noqa: E501
+
+    ok: Union[Unset, bool] = False
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        url = self.url
+        ok = self.ok
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if url is not UNSET:
-            field_dict['url'] = url
+        if ok is not UNSET:
+            field_dict["ok"] = ok
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
-        url = d.pop("url", UNSET)
+        ok = d.pop("ok", UNSET)
 
-        app_client_info = cls(
-            url=url,
+        cache_metadata = cls(
+            ok=ok,
         )
 
-        app_client_info.additional_properties = d
-        return app_client_info
+        cache_metadata.additional_properties = d
+        return cache_metadata
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/async_api_call.py` & `kittycad-0.3.8/kittycad/models/async_api_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
 from ..models.api_call_status import ApiCallStatus
 from ..models.async_api_call_type import AsyncApiCallType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="AsyncApiCall")
+Z = TypeVar("Z", bound="AsyncApiCall")
 
 
 @attr.s(auto_attribs=True)
 class AsyncApiCall:
-    """ """
+    """An async API call."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, Any] = UNSET
     output: Union[Unset, Any] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
@@ -40,58 +40,56 @@
         error = self.error
         id = self.id
         input = self.input
         output = self.output
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
-        type: Union[Unset, str] = UNSET
+            status = self.status
         if not isinstance(self.type, Unset):
-            type = self.type.value
+            type = self.type
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
         worker = self.worker
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if type is not UNSET:
-            field_dict['type'] = type
+            field_dict["type"] = type
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
         if worker is not UNSET:
-            field_dict['worker'] = worker
+            field_dict["worker"] = worker
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[Z], src_dict: Dict[str, Any]) -> Z:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/async_api_call_results_page.py` & `kittycad-0.3.8/kittycad/models/async_api_call_results_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="AsyncApiCallResultsPage")
+H = TypeVar("H", bound="AsyncApiCallResultsPage")
 
 
 @attr.s(auto_attribs=True)
 class AsyncApiCallResultsPage:
-    """ """
+    """A single page of results"""  # noqa: E501
+
     from ..models.async_api_call import AsyncApiCall
+
     items: Union[Unset, List[AsyncApiCall]] = UNSET
     next_page: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         from ..models.async_api_call import AsyncApiCall
+
         items: Union[Unset, List[AsyncApiCall]] = UNSET
         if not isinstance(self.items, Unset):
             items = self.items
         next_page = self.next_page
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if items is not UNSET:
-            field_dict['items'] = items
+            field_dict["items"] = items
         if next_page is not UNSET:
-            field_dict['next_page'] = next_page
+            field_dict["next_page"] = next_page
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         from ..models.async_api_call import AsyncApiCall
+
         items = cast(List[AsyncApiCall], d.pop("items", UNSET))
 
         next_page = d.pop("next_page", UNSET)
 
         async_api_call_results_page = cls(
             items=items,
             next_page=next_page,
```

### Comparing `kittycad-0.3.7/kittycad/models/billing_info.py` & `kittycad-0.3.8/kittycad/models/billing_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.new_address import NewAddress
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="BillingInfo")
+X = TypeVar("X", bound="BillingInfo")
 
 
 @attr.s(auto_attribs=True)
 class BillingInfo:
-    """ """
+    """The billing information for payments."""  # noqa: E501
+
     address: Union[Unset, NewAddress] = UNSET
     name: Union[Unset, str] = UNSET
     phone: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        address: Union[Unset, str] = UNSET
         if not isinstance(self.address, Unset):
-            address = self.address.value
+            address = self.address
         name = self.name
         phone = self.phone
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if address is not UNSET:
-            field_dict['address'] = address
+            field_dict["address"] = address
         if name is not UNSET:
-            field_dict['name'] = name
+            field_dict["name"] = name
         if phone is not UNSET:
-            field_dict['phone'] = phone
+            field_dict["phone"] = phone
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[X], src_dict: Dict[str, Any]) -> X:
         d = src_dict.copy()
         _address = d.pop("address", UNSET)
         address: Union[Unset, NewAddress]
         if isinstance(_address, Unset):
             address = UNSET
         else:
             address = NewAddress(_address)
```

### Comparing `kittycad-0.3.7/kittycad/models/cache_metadata.py` & `kittycad-0.3.8/kittycad/models/pong.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CacheMetadata")
+E = TypeVar("E", bound="Pong")
 
 
 @attr.s(auto_attribs=True)
-class CacheMetadata:
-    """ """
-    ok: Union[Unset, bool] = False
+class Pong:
+    """The response from the `/ping` endpoint."""  # noqa: E501
+
+    message: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        ok = self.ok
+        message = self.message
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if ok is not UNSET:
-            field_dict['ok'] = ok
+        if message is not UNSET:
+            field_dict["message"] = message
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
         d = src_dict.copy()
-        ok = d.pop("ok", UNSET)
+        message = d.pop("message", UNSET)
 
-        cache_metadata = cls(
-            ok=ok,
+        pong = cls(
+            message=message,
         )
 
-        cache_metadata.additional_properties = d
-        return cache_metadata
+        pong.additional_properties = d
+        return pong
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/card_details.py` & `kittycad-0.3.8/kittycad/models/card_details.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.payment_method_card_checks import PaymentMethodCardChecks
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CardDetails")
+B = TypeVar("B", bound="CardDetails")
 
 
 @attr.s(auto_attribs=True)
 class CardDetails:
-    """ """
+    """The card details of a payment method."""  # noqa: E501
+
     brand: Union[Unset, str] = UNSET
     checks: Union[Unset, PaymentMethodCardChecks] = UNSET
     country: Union[Unset, str] = UNSET
     exp_month: Union[Unset, int] = UNSET
     exp_year: Union[Unset, int] = UNSET
     fingerprint: Union[Unset, str] = UNSET
     funding: Union[Unset, str] = UNSET
     last4: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         brand = self.brand
-        checks: Union[Unset, str] = UNSET
         if not isinstance(self.checks, Unset):
-            checks = self.checks.value
+            checks = self.checks
         country = self.country
         exp_month = self.exp_month
         exp_year = self.exp_year
         fingerprint = self.fingerprint
         funding = self.funding
         last4 = self.last4
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if brand is not UNSET:
-            field_dict['brand'] = brand
+            field_dict["brand"] = brand
         if checks is not UNSET:
-            field_dict['checks'] = checks
+            field_dict["checks"] = checks
         if country is not UNSET:
-            field_dict['country'] = country
+            field_dict["country"] = country
         if exp_month is not UNSET:
-            field_dict['exp_month'] = exp_month
+            field_dict["exp_month"] = exp_month
         if exp_year is not UNSET:
-            field_dict['exp_year'] = exp_year
+            field_dict["exp_year"] = exp_year
         if fingerprint is not UNSET:
-            field_dict['fingerprint'] = fingerprint
+            field_dict["fingerprint"] = fingerprint
         if funding is not UNSET:
-            field_dict['funding'] = funding
+            field_dict["funding"] = funding
         if last4 is not UNSET:
-            field_dict['last4'] = last4
+            field_dict["last4"] = last4
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
         d = src_dict.copy()
         brand = d.pop("brand", UNSET)
 
         _checks = d.pop("checks", UNSET)
         checks: Union[Unset, PaymentMethodCardChecks]
         if isinstance(_checks, Unset):
             checks = UNSET
```

### Comparing `kittycad-0.3.7/kittycad/models/cluster.py` & `kittycad-0.3.8/kittycad/models/cluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Cluster")
+N = TypeVar("N", bound="Cluster")
 
 
 @attr.s(auto_attribs=True)
 class Cluster:
-    """ """
+    """Cluster information."""  # noqa: E501
+
     addr: Union[Unset, str] = UNSET
     auth_timeout: Union[Unset, int] = UNSET
     cluster_port: Union[Unset, int] = UNSET
     name: Union[Unset, str] = UNSET
     tls_timeout: Union[Unset, int] = UNSET
     urls: Union[Unset, List[str]] = UNSET
 
@@ -29,30 +30,30 @@
         if not isinstance(self.urls, Unset):
             urls = self.urls
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if addr is not UNSET:
-            field_dict['addr'] = addr
+            field_dict["addr"] = addr
         if auth_timeout is not UNSET:
-            field_dict['auth_timeout'] = auth_timeout
+            field_dict["auth_timeout"] = auth_timeout
         if cluster_port is not UNSET:
-            field_dict['cluster_port'] = cluster_port
+            field_dict["cluster_port"] = cluster_port
         if name is not UNSET:
-            field_dict['name'] = name
+            field_dict["name"] = name
         if tls_timeout is not UNSET:
-            field_dict['tls_timeout'] = tls_timeout
+            field_dict["tls_timeout"] = tls_timeout
         if urls is not UNSET:
-            field_dict['urls'] = urls
+            field_dict["urls"] = urls
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         addr = d.pop("addr", UNSET)
 
         auth_timeout = d.pop("auth_timeout", UNSET)
 
         cluster_port = d.pop("cluster_port", UNSET)
```

### Comparing `kittycad-0.3.7/kittycad/models/code_output.py` & `kittycad-0.3.8/kittycad/models/code_output.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CodeOutput")
+E = TypeVar("E", bound="CodeOutput")
 
 
 @attr.s(auto_attribs=True)
 class CodeOutput:
-    """ """
+    """Output of the code being executed."""  # noqa: E501
+
     from ..models.output_file import OutputFile
+
     output_files: Union[Unset, List[OutputFile]] = UNSET
     stderr: Union[Unset, str] = UNSET
     stdout: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         from ..models.output_file import OutputFile
+
         output_files: Union[Unset, List[OutputFile]] = UNSET
         if not isinstance(self.output_files, Unset):
             output_files = self.output_files
         stderr = self.stderr
         stdout = self.stdout
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if output_files is not UNSET:
-            field_dict['output_files'] = output_files
+            field_dict["output_files"] = output_files
         if stderr is not UNSET:
-            field_dict['stderr'] = stderr
+            field_dict["stderr"] = stderr
         if stdout is not UNSET:
-            field_dict['stdout'] = stdout
+            field_dict["stdout"] = stdout
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
         d = src_dict.copy()
         from ..models.output_file import OutputFile
+
         output_files = cast(List[OutputFile], d.pop("output_files", UNSET))
 
         stderr = d.pop("stderr", UNSET)
 
         stdout = d.pop("stdout", UNSET)
 
         code_output = cls(
```

### Comparing `kittycad-0.3.7/kittycad/models/commit.py` & `kittycad-0.3.8/kittycad/models/mesh.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,44 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Commit")
+F = TypeVar("F", bound="Mesh")
 
 
 @attr.s(auto_attribs=True)
-class Commit:
-    """ """
-    expected: Union[Unset, str] = UNSET
-    id: Union[Unset, str] = UNSET
+class Mesh:
+    mesh: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        expected = self.expected
-        id = self.id
+        mesh = self.mesh
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if expected is not UNSET:
-            field_dict['expected'] = expected
-        if id is not UNSET:
-            field_dict['id'] = id
+        if mesh is not UNSET:
+            field_dict["mesh"] = mesh
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
-        expected = d.pop("expected", UNSET)
+        mesh = d.pop("mesh", UNSET)
 
-        id = d.pop("id", UNSET)
-
-        commit = cls(
-            expected=expected,
-            id=id,
+        mesh = cls(
+            mesh=mesh,
         )
 
-        commit.additional_properties = d
-        return commit
+        mesh.additional_properties = d
+        return mesh
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/connection.py` & `kittycad-0.3.8/kittycad/models/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.cluster import Cluster
 from ..models.gateway import Gateway
 from ..models.jetstream import Jetstream
 from ..models.leaf_node import LeafNode
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Connection")
+L = TypeVar("L", bound="Connection")
 
 
 @attr.s(auto_attribs=True)
 class Connection:
-    """ """
+    """Metadata about a pub-sub connection.
+
+    This is mostly used for internal purposes and debugging."""  # noqa: E501
+
     auth_timeout: Union[Unset, int] = UNSET
     cluster: Union[Unset, Cluster] = UNSET
     config_load_time: Union[Unset, datetime.datetime] = UNSET
     connections: Union[Unset, int] = UNSET
     cores: Union[Unset, int] = UNSET
     cpu: Union[Unset, float] = UNSET
     gateway: Union[Unset, Gateway] = UNSET
@@ -63,43 +66,39 @@
     version: Union[Unset, str] = UNSET
     write_deadline: Union[Unset, int] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         auth_timeout = self.auth_timeout
-        cluster: Union[Unset, str] = UNSET
         if not isinstance(self.cluster, Unset):
-            cluster = self.cluster.value
+            cluster = self.cluster
         config_load_time: Union[Unset, str] = UNSET
         if not isinstance(self.config_load_time, Unset):
             config_load_time = self.config_load_time.isoformat()
         connections = self.connections
         cores = self.cores
         cpu = self.cpu
-        gateway: Union[Unset, str] = UNSET
         if not isinstance(self.gateway, Unset):
-            gateway = self.gateway.value
+            gateway = self.gateway
         git_commit = self.git_commit
         go = self.go
         gomaxprocs = self.gomaxprocs
         host = self.host
         http_base_path = self.http_base_path
         http_host = self.http_host
         http_port = self.http_port
         http_req_stats = self.http_req_stats
         https_port = self.https_port
         in_bytes = self.in_bytes
         in_msgs = self.in_msgs
-        jetstream: Union[Unset, str] = UNSET
         if not isinstance(self.jetstream, Unset):
-            jetstream = self.jetstream.value
-        leaf: Union[Unset, str] = UNSET
+            jetstream = self.jetstream
         if not isinstance(self.leaf, Unset):
-            leaf = self.leaf.value
+            leaf = self.leaf
         leafnodes = self.leafnodes
         max_connections = self.max_connections
         max_control_line = self.max_control_line
         max_payload = self.max_payload
         max_pending = self.max_pending
         mem = self.mem
         now: Union[Unset, str] = UNSET
@@ -127,110 +126,110 @@
         version = self.version
         write_deadline = self.write_deadline
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if auth_timeout is not UNSET:
-            field_dict['auth_timeout'] = auth_timeout
+            field_dict["auth_timeout"] = auth_timeout
         if cluster is not UNSET:
-            field_dict['cluster'] = cluster
+            field_dict["cluster"] = cluster
         if config_load_time is not UNSET:
-            field_dict['config_load_time'] = config_load_time
+            field_dict["config_load_time"] = config_load_time
         if connections is not UNSET:
-            field_dict['connections'] = connections
+            field_dict["connections"] = connections
         if cores is not UNSET:
-            field_dict['cores'] = cores
+            field_dict["cores"] = cores
         if cpu is not UNSET:
-            field_dict['cpu'] = cpu
+            field_dict["cpu"] = cpu
         if gateway is not UNSET:
-            field_dict['gateway'] = gateway
+            field_dict["gateway"] = gateway
         if git_commit is not UNSET:
-            field_dict['git_commit'] = git_commit
+            field_dict["git_commit"] = git_commit
         if go is not UNSET:
-            field_dict['go'] = go
+            field_dict["go"] = go
         if gomaxprocs is not UNSET:
-            field_dict['gomaxprocs'] = gomaxprocs
+            field_dict["gomaxprocs"] = gomaxprocs
         if host is not UNSET:
-            field_dict['host'] = host
+            field_dict["host"] = host
         if http_base_path is not UNSET:
-            field_dict['http_base_path'] = http_base_path
+            field_dict["http_base_path"] = http_base_path
         if http_host is not UNSET:
-            field_dict['http_host'] = http_host
+            field_dict["http_host"] = http_host
         if http_port is not UNSET:
-            field_dict['http_port'] = http_port
+            field_dict["http_port"] = http_port
         if http_req_stats is not UNSET:
-            field_dict['http_req_stats'] = http_req_stats
+            field_dict["http_req_stats"] = http_req_stats
         if https_port is not UNSET:
-            field_dict['https_port'] = https_port
+            field_dict["https_port"] = https_port
         if in_bytes is not UNSET:
-            field_dict['in_bytes'] = in_bytes
+            field_dict["in_bytes"] = in_bytes
         if in_msgs is not UNSET:
-            field_dict['in_msgs'] = in_msgs
+            field_dict["in_msgs"] = in_msgs
         if jetstream is not UNSET:
-            field_dict['jetstream'] = jetstream
+            field_dict["jetstream"] = jetstream
         if leaf is not UNSET:
-            field_dict['leaf'] = leaf
+            field_dict["leaf"] = leaf
         if leafnodes is not UNSET:
-            field_dict['leafnodes'] = leafnodes
+            field_dict["leafnodes"] = leafnodes
         if max_connections is not UNSET:
-            field_dict['max_connections'] = max_connections
+            field_dict["max_connections"] = max_connections
         if max_control_line is not UNSET:
-            field_dict['max_control_line'] = max_control_line
+            field_dict["max_control_line"] = max_control_line
         if max_payload is not UNSET:
-            field_dict['max_payload'] = max_payload
+            field_dict["max_payload"] = max_payload
         if max_pending is not UNSET:
-            field_dict['max_pending'] = max_pending
+            field_dict["max_pending"] = max_pending
         if mem is not UNSET:
-            field_dict['mem'] = mem
+            field_dict["mem"] = mem
         if now is not UNSET:
-            field_dict['now'] = now
+            field_dict["now"] = now
         if out_bytes is not UNSET:
-            field_dict['out_bytes'] = out_bytes
+            field_dict["out_bytes"] = out_bytes
         if out_msgs is not UNSET:
-            field_dict['out_msgs'] = out_msgs
+            field_dict["out_msgs"] = out_msgs
         if ping_interval is not UNSET:
-            field_dict['ping_interval'] = ping_interval
+            field_dict["ping_interval"] = ping_interval
         if ping_max is not UNSET:
-            field_dict['ping_max'] = ping_max
+            field_dict["ping_max"] = ping_max
         if port is not UNSET:
-            field_dict['port'] = port
+            field_dict["port"] = port
         if proto is not UNSET:
-            field_dict['proto'] = proto
+            field_dict["proto"] = proto
         if remotes is not UNSET:
-            field_dict['remotes'] = remotes
+            field_dict["remotes"] = remotes
         if routes is not UNSET:
-            field_dict['routes'] = routes
+            field_dict["routes"] = routes
         if server_id is not UNSET:
-            field_dict['server_id'] = server_id
+            field_dict["server_id"] = server_id
         if server_name is not UNSET:
-            field_dict['server_name'] = server_name
+            field_dict["server_name"] = server_name
         if slow_consumers is not UNSET:
-            field_dict['slow_consumers'] = slow_consumers
+            field_dict["slow_consumers"] = slow_consumers
         if start is not UNSET:
-            field_dict['start'] = start
+            field_dict["start"] = start
         if subscriptions is not UNSET:
-            field_dict['subscriptions'] = subscriptions
+            field_dict["subscriptions"] = subscriptions
         if system_account is not UNSET:
-            field_dict['system_account'] = system_account
+            field_dict["system_account"] = system_account
         if tls_timeout is not UNSET:
-            field_dict['tls_timeout'] = tls_timeout
+            field_dict["tls_timeout"] = tls_timeout
         if total_connections is not UNSET:
-            field_dict['total_connections'] = total_connections
+            field_dict["total_connections"] = total_connections
         if uptime is not UNSET:
-            field_dict['uptime'] = uptime
+            field_dict["uptime"] = uptime
         if version is not UNSET:
-            field_dict['version'] = version
+            field_dict["version"] = version
         if write_deadline is not UNSET:
-            field_dict['write_deadline'] = write_deadline
+            field_dict["write_deadline"] = write_deadline
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         auth_timeout = d.pop("auth_timeout", UNSET)
 
         _cluster = d.pop("cluster", UNSET)
         cluster: Union[Unset, Cluster]
         if isinstance(_cluster, Unset):
             cluster = UNSET
```

### Comparing `kittycad-0.3.7/kittycad/models/customer.py` & `kittycad-0.3.8/kittycad/models/customer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,81 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.new_address import NewAddress
 from ..models.currency import Currency
+from ..models.new_address import NewAddress
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Customer")
+M = TypeVar("M", bound="Customer")
 
 
 @attr.s(auto_attribs=True)
 class Customer:
-    """ """
+    """The resource representing a payment "Customer"."""  # noqa: E501
+
     address: Union[Unset, NewAddress] = UNSET
     balance: Union[Unset, float] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     currency: Union[Unset, Currency] = UNSET
     delinquent: Union[Unset, bool] = False
     email: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     metadata: Union[Unset, Any] = UNSET
     name: Union[Unset, str] = UNSET
     phone: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        address: Union[Unset, str] = UNSET
         if not isinstance(self.address, Unset):
-            address = self.address.value
+            address = self.address
         balance = self.balance
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
-        currency: Union[Unset, str] = UNSET
         if not isinstance(self.currency, Unset):
-            currency = self.currency.value
+            currency = self.currency
         delinquent = self.delinquent
         email = self.email
         id = self.id
         metadata = self.metadata
         name = self.name
         phone = self.phone
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if address is not UNSET:
-            field_dict['address'] = address
+            field_dict["address"] = address
         if balance is not UNSET:
-            field_dict['balance'] = balance
+            field_dict["balance"] = balance
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if currency is not UNSET:
-            field_dict['currency'] = currency
+            field_dict["currency"] = currency
         if delinquent is not UNSET:
-            field_dict['delinquent'] = delinquent
+            field_dict["delinquent"] = delinquent
         if email is not UNSET:
-            field_dict['email'] = email
+            field_dict["email"] = email
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if metadata is not UNSET:
-            field_dict['metadata'] = metadata
+            field_dict["metadata"] = metadata
         if name is not UNSET:
-            field_dict['name'] = name
+            field_dict["name"] = name
         if phone is not UNSET:
-            field_dict['phone'] = phone
+            field_dict["phone"] = phone
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[M], src_dict: Dict[str, Any]) -> M:
         d = src_dict.copy()
         _address = d.pop("address", UNSET)
         address: Union[Unset, NewAddress]
         if isinstance(_address, Unset):
             address = UNSET
         else:
             address = NewAddress(_address)
```

### Comparing `kittycad-0.3.7/kittycad/models/customer_balance.py` & `kittycad-0.3.8/kittycad/models/customer_balance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CustomerBalance")
+N = TypeVar("N", bound="CustomerBalance")
 
 
 @attr.s(auto_attribs=True)
 class CustomerBalance:
-    """ """
+    """A balance for a user.
+
+    This holds information about the financial balance for the user."""  # noqa: E501
+
     created_at: Union[Unset, datetime.datetime] = UNSET
     id: Union[Unset, str] = UNSET
     monthly_credits_remaining: Union[Unset, float] = UNSET
     pre_pay_cash_remaining: Union[Unset, float] = UNSET
     pre_pay_credits_remaining: Union[Unset, float] = UNSET
     total_due: Union[Unset, float] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
@@ -38,34 +40,34 @@
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if monthly_credits_remaining is not UNSET:
-            field_dict['monthly_credits_remaining'] = monthly_credits_remaining
+            field_dict["monthly_credits_remaining"] = monthly_credits_remaining
         if pre_pay_cash_remaining is not UNSET:
-            field_dict['pre_pay_cash_remaining'] = pre_pay_cash_remaining
+            field_dict["pre_pay_cash_remaining"] = pre_pay_cash_remaining
         if pre_pay_credits_remaining is not UNSET:
-            field_dict['pre_pay_credits_remaining'] = pre_pay_credits_remaining
+            field_dict["pre_pay_credits_remaining"] = pre_pay_credits_remaining
         if total_due is not UNSET:
-            field_dict['total_due'] = total_due
+            field_dict["total_due"] = total_due
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/device_access_token_request_form.py` & `kittycad-0.3.8/kittycad/models/device_access_token_request_form.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.o_auth2_grant_type import OAuth2GrantType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="DeviceAccessTokenRequestForm")
+J = TypeVar("J", bound="DeviceAccessTokenRequestForm")
 
 
 @attr.s(auto_attribs=True)
 class DeviceAccessTokenRequestForm:
-    """ """
+    """The form for a device access token request."""  # noqa: E501
+
     client_id: Union[Unset, str] = UNSET
     device_code: Union[Unset, str] = UNSET
     grant_type: Union[Unset, OAuth2GrantType] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         client_id = self.client_id
         device_code = self.device_code
-        grant_type: Union[Unset, str] = UNSET
         if not isinstance(self.grant_type, Unset):
-            grant_type = self.grant_type.value
+            grant_type = self.grant_type
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if client_id is not UNSET:
-            field_dict['client_id'] = client_id
+            field_dict["client_id"] = client_id
         if device_code is not UNSET:
-            field_dict['device_code'] = device_code
+            field_dict["device_code"] = device_code
         if grant_type is not UNSET:
-            field_dict['grant_type'] = grant_type
+            field_dict["grant_type"] = grant_type
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
         d = src_dict.copy()
         client_id = d.pop("client_id", UNSET)
 
         device_code = d.pop("device_code", UNSET)
 
         _grant_type = d.pop("grant_type", UNSET)
         grant_type: Union[Unset, OAuth2GrantType]
```

### Comparing `kittycad-0.3.7/kittycad/models/device_auth_request_form.py` & `kittycad-0.3.8/kittycad/models/payment_intent.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="DeviceAuthRequestForm")
+J = TypeVar("J", bound="PaymentIntent")
 
 
 @attr.s(auto_attribs=True)
-class DeviceAuthRequestForm:
-    """ """
-    client_id: Union[Unset, str] = UNSET
+class PaymentIntent:
+    """A payment intent response."""  # noqa: E501
+
+    client_secret: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        client_id = self.client_id
+        client_secret = self.client_secret
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if client_id is not UNSET:
-            field_dict['client_id'] = client_id
+        if client_secret is not UNSET:
+            field_dict["client_secret"] = client_secret
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
         d = src_dict.copy()
-        client_id = d.pop("client_id", UNSET)
+        client_secret = d.pop("client_secret", UNSET)
 
-        device_auth_request_form = cls(
-            client_id=client_id,
+        payment_intent = cls(
+            client_secret=client_secret,
         )
 
-        device_auth_request_form.additional_properties = d
-        return device_auth_request_form
+        payment_intent.additional_properties = d
+        return payment_intent
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/device_auth_verify_params.py` & `kittycad-0.3.8/kittycad/models/device_auth_verify_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="DeviceAuthVerifyParams")
+F = TypeVar("F", bound="DeviceAuthVerifyParams")
 
 
 @attr.s(auto_attribs=True)
 class DeviceAuthVerifyParams:
-    """ """
+    """The request parameters to verify the `user_code` for the OAuth 2.0 Device Authorization Grant."""  # noqa: E501
+
     user_code: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         user_code = self.user_code
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if user_code is not UNSET:
-            field_dict['user_code'] = user_code
+            field_dict["user_code"] = user_code
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         user_code = d.pop("user_code", UNSET)
 
         device_auth_verify_params = cls(
             user_code=user_code,
         )
```

### Comparing `kittycad-0.3.7/kittycad/models/docker_system_info.py` & `kittycad-0.3.8/kittycad/models/docker_system_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
-from ..models.system_info_cgroup_driver_enum import SystemInfoCgroupDriverEnum
-from ..models.system_info_cgroup_version_enum import SystemInfoCgroupVersionEnum
 from ..models.commit import Commit
-from ..models.system_info_isolation_enum import SystemInfoIsolationEnum
 from ..models.plugins_info import PluginsInfo
 from ..models.registry_service_config import RegistryServiceConfig
-from ..models.runtime import Runtime
+from ..models.system_info_cgroup_driver_enum import SystemInfoCgroupDriverEnum
+from ..models.system_info_cgroup_version_enum import SystemInfoCgroupVersionEnum
+from ..models.system_info_isolation_enum import SystemInfoIsolationEnum
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="DockerSystemInfo")
+V = TypeVar("V", bound="DockerSystemInfo")
 
 
 @attr.s(auto_attribs=True)
 class DockerSystemInfo:
-    """ """
+    """Docker system info."""  # noqa: E501
+
     architecture: Union[Unset, str] = UNSET
     bridge_nf_ip6tables: Union[Unset, bool] = False
     bridge_nf_iptables: Union[Unset, bool] = False
     cgroup_driver: Union[Unset, SystemInfoCgroupDriverEnum] = UNSET
     cgroup_version: Union[Unset, SystemInfoCgroupVersionEnum] = UNSET
     cluster_advertise: Union[Unset, str] = UNSET
     cluster_store: Union[Unset, str] = UNSET
@@ -31,16 +31,16 @@
     containers_stopped: Union[Unset, int] = UNSET
     cpu_cfs_period: Union[Unset, bool] = False
     cpu_cfs_quota: Union[Unset, bool] = False
     cpu_set: Union[Unset, bool] = False
     cpu_shares: Union[Unset, bool] = False
     debug: Union[Unset, bool] = False
     from ..models.system_info_default_address_pools import SystemInfoDefaultAddressPools
-    default_address_pools: Union[Unset,
-                                 List[SystemInfoDefaultAddressPools]] = UNSET
+
+    default_address_pools: Union[Unset, List[SystemInfoDefaultAddressPools]] = UNSET
     default_runtime: Union[Unset, str] = UNSET
     docker_root_dir: Union[Unset, str] = UNSET
     driver: Union[Unset, str] = UNSET
     driver_status: Union[Unset, List[List[str]]] = UNSET
     experimental_build: Union[Unset, bool] = False
     http_proxy: Union[Unset, str] = UNSET
     https_proxy: Union[Unset, str] = UNSET
@@ -82,37 +82,36 @@
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         architecture = self.architecture
         bridge_nf_ip6tables = self.bridge_nf_ip6tables
         bridge_nf_iptables = self.bridge_nf_iptables
-        cgroup_driver: Union[Unset, str] = UNSET
         if not isinstance(self.cgroup_driver, Unset):
-            cgroup_driver = self.cgroup_driver.value
-        cgroup_version: Union[Unset, str] = UNSET
+            cgroup_driver = self.cgroup_driver
         if not isinstance(self.cgroup_version, Unset):
-            cgroup_version = self.cgroup_version.value
+            cgroup_version = self.cgroup_version
         cluster_advertise = self.cluster_advertise
         cluster_store = self.cluster_store
-        containerd_commit: Union[Unset, str] = UNSET
         if not isinstance(self.containerd_commit, Unset):
-            containerd_commit = self.containerd_commit.value
+            containerd_commit = self.containerd_commit
         containers = self.containers
         containers_paused = self.containers_paused
         containers_running = self.containers_running
         containers_stopped = self.containers_stopped
         cpu_cfs_period = self.cpu_cfs_period
         cpu_cfs_quota = self.cpu_cfs_quota
         cpu_set = self.cpu_set
         cpu_shares = self.cpu_shares
         debug = self.debug
-        from ..models.system_info_default_address_pools import SystemInfoDefaultAddressPools
-        default_address_pools: Union[Unset,
-                                     List[SystemInfoDefaultAddressPools]] = UNSET
+        from ..models.system_info_default_address_pools import (
+            SystemInfoDefaultAddressPools,
+        )
+
+        default_address_pools: Union[Unset, List[SystemInfoDefaultAddressPools]] = UNSET
         if not isinstance(self.default_address_pools, Unset):
             default_address_pools = self.default_address_pools
         default_runtime = self.default_runtime
         docker_root_dir = self.docker_root_dir
         driver = self.driver
         driver_status: Union[Unset, List[List[str]]] = UNSET
         if not isinstance(self.driver_status, Unset):
@@ -120,21 +119,19 @@
         experimental_build = self.experimental_build
         http_proxy = self.http_proxy
         https_proxy = self.https_proxy
         id = self.id
         images = self.images
         index_server_address = self.index_server_address
         init_binary = self.init_binary
-        init_commit: Union[Unset, str] = UNSET
         if not isinstance(self.init_commit, Unset):
-            init_commit = self.init_commit.value
+            init_commit = self.init_commit
         ipv4_forwarding = self.ipv4_forwarding
-        isolation: Union[Unset, str] = UNSET
         if not isinstance(self.isolation, Unset):
-            isolation = self.isolation.value
+            isolation = self.isolation
         kernel_memory = self.kernel_memory
         kernel_memory_tcp = self.kernel_memory_tcp
         kernel_version = self.kernel_version
         labels: Union[Unset, List[str]] = UNSET
         if not isinstance(self.labels, Unset):
             labels = self.labels
         live_restore_enabled = self.live_restore_enabled
@@ -147,24 +144,21 @@
         ncpu = self.ncpu
         no_proxy = self.no_proxy
         oom_kill_disable = self.oom_kill_disable
         operating_system = self.operating_system
         os_type = self.os_type
         os_version = self.os_version
         pids_limit = self.pids_limit
-        plugins: Union[Unset, str] = UNSET
         if not isinstance(self.plugins, Unset):
-            plugins = self.plugins.value
+            plugins = self.plugins
         product_license = self.product_license
-        registry_config: Union[Unset, str] = UNSET
         if not isinstance(self.registry_config, Unset):
-            registry_config = self.registry_config.value
-        runc_commit: Union[Unset, str] = UNSET
+            registry_config = self.registry_config
         if not isinstance(self.runc_commit, Unset):
-            runc_commit = self.runc_commit.value
+            runc_commit = self.runc_commit
         runtimes = self.runtimes
         security_options: Union[Unset, List[str]] = UNSET
         if not isinstance(self.security_options, Unset):
             security_options = self.security_options
         server_version = self.server_version
         swap_limit = self.swap_limit
         system_time = self.system_time
@@ -172,138 +166,138 @@
         if not isinstance(self.warnings, Unset):
             warnings = self.warnings
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if architecture is not UNSET:
-            field_dict['architecture'] = architecture
+            field_dict["architecture"] = architecture
         if bridge_nf_ip6tables is not UNSET:
-            field_dict['bridge_nf_ip6tables'] = bridge_nf_ip6tables
+            field_dict["bridge_nf_ip6tables"] = bridge_nf_ip6tables
         if bridge_nf_iptables is not UNSET:
-            field_dict['bridge_nf_iptables'] = bridge_nf_iptables
+            field_dict["bridge_nf_iptables"] = bridge_nf_iptables
         if cgroup_driver is not UNSET:
-            field_dict['cgroup_driver'] = cgroup_driver
+            field_dict["cgroup_driver"] = cgroup_driver
         if cgroup_version is not UNSET:
-            field_dict['cgroup_version'] = cgroup_version
+            field_dict["cgroup_version"] = cgroup_version
         if cluster_advertise is not UNSET:
-            field_dict['cluster_advertise'] = cluster_advertise
+            field_dict["cluster_advertise"] = cluster_advertise
         if cluster_store is not UNSET:
-            field_dict['cluster_store'] = cluster_store
+            field_dict["cluster_store"] = cluster_store
         if containerd_commit is not UNSET:
-            field_dict['containerd_commit'] = containerd_commit
+            field_dict["containerd_commit"] = containerd_commit
         if containers is not UNSET:
-            field_dict['containers'] = containers
+            field_dict["containers"] = containers
         if containers_paused is not UNSET:
-            field_dict['containers_paused'] = containers_paused
+            field_dict["containers_paused"] = containers_paused
         if containers_running is not UNSET:
-            field_dict['containers_running'] = containers_running
+            field_dict["containers_running"] = containers_running
         if containers_stopped is not UNSET:
-            field_dict['containers_stopped'] = containers_stopped
+            field_dict["containers_stopped"] = containers_stopped
         if cpu_cfs_period is not UNSET:
-            field_dict['cpu_cfs_period'] = cpu_cfs_period
+            field_dict["cpu_cfs_period"] = cpu_cfs_period
         if cpu_cfs_quota is not UNSET:
-            field_dict['cpu_cfs_quota'] = cpu_cfs_quota
+            field_dict["cpu_cfs_quota"] = cpu_cfs_quota
         if cpu_set is not UNSET:
-            field_dict['cpu_set'] = cpu_set
+            field_dict["cpu_set"] = cpu_set
         if cpu_shares is not UNSET:
-            field_dict['cpu_shares'] = cpu_shares
+            field_dict["cpu_shares"] = cpu_shares
         if debug is not UNSET:
-            field_dict['debug'] = debug
+            field_dict["debug"] = debug
         if default_address_pools is not UNSET:
-            field_dict['default_address_pools'] = default_address_pools
+            field_dict["default_address_pools"] = default_address_pools
         if default_runtime is not UNSET:
-            field_dict['default_runtime'] = default_runtime
+            field_dict["default_runtime"] = default_runtime
         if docker_root_dir is not UNSET:
-            field_dict['docker_root_dir'] = docker_root_dir
+            field_dict["docker_root_dir"] = docker_root_dir
         if driver is not UNSET:
-            field_dict['driver'] = driver
+            field_dict["driver"] = driver
         if driver_status is not UNSET:
-            field_dict['driver_status'] = driver_status
+            field_dict["driver_status"] = driver_status
         if experimental_build is not UNSET:
-            field_dict['experimental_build'] = experimental_build
+            field_dict["experimental_build"] = experimental_build
         if http_proxy is not UNSET:
-            field_dict['http_proxy'] = http_proxy
+            field_dict["http_proxy"] = http_proxy
         if https_proxy is not UNSET:
-            field_dict['https_proxy'] = https_proxy
+            field_dict["https_proxy"] = https_proxy
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if images is not UNSET:
-            field_dict['images'] = images
+            field_dict["images"] = images
         if index_server_address is not UNSET:
-            field_dict['index_server_address'] = index_server_address
+            field_dict["index_server_address"] = index_server_address
         if init_binary is not UNSET:
-            field_dict['init_binary'] = init_binary
+            field_dict["init_binary"] = init_binary
         if init_commit is not UNSET:
-            field_dict['init_commit'] = init_commit
+            field_dict["init_commit"] = init_commit
         if ipv4_forwarding is not UNSET:
-            field_dict['ipv4_forwarding'] = ipv4_forwarding
+            field_dict["ipv4_forwarding"] = ipv4_forwarding
         if isolation is not UNSET:
-            field_dict['isolation'] = isolation
+            field_dict["isolation"] = isolation
         if kernel_memory is not UNSET:
-            field_dict['kernel_memory'] = kernel_memory
+            field_dict["kernel_memory"] = kernel_memory
         if kernel_memory_tcp is not UNSET:
-            field_dict['kernel_memory_tcp'] = kernel_memory_tcp
+            field_dict["kernel_memory_tcp"] = kernel_memory_tcp
         if kernel_version is not UNSET:
-            field_dict['kernel_version'] = kernel_version
+            field_dict["kernel_version"] = kernel_version
         if labels is not UNSET:
-            field_dict['labels'] = labels
+            field_dict["labels"] = labels
         if live_restore_enabled is not UNSET:
-            field_dict['live_restore_enabled'] = live_restore_enabled
+            field_dict["live_restore_enabled"] = live_restore_enabled
         if logging_driver is not UNSET:
-            field_dict['logging_driver'] = logging_driver
+            field_dict["logging_driver"] = logging_driver
         if mem_total is not UNSET:
-            field_dict['mem_total'] = mem_total
+            field_dict["mem_total"] = mem_total
         if memory_limit is not UNSET:
-            field_dict['memory_limit'] = memory_limit
+            field_dict["memory_limit"] = memory_limit
         if n_events_listener is not UNSET:
-            field_dict['n_events_listener'] = n_events_listener
+            field_dict["n_events_listener"] = n_events_listener
         if n_fd is not UNSET:
-            field_dict['n_fd'] = n_fd
+            field_dict["n_fd"] = n_fd
         if name is not UNSET:
-            field_dict['name'] = name
+            field_dict["name"] = name
         if ncpu is not UNSET:
-            field_dict['ncpu'] = ncpu
+            field_dict["ncpu"] = ncpu
         if no_proxy is not UNSET:
-            field_dict['no_proxy'] = no_proxy
+            field_dict["no_proxy"] = no_proxy
         if oom_kill_disable is not UNSET:
-            field_dict['oom_kill_disable'] = oom_kill_disable
+            field_dict["oom_kill_disable"] = oom_kill_disable
         if operating_system is not UNSET:
-            field_dict['operating_system'] = operating_system
+            field_dict["operating_system"] = operating_system
         if os_type is not UNSET:
-            field_dict['os_type'] = os_type
+            field_dict["os_type"] = os_type
         if os_version is not UNSET:
-            field_dict['os_version'] = os_version
+            field_dict["os_version"] = os_version
         if pids_limit is not UNSET:
-            field_dict['pids_limit'] = pids_limit
+            field_dict["pids_limit"] = pids_limit
         if plugins is not UNSET:
-            field_dict['plugins'] = plugins
+            field_dict["plugins"] = plugins
         if product_license is not UNSET:
-            field_dict['product_license'] = product_license
+            field_dict["product_license"] = product_license
         if registry_config is not UNSET:
-            field_dict['registry_config'] = registry_config
+            field_dict["registry_config"] = registry_config
         if runc_commit is not UNSET:
-            field_dict['runc_commit'] = runc_commit
+            field_dict["runc_commit"] = runc_commit
         if runtimes is not UNSET:
-            field_dict['runtimes'] = runtimes
+            field_dict["runtimes"] = runtimes
         if security_options is not UNSET:
-            field_dict['security_options'] = security_options
+            field_dict["security_options"] = security_options
         if server_version is not UNSET:
-            field_dict['server_version'] = server_version
+            field_dict["server_version"] = server_version
         if swap_limit is not UNSET:
-            field_dict['swap_limit'] = swap_limit
+            field_dict["swap_limit"] = swap_limit
         if system_time is not UNSET:
-            field_dict['system_time'] = system_time
+            field_dict["system_time"] = system_time
         if warnings is not UNSET:
-            field_dict['warnings'] = warnings
+            field_dict["warnings"] = warnings
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
         architecture = d.pop("architecture", UNSET)
 
         bridge_nf_ip6tables = d.pop("bridge_nf_ip6tables", UNSET)
 
         bridge_nf_iptables = d.pop("bridge_nf_iptables", UNSET)
 
@@ -346,18 +340,21 @@
 
         cpu_set = d.pop("cpu_set", UNSET)
 
         cpu_shares = d.pop("cpu_shares", UNSET)
 
         debug = d.pop("debug", UNSET)
 
-        from ..models.system_info_default_address_pools import SystemInfoDefaultAddressPools
+        from ..models.system_info_default_address_pools import (
+            SystemInfoDefaultAddressPools,
+        )
+
         default_address_pools = cast(
-            List[SystemInfoDefaultAddressPools], d.pop(
-                "default_address_pools", UNSET))
+            List[SystemInfoDefaultAddressPools], d.pop("default_address_pools", UNSET)
+        )
 
         default_runtime = d.pop("default_runtime", UNSET)
 
         docker_root_dir = d.pop("docker_root_dir", UNSET)
 
         driver = d.pop("driver", UNSET)
```

### Comparing `kittycad-0.3.7/kittycad/models/email_authentication_form.py` & `kittycad-0.3.8/kittycad/models/email_authentication_form.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="EmailAuthenticationForm")
+M = TypeVar("M", bound="EmailAuthenticationForm")
 
 
 @attr.s(auto_attribs=True)
 class EmailAuthenticationForm:
-    """ """
+    """The body of the form for email authentication."""  # noqa: E501
+
     callback_url: Union[Unset, str] = UNSET
     email: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         callback_url = self.callback_url
         email = self.email
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if callback_url is not UNSET:
-            field_dict['callback_url'] = callback_url
+            field_dict["callback_url"] = callback_url
         if email is not UNSET:
-            field_dict['email'] = email
+            field_dict["email"] = email
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[M], src_dict: Dict[str, Any]) -> M:
         d = src_dict.copy()
         callback_url = d.pop("callback_url", UNSET)
 
         email = d.pop("email", UNSET)
 
         email_authentication_form = cls(
             callback_url=callback_url,
```

### Comparing `kittycad-0.3.7/kittycad/models/engine_metadata.py` & `kittycad-0.3.8/kittycad/models/engine_metadata.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,67 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.cache_metadata import CacheMetadata
+from ..models.connection import Connection
 from ..models.environment import Environment
 from ..models.file_system_metadata import FileSystemMetadata
-from ..models.connection import Connection
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="EngineMetadata")
+B = TypeVar("B", bound="EngineMetadata")
 
 
 @attr.s(auto_attribs=True)
 class EngineMetadata:
-    """ """
+    """Metadata about our currently running server.
+
+    This is mostly used for internal purposes and debugging."""  # noqa: E501
+
     async_jobs_running: Union[Unset, bool] = False
     cache: Union[Unset, CacheMetadata] = UNSET
     environment: Union[Unset, Environment] = UNSET
     fs: Union[Unset, FileSystemMetadata] = UNSET
     git_hash: Union[Unset, str] = UNSET
     pubsub: Union[Unset, Connection] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         async_jobs_running = self.async_jobs_running
-        cache: Union[Unset, str] = UNSET
         if not isinstance(self.cache, Unset):
-            cache = self.cache.value
-        environment: Union[Unset, str] = UNSET
+            cache = self.cache
         if not isinstance(self.environment, Unset):
-            environment = self.environment.value
-        fs: Union[Unset, str] = UNSET
+            environment = self.environment
         if not isinstance(self.fs, Unset):
-            fs = self.fs.value
+            fs = self.fs
         git_hash = self.git_hash
-        pubsub: Union[Unset, str] = UNSET
         if not isinstance(self.pubsub, Unset):
-            pubsub = self.pubsub.value
+            pubsub = self.pubsub
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if async_jobs_running is not UNSET:
-            field_dict['async_jobs_running'] = async_jobs_running
+            field_dict["async_jobs_running"] = async_jobs_running
         if cache is not UNSET:
-            field_dict['cache'] = cache
+            field_dict["cache"] = cache
         if environment is not UNSET:
-            field_dict['environment'] = environment
+            field_dict["environment"] = environment
         if fs is not UNSET:
-            field_dict['fs'] = fs
+            field_dict["fs"] = fs
         if git_hash is not UNSET:
-            field_dict['git_hash'] = git_hash
+            field_dict["git_hash"] = git_hash
         if pubsub is not UNSET:
-            field_dict['pubsub'] = pubsub
+            field_dict["pubsub"] = pubsub
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
         d = src_dict.copy()
         async_jobs_running = d.pop("async_jobs_running", UNSET)
 
         _cache = d.pop("cache", UNSET)
         cache: Union[Unset, CacheMetadata]
         if isinstance(_cache, Unset):
             cache = UNSET
```

### Comparing `kittycad-0.3.7/kittycad/models/error.py` & `kittycad-0.3.8/kittycad/models/error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Error")
+S = TypeVar("S", bound="Error")
 
 
 @attr.s(auto_attribs=True)
 class Error:
-    """ """
+    """Error information from a response."""  # noqa: E501
+
     error_code: Union[Unset, str] = UNSET
     message: Union[Unset, str] = UNSET
     request_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
@@ -21,24 +22,24 @@
         message = self.message
         request_id = self.request_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if error_code is not UNSET:
-            field_dict['error_code'] = error_code
+            field_dict["error_code"] = error_code
         if message is not UNSET:
-            field_dict['message'] = message
+            field_dict["message"] = message
         if request_id is not UNSET:
-            field_dict['request_id'] = request_id
+            field_dict["request_id"] = request_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
         d = src_dict.copy()
         error_code = d.pop("error_code", UNSET)
 
         message = d.pop("message", UNSET)
 
         request_id = d.pop("request_id", UNSET)
```

### Comparing `kittycad-0.3.7/kittycad/models/executor_metadata.py` & `kittycad-0.3.8/kittycad/models/executor_metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.docker_system_info import DockerSystemInfo
 from ..models.environment import Environment
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ExecutorMetadata")
+A = TypeVar("A", bound="ExecutorMetadata")
 
 
 @attr.s(auto_attribs=True)
 class ExecutorMetadata:
-    """ """
+    """Metadata about our currently running server.
+
+    This is mostly used for internal purposes and debugging."""  # noqa: E501
+
     docker_info: Union[Unset, DockerSystemInfo] = UNSET
     environment: Union[Unset, Environment] = UNSET
     git_hash: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        docker_info: Union[Unset, str] = UNSET
         if not isinstance(self.docker_info, Unset):
-            docker_info = self.docker_info.value
-        environment: Union[Unset, str] = UNSET
+            docker_info = self.docker_info
         if not isinstance(self.environment, Unset):
-            environment = self.environment.value
+            environment = self.environment
         git_hash = self.git_hash
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if docker_info is not UNSET:
-            field_dict['docker_info'] = docker_info
+            field_dict["docker_info"] = docker_info
         if environment is not UNSET:
-            field_dict['environment'] = environment
+            field_dict["environment"] = environment
         if git_hash is not UNSET:
-            field_dict['git_hash'] = git_hash
+            field_dict["git_hash"] = git_hash
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[A], src_dict: Dict[str, Any]) -> A:
         d = src_dict.copy()
         _docker_info = d.pop("docker_info", UNSET)
         docker_info: Union[Unset, DockerSystemInfo]
         if isinstance(_docker_info, Unset):
             docker_info = UNSET
         else:
             docker_info = DockerSystemInfo(_docker_info)
```

### Comparing `kittycad-0.3.7/kittycad/models/extended_user.py` & `kittycad-0.3.8/kittycad/models/extended_user.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ExtendedUser")
+H = TypeVar("H", bound="ExtendedUser")
 
 
 @attr.s(auto_attribs=True)
 class ExtendedUser:
-    """ """
+    """Extended user information.
+
+    This is mostly used for internal purposes. It returns a mapping of the user's information, including that of our third party services we use for users: MailChimp, Stripe, and Front"""  # noqa: E501
+
     company: Union[Unset, str] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     discord: Union[Unset, str] = UNSET
     email: Union[Unset, str] = UNSET
     email_verified: Union[Unset, datetime.datetime] = UNSET
     first_name: Union[Unset, str] = UNSET
     front_id: Union[Unset, str] = UNSET
@@ -55,50 +58,50 @@
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if company is not UNSET:
-            field_dict['company'] = company
+            field_dict["company"] = company
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if discord is not UNSET:
-            field_dict['discord'] = discord
+            field_dict["discord"] = discord
         if email is not UNSET:
-            field_dict['email'] = email
+            field_dict["email"] = email
         if email_verified is not UNSET:
-            field_dict['email_verified'] = email_verified
+            field_dict["email_verified"] = email_verified
         if first_name is not UNSET:
-            field_dict['first_name'] = first_name
+            field_dict["first_name"] = first_name
         if front_id is not UNSET:
-            field_dict['front_id'] = front_id
+            field_dict["front_id"] = front_id
         if github is not UNSET:
-            field_dict['github'] = github
+            field_dict["github"] = github
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if image is not UNSET:
-            field_dict['image'] = image
+            field_dict["image"] = image
         if last_name is not UNSET:
-            field_dict['last_name'] = last_name
+            field_dict["last_name"] = last_name
         if mailchimp_id is not UNSET:
-            field_dict['mailchimp_id'] = mailchimp_id
+            field_dict["mailchimp_id"] = mailchimp_id
         if name is not UNSET:
-            field_dict['name'] = name
+            field_dict["name"] = name
         if phone is not UNSET:
-            field_dict['phone'] = phone
+            field_dict["phone"] = phone
         if stripe_id is not UNSET:
-            field_dict['stripe_id'] = stripe_id
+            field_dict["stripe_id"] = stripe_id
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         company = d.pop("company", UNSET)
 
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
```

### Comparing `kittycad-0.3.7/kittycad/models/extended_user_results_page.py` & `kittycad-0.3.8/kittycad/models/user_results_page.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ExtendedUserResultsPage")
+A = TypeVar("A", bound="UserResultsPage")
 
 
 @attr.s(auto_attribs=True)
-class ExtendedUserResultsPage:
-    """ """
-    from ..models.extended_user import ExtendedUser
-    items: Union[Unset, List[ExtendedUser]] = UNSET
+class UserResultsPage:
+    """A single page of results"""  # noqa: E501
+
+    from ..models.user import User
+
+    items: Union[Unset, List[User]] = UNSET
     next_page: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        from ..models.extended_user import ExtendedUser
-        items: Union[Unset, List[ExtendedUser]] = UNSET
+        from ..models.user import User
+
+        items: Union[Unset, List[User]] = UNSET
         if not isinstance(self.items, Unset):
             items = self.items
         next_page = self.next_page
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if items is not UNSET:
-            field_dict['items'] = items
+            field_dict["items"] = items
         if next_page is not UNSET:
-            field_dict['next_page'] = next_page
+            field_dict["next_page"] = next_page
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[A], src_dict: Dict[str, Any]) -> A:
         d = src_dict.copy()
-        from ..models.extended_user import ExtendedUser
-        items = cast(List[ExtendedUser], d.pop("items", UNSET))
+        from ..models.user import User
+
+        items = cast(List[User], d.pop("items", UNSET))
 
         next_page = d.pop("next_page", UNSET)
 
-        extended_user_results_page = cls(
+        user_results_page = cls(
             items=items,
             next_page=next_page,
         )
 
-        extended_user_results_page.additional_properties = d
-        return extended_user_results_page
+        user_results_page.additional_properties = d
+        return user_results_page
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/file2_d_vector_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_concentration_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.file2_d_vector_export_format import File2DVectorExportFormat
-from ..models.file2_d_vector_import_format import File2DVectorImportFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_concentration_format import UnitConcentrationFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="File2DVectorConversion")
+F = TypeVar("F", bound="UnitConcentrationConversion")
 
 
 @attr.s(auto_attribs=True)
-class File2DVectorConversion:
-    """ """
+class UnitConcentrationConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    output: Union[Unset, str] = UNSET
-    output_format: Union[Unset, File2DVectorExportFormat] = UNSET
-    src_format: Union[Unset, File2DVectorImportFormat] = UNSET
+    input: Union[Unset, float] = UNSET
+    output: Union[Unset, float] = UNSET
+    output_format: Union[Unset, UnitConcentrationFormat] = UNSET
+    src_format: Union[Unset, UnitConcentrationFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -35,62 +35,62 @@
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
+        input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
+        if input is not UNSET:
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -102,29 +102,31 @@
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
         id = d.pop("id", UNSET)
 
+        input = d.pop("input", UNSET)
+
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, File2DVectorExportFormat]
+        output_format: Union[Unset, UnitConcentrationFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = File2DVectorExportFormat(_output_format)
+            output_format = UnitConcentrationFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, File2DVectorImportFormat]
+        src_format: Union[Unset, UnitConcentrationFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = File2DVectorImportFormat(_src_format)
+            src_format = UnitConcentrationFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -141,30 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        file2_d_vector_conversion = cls(
+        unit_concentration_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
+            input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        file2_d_vector_conversion.additional_properties = d
-        return file2_d_vector_conversion
+        unit_concentration_conversion.additional_properties = d
+        return unit_concentration_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/file_center_of_mass.py` & `kittycad-0.3.8/kittycad/models/file_center_of_mass.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.file3_d_import_format import File3DImportFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.file_import_format import FileImportFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FileCenterOfMass")
+G = TypeVar("G", bound="FileCenterOfMass")
 
 
 @attr.s(auto_attribs=True)
 class FileCenterOfMass:
-    """ """
+    """A file center of mass result."""  # noqa: E501
+
     center_of_mass: Union[Unset, List[float]] = UNSET
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    src_format: Union[Unset, File3DImportFormat] = UNSET
+    src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -36,56 +36,54 @@
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
-        src_format: Union[Unset, str] = UNSET
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if center_of_mass is not UNSET:
-            field_dict['center_of_mass'] = center_of_mass
+            field_dict["center_of_mass"] = center_of_mass
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[G], src_dict: Dict[str, Any]) -> G:
         d = src_dict.copy()
         center_of_mass = cast(List[float], d.pop("center_of_mass", UNSET))
 
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
@@ -100,19 +98,19 @@
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
         id = d.pop("id", UNSET)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, File3DImportFormat]
+        src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = File3DImportFormat(_src_format)
+            src_format = FileImportFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/file_conversion.py` & `kittycad-0.3.8/kittycad/models/file_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
+from ..models.api_call_status import ApiCallStatus
 from ..models.file_export_format import FileExportFormat
 from ..models.file_import_format import FileImportFormat
-from ..models.api_call_status import ApiCallStatus
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FileConversion")
+J = TypeVar("J", bound="FileConversion")
 
 
 @attr.s(auto_attribs=True)
 class FileConversion:
-    """ """
+    """A file conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     output: Union[Unset, str] = UNSET
     output_format: Union[Unset, FileExportFormat] = UNSET
     src_format: Union[Unset, FileImportFormat] = UNSET
@@ -36,61 +36,58 @@
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/file_density.py` & `kittycad-0.3.8/kittycad/models/unit_data_conversion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,93 +1,96 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.file3_d_import_format import File3DImportFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_data_format import UnitDataFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FileDensity")
+Z = TypeVar("Z", bound="UnitDataConversion")
 
 
 @attr.s(auto_attribs=True)
-class FileDensity:
-    """ """
+class UnitDataConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
-    density: Union[Unset, float] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    material_mass: Union[Unset, float] = UNSET
-    src_format: Union[Unset, File3DImportFormat] = UNSET
+    input: Union[Unset, float] = UNSET
+    output: Union[Unset, float] = UNSET
+    output_format: Union[Unset, UnitDataFormat] = UNSET
+    src_format: Union[Unset, UnitDataFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
-        density = self.density
         error = self.error
         id = self.id
-        material_mass = self.material_mass
-        src_format: Union[Unset, str] = UNSET
+        input = self.input
+        output = self.output
+        if not isinstance(self.output_format, Unset):
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
-        if density is not UNSET:
-            field_dict['density'] = density
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
-        if material_mass is not UNSET:
-            field_dict['material_mass'] = material_mass
+            field_dict["id"] = id
+        if input is not UNSET:
+            field_dict["input"] = input
+        if output is not UNSET:
+            field_dict["output"] = output
+        if output_format is not UNSET:
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[Z], src_dict: Dict[str, Any]) -> Z:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -95,28 +98,35 @@
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        density = d.pop("density", UNSET)
-
         error = d.pop("error", UNSET)
 
         id = d.pop("id", UNSET)
 
-        material_mass = d.pop("material_mass", UNSET)
+        input = d.pop("input", UNSET)
+
+        output = d.pop("output", UNSET)
+
+        _output_format = d.pop("output_format", UNSET)
+        output_format: Union[Unset, UnitDataFormat]
+        if isinstance(_output_format, Unset):
+            output_format = UNSET
+        else:
+            output_format = UnitDataFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, File3DImportFormat]
+        src_format: Union[Unset, UnitDataFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = File3DImportFormat(_src_format)
+            src_format = UnitDataFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -133,30 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        file_density = cls(
+        unit_data_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
-            density=density,
             error=error,
             id=id,
-            material_mass=material_mass,
+            input=input,
+            output=output,
+            output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        file_density.additional_properties = d
-        return file_density
+        unit_data_conversion.additional_properties = d
+        return unit_data_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/file_mass.py` & `kittycad-0.3.8/kittycad/models/file_mass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.file3_d_import_format import File3DImportFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.file_import_format import FileImportFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FileMass")
+L = TypeVar("L", bound="FileMass")
 
 
 @attr.s(auto_attribs=True)
 class FileMass:
-    """ """
+    """A file mass result."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     mass: Union[Unset, float] = UNSET
     material_density: Union[Unset, float] = UNSET
-    src_format: Union[Unset, File3DImportFormat] = UNSET
+    src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -36,58 +36,56 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         mass = self.mass
         material_density = self.material_density
-        src_format: Union[Unset, str] = UNSET
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if mass is not UNSET:
-            field_dict['mass'] = mass
+            field_dict["mass"] = mass
         if material_density is not UNSET:
-            field_dict['material_density'] = material_density
+            field_dict["material_density"] = material_density
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -104,19 +102,19 @@
         id = d.pop("id", UNSET)
 
         mass = d.pop("mass", UNSET)
 
         material_density = d.pop("material_density", UNSET)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, File3DImportFormat]
+        src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = File3DImportFormat(_src_format)
+            src_format = FileImportFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/file_surface_area.py` & `kittycad-0.3.8/kittycad/models/file_surface_area.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.file3_d_import_format import File3DImportFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.file_import_format import FileImportFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FileSurfaceArea")
+Y = TypeVar("Y", bound="FileSurfaceArea")
 
 
 @attr.s(auto_attribs=True)
 class FileSurfaceArea:
-    """ """
+    """A file surface area result."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    src_format: Union[Unset, File3DImportFormat] = UNSET
+    src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     surface_area: Union[Unset, float] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -33,57 +33,55 @@
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
-        src_format: Union[Unset, str] = UNSET
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         surface_area = self.surface_area
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if surface_area is not UNSET:
-            field_dict['surface_area'] = surface_area
+            field_dict["surface_area"] = surface_area
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -96,19 +94,19 @@
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
         id = d.pop("id", UNSET)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, File3DImportFormat]
+        src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = File3DImportFormat(_src_format)
+            src_format = FileImportFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/file_system_metadata.py` & `kittycad-0.3.8/kittycad/models/drawing_outcomes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FileSystemMetadata")
+T = TypeVar("T", bound="DrawingOutcomes")
 
 
 @attr.s(auto_attribs=True)
-class FileSystemMetadata:
-    """ """
-    ok: Union[Unset, bool] = False
+class DrawingOutcomes:
+    """The result from a batch of drawing commands."""  # noqa: E501
+
+    outcomes: Union[Unset, Any] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        ok = self.ok
+        outcomes = self.outcomes
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if ok is not UNSET:
-            field_dict['ok'] = ok
+        if outcomes is not UNSET:
+            field_dict["outcomes"] = outcomes
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        ok = d.pop("ok", UNSET)
+        outcomes = d.pop("outcomes", UNSET)
 
-        file_system_metadata = cls(
-            ok=ok,
+        drawing_outcomes = cls(
+            outcomes=outcomes,
         )
 
-        file_system_metadata.additional_properties = d
-        return file_system_metadata
+        drawing_outcomes.additional_properties = d
+        return drawing_outcomes
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/file_volume.py` & `kittycad-0.3.8/kittycad/models/file_volume.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.file3_d_import_format import File3DImportFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.file_import_format import FileImportFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FileVolume")
+K = TypeVar("K", bound="FileVolume")
 
 
 @attr.s(auto_attribs=True)
 class FileVolume:
-    """ """
+    """A file volume result."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    src_format: Union[Unset, File3DImportFormat] = UNSET
+    src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
     volume: Union[Unset, float] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -33,57 +33,55 @@
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
-        src_format: Union[Unset, str] = UNSET
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
         volume = self.volume
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
         if volume is not UNSET:
-            field_dict['volume'] = volume
+            field_dict["volume"] = volume
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -96,19 +94,19 @@
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
         id = d.pop("id", UNSET)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, File3DImportFormat]
+        src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = File3DImportFormat(_src_format)
+            src_format = FileImportFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/gateway.py` & `kittycad-0.3.8/kittycad/models/leaf_node.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,73 +1,67 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Gateway")
+Q = TypeVar("Q", bound="LeafNode")
 
 
 @attr.s(auto_attribs=True)
-class Gateway:
-    """ """
+class LeafNode:
+    """Leaf node information."""  # noqa: E501
+
     auth_timeout: Union[Unset, int] = UNSET
     host: Union[Unset, str] = UNSET
-    name: Union[Unset, str] = UNSET
     port: Union[Unset, int] = UNSET
     tls_timeout: Union[Unset, int] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         auth_timeout = self.auth_timeout
         host = self.host
-        name = self.name
         port = self.port
         tls_timeout = self.tls_timeout
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if auth_timeout is not UNSET:
-            field_dict['auth_timeout'] = auth_timeout
+            field_dict["auth_timeout"] = auth_timeout
         if host is not UNSET:
-            field_dict['host'] = host
-        if name is not UNSET:
-            field_dict['name'] = name
+            field_dict["host"] = host
         if port is not UNSET:
-            field_dict['port'] = port
+            field_dict["port"] = port
         if tls_timeout is not UNSET:
-            field_dict['tls_timeout'] = tls_timeout
+            field_dict["tls_timeout"] = tls_timeout
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[Q], src_dict: Dict[str, Any]) -> Q:
         d = src_dict.copy()
         auth_timeout = d.pop("auth_timeout", UNSET)
 
         host = d.pop("host", UNSET)
 
-        name = d.pop("name", UNSET)
-
         port = d.pop("port", UNSET)
 
         tls_timeout = d.pop("tls_timeout", UNSET)
 
-        gateway = cls(
+        leaf_node = cls(
             auth_timeout=auth_timeout,
             host=host,
-            name=name,
             port=port,
             tls_timeout=tls_timeout,
         )
 
-        gateway.additional_properties = d
-        return gateway
+        leaf_node.additional_properties = d
+        return leaf_node
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/index_info.py` & `kittycad-0.3.8/kittycad/models/index_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="IndexInfo")
+R = TypeVar("R", bound="IndexInfo")
 
 
 @attr.s(auto_attribs=True)
 class IndexInfo:
-    """ """
+    """IndexInfo contains information about a registry."""  # noqa: E501
+
     mirrors: Union[Unset, List[str]] = UNSET
     name: Union[Unset, str] = UNSET
     official: Union[Unset, bool] = False
     secure: Union[Unset, bool] = False
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -25,26 +26,26 @@
         official = self.official
         secure = self.secure
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if mirrors is not UNSET:
-            field_dict['mirrors'] = mirrors
+            field_dict["mirrors"] = mirrors
         if name is not UNSET:
-            field_dict['name'] = name
+            field_dict["name"] = name
         if official is not UNSET:
-            field_dict['official'] = official
+            field_dict["official"] = official
         if secure is not UNSET:
-            field_dict['secure'] = secure
+            field_dict["secure"] = secure
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
         d = src_dict.copy()
         mirrors = cast(List[str], d.pop("mirrors", UNSET))
 
         name = d.pop("name", UNSET)
 
         official = d.pop("official", UNSET)
```

### Comparing `kittycad-0.3.7/kittycad/models/invoice.py` & `kittycad-0.3.8/kittycad/models/invoice.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,33 +4,35 @@
 import attr
 from dateutil.parser import isoparse
 
 from ..models.currency import Currency
 from ..models.invoice_status import InvoiceStatus
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Invoice")
+N = TypeVar("N", bound="Invoice")
 
 
 @attr.s(auto_attribs=True)
 class Invoice:
-    """ """
+    """An invoice."""  # noqa: E501
+
     amount_due: Union[Unset, float] = UNSET
     amount_paid: Union[Unset, float] = UNSET
     amount_remaining: Union[Unset, float] = UNSET
     attempt_count: Union[Unset, int] = UNSET
     attempted: Union[Unset, bool] = False
     created_at: Union[Unset, datetime.datetime] = UNSET
     currency: Union[Unset, Currency] = UNSET
     customer_email: Union[Unset, str] = UNSET
     customer_id: Union[Unset, str] = UNSET
     default_payment_method: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     from ..models.invoice_line_item import InvoiceLineItem
+
     lines: Union[Unset, List[InvoiceLineItem]] = UNSET
     metadata: Union[Unset, Any] = UNSET
     number: Union[Unset, str] = UNSET
     paid: Union[Unset, bool] = False
     pdf: Union[Unset, str] = UNSET
     receipt_number: Union[Unset, str] = UNSET
     statement_descriptor: Union[Unset, str] = UNSET
@@ -47,96 +49,95 @@
         amount_paid = self.amount_paid
         amount_remaining = self.amount_remaining
         attempt_count = self.attempt_count
         attempted = self.attempted
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
-        currency: Union[Unset, str] = UNSET
         if not isinstance(self.currency, Unset):
-            currency = self.currency.value
+            currency = self.currency
         customer_email = self.customer_email
         customer_id = self.customer_id
         default_payment_method = self.default_payment_method
         description = self.description
         id = self.id
         from ..models.invoice_line_item import InvoiceLineItem
+
         lines: Union[Unset, List[InvoiceLineItem]] = UNSET
         if not isinstance(self.lines, Unset):
             lines = self.lines
         metadata = self.metadata
         number = self.number
         paid = self.paid
         pdf = self.pdf
         receipt_number = self.receipt_number
         statement_descriptor = self.statement_descriptor
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         subtotal = self.subtotal
         tax = self.tax
         total = self.total
         url = self.url
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if amount_due is not UNSET:
-            field_dict['amount_due'] = amount_due
+            field_dict["amount_due"] = amount_due
         if amount_paid is not UNSET:
-            field_dict['amount_paid'] = amount_paid
+            field_dict["amount_paid"] = amount_paid
         if amount_remaining is not UNSET:
-            field_dict['amount_remaining'] = amount_remaining
+            field_dict["amount_remaining"] = amount_remaining
         if attempt_count is not UNSET:
-            field_dict['attempt_count'] = attempt_count
+            field_dict["attempt_count"] = attempt_count
         if attempted is not UNSET:
-            field_dict['attempted'] = attempted
+            field_dict["attempted"] = attempted
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if currency is not UNSET:
-            field_dict['currency'] = currency
+            field_dict["currency"] = currency
         if customer_email is not UNSET:
-            field_dict['customer_email'] = customer_email
+            field_dict["customer_email"] = customer_email
         if customer_id is not UNSET:
-            field_dict['customer_id'] = customer_id
+            field_dict["customer_id"] = customer_id
         if default_payment_method is not UNSET:
-            field_dict['default_payment_method'] = default_payment_method
+            field_dict["default_payment_method"] = default_payment_method
         if description is not UNSET:
-            field_dict['description'] = description
+            field_dict["description"] = description
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if lines is not UNSET:
-            field_dict['lines'] = lines
+            field_dict["lines"] = lines
         if metadata is not UNSET:
-            field_dict['metadata'] = metadata
+            field_dict["metadata"] = metadata
         if number is not UNSET:
-            field_dict['number'] = number
+            field_dict["number"] = number
         if paid is not UNSET:
-            field_dict['paid'] = paid
+            field_dict["paid"] = paid
         if pdf is not UNSET:
-            field_dict['pdf'] = pdf
+            field_dict["pdf"] = pdf
         if receipt_number is not UNSET:
-            field_dict['receipt_number'] = receipt_number
+            field_dict["receipt_number"] = receipt_number
         if statement_descriptor is not UNSET:
-            field_dict['statement_descriptor'] = statement_descriptor
+            field_dict["statement_descriptor"] = statement_descriptor
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if subtotal is not UNSET:
-            field_dict['subtotal'] = subtotal
+            field_dict["subtotal"] = subtotal
         if tax is not UNSET:
-            field_dict['tax'] = tax
+            field_dict["tax"] = tax
         if total is not UNSET:
-            field_dict['total'] = total
+            field_dict["total"] = total
         if url is not UNSET:
-            field_dict['url'] = url
+            field_dict["url"] = url
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         amount_due = d.pop("amount_due", UNSET)
 
         amount_paid = d.pop("amount_paid", UNSET)
 
         amount_remaining = d.pop("amount_remaining", UNSET)
 
@@ -165,14 +166,15 @@
         default_payment_method = d.pop("default_payment_method", UNSET)
 
         description = d.pop("description", UNSET)
 
         id = d.pop("id", UNSET)
 
         from ..models.invoice_line_item import InvoiceLineItem
+
         lines = cast(List[InvoiceLineItem], d.pop("lines", UNSET))
 
         metadata = d.pop("metadata", UNSET)
         number = d.pop("number", UNSET)
 
         paid = d.pop("paid", UNSET)
```

### Comparing `kittycad-0.3.7/kittycad/models/invoice_line_item.py` & `kittycad-0.3.8/kittycad/models/invoice_line_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.currency import Currency
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="InvoiceLineItem")
+P = TypeVar("P", bound="InvoiceLineItem")
 
 
 @attr.s(auto_attribs=True)
 class InvoiceLineItem:
-    """ """
+    """An invoice line item."""  # noqa: E501
+
     amount: Union[Unset, float] = UNSET
     currency: Union[Unset, Currency] = UNSET
     description: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     invoice_item: Union[Unset, str] = UNSET
     metadata: Union[Unset, Any] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         amount = self.amount
-        currency: Union[Unset, str] = UNSET
         if not isinstance(self.currency, Unset):
-            currency = self.currency.value
+            currency = self.currency
         description = self.description
         id = self.id
         invoice_item = self.invoice_item
         metadata = self.metadata
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if amount is not UNSET:
-            field_dict['amount'] = amount
+            field_dict["amount"] = amount
         if currency is not UNSET:
-            field_dict['currency'] = currency
+            field_dict["currency"] = currency
         if description is not UNSET:
-            field_dict['description'] = description
+            field_dict["description"] = description
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if invoice_item is not UNSET:
-            field_dict['invoice_item'] = invoice_item
+            field_dict["invoice_item"] = invoice_item
         if metadata is not UNSET:
-            field_dict['metadata'] = metadata
+            field_dict["metadata"] = metadata
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
         d = src_dict.copy()
         amount = d.pop("amount", UNSET)
 
         _currency = d.pop("currency", UNSET)
         currency: Union[Unset, Currency]
         if isinstance(_currency, Unset):
             currency = UNSET
```

### Comparing `kittycad-0.3.7/kittycad/models/jetstream.py` & `kittycad-0.3.8/kittycad/models/jetstream.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,51 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.jetstream_config import JetstreamConfig
-from ..models.meta_cluster_info import MetaClusterInfo
 from ..models.jetstream_stats import JetstreamStats
+from ..models.meta_cluster_info import MetaClusterInfo
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Jetstream")
+C = TypeVar("C", bound="Jetstream")
 
 
 @attr.s(auto_attribs=True)
 class Jetstream:
-    """ """
+    """Jetstream information."""  # noqa: E501
+
     config: Union[Unset, JetstreamConfig] = UNSET
     meta: Union[Unset, MetaClusterInfo] = UNSET
     stats: Union[Unset, JetstreamStats] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        config: Union[Unset, str] = UNSET
         if not isinstance(self.config, Unset):
-            config = self.config.value
-        meta: Union[Unset, str] = UNSET
+            config = self.config
         if not isinstance(self.meta, Unset):
-            meta = self.meta.value
-        stats: Union[Unset, str] = UNSET
+            meta = self.meta
         if not isinstance(self.stats, Unset):
-            stats = self.stats.value
+            stats = self.stats
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if config is not UNSET:
-            field_dict['config'] = config
+            field_dict["config"] = config
         if meta is not UNSET:
-            field_dict['meta'] = meta
+            field_dict["meta"] = meta
         if stats is not UNSET:
-            field_dict['stats'] = stats
+            field_dict["stats"] = stats
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
         d = src_dict.copy()
         _config = d.pop("config", UNSET)
         config: Union[Unset, JetstreamConfig]
         if isinstance(_config, Unset):
             config = UNSET
         else:
             config = JetstreamConfig(_config)
```

### Comparing `kittycad-0.3.7/kittycad/models/jetstream_api_stats.py` & `kittycad-0.3.8/kittycad/models/file_system_metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,48 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="JetstreamApiStats")
+H = TypeVar("H", bound="FileSystemMetadata")
 
 
 @attr.s(auto_attribs=True)
-class JetstreamApiStats:
-    """ """
-    errors: Union[Unset, int] = UNSET
-    inflight: Union[Unset, int] = UNSET
-    total: Union[Unset, int] = UNSET
+class FileSystemMetadata:
+    """Metadata about our file system.
+
+    This is mostly used for internal purposes and debugging."""  # noqa: E501
+
+    ok: Union[Unset, bool] = False
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        errors = self.errors
-        inflight = self.inflight
-        total = self.total
+        ok = self.ok
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if errors is not UNSET:
-            field_dict['errors'] = errors
-        if inflight is not UNSET:
-            field_dict['inflight'] = inflight
-        if total is not UNSET:
-            field_dict['total'] = total
+        if ok is not UNSET:
+            field_dict["ok"] = ok
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
-        errors = d.pop("errors", UNSET)
-
-        inflight = d.pop("inflight", UNSET)
-
-        total = d.pop("total", UNSET)
+        ok = d.pop("ok", UNSET)
 
-        jetstream_api_stats = cls(
-            errors=errors,
-            inflight=inflight,
-            total=total,
+        file_system_metadata = cls(
+            ok=ok,
         )
 
-        jetstream_api_stats.additional_properties = d
-        return jetstream_api_stats
+        file_system_metadata.additional_properties = d
+        return file_system_metadata
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/jetstream_config.py` & `kittycad-0.3.8/kittycad/models/jetstream_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="JetstreamConfig")
+S = TypeVar("S", bound="JetstreamConfig")
 
 
 @attr.s(auto_attribs=True)
 class JetstreamConfig:
-    """ """
+    """Jetstream configuration."""  # noqa: E501
+
     domain: Union[Unset, str] = UNSET
     max_memory: Union[Unset, int] = UNSET
     max_storage: Union[Unset, int] = UNSET
     store_dir: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -23,26 +24,26 @@
         max_storage = self.max_storage
         store_dir = self.store_dir
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if domain is not UNSET:
-            field_dict['domain'] = domain
+            field_dict["domain"] = domain
         if max_memory is not UNSET:
-            field_dict['max_memory'] = max_memory
+            field_dict["max_memory"] = max_memory
         if max_storage is not UNSET:
-            field_dict['max_storage'] = max_storage
+            field_dict["max_storage"] = max_storage
         if store_dir is not UNSET:
-            field_dict['store_dir'] = store_dir
+            field_dict["store_dir"] = store_dir
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
         d = src_dict.copy()
         domain = d.pop("domain", UNSET)
 
         max_memory = d.pop("max_memory", UNSET)
 
         max_storage = d.pop("max_storage", UNSET)
```

### Comparing `kittycad-0.3.7/kittycad/models/jetstream_stats.py` & `kittycad-0.3.8/kittycad/models/jetstream_stats.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.jetstream_api_stats import JetstreamApiStats
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="JetstreamStats")
+K = TypeVar("K", bound="JetstreamStats")
 
 
 @attr.s(auto_attribs=True)
 class JetstreamStats:
-    """ """
+    """Jetstream statistics."""  # noqa: E501
+
     accounts: Union[Unset, int] = UNSET
     api: Union[Unset, JetstreamApiStats] = UNSET
     ha_assets: Union[Unset, int] = UNSET
     memory: Union[Unset, int] = UNSET
     reserved_memory: Union[Unset, int] = UNSET
     reserved_store: Union[Unset, int] = UNSET
     store: Union[Unset, int] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         accounts = self.accounts
-        api: Union[Unset, str] = UNSET
         if not isinstance(self.api, Unset):
-            api = self.api.value
+            api = self.api
         ha_assets = self.ha_assets
         memory = self.memory
         reserved_memory = self.reserved_memory
         reserved_store = self.reserved_store
         store = self.store
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if accounts is not UNSET:
-            field_dict['accounts'] = accounts
+            field_dict["accounts"] = accounts
         if api is not UNSET:
-            field_dict['api'] = api
+            field_dict["api"] = api
         if ha_assets is not UNSET:
-            field_dict['ha_assets'] = ha_assets
+            field_dict["ha_assets"] = ha_assets
         if memory is not UNSET:
-            field_dict['memory'] = memory
+            field_dict["memory"] = memory
         if reserved_memory is not UNSET:
-            field_dict['reserved_memory'] = reserved_memory
+            field_dict["reserved_memory"] = reserved_memory
         if reserved_store is not UNSET:
-            field_dict['reserved_store'] = reserved_store
+            field_dict["reserved_store"] = reserved_store
         if store is not UNSET:
-            field_dict['store'] = store
+            field_dict["store"] = store
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
         d = src_dict.copy()
         accounts = d.pop("accounts", UNSET)
 
         _api = d.pop("api", UNSET)
         api: Union[Unset, JetstreamApiStats]
         if isinstance(_api, Unset):
             api = UNSET
```

### Comparing `kittycad-0.3.7/kittycad/models/leaf_node.py` & `kittycad-0.3.8/kittycad/models/gateway.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,74 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="LeafNode")
+V = TypeVar("V", bound="Gateway")
 
 
 @attr.s(auto_attribs=True)
-class LeafNode:
-    """ """
+class Gateway:
+    """Gateway information."""  # noqa: E501
+
     auth_timeout: Union[Unset, int] = UNSET
     host: Union[Unset, str] = UNSET
+    name: Union[Unset, str] = UNSET
     port: Union[Unset, int] = UNSET
     tls_timeout: Union[Unset, int] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         auth_timeout = self.auth_timeout
         host = self.host
+        name = self.name
         port = self.port
         tls_timeout = self.tls_timeout
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if auth_timeout is not UNSET:
-            field_dict['auth_timeout'] = auth_timeout
+            field_dict["auth_timeout"] = auth_timeout
         if host is not UNSET:
-            field_dict['host'] = host
+            field_dict["host"] = host
+        if name is not UNSET:
+            field_dict["name"] = name
         if port is not UNSET:
-            field_dict['port'] = port
+            field_dict["port"] = port
         if tls_timeout is not UNSET:
-            field_dict['tls_timeout'] = tls_timeout
+            field_dict["tls_timeout"] = tls_timeout
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
         auth_timeout = d.pop("auth_timeout", UNSET)
 
         host = d.pop("host", UNSET)
 
+        name = d.pop("name", UNSET)
+
         port = d.pop("port", UNSET)
 
         tls_timeout = d.pop("tls_timeout", UNSET)
 
-        leaf_node = cls(
+        gateway = cls(
             auth_timeout=auth_timeout,
             host=host,
+            name=name,
             port=port,
             tls_timeout=tls_timeout,
         )
 
-        leaf_node.additional_properties = d
-        return leaf_node
+        gateway.additional_properties = d
+        return gateway
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/mesh.py` & `kittycad-0.3.8/kittycad/models/system_info_default_address_pools.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,51 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Mesh")
+T = TypeVar("T", bound="SystemInfoDefaultAddressPools")
 
 
 @attr.s(auto_attribs=True)
-class Mesh:
-    """ """
-    mesh: Union[Unset, str] = UNSET
+class SystemInfoDefaultAddressPools:
+    base: Union[Unset, str] = UNSET
+    size: Union[Unset, int] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        mesh = self.mesh
+        base = self.base
+        size = self.size
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if mesh is not UNSET:
-            field_dict['mesh'] = mesh
+        if base is not UNSET:
+            field_dict["base"] = base
+        if size is not UNSET:
+            field_dict["size"] = size
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        mesh = d.pop("mesh", UNSET)
+        base = d.pop("base", UNSET)
 
-        mesh = cls(
-            mesh=mesh,
+        size = d.pop("size", UNSET)
+
+        system_info_default_address_pools = cls(
+            base=base,
+            size=size,
         )
 
-        mesh.additional_properties = d
-        return mesh
+        system_info_default_address_pools.additional_properties = d
+        return system_info_default_address_pools
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/meta_cluster_info.py` & `kittycad-0.3.8/kittycad/models/meta_cluster_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="MetaClusterInfo")
+H = TypeVar("H", bound="MetaClusterInfo")
 
 
 @attr.s(auto_attribs=True)
 class MetaClusterInfo:
-    """ """
+    """Jetstream statistics."""  # noqa: E501
+
     cluster_size: Union[Unset, int] = UNSET
     leader: Union[Unset, str] = UNSET
     name: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
@@ -21,24 +22,24 @@
         leader = self.leader
         name = self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if cluster_size is not UNSET:
-            field_dict['cluster_size'] = cluster_size
+            field_dict["cluster_size"] = cluster_size
         if leader is not UNSET:
-            field_dict['leader'] = leader
+            field_dict["leader"] = leader
         if name is not UNSET:
-            field_dict['name'] = name
+            field_dict["name"] = name
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         cluster_size = d.pop("cluster_size", UNSET)
 
         leader = d.pop("leader", UNSET)
 
         name = d.pop("name", UNSET)
```

### Comparing `kittycad-0.3.7/kittycad/models/metadata.py` & `kittycad-0.3.8/kittycad/models/metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,81 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.cache_metadata import CacheMetadata
+from ..models.connection import Connection
 from ..models.engine_metadata import EngineMetadata
 from ..models.environment import Environment
 from ..models.executor_metadata import ExecutorMetadata
 from ..models.file_system_metadata import FileSystemMetadata
 from ..models.point_e_metadata import PointEMetadata
-from ..models.connection import Connection
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Metadata")
+N = TypeVar("N", bound="Metadata")
 
 
 @attr.s(auto_attribs=True)
 class Metadata:
-    """ """
+    """Metadata about our currently running server.
+
+    This is mostly used for internal purposes and debugging."""  # noqa: E501
+
     cache: Union[Unset, CacheMetadata] = UNSET
     engine: Union[Unset, EngineMetadata] = UNSET
     environment: Union[Unset, Environment] = UNSET
     executor: Union[Unset, ExecutorMetadata] = UNSET
     fs: Union[Unset, FileSystemMetadata] = UNSET
     git_hash: Union[Unset, str] = UNSET
     point_e: Union[Unset, PointEMetadata] = UNSET
     pubsub: Union[Unset, Connection] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cache: Union[Unset, str] = UNSET
         if not isinstance(self.cache, Unset):
-            cache = self.cache.value
-        engine: Union[Unset, str] = UNSET
+            cache = self.cache
         if not isinstance(self.engine, Unset):
-            engine = self.engine.value
-        environment: Union[Unset, str] = UNSET
+            engine = self.engine
         if not isinstance(self.environment, Unset):
-            environment = self.environment.value
-        executor: Union[Unset, str] = UNSET
+            environment = self.environment
         if not isinstance(self.executor, Unset):
-            executor = self.executor.value
-        fs: Union[Unset, str] = UNSET
+            executor = self.executor
         if not isinstance(self.fs, Unset):
-            fs = self.fs.value
+            fs = self.fs
         git_hash = self.git_hash
-        point_e: Union[Unset, str] = UNSET
         if not isinstance(self.point_e, Unset):
-            point_e = self.point_e.value
-        pubsub: Union[Unset, str] = UNSET
+            point_e = self.point_e
         if not isinstance(self.pubsub, Unset):
-            pubsub = self.pubsub.value
+            pubsub = self.pubsub
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if cache is not UNSET:
-            field_dict['cache'] = cache
+            field_dict["cache"] = cache
         if engine is not UNSET:
-            field_dict['engine'] = engine
+            field_dict["engine"] = engine
         if environment is not UNSET:
-            field_dict['environment'] = environment
+            field_dict["environment"] = environment
         if executor is not UNSET:
-            field_dict['executor'] = executor
+            field_dict["executor"] = executor
         if fs is not UNSET:
-            field_dict['fs'] = fs
+            field_dict["fs"] = fs
         if git_hash is not UNSET:
-            field_dict['git_hash'] = git_hash
+            field_dict["git_hash"] = git_hash
         if point_e is not UNSET:
-            field_dict['point_e'] = point_e
+            field_dict["point_e"] = point_e
         if pubsub is not UNSET:
-            field_dict['pubsub'] = pubsub
+            field_dict["pubsub"] = pubsub
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         _cache = d.pop("cache", UNSET)
         cache: Union[Unset, CacheMetadata]
         if isinstance(_cache, Unset):
             cache = UNSET
         else:
             cache = CacheMetadata(_cache)
```

### Comparing `kittycad-0.3.7/kittycad/models/new_address.py` & `kittycad-0.3.8/kittycad/models/new_address.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.country_code import CountryCode
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="NewAddress")
+H = TypeVar("H", bound="NewAddress")
 
 
 @attr.s(auto_attribs=True)
 class NewAddress:
-    """ """
+    """The struct that is used to create a new record. This is automatically generated and has all the same fields as the main struct only it is missing the `id`."""  # noqa: E501
+
     city: Union[Unset, str] = UNSET
     country: Union[Unset, CountryCode] = UNSET
     state: Union[Unset, str] = UNSET
     street1: Union[Unset, str] = UNSET
     street2: Union[Unset, str] = UNSET
     user_id: Union[Unset, str] = UNSET
     zip: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         city = self.city
-        country: Union[Unset, str] = UNSET
         if not isinstance(self.country, Unset):
-            country = self.country.value
+            country = self.country
         state = self.state
         street1 = self.street1
         street2 = self.street2
         user_id = self.user_id
         zip = self.zip
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if city is not UNSET:
-            field_dict['city'] = city
+            field_dict["city"] = city
         if country is not UNSET:
-            field_dict['country'] = country
+            field_dict["country"] = country
         if state is not UNSET:
-            field_dict['state'] = state
+            field_dict["state"] = state
         if street1 is not UNSET:
-            field_dict['street1'] = street1
+            field_dict["street1"] = street1
         if street2 is not UNSET:
-            field_dict['street2'] = street2
+            field_dict["street2"] = street2
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
         if zip is not UNSET:
-            field_dict['zip'] = zip
+            field_dict["zip"] = zip
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         city = d.pop("city", UNSET)
 
         _country = d.pop("country", UNSET)
         country: Union[Unset, CountryCode]
         if isinstance(_country, Unset):
             country = UNSET
```

### Comparing `kittycad-0.3.7/kittycad/models/o_auth2_client_info.py` & `kittycad-0.3.8/kittycad/models/o_auth2_client_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OAuth2ClientInfo")
+B = TypeVar("B", bound="OAuth2ClientInfo")
 
 
 @attr.s(auto_attribs=True)
 class OAuth2ClientInfo:
-    """ """
+    """Information about an OAuth 2.0 client."""  # noqa: E501
+
     csrf_token: Union[Unset, str] = UNSET
     pkce_code_verifier: Union[Unset, str] = UNSET
     url: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
@@ -21,24 +22,24 @@
         pkce_code_verifier = self.pkce_code_verifier
         url = self.url
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if csrf_token is not UNSET:
-            field_dict['csrf_token'] = csrf_token
+            field_dict["csrf_token"] = csrf_token
         if pkce_code_verifier is not UNSET:
-            field_dict['pkce_code_verifier'] = pkce_code_verifier
+            field_dict["pkce_code_verifier"] = pkce_code_verifier
         if url is not UNSET:
-            field_dict['url'] = url
+            field_dict["url"] = url
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
         d = src_dict.copy()
         csrf_token = d.pop("csrf_token", UNSET)
 
         pkce_code_verifier = d.pop("pkce_code_verifier", UNSET)
 
         url = d.pop("url", UNSET)
```

### Comparing `kittycad-0.3.7/kittycad/models/onboarding.py` & `kittycad-0.3.8/kittycad/models/onboarding.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Onboarding")
+B = TypeVar("B", bound="Onboarding")
 
 
 @attr.s(auto_attribs=True)
 class Onboarding:
-    """ """
+    """Onboarding details"""  # noqa: E501
+
     first_call_from_their_machine_date: Union[Unset, str] = UNSET
     first_litterbox_execute_date: Union[Unset, str] = UNSET
     first_token_date: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
@@ -21,30 +22,32 @@
         first_litterbox_execute_date = self.first_litterbox_execute_date
         first_token_date = self.first_token_date
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if first_call_from_their_machine_date is not UNSET:
-            field_dict['first_call_from_their_machine_date'] = first_call_from_their_machine_date
+            field_dict[
+                "first_call_from_their_machine_date"
+            ] = first_call_from_their_machine_date
         if first_litterbox_execute_date is not UNSET:
-            field_dict['first_litterbox_execute_date'] = first_litterbox_execute_date
+            field_dict["first_litterbox_execute_date"] = first_litterbox_execute_date
         if first_token_date is not UNSET:
-            field_dict['first_token_date'] = first_token_date
+            field_dict["first_token_date"] = first_token_date
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
         d = src_dict.copy()
         first_call_from_their_machine_date = d.pop(
-            "first_call_from_their_machine_date", UNSET)
+            "first_call_from_their_machine_date", UNSET
+        )
 
-        first_litterbox_execute_date = d.pop(
-            "first_litterbox_execute_date", UNSET)
+        first_litterbox_execute_date = d.pop("first_litterbox_execute_date", UNSET)
 
         first_token_date = d.pop("first_token_date", UNSET)
 
         onboarding = cls(
             first_call_from_their_machine_date=first_call_from_their_machine_date,
             first_litterbox_execute_date=first_litterbox_execute_date,
             first_token_date=first_token_date,
```

### Comparing `kittycad-0.3.7/kittycad/models/output_file.py` & `kittycad-0.3.8/kittycad/models/output_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OutputFile")
+P = TypeVar("P", bound="OutputFile")
 
 
 @attr.s(auto_attribs=True)
 class OutputFile:
-    """ """
+    """Output file contents."""  # noqa: E501
+
     contents: Union[Unset, str] = UNSET
     name: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         contents = self.contents
         name = self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if contents is not UNSET:
-            field_dict['contents'] = contents
+            field_dict["contents"] = contents
         if name is not UNSET:
-            field_dict['name'] = name
+            field_dict["name"] = name
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
         d = src_dict.copy()
         contents = d.pop("contents", UNSET)
 
         name = d.pop("name", UNSET)
 
         output_file = cls(
             contents=contents,
```

### Comparing `kittycad-0.3.7/kittycad/models/payment_intent.py` & `kittycad-0.3.8/kittycad/models/device_auth_request_form.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PaymentIntent")
+V = TypeVar("V", bound="DeviceAuthRequestForm")
 
 
 @attr.s(auto_attribs=True)
-class PaymentIntent:
-    """ """
-    client_secret: Union[Unset, str] = UNSET
+class DeviceAuthRequestForm:
+    """The request parameters for the OAuth 2.0 Device Authorization Grant flow."""  # noqa: E501
+
+    client_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        client_secret = self.client_secret
+        client_id = self.client_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if client_secret is not UNSET:
-            field_dict['client_secret'] = client_secret
+        if client_id is not UNSET:
+            field_dict["client_id"] = client_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
-        client_secret = d.pop("client_secret", UNSET)
+        client_id = d.pop("client_id", UNSET)
 
-        payment_intent = cls(
-            client_secret=client_secret,
+        device_auth_request_form = cls(
+            client_id=client_id,
         )
 
-        payment_intent.additional_properties = d
-        return payment_intent
+        device_auth_request_form.additional_properties = d
+        return device_auth_request_form
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/payment_method.py` & `kittycad-0.3.8/kittycad/models/payment_method.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.billing_info import BillingInfo
 from ..models.card_details import CardDetails
 from ..models.payment_method_type import PaymentMethodType
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="PaymentMethod")
 
 
 @attr.s(auto_attribs=True)
 class PaymentMethod:
-    """ """
+    """A payment method."""  # noqa: E501
+
     billing_info: Union[Unset, BillingInfo] = UNSET
     card: Union[Unset, CardDetails] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     id: Union[Unset, str] = UNSET
     metadata: Union[Unset, Any] = UNSET
     type: Union[Unset, PaymentMethodType] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        billing_info: Union[Unset, str] = UNSET
         if not isinstance(self.billing_info, Unset):
-            billing_info = self.billing_info.value
-        card: Union[Unset, str] = UNSET
+            billing_info = self.billing_info
         if not isinstance(self.card, Unset):
-            card = self.card.value
+            card = self.card
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         id = self.id
         metadata = self.metadata
-        type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
-            type = self.type.value
+            type = self.type
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if billing_info is not UNSET:
-            field_dict['billing_info'] = billing_info
+            field_dict["billing_info"] = billing_info
         if card is not UNSET:
-            field_dict['card'] = card
+            field_dict["card"] = card
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if metadata is not UNSET:
-            field_dict['metadata'] = metadata
+            field_dict["metadata"] = metadata
         if type is not UNSET:
-            field_dict['type'] = type
+            field_dict["type"] = type
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _billing_info = d.pop("billing_info", UNSET)
```

### Comparing `kittycad-0.3.7/kittycad/models/payment_method_card_checks.py` & `kittycad-0.3.8/kittycad/models/payment_method_card_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PaymentMethodCardChecks")
+V = TypeVar("V", bound="PaymentMethodCardChecks")
 
 
 @attr.s(auto_attribs=True)
 class PaymentMethodCardChecks:
-    """ """
+    """Card checks."""  # noqa: E501
+
     address_line1_check: Union[Unset, str] = UNSET
     address_postal_code_check: Union[Unset, str] = UNSET
     cvc_check: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
@@ -21,24 +22,24 @@
         address_postal_code_check = self.address_postal_code_check
         cvc_check = self.cvc_check
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if address_line1_check is not UNSET:
-            field_dict['address_line1_check'] = address_line1_check
+            field_dict["address_line1_check"] = address_line1_check
         if address_postal_code_check is not UNSET:
-            field_dict['address_postal_code_check'] = address_postal_code_check
+            field_dict["address_postal_code_check"] = address_postal_code_check
         if cvc_check is not UNSET:
-            field_dict['cvc_check'] = cvc_check
+            field_dict["cvc_check"] = cvc_check
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
         address_line1_check = d.pop("address_line1_check", UNSET)
 
         address_postal_code_check = d.pop("address_postal_code_check", UNSET)
 
         cvc_check = d.pop("cvc_check", UNSET)
```

### Comparing `kittycad-0.3.7/kittycad/models/physics_constant.py` & `kittycad-0.3.8/kittycad/models/file_density.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,115 +1,121 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.physics_constant_name import PhysicsConstantName
-from ..models.uuid import Uuid
 from ..models.api_call_status import ApiCallStatus
+from ..models.file_import_format import FileImportFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PhysicsConstant")
+R = TypeVar("R", bound="FileDensity")
 
 
 @attr.s(auto_attribs=True)
-class PhysicsConstant:
-    """ """
+class FileDensity:
+    """A file density result."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
-    constant: Union[Unset, PhysicsConstantName] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
+    density: Union[Unset, float] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
+    material_mass: Union[Unset, float] = UNSET
+    src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
-    value: Union[Unset, float] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
-        constant: Union[Unset, str] = UNSET
-        if not isinstance(self.constant, Unset):
-            constant = self.constant.value
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
+        density = self.density
         error = self.error
         id = self.id
+        material_mass = self.material_mass
+        if not isinstance(self.src_format, Unset):
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
-        value = self.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
-        if constant is not UNSET:
-            field_dict['constant'] = constant
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
+        if density is not UNSET:
+            field_dict["density"] = density
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
+        if material_mass is not UNSET:
+            field_dict["material_mass"] = material_mass
+        if src_format is not UNSET:
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
-        if value is not UNSET:
-            field_dict['value'] = value
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
 
-        _constant = d.pop("constant", UNSET)
-        constant: Union[Unset, PhysicsConstantName]
-        if isinstance(_constant, Unset):
-            constant = UNSET
-        else:
-            constant = PhysicsConstantName(_constant)
-
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
+        density = d.pop("density", UNSET)
+
         error = d.pop("error", UNSET)
 
         id = d.pop("id", UNSET)
 
+        material_mass = d.pop("material_mass", UNSET)
+
+        _src_format = d.pop("src_format", UNSET)
+        src_format: Union[Unset, FileImportFormat]
+        if isinstance(_src_format, Unset):
+            src_format = UNSET
+        else:
+            src_format = FileImportFormat(_src_format)
+
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
@@ -125,31 +131,30 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        value = d.pop("value", UNSET)
-
-        physics_constant = cls(
+        file_density = cls(
             completed_at=completed_at,
-            constant=constant,
             created_at=created_at,
+            density=density,
             error=error,
             id=id,
+            material_mass=material_mass,
+            src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
-            value=value,
         )
 
-        physics_constant.additional_properties = d
-        return physics_constant
+        file_density.additional_properties = d
+        return file_density
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/plugins_info.py` & `kittycad-0.3.8/kittycad/models/plugins_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PluginsInfo")
+R = TypeVar("R", bound="PluginsInfo")
 
 
 @attr.s(auto_attribs=True)
 class PluginsInfo:
-    """ """
+    """Available plugins per type.
+
+    **Note**: Only unmanaged (V1) plugins are included in this list. V1 plugins are \"lazily\" loaded, and are not returned in this list if there is no resource using the plugin."""  # noqa: E501
+
     authorization: Union[Unset, List[str]] = UNSET
     log: Union[Unset, List[str]] = UNSET
     network: Union[Unset, List[str]] = UNSET
     volume: Union[Unset, List[str]] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -31,26 +34,26 @@
         if not isinstance(self.volume, Unset):
             volume = self.volume
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if authorization is not UNSET:
-            field_dict['authorization'] = authorization
+            field_dict["authorization"] = authorization
         if log is not UNSET:
-            field_dict['log'] = log
+            field_dict["log"] = log
         if network is not UNSET:
-            field_dict['network'] = network
+            field_dict["network"] = network
         if volume is not UNSET:
-            field_dict['volume'] = volume
+            field_dict["volume"] = volume
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
         d = src_dict.copy()
         authorization = cast(List[str], d.pop("authorization", UNSET))
 
         log = cast(List[str], d.pop("log", UNSET))
 
         network = cast(List[str], d.pop("network", UNSET))
```

### Comparing `kittycad-0.3.7/kittycad/models/point_e_metadata.py` & `kittycad-0.3.8/kittycad/models/drawing_outcome.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,58 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.drawing_cmd_id import DrawingCmdId
 from ..types import UNSET, Unset
+from .drawing_error import DrawingError
 
-T = TypeVar("T", bound="PointEMetadata")
+Success = Any
+
+
+Error = DrawingError
+
+
+H = TypeVar("H", bound="Cancelled")
 
 
 @attr.s(auto_attribs=True)
-class PointEMetadata:
-    """ """
-    ok: Union[Unset, bool] = False
+class Cancelled:
+    what_failed: Union[Unset, DrawingCmdId] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        ok = self.ok
+        if not isinstance(self.what_failed, Unset):
+            what_failed = self.what_failed
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if ok is not UNSET:
-            field_dict['ok'] = ok
+        if what_failed is not UNSET:
+            field_dict["what_failed"] = what_failed
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
-        ok = d.pop("ok", UNSET)
+        _what_failed = d.pop("what_failed", UNSET)
+        what_failed: Union[Unset, DrawingCmdId]
+        if isinstance(_what_failed, Unset):
+            what_failed = UNSET
+        else:
+            what_failed = DrawingCmdId(_what_failed)
 
-        point_e_metadata = cls(
-            ok=ok,
+        cancelled = cls(
+            what_failed=what_failed,
         )
 
-        point_e_metadata.additional_properties = d
-        return point_e_metadata
+        cancelled.additional_properties = d
+        return cancelled
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
@@ -48,7 +61,10 @@
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
+
+
+DrawingOutcome = Union[Success, Error, Cancelled]
```

### Comparing `kittycad-0.3.7/kittycad/models/registry_service_config.py` & `kittycad-0.3.8/kittycad/models/registry_service_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,82 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
-from ..models.index_info import IndexInfo
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RegistryServiceConfig")
+M = TypeVar("M", bound="RegistryServiceConfig")
 
 
 @attr.s(auto_attribs=True)
 class RegistryServiceConfig:
-    """ """
+    """RegistryServiceConfig stores daemon registry services configuration."""  # noqa: E501
+
     allow_nondistributable_artifacts_cid_rs: Union[Unset, List[str]] = UNSET
     allow_nondistributable_artifacts_hostnames: Union[Unset, List[str]] = UNSET
     index_configs: Union[Unset, Any] = UNSET
     insecure_registry_cid_rs: Union[Unset, List[str]] = UNSET
     mirrors: Union[Unset, List[str]] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        allow_nondistributable_artifacts_cid_rs: Union[Unset,
-                                                       List[str]] = UNSET
+        allow_nondistributable_artifacts_cid_rs: Union[Unset, List[str]] = UNSET
         if not isinstance(self.allow_nondistributable_artifacts_cid_rs, Unset):
-            allow_nondistributable_artifacts_cid_rs = self.allow_nondistributable_artifacts_cid_rs
-        allow_nondistributable_artifacts_hostnames: Union[Unset,
-                                                          List[str]] = UNSET
-        if not isinstance(
-                self.allow_nondistributable_artifacts_hostnames,
-                Unset):
-            allow_nondistributable_artifacts_hostnames = self.allow_nondistributable_artifacts_hostnames
+            allow_nondistributable_artifacts_cid_rs = (
+                self.allow_nondistributable_artifacts_cid_rs
+            )
+        allow_nondistributable_artifacts_hostnames: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.allow_nondistributable_artifacts_hostnames, Unset):
+            allow_nondistributable_artifacts_hostnames = (
+                self.allow_nondistributable_artifacts_hostnames
+            )
         index_configs = self.index_configs
         insecure_registry_cid_rs: Union[Unset, List[str]] = UNSET
         if not isinstance(self.insecure_registry_cid_rs, Unset):
             insecure_registry_cid_rs = self.insecure_registry_cid_rs
         mirrors: Union[Unset, List[str]] = UNSET
         if not isinstance(self.mirrors, Unset):
             mirrors = self.mirrors
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if allow_nondistributable_artifacts_cid_rs is not UNSET:
-            field_dict['allow_nondistributable_artifacts_cid_rs'] = allow_nondistributable_artifacts_cid_rs
+            field_dict[
+                "allow_nondistributable_artifacts_cid_rs"
+            ] = allow_nondistributable_artifacts_cid_rs
         if allow_nondistributable_artifacts_hostnames is not UNSET:
-            field_dict['allow_nondistributable_artifacts_hostnames'] = allow_nondistributable_artifacts_hostnames
+            field_dict[
+                "allow_nondistributable_artifacts_hostnames"
+            ] = allow_nondistributable_artifacts_hostnames
         if index_configs is not UNSET:
-            field_dict['index_configs'] = index_configs
+            field_dict["index_configs"] = index_configs
         if insecure_registry_cid_rs is not UNSET:
-            field_dict['insecure_registry_cid_rs'] = insecure_registry_cid_rs
+            field_dict["insecure_registry_cid_rs"] = insecure_registry_cid_rs
         if mirrors is not UNSET:
-            field_dict['mirrors'] = mirrors
+            field_dict["mirrors"] = mirrors
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[M], src_dict: Dict[str, Any]) -> M:
         d = src_dict.copy()
         allow_nondistributable_artifacts_cid_rs = cast(
-            List[str], d.pop("allow_nondistributable_artifacts_cid_rs", UNSET))
+            List[str], d.pop("allow_nondistributable_artifacts_cid_rs", UNSET)
+        )
 
         allow_nondistributable_artifacts_hostnames = cast(
-            List[str], d.pop("allow_nondistributable_artifacts_hostnames", UNSET))
+            List[str], d.pop("allow_nondistributable_artifacts_hostnames", UNSET)
+        )
 
         index_configs = d.pop("index_configs", UNSET)
         insecure_registry_cid_rs = cast(
-            List[str], d.pop(
-                "insecure_registry_cid_rs", UNSET))
+            List[str], d.pop("insecure_registry_cid_rs", UNSET)
+        )
 
         mirrors = cast(List[str], d.pop("mirrors", UNSET))
 
         registry_service_config = cls(
             allow_nondistributable_artifacts_cid_rs=allow_nondistributable_artifacts_cid_rs,
             allow_nondistributable_artifacts_hostnames=allow_nondistributable_artifacts_hostnames,
             index_configs=index_configs,
```

### Comparing `kittycad-0.3.7/kittycad/models/runtime.py` & `kittycad-0.3.8/kittycad/models/runtime.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Runtime")
+S = TypeVar("S", bound="Runtime")
 
 
 @attr.s(auto_attribs=True)
 class Runtime:
-    """ """
+    """Runtime describes an [OCI compliant](https://github.com/opencontainers/runtime-spec) runtime.  The runtime is invoked by the daemon via the `containerd` daemon. OCI runtimes act as an interface to the Linux kernel namespaces, cgroups, and SELinux."""  # noqa: E501
+
     path: Union[Unset, str] = UNSET
     runtime_args: Union[Unset, List[str]] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         path = self.path
@@ -21,22 +22,22 @@
         if not isinstance(self.runtime_args, Unset):
             runtime_args = self.runtime_args
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if path is not UNSET:
-            field_dict['path'] = path
+            field_dict["path"] = path
         if runtime_args is not UNSET:
-            field_dict['runtime_args'] = runtime_args
+            field_dict["runtime_args"] = runtime_args
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
         d = src_dict.copy()
         path = d.pop("path", UNSET)
 
         runtime_args = cast(List[str], d.pop("runtime_args", UNSET))
 
         runtime = cls(
             path=path,
```

### Comparing `kittycad-0.3.7/kittycad/models/session.py` & `kittycad-0.3.8/kittycad/models/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Session")
+L = TypeVar("L", bound="Session")
 
 
 @attr.s(auto_attribs=True)
 class Session:
-    """ """
+    """An authentication session.
+
+    For our UIs, these are automatically created by Next.js."""  # noqa: E501
+
     created_at: Union[Unset, datetime.datetime] = UNSET
     expires: Union[Unset, datetime.datetime] = UNSET
     id: Union[Unset, str] = UNSET
     session_token: Union[Unset, str] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
@@ -36,30 +38,30 @@
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if expires is not UNSET:
-            field_dict['expires'] = expires
+            field_dict["expires"] = expires
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if session_token is not UNSET:
-            field_dict['session_token'] = session_token
+            field_dict["session_token"] = session_token
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_acceleration_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_acceleration_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_acceleration_format import UnitAccelerationFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_acceleration_format import UnitAccelerationFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitAccelerationConversion")
+E = TypeVar("E", bound="UnitAccelerationConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitAccelerationConversion:
-    """ """
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
     output_format: Union[Unset, UnitAccelerationFormat] = UNSET
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_angle_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_time_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_angle_format import UnitAngleFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_time_format import UnitTimeFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitAngleConversion")
+P = TypeVar("P", bound="UnitTimeConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitAngleConversion:
-    """ """
+class UnitTimeConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitAngleFormat] = UNSET
-    src_format: Union[Unset, UnitAngleFormat] = UNSET
+    output_format: Union[Unset, UnitTimeFormat] = UNSET
+    src_format: Union[Unset, UnitTimeFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitAngleFormat]
+        output_format: Union[Unset, UnitTimeFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitAngleFormat(_output_format)
+            output_format = UnitTimeFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitAngleFormat]
+        src_format: Union[Unset, UnitTimeFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitAngleFormat(_src_format)
+            src_format = UnitTimeFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_angle_conversion = cls(
+        unit_time_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_angle_conversion.additional_properties = d
-        return unit_angle_conversion
+        unit_time_conversion.additional_properties = d
+        return unit_time_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_angular_velocity_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_angular_velocity_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_angular_velocity_format import UnitAngularVelocityFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_angular_velocity_format import UnitAngularVelocityFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitAngularVelocityConversion")
+Y = TypeVar("Y", bound="UnitAngularVelocityConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitAngularVelocityConversion:
-    """ """
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
     output_format: Union[Unset, UnitAngularVelocityFormat] = UNSET
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_area_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_volume_conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_area_format import UnitAreaFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_volume_format import UnitVolumeFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitAreaConversion")
+K = TypeVar("K", bound="UnitVolumeConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitAreaConversion:
-    """ """
+class UnitVolumeConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitAreaFormat] = UNSET
-    src_format: Union[Unset, UnitAreaFormat] = UNSET
+    output_format: Union[Unset, UnitVolumeFormat] = UNSET
+    src_format: Union[Unset, UnitVolumeFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitAreaFormat]
+        output_format: Union[Unset, UnitVolumeFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitAreaFormat(_output_format)
+            output_format = UnitVolumeFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitAreaFormat]
+        src_format: Union[Unset, UnitVolumeFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitAreaFormat(_src_format)
+            src_format = UnitVolumeFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_area_conversion = cls(
+        unit_volume_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_area_conversion.additional_properties = d
-        return unit_area_conversion
+        unit_volume_conversion.additional_properties = d
+        return unit_volume_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_charge_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_charge_conversion.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_charge_format import UnitChargeFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_charge_format import UnitChargeFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitChargeConversion")
+D = TypeVar("D", bound="UnitChargeConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitChargeConversion:
-    """ """
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
     output_format: Union[Unset, UnitChargeFormat] = UNSET
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[D], src_dict: Dict[str, Any]) -> D:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_concentration_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_force_conversion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_concentration_format import UnitConcentrationFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_force_format import UnitForceFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitConcentrationConversion")
+N = TypeVar("N", bound="UnitForceConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitConcentrationConversion:
-    """ """
+class UnitForceConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitConcentrationFormat] = UNSET
-    src_format: Union[Unset, UnitConcentrationFormat] = UNSET
+    output_format: Union[Unset, UnitForceFormat] = UNSET
+    src_format: Union[Unset, UnitForceFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitConcentrationFormat]
+        output_format: Union[Unset, UnitForceFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitConcentrationFormat(_output_format)
+            output_format = UnitForceFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitConcentrationFormat]
+        src_format: Union[Unset, UnitForceFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitConcentrationFormat(_src_format)
+            src_format = UnitForceFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_concentration_conversion = cls(
+        unit_force_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_concentration_conversion.additional_properties = d
-        return unit_concentration_conversion
+        unit_force_conversion.additional_properties = d
+        return unit_force_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_data_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_voltage_conversion.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_data_format import UnitDataFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_voltage_format import UnitVoltageFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitDataConversion")
+L = TypeVar("L", bound="UnitVoltageConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitDataConversion:
-    """ """
+class UnitVoltageConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitDataFormat] = UNSET
-    src_format: Union[Unset, UnitDataFormat] = UNSET
+    output_format: Union[Unset, UnitVoltageFormat] = UNSET
+    src_format: Union[Unset, UnitVoltageFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitDataFormat]
+        output_format: Union[Unset, UnitVoltageFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitDataFormat(_output_format)
+            output_format = UnitVoltageFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitDataFormat]
+        src_format: Union[Unset, UnitVoltageFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitDataFormat(_src_format)
+            src_format = UnitVoltageFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_data_conversion = cls(
+        unit_voltage_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_data_conversion.additional_properties = d
-        return unit_data_conversion
+        unit_voltage_conversion.additional_properties = d
+        return unit_voltage_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_data_transfer_rate_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_data_transfer_rate_conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_data_transfer_rate_format import UnitDataTransferRateFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_data_transfer_rate_format import UnitDataTransferRateFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitDataTransferRateConversion")
+G = TypeVar("G", bound="UnitDataTransferRateConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitDataTransferRateConversion:
-    """ """
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
     output_format: Union[Unset, UnitDataTransferRateFormat] = UNSET
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[G], src_dict: Dict[str, Any]) -> G:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_density_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_velocity_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_density_format import UnitDensityFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_velocity_format import UnitVelocityFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitDensityConversion")
+Y = TypeVar("Y", bound="UnitVelocityConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitDensityConversion:
-    """ """
+class UnitVelocityConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitDensityFormat] = UNSET
-    src_format: Union[Unset, UnitDensityFormat] = UNSET
+    output_format: Union[Unset, UnitVelocityFormat] = UNSET
+    src_format: Union[Unset, UnitVelocityFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitDensityFormat]
+        output_format: Union[Unset, UnitVelocityFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitDensityFormat(_output_format)
+            output_format = UnitVelocityFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitDensityFormat]
+        src_format: Union[Unset, UnitVelocityFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitDensityFormat(_src_format)
+            src_format = UnitVelocityFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_density_conversion = cls(
+        unit_velocity_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_density_conversion.additional_properties = d
-        return unit_density_conversion
+        unit_velocity_conversion.additional_properties = d
+        return unit_velocity_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_energy_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_magnetic_flux_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_energy_format import UnitEnergyFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_magnetic_flux_format import UnitMagneticFluxFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitEnergyConversion")
+T = TypeVar("T", bound="UnitMagneticFluxConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitEnergyConversion:
-    """ """
+class UnitMagneticFluxConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitEnergyFormat] = UNSET
-    src_format: Union[Unset, UnitEnergyFormat] = UNSET
+    output_format: Union[Unset, UnitMagneticFluxFormat] = UNSET
+    src_format: Union[Unset, UnitMagneticFluxFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,58 +37,55 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitEnergyFormat]
+        output_format: Union[Unset, UnitMagneticFluxFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitEnergyFormat(_output_format)
+            output_format = UnitMagneticFluxFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitEnergyFormat]
+        src_format: Union[Unset, UnitMagneticFluxFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitEnergyFormat(_src_format)
+            src_format = UnitMagneticFluxFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_energy_conversion = cls(
+        unit_magnetic_flux_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_energy_conversion.additional_properties = d
-        return unit_energy_conversion
+        unit_magnetic_flux_conversion.additional_properties = d
+        return unit_magnetic_flux_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_force_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_illuminance_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_force_format import UnitForceFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_illuminance_format import UnitIlluminanceFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitForceConversion")
+H = TypeVar("H", bound="UnitIlluminanceConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitForceConversion:
-    """ """
+class UnitIlluminanceConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitForceFormat] = UNSET
-    src_format: Union[Unset, UnitForceFormat] = UNSET
+    output_format: Union[Unset, UnitIlluminanceFormat] = UNSET
+    src_format: Union[Unset, UnitIlluminanceFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitForceFormat]
+        output_format: Union[Unset, UnitIlluminanceFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitForceFormat(_output_format)
+            output_format = UnitIlluminanceFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitForceFormat]
+        src_format: Union[Unset, UnitIlluminanceFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitForceFormat(_src_format)
+            src_format = UnitIlluminanceFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_force_conversion = cls(
+        unit_illuminance_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_force_conversion.additional_properties = d
-        return unit_force_conversion
+        unit_illuminance_conversion.additional_properties = d
+        return unit_illuminance_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_illuminance_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_angle_conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_illuminance_format import UnitIlluminanceFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_angle_format import UnitAngleFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitIlluminanceConversion")
+D = TypeVar("D", bound="UnitAngleConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitIlluminanceConversion:
-    """ """
+class UnitAngleConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitIlluminanceFormat] = UNSET
-    src_format: Union[Unset, UnitIlluminanceFormat] = UNSET
+    output_format: Union[Unset, UnitAngleFormat] = UNSET
+    src_format: Union[Unset, UnitAngleFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[D], src_dict: Dict[str, Any]) -> D:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitIlluminanceFormat]
+        output_format: Union[Unset, UnitAngleFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitIlluminanceFormat(_output_format)
+            output_format = UnitAngleFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitIlluminanceFormat]
+        src_format: Union[Unset, UnitAngleFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitIlluminanceFormat(_src_format)
+            src_format = UnitAngleFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_illuminance_conversion = cls(
+        unit_angle_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_illuminance_conversion.additional_properties = d
-        return unit_illuminance_conversion
+        unit_angle_conversion.additional_properties = d
+        return unit_angle_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_length_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_mass_conversion.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_length_format import UnitLengthFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_mass_format import UnitMassFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitLengthConversion")
+Q = TypeVar("Q", bound="UnitMassConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitLengthConversion:
-    """ """
+class UnitMassConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitLengthFormat] = UNSET
-    src_format: Union[Unset, UnitLengthFormat] = UNSET
+    output_format: Union[Unset, UnitMassFormat] = UNSET
+    src_format: Union[Unset, UnitMassFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[Q], src_dict: Dict[str, Any]) -> Q:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitLengthFormat]
+        output_format: Union[Unset, UnitMassFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitLengthFormat(_output_format)
+            output_format = UnitMassFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitLengthFormat]
+        src_format: Union[Unset, UnitMassFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitLengthFormat(_src_format)
+            src_format = UnitMassFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_length_conversion = cls(
+        unit_mass_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_length_conversion.additional_properties = d
-        return unit_length_conversion
+        unit_mass_conversion.additional_properties = d
+        return unit_mass_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_magnetic_field_strength_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_metric_power_squared_conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_magnetic_field_strength_format import UnitMagneticFieldStrengthFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_metric_power import UnitMetricPower
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitMagneticFieldStrengthConversion")
+J = TypeVar("J", bound="UnitMetricPowerSquaredConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitMagneticFieldStrengthConversion:
-    """ """
+class UnitMetricPowerSquaredConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitMagneticFieldStrengthFormat] = UNSET
-    src_format: Union[Unset, UnitMagneticFieldStrengthFormat] = UNSET
+    output_format: Union[Unset, UnitMetricPower] = UNSET
+    src_format: Union[Unset, UnitMetricPower] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitMagneticFieldStrengthFormat]
+        output_format: Union[Unset, UnitMetricPower]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitMagneticFieldStrengthFormat(_output_format)
+            output_format = UnitMetricPower(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitMagneticFieldStrengthFormat]
+        src_format: Union[Unset, UnitMetricPower]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitMagneticFieldStrengthFormat(_src_format)
+            src_format = UnitMetricPower(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_magnetic_field_strength_conversion = cls(
+        unit_metric_power_squared_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_magnetic_field_strength_conversion.additional_properties = d
-        return unit_magnetic_field_strength_conversion
+        unit_metric_power_squared_conversion.additional_properties = d
+        return unit_metric_power_squared_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_magnetic_flux_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_solid_angle_conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_magnetic_flux_format import UnitMagneticFluxFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_solid_angle_format import UnitSolidAngleFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitMagneticFluxConversion")
+Y = TypeVar("Y", bound="UnitSolidAngleConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitMagneticFluxConversion:
-    """ """
+class UnitSolidAngleConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitMagneticFluxFormat] = UNSET
-    src_format: Union[Unset, UnitMagneticFluxFormat] = UNSET
+    output_format: Union[Unset, UnitSolidAngleFormat] = UNSET
+    src_format: Union[Unset, UnitSolidAngleFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitMagneticFluxFormat]
+        output_format: Union[Unset, UnitSolidAngleFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitMagneticFluxFormat(_output_format)
+            output_format = UnitSolidAngleFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitMagneticFluxFormat]
+        src_format: Union[Unset, UnitSolidAngleFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitMagneticFluxFormat(_src_format)
+            src_format = UnitSolidAngleFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_magnetic_flux_conversion = cls(
+        unit_solid_angle_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_magnetic_flux_conversion.additional_properties = d
-        return unit_magnetic_flux_conversion
+        unit_solid_angle_conversion.additional_properties = d
+        return unit_solid_angle_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_mass_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_pressure_conversion.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_mass_format import UnitMassFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_pressure_format import UnitPressureFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitMassConversion")
+V = TypeVar("V", bound="UnitPressureConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitMassConversion:
-    """ """
+class UnitPressureConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitMassFormat] = UNSET
-    src_format: Union[Unset, UnitMassFormat] = UNSET
+    output_format: Union[Unset, UnitPressureFormat] = UNSET
+    src_format: Union[Unset, UnitPressureFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitMassFormat]
+        output_format: Union[Unset, UnitPressureFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitMassFormat(_output_format)
+            output_format = UnitPressureFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitMassFormat]
+        src_format: Union[Unset, UnitPressureFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitMassFormat(_src_format)
+            src_format = UnitPressureFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_mass_conversion = cls(
+        unit_pressure_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_mass_conversion.additional_properties = d
-        return unit_mass_conversion
+        unit_pressure_conversion.additional_properties = d
+        return unit_pressure_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_metric_power_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_metric_power_cubed_conversion.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_metric_power import UnitMetricPower
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_metric_power import UnitMetricPower
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitMetricPowerConversion")
+D = TypeVar("D", bound="UnitMetricPowerCubedConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitMetricPowerConversion:
-    """ """
+class UnitMetricPowerCubedConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
     output_format: Union[Unset, UnitMetricPower] = UNSET
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[D], src_dict: Dict[str, Any]) -> D:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_metric_power_conversion = cls(
+        unit_metric_power_cubed_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_metric_power_conversion.additional_properties = d
-        return unit_metric_power_conversion
+        unit_metric_power_cubed_conversion.additional_properties = d
+        return unit_metric_power_cubed_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_metric_power_cubed_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_metric_power_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_metric_power import UnitMetricPower
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_metric_power import UnitMetricPower
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitMetricPowerCubedConversion")
+F = TypeVar("F", bound="UnitMetricPowerConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitMetricPowerCubedConversion:
-    """ """
+class UnitMetricPowerConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
     output_format: Union[Unset, UnitMetricPower] = UNSET
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_metric_power_cubed_conversion = cls(
+        unit_metric_power_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_metric_power_cubed_conversion.additional_properties = d
-        return unit_metric_power_cubed_conversion
+        unit_metric_power_conversion.additional_properties = d
+        return unit_metric_power_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_metric_power_squared_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_temperature_conversion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_metric_power import UnitMetricPower
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_temperature_format import UnitTemperatureFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitMetricPowerSquaredConversion")
+F = TypeVar("F", bound="UnitTemperatureConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitMetricPowerSquaredConversion:
-    """ """
+class UnitTemperatureConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitMetricPower] = UNSET
-    src_format: Union[Unset, UnitMetricPower] = UNSET
+    output_format: Union[Unset, UnitTemperatureFormat] = UNSET
+    src_format: Union[Unset, UnitTemperatureFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitMetricPower]
+        output_format: Union[Unset, UnitTemperatureFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitMetricPower(_output_format)
+            output_format = UnitTemperatureFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitMetricPower]
+        src_format: Union[Unset, UnitTemperatureFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitMetricPower(_src_format)
+            src_format = UnitTemperatureFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_metric_power_squared_conversion = cls(
+        unit_temperature_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_metric_power_squared_conversion.additional_properties = d
-        return unit_metric_power_squared_conversion
+        unit_temperature_conversion.additional_properties = d
+        return unit_temperature_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_power_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_power_conversion.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_power_format import UnitPowerFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_power_format import UnitPowerFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitPowerConversion")
+F = TypeVar("F", bound="UnitPowerConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitPowerConversion:
-    """ """
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
     output_format: Union[Unset, UnitPowerFormat] = UNSET
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_pressure_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_area_conversion.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_pressure_format import UnitPressureFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_area_format import UnitAreaFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitPressureConversion")
+Y = TypeVar("Y", bound="UnitAreaConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitPressureConversion:
-    """ """
+class UnitAreaConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitPressureFormat] = UNSET
-    src_format: Union[Unset, UnitPressureFormat] = UNSET
+    output_format: Union[Unset, UnitAreaFormat] = UNSET
+    src_format: Union[Unset, UnitAreaFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitPressureFormat]
+        output_format: Union[Unset, UnitAreaFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitPressureFormat(_output_format)
+            output_format = UnitAreaFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitPressureFormat]
+        src_format: Union[Unset, UnitAreaFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitPressureFormat(_src_format)
+            src_format = UnitAreaFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_pressure_conversion = cls(
+        unit_area_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_pressure_conversion.additional_properties = d
-        return unit_pressure_conversion
+        unit_area_conversion.additional_properties = d
+        return unit_area_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_radiation_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_length_conversion.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_radiation_format import UnitRadiationFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_length_format import UnitLengthFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitRadiationConversion")
+V = TypeVar("V", bound="UnitLengthConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitRadiationConversion:
-    """ """
+class UnitLengthConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitRadiationFormat] = UNSET
-    src_format: Union[Unset, UnitRadiationFormat] = UNSET
+    output_format: Union[Unset, UnitLengthFormat] = UNSET
+    src_format: Union[Unset, UnitLengthFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitRadiationFormat]
+        output_format: Union[Unset, UnitLengthFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitRadiationFormat(_output_format)
+            output_format = UnitLengthFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitRadiationFormat]
+        src_format: Union[Unset, UnitLengthFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitRadiationFormat(_src_format)
+            src_format = UnitLengthFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_radiation_conversion = cls(
+        unit_length_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_radiation_conversion.additional_properties = d
-        return unit_radiation_conversion
+        unit_length_conversion.additional_properties = d
+        return unit_length_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_radioactivity_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_radioactivity_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_radioactivity_format import UnitRadioactivityFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_radioactivity_format import UnitRadioactivityFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitRadioactivityConversion")
+F = TypeVar("F", bound="UnitRadioactivityConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitRadioactivityConversion:
-    """ """
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
     output_format: Union[Unset, UnitRadioactivityFormat] = UNSET
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_solid_angle_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_radiation_conversion.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_solid_angle_format import UnitSolidAngleFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_radiation_format import UnitRadiationFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitSolidAngleConversion")
+U = TypeVar("U", bound="UnitRadiationConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitSolidAngleConversion:
-    """ """
+class UnitRadiationConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitSolidAngleFormat] = UNSET
-    src_format: Union[Unset, UnitSolidAngleFormat] = UNSET
+    output_format: Union[Unset, UnitRadiationFormat] = UNSET
+    src_format: Union[Unset, UnitRadiationFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[U], src_dict: Dict[str, Any]) -> U:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitSolidAngleFormat]
+        output_format: Union[Unset, UnitRadiationFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitSolidAngleFormat(_output_format)
+            output_format = UnitRadiationFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitSolidAngleFormat]
+        src_format: Union[Unset, UnitRadiationFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitSolidAngleFormat(_src_format)
+            src_format = UnitRadiationFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_solid_angle_conversion = cls(
+        unit_radiation_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_solid_angle_conversion.additional_properties = d
-        return unit_solid_angle_conversion
+        unit_radiation_conversion.additional_properties = d
+        return unit_radiation_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_temperature_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_energy_conversion.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_temperature_format import UnitTemperatureFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_energy_format import UnitEnergyFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitTemperatureConversion")
+N = TypeVar("N", bound="UnitEnergyConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitTemperatureConversion:
-    """ """
+class UnitEnergyConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitTemperatureFormat] = UNSET
-    src_format: Union[Unset, UnitTemperatureFormat] = UNSET
+    output_format: Union[Unset, UnitEnergyFormat] = UNSET
+    src_format: Union[Unset, UnitEnergyFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitTemperatureFormat]
+        output_format: Union[Unset, UnitEnergyFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitTemperatureFormat(_output_format)
+            output_format = UnitEnergyFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitTemperatureFormat]
+        src_format: Union[Unset, UnitEnergyFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitTemperatureFormat(_src_format)
+            src_format = UnitEnergyFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_temperature_conversion = cls(
+        unit_energy_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_temperature_conversion.additional_properties = d
-        return unit_temperature_conversion
+        unit_energy_conversion.additional_properties = d
+        return unit_energy_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_time_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_density_conversion.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_time_format import UnitTimeFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_density_format import UnitDensityFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitTimeConversion")
+L = TypeVar("L", bound="UnitDensityConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitTimeConversion:
-    """ """
+class UnitDensityConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitTimeFormat] = UNSET
-    src_format: Union[Unset, UnitTimeFormat] = UNSET
+    output_format: Union[Unset, UnitDensityFormat] = UNSET
+    src_format: Union[Unset, UnitDensityFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitTimeFormat]
+        output_format: Union[Unset, UnitDensityFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitTimeFormat(_output_format)
+            output_format = UnitDensityFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitTimeFormat]
+        src_format: Union[Unset, UnitDensityFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitTimeFormat(_src_format)
+            src_format = UnitDensityFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_time_conversion = cls(
+        unit_density_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_time_conversion.additional_properties = d
-        return unit_time_conversion
+        unit_density_conversion.additional_properties = d
+        return unit_density_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/unit_velocity_conversion.py` & `kittycad-0.3.8/kittycad/models/unit_magnetic_field_strength_conversion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.uuid import Uuid
-from ..models.unit_velocity_format import UnitVelocityFormat
 from ..models.api_call_status import ApiCallStatus
+from ..models.unit_magnetic_field_strength_format import UnitMagneticFieldStrengthFormat
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitVelocityConversion")
+E = TypeVar("E", bound="UnitMagneticFieldStrengthConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitVelocityConversion:
-    """ """
+class UnitMagneticFieldStrengthConversion:
+    """A unit conversion."""  # noqa: E501
+
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitVelocityFormat] = UNSET
-    src_format: Union[Unset, UnitVelocityFormat] = UNSET
+    output_format: Union[Unset, UnitMagneticFieldStrengthFormat] = UNSET
+    src_format: Union[Unset, UnitMagneticFieldStrengthFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -37,63 +37,60 @@
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         input = self.input
         output = self.output
-        output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
-            output_format = self.output_format.value
-        src_format: Union[Unset, str] = UNSET
+            output_format = self.output_format
         if not isinstance(self.src_format, Unset):
-            src_format = self.src_format.value
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
-        status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
-            field_dict['completed_at'] = completed_at
+            field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if error is not UNSET:
-            field_dict['error'] = error
+            field_dict["error"] = error
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if input is not UNSET:
-            field_dict['input'] = input
+            field_dict["input"] = input
         if output is not UNSET:
-            field_dict['output'] = output
+            field_dict["output"] = output
         if output_format is not UNSET:
-            field_dict['output_format'] = output_format
+            field_dict["output_format"] = output_format
         if src_format is not UNSET:
-            field_dict['src_format'] = src_format
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
-            field_dict['started_at'] = started_at
+            field_dict["started_at"] = started_at
         if status is not UNSET:
-            field_dict['status'] = status
+            field_dict["status"] = status
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
-            field_dict['user_id'] = user_id
+            field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -110,26 +107,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitVelocityFormat]
+        output_format: Union[Unset, UnitMagneticFieldStrengthFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitVelocityFormat(_output_format)
+            output_format = UnitMagneticFieldStrengthFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitVelocityFormat]
+        src_format: Union[Unset, UnitMagneticFieldStrengthFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitVelocityFormat(_src_format)
+            src_format = UnitMagneticFieldStrengthFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +143,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_velocity_conversion = cls(
+        unit_magnetic_field_strength_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_velocity_conversion.additional_properties = d
-        return unit_velocity_conversion
+        unit_magnetic_field_strength_conversion.additional_properties = d
+        return unit_magnetic_field_strength_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/update_user.py` & `kittycad-0.3.8/kittycad/models/update_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UpdateUser")
+N = TypeVar("N", bound="UpdateUser")
 
 
 @attr.s(auto_attribs=True)
 class UpdateUser:
-    """ """
+    """The user-modifiable parts of a User."""  # noqa: E501
+
     company: Union[Unset, str] = UNSET
     discord: Union[Unset, str] = UNSET
     first_name: Union[Unset, str] = UNSET
     github: Union[Unset, str] = UNSET
     last_name: Union[Unset, str] = UNSET
     phone: Union[Unset, str] = UNSET
 
@@ -27,30 +28,30 @@
         last_name = self.last_name
         phone = self.phone
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if company is not UNSET:
-            field_dict['company'] = company
+            field_dict["company"] = company
         if discord is not UNSET:
-            field_dict['discord'] = discord
+            field_dict["discord"] = discord
         if first_name is not UNSET:
-            field_dict['first_name'] = first_name
+            field_dict["first_name"] = first_name
         if github is not UNSET:
-            field_dict['github'] = github
+            field_dict["github"] = github
         if last_name is not UNSET:
-            field_dict['last_name'] = last_name
+            field_dict["last_name"] = last_name
         if phone is not UNSET:
-            field_dict['phone'] = phone
+            field_dict["phone"] = phone
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         company = d.pop("company", UNSET)
 
         discord = d.pop("discord", UNSET)
 
         first_name = d.pop("first_name", UNSET)
```

### Comparing `kittycad-0.3.7/kittycad/models/user.py` & `kittycad-0.3.8/kittycad/models/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="User")
+H = TypeVar("H", bound="User")
 
 
 @attr.s(auto_attribs=True)
 class User:
-    """ """
+    """A user."""  # noqa: E501
+
     company: Union[Unset, str] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     discord: Union[Unset, str] = UNSET
     email: Union[Unset, str] = UNSET
     email_verified: Union[Unset, datetime.datetime] = UNSET
     first_name: Union[Unset, str] = UNSET
     github: Union[Unset, str] = UNSET
@@ -49,44 +50,44 @@
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if company is not UNSET:
-            field_dict['company'] = company
+            field_dict["company"] = company
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if discord is not UNSET:
-            field_dict['discord'] = discord
+            field_dict["discord"] = discord
         if email is not UNSET:
-            field_dict['email'] = email
+            field_dict["email"] = email
         if email_verified is not UNSET:
-            field_dict['email_verified'] = email_verified
+            field_dict["email_verified"] = email_verified
         if first_name is not UNSET:
-            field_dict['first_name'] = first_name
+            field_dict["first_name"] = first_name
         if github is not UNSET:
-            field_dict['github'] = github
+            field_dict["github"] = github
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if image is not UNSET:
-            field_dict['image'] = image
+            field_dict["image"] = image
         if last_name is not UNSET:
-            field_dict['last_name'] = last_name
+            field_dict["last_name"] = last_name
         if name is not UNSET:
-            field_dict['name'] = name
+            field_dict["name"] = name
         if phone is not UNSET:
-            field_dict['phone'] = phone
+            field_dict["phone"] = phone
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         company = d.pop("company", UNSET)
 
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
```

### Comparing `kittycad-0.3.7/kittycad/models/user_results_page.py` & `kittycad-0.3.8/kittycad/models/app_client_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,46 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UserResultsPage")
+U = TypeVar("U", bound="AppClientInfo")
 
 
 @attr.s(auto_attribs=True)
-class UserResultsPage:
-    """ """
-    from ..models.user import User
-    items: Union[Unset, List[User]] = UNSET
-    next_page: Union[Unset, str] = UNSET
+class AppClientInfo:
+    """Information about a third party app client."""  # noqa: E501
+
+    url: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        from ..models.user import User
-        items: Union[Unset, List[User]] = UNSET
-        if not isinstance(self.items, Unset):
-            items = self.items
-        next_page = self.next_page
+        url = self.url
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if items is not UNSET:
-            field_dict['items'] = items
-        if next_page is not UNSET:
-            field_dict['next_page'] = next_page
+        if url is not UNSET:
+            field_dict["url"] = url
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[U], src_dict: Dict[str, Any]) -> U:
         d = src_dict.copy()
-        from ..models.user import User
-        items = cast(List[User], d.pop("items", UNSET))
-
-        next_page = d.pop("next_page", UNSET)
+        url = d.pop("url", UNSET)
 
-        user_results_page = cls(
-            items=items,
-            next_page=next_page,
+        app_client_info = cls(
+            url=url,
         )
 
-        user_results_page.additional_properties = d
-        return user_results_page
+        app_client_info.additional_properties = d
+        return app_client_info
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.7/kittycad/models/verification_token.py` & `kittycad-0.3.8/kittycad/models/verification_token.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="VerificationToken")
+R = TypeVar("R", bound="VerificationToken")
 
 
 @attr.s(auto_attribs=True)
 class VerificationToken:
-    """ """
+    """A verification token for a user.
+
+    This is typically used to verify a user's email address."""  # noqa: E501
+
     created_at: Union[Unset, datetime.datetime] = UNSET
     expires: Union[Unset, datetime.datetime] = UNSET
     id: Union[Unset, str] = UNSET
     identifier: Union[Unset, str] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -33,28 +36,28 @@
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if created_at is not UNSET:
-            field_dict['created_at'] = created_at
+            field_dict["created_at"] = created_at
         if expires is not UNSET:
-            field_dict['expires'] = expires
+            field_dict["expires"] = expires
         if id is not UNSET:
-            field_dict['id'] = id
+            field_dict["id"] = id
         if identifier is not UNSET:
-            field_dict['identifier'] = identifier
+            field_dict["identifier"] = identifier
         if updated_at is not UNSET:
-            field_dict['updated_at'] = updated_at
+            field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
         d = src_dict.copy()
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
```

### Comparing `kittycad-0.3.7/kittycad/types.py` & `kittycad-0.3.8/kittycad/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 """ Contains some shared types for properties """
-from typing import BinaryIO, Generic, MutableMapping, Optional, TextIO, Tuple, TypeVar, Union
+from typing import (
+    BinaryIO,
+    Generic,
+    MutableMapping,
+    Optional,
+    TextIO,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 import attr
 
 
 class Unset:
     def __bool__(self) -> bool:
         return False
@@ -19,24 +28,24 @@
     """Contains information for file uploads"""
 
     payload: Union[BinaryIO, TextIO]
     file_name: Optional[str] = None
     mime_type: Optional[str] = None
 
     def to_tuple(self) -> FileJsonType:
-        """Return a tuple representation that httpx will accept for multipart/form-data"""
+        """Return a tuple representation that httpx will accept for multipart/form-data"""  # noqa: E501
         return self.file_name, self.payload, self.mime_type
 
 
 T = TypeVar("T")
 
 
 @attr.s(auto_attribs=True)
 class Response(Generic[T]):
-    """A response from an endpoint"""
+    """A response from an endpoint"""  # noqa: E501
 
     status_code: int
     content: bytes
     headers: MutableMapping[str, str]
     parsed: Optional[T]
```

### Comparing `kittycad-0.3.7/PKG-INFO` & `kittycad-0.3.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: kittycad
-Version: 0.3.7
+Version: 0.3.8
 Summary: A client library for accessing KittyCAD
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=20.1.0,<24.0.0)
 Requires-Dist: httpx (>=0.15.4,<0.25.0)
 Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
```

