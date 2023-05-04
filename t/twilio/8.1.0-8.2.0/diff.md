# Comparing `tmp/twilio-8.1.0.tar.gz` & `tmp/twilio-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twilio-8.1.0.tar", last modified: Thu Apr 20 07:29:22 2023, max compression
+gzip compressed data, was "twilio-8.2.0.tar", last modified: Thu May  4 09:30:45 2023, max compression
```

## Comparing `twilio-8.1.0.tar` & `twilio-8.2.0.tar`

### file list

```diff
@@ -1,852 +1,851 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.091783 twilio-8.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-20 07:29:07.000000 twilio-8.1.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-20 07:29:07.000000 twilio-8.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-20 07:29:07.000000 twilio-8.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-04-20 07:29:22.091783 twilio-8.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-04-20 07:29:07.000000 twilio-8.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-20 07:29:22.091783 twilio-8.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1694 2023-04-20 07:29:07.000000 twilio-8.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.975781 twilio-8.1.0/twilio/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.979781 twilio-8.1.0/twilio/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/base/client_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/base/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/base/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/base/instance_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/base/instance_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/base/list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/base/obsolete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/base/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/base/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/base/values.py
--rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/base/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.979781 twilio-8.1.0/twilio/http/
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/http/async_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/http/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/http/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/http/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/http/validation_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.979781 twilio-8.1.0/twilio/jwt/
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/jwt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.979781 twilio-8.1.0/twilio/jwt/access_token/
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/jwt/access_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/jwt/access_token/grants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.979781 twilio-8.1.0/twilio/jwt/client/
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/jwt/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.979781 twilio-8.1.0/twilio/jwt/taskrouter/
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/jwt/taskrouter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/jwt/taskrouter/capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.979781 twilio-8.1.0/twilio/jwt/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/jwt/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/request_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.979781 twilio-8.1.0/twilio/rest/
--rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.979781 twilio-8.1.0/twilio/rest/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/accounts/AccountsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.979781 twilio-8.1.0/twilio/rest/accounts/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/accounts/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/accounts/v1/auth_token_promotion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.983781 twilio-8.1.0/twilio/rest/accounts/v1/credential/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/accounts/v1/credential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19489 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/accounts/v1/credential/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    20007 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/accounts/v1/credential/public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/accounts/v1/secondary_auth_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.983781 twilio-8.1.0/twilio/rest/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/ApiBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.983781 twilio-8.1.0/twilio/rest/api/v2010/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.983781 twilio-8.1.0/twilio/rest/api/v2010/account/
--rw-r--r--   0 runner    (1001) docker     (123)    36206 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.987781 twilio-8.1.0/twilio/rest/api/v2010/account/address/
--rw-r--r--   0 runner    (1001) docker     (123)    35858 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    47553 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/authorized_connect_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.987781 twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/
--rw-r--r--   0 runner    (1001) docker     (123)    21427 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46239 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    46210 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)    45860 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py
--rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py
--rw-r--r--   0 runner    (1001) docker     (123)    46000 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py
--rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py
--rw-r--r--   0 runner    (1001) docker     (123)    45790 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/balance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.991781 twilio-8.1.0/twilio/rest/api/v2010/account/call/
--rw-r--r--   0 runner    (1001) docker     (123)    92392 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/call/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/call/feedback.py
--rw-r--r--   0 runner    (1001) docker     (123)    13986 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/call/feedback_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    28363 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/call/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    23472 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/call/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)    38495 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/call/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)    77226 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/call/siprec.py
--rw-r--r--   0 runner    (1001) docker     (123)    77116 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/call/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/call/user_defined_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.991781 twilio-8.1.0/twilio/rest/api/v2010/account/conference/
--rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/conference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    74737 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/conference/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    32729 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/conference/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)    26539 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/connect_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.991781 twilio-8.1.0/twilio/rest/api/v2010/account/incoming_phone_number/
--rw-r--r--   0 runner    (1001) docker     (123)    73374 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.991781 twilio-8.1.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/
--rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18341 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    36935 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    37019 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py
--rw-r--r--   0 runner    (1001) docker     (123)    37103 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py
--rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.991781 twilio-8.1.0/twilio/rest/api/v2010/account/message/
--rw-r--r--   0 runner    (1001) docker     (123)    53984 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/message/feedback.py
--rw-r--r--   0 runner    (1001) docker     (123)    27246 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/message/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/new_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/new_signing_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    27505 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    22199 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/outgoing_caller_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.991781 twilio-8.1.0/twilio/rest/api/v2010/account/queue/
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19131 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/queue/member.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.991781 twilio-8.1.0/twilio/rest/api/v2010/account/recording/
--rw-r--r--   0 runner    (1001) docker     (123)    37769 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/recording/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.995781 twilio-8.1.0/twilio/rest/api/v2010/account/recording/add_on_result/
--rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19233 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/recording/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)    26406 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/short_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/signing_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.995781 twilio-8.1.0/twilio/rest/api/v2010/account/sip/
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/sip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.995781 twilio-8.1.0/twilio/rest/api/v2010/account/sip/credential_list/
--rw-r--r--   0 runner    (1001) docker     (123)    21278 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22757 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.995781 twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/
--rw-r--r--   0 runner    (1001) docker     (123)    45116 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.995781 twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.995781 twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.995781 twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21048 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.995781 twilio-8.1.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/
--rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26238 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/transcription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.995781 twilio-8.1.0/twilio/rest/api/v2010/account/usage/
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/usage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.999781 twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/
--rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/all_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/daily.py
--rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/last_month.py
--rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/monthly.py
--rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/this_month.py
--rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/today.py
--rw-r--r--   0 runner    (1001) docker     (123)    38293 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/yearly.py
--rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/yesterday.py
--rw-r--r--   0 runner    (1001) docker     (123)    49245 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/usage/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/api/v2010/account/validation_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.999781 twilio-8.1.0/twilio/rest/autopilot/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/AutopilotBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.999781 twilio-8.1.0/twilio/rest/autopilot/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.999781 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)    35087 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/dialogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.999781 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/field_type/
--rw-r--r--   0 runner    (1001) docker     (123)    23752 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/field_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/field_type/field_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    22851 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/model_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    29877 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/style_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.003781 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/task/
--rw-r--r--   0 runner    (1001) docker     (123)    28213 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/task/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    27891 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/task/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/task/task_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/task/task_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    24728 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/assistant/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/autopilot/v1/restore_assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.003781 twilio-8.1.0/twilio/rest/bulkexports/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/bulkexports/BulkexportsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/bulkexports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.003781 twilio-8.1.0/twilio/rest/bulkexports/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/bulkexports/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.003781 twilio-8.1.0/twilio/rest/bulkexports/v1/export/
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/bulkexports/v1/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/bulkexports/v1/export/day.py
--rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/bulkexports/v1/export/export_custom_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/bulkexports/v1/export/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/bulkexports/v1/export_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.003781 twilio-8.1.0/twilio/rest/chat/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.003781 twilio-8.1.0/twilio/rest/chat/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27856 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v1/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.003781 twilio-8.1.0/twilio/rest/chat/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    92674 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.003781 twilio-8.1.0/twilio/rest/chat/v1/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    28967 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v1/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v1/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v1/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    26356 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v1/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    21831 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v1/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.007781 twilio-8.1.0/twilio/rest/chat/v1/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    26317 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v1/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v1/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.007781 twilio-8.1.0/twilio/rest/chat/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27486 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v2/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.007781 twilio-8.1.0/twilio/rest/chat/v2/service/
--rw-r--r--   0 runner    (1001) docker     (123)    66570 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22118 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v2/service/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.007781 twilio-8.1.0/twilio/rest/chat/v2/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    39123 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v2/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22292 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v2/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v2/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    37545 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v2/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    33770 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v2/service/channel/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v2/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.007781 twilio-8.1.0/twilio/rest/chat/v2/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    29035 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v2/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v2/service/user/user_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    27050 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v2/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.007781 twilio-8.1.0/twilio/rest/chat/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/chat/v3/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.007781 twilio-8.1.0/twilio/rest/content/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/content/ContentBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/content/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.011782 twilio-8.1.0/twilio/rest/content/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/content/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.011782 twilio-8.1.0/twilio/rest/content/v1/content/
--rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/content/v1/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/content/v1/content/approval_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/content/v1/content_and_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/content/v1/legacy_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.011782 twilio-8.1.0/twilio/rest/conversations/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/ConversationsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.011782 twilio-8.1.0/twilio/rest/conversations/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36854 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/address_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.011782 twilio-8.1.0/twilio/rest/conversations/v1/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/configuration/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.011782 twilio-8.1.0/twilio/rest/conversations/v1/conversation/
--rw-r--r--   0 runner    (1001) docker     (123)    42957 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/conversation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.011782 twilio-8.1.0/twilio/rest/conversations/v1/conversation/message/
--rw-r--r--   0 runner    (1001) docker     (123)    34972 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/conversation/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)    40116 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/conversation/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    27236 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/conversation/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    27935 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/participant_conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20943 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.011782 twilio-8.1.0/twilio/rest/conversations/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22289 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/service/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.015781 twilio-8.1.0/twilio/rest/conversations/v1/service/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/service/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24410 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/service/configuration/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/service/configuration/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.015781 twilio-8.1.0/twilio/rest/conversations/v1/service/conversation/
--rw-r--r--   0 runner    (1001) docker     (123)    44808 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/service/conversation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.015781 twilio-8.1.0/twilio/rest/conversations/v1/service/conversation/message/
--rw-r--r--   0 runner    (1001) docker     (123)    36629 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/service/conversation/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    28926 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/service/conversation/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/service/participant_conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22534 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.015781 twilio-8.1.0/twilio/rest/conversations/v1/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    29682 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26510 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/service/user/user_conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.015781 twilio-8.1.0/twilio/rest/conversations/v1/user/
--rw-r--r--   0 runner    (1001) docker     (123)    28016 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25215 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/conversations/v1/user/user_conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.015781 twilio-8.1.0/twilio/rest/events/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/events/EventsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.015781 twilio-8.1.0/twilio/rest/events/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/events/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15317 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/events/v1/event_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.015781 twilio-8.1.0/twilio/rest/events/v1/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/events/v1/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/events/v1/schema/schema_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.019782 twilio-8.1.0/twilio/rest/events/v1/sink/
--rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/events/v1/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/events/v1/sink/sink_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/events/v1/sink/sink_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.019782 twilio-8.1.0/twilio/rest/events/v1/subscription/
--rw-r--r--   0 runner    (1001) docker     (123)    22609 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/events/v1/subscription/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/events/v1/subscription/subscribed_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.019782 twilio-8.1.0/twilio/rest/flex_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/FlexApiBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.019782 twilio-8.1.0/twilio/rest/flex_api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23338 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/assessments.py
--rw-r--r--   0 runner    (1001) docker     (123)    19793 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    46860 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/flex_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/insights_assessments_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/insights_conversations.py
--rw-r--r--   0 runner    (1001) docker     (123)    26467 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/insights_questionnaires.py
--rw-r--r--   0 runner    (1001) docker     (123)    20324 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py
--rw-r--r--   0 runner    (1001) docker     (123)    25940 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py
--rw-r--r--   0 runner    (1001) docker     (123)    19100 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/insights_segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/insights_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/insights_settings_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/insights_user_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.019782 twilio-8.1.0/twilio/rest/flex_api/v1/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/interaction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.023782 twilio-8.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v1/web_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.023782 twilio-8.1.0/twilio/rest/flex_api/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/flex_api/v2/web_channels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.023782 twilio-8.1.0/twilio/rest/frontline_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/frontline_api/FrontlineApiBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/frontline_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.023782 twilio-8.1.0/twilio/rest/frontline_api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/frontline_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/frontline_api/v1/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.023782 twilio-8.1.0/twilio/rest/insights/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/insights/InsightsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/insights/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.023782 twilio-8.1.0/twilio/rest/insights/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/insights/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.023782 twilio-8.1.0/twilio/rest/insights/v1/call/
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/insights/v1/call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/insights/v1/call/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/insights/v1/call/call_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/insights/v1/call/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/insights/v1/call/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    28813 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/insights/v1/call_summaries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.023782 twilio-8.1.0/twilio/rest/insights/v1/conference/
--rw-r--r--   0 runner    (1001) docker     (123)    31370 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/insights/v1/conference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/insights/v1/conference/conference_participant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.023782 twilio-8.1.0/twilio/rest/insights/v1/room/
--rw-r--r--   0 runner    (1001) docker     (123)    25243 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/insights/v1/room/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17908 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/insights/v1/room/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/insights/v1/setting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.027782 twilio-8.1.0/twilio/rest/ip_messaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/IpMessagingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.027782 twilio-8.1.0/twilio/rest/ip_messaging/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v1/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.027782 twilio-8.1.0/twilio/rest/ip_messaging/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    62960 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.027782 twilio-8.1.0/twilio/rest/ip_messaging/v1/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    24064 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v1/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    21725 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v1/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v1/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v1/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.027782 twilio-8.1.0/twilio/rest/ip_messaging/v1/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v1/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.027782 twilio-8.1.0/twilio/rest/ip_messaging/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v2/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.027782 twilio-8.1.0/twilio/rest/ip_messaging/v2/service/
--rw-r--r--   0 runner    (1001) docker     (123)    45390 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v2/service/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.031782 twilio-8.1.0/twilio/rest/ip_messaging/v2/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v2/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    29520 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v2/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    28798 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v2/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v2/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.031782 twilio-8.1.0/twilio/rest/ip_messaging/v2/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    24051 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v2/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    21476 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.031782 twilio-8.1.0/twilio/rest/lookups/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/lookups/LookupsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/lookups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.031782 twilio-8.1.0/twilio/rest/lookups/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/lookups/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/lookups/v1/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.031782 twilio-8.1.0/twilio/rest/lookups/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/lookups/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20961 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/lookups/v2/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.031782 twilio-8.1.0/twilio/rest/media/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/media/MediaBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/media/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.031782 twilio-8.1.0/twilio/rest/media/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/media/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26533 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/media/v1/media_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/media/v1/media_recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.031782 twilio-8.1.0/twilio/rest/media/v1/player_streamer/
--rw-r--r--   0 runner    (1001) docker     (123)    25414 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/media/v1/player_streamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/media/v1/player_streamer/playback_grant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.031782 twilio-8.1.0/twilio/rest/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/MessagingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.035782 twilio-8.1.0/twilio/rest/messaging/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.035782 twilio-8.1.0/twilio/rest/messaging/v1/brand_registration/
--rw-r--r--   0 runner    (1001) docker     (123)    24289 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/brand_registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19914 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/deactivations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/domain_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/domain_config_messaging_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/external_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.035782 twilio-8.1.0/twilio/rest/messaging/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    54653 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/service/alpha_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/service/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/service/short_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    33395 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/service/us_app_to_person.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py
--rw-r--r--   0 runner    (1001) docker     (123)    55732 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/tollfree_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/messaging/v1/usecase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.035782 twilio-8.1.0/twilio/rest/microvisor/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/microvisor/MicrovisorBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/microvisor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.035782 twilio-8.1.0/twilio/rest/microvisor/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/microvisor/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/microvisor/v1/account_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/microvisor/v1/account_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.039782 twilio-8.1.0/twilio/rest/microvisor/v1/app/
--rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/microvisor/v1/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/microvisor/v1/app/app_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.039782 twilio-8.1.0/twilio/rest/microvisor/v1/device/
--rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/microvisor/v1/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/microvisor/v1/device/device_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/microvisor/v1/device/device_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.039782 twilio-8.1.0/twilio/rest/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/monitor/MonitorBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.039782 twilio-8.1.0/twilio/rest/monitor/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/monitor/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22723 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/monitor/v1/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    25437 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/monitor/v1/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.039782 twilio-8.1.0/twilio/rest/notify/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/notify/NotifyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/notify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.039782 twilio-8.1.0/twilio/rest/notify/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/notify/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/notify/v1/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.039782 twilio-8.1.0/twilio/rest/notify/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    47060 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/notify/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/notify/v1/service/binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    25490 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/notify/v1/service/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.039782 twilio-8.1.0/twilio/rest/numbers/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/numbers/NumbersBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/numbers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.039782 twilio-8.1.0/twilio/rest/numbers/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/numbers/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.043782 twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.043782 twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/
--rw-r--r--   0 runner    (1001) docker     (123)    47502 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py
--rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.043782 twilio-8.1.0/twilio/rest/oauth/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/oauth/OauthBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/oauth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.043782 twilio-8.1.0/twilio/rest/oauth/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/oauth/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/oauth/v1/device_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/oauth/v1/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/oauth/v1/openid_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/oauth/v1/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/oauth/v1/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.043782 twilio-8.1.0/twilio/rest/preview/
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/PreviewBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.043782 twilio-8.1.0/twilio/rest/preview/deployed_devices/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/deployed_devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.047782 twilio-8.1.0/twilio/rest/preview/deployed_devices/fleet/
--rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/deployed_devices/fleet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24118 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/deployed_devices/fleet/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    22163 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/deployed_devices/fleet/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    26656 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/deployed_devices/fleet/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/deployed_devices/fleet/key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.047782 twilio-8.1.0/twilio/rest/preview/hosted_numbers/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/hosted_numbers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.047782 twilio-8.1.0/twilio/rest/preview/hosted_numbers/authorization_document/
--rw-r--r--   0 runner    (1001) docker     (123)    32009 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24829 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    48143 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.047782 twilio-8.1.0/twilio/rest/preview/marketplace/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/marketplace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.047782 twilio-8.1.0/twilio/rest/preview/marketplace/available_add_on/
--rw-r--r--   0 runner    (1001) docker     (123)    15067 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/marketplace/available_add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.047782 twilio-8.1.0/twilio/rest/preview/marketplace/installed_add_on/
--rw-r--r--   0 runner    (1001) docker     (123)    23293 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.047782 twilio-8.1.0/twilio/rest/preview/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.047782 twilio-8.1.0/twilio/rest/preview/sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/sync/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.047782 twilio-8.1.0/twilio/rest/preview/sync/service/document/
--rw-r--r--   0 runner    (1001) docker     (123)    20547 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/sync/service/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/sync/service/document/document_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.047782 twilio-8.1.0/twilio/rest/preview/sync/service/sync_list/
--rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/sync/service/sync_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.051782 twilio-8.1.0/twilio/rest/preview/sync/service/sync_map/
--rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/sync/service/sync_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24063 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21250 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.051782 twilio-8.1.0/twilio/rest/preview/understand/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/understand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.051782 twilio-8.1.0/twilio/rest/preview/understand/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/understand/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/understand/assistant/dialogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.051782 twilio-8.1.0/twilio/rest/preview/understand/assistant/field_type/
--rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/understand/assistant/field_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20410 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/understand/assistant/field_type/field_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/understand/assistant/model_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/understand/assistant/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/understand/assistant/style_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.051782 twilio-8.1.0/twilio/rest/preview/understand/assistant/task/
--rw-r--r--   0 runner    (1001) docker     (123)    26813 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/understand/assistant/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/understand/assistant/task/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/understand/assistant/task/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/understand/assistant/task/task_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/understand/assistant/task/task_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.051782 twilio-8.1.0/twilio/rest/preview/wireless/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/wireless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/wireless/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/wireless/rate_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.051782 twilio-8.1.0/twilio/rest/preview/wireless/sim/
--rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/wireless/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/preview/wireless/sim/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.055782 twilio-8.1.0/twilio/rest/pricing/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/PricingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.055782 twilio-8.1.0/twilio/rest/pricing/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.055782 twilio-8.1.0/twilio/rest/pricing/v1/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/v1/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/v1/messaging/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.055782 twilio-8.1.0/twilio/rest/pricing/v1/phone_number/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/v1/phone_number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/v1/phone_number/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.055782 twilio-8.1.0/twilio/rest/pricing/v1/voice/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/v1/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/v1/voice/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/v1/voice/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.055782 twilio-8.1.0/twilio/rest/pricing/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/v2/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/v2/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.055782 twilio-8.1.0/twilio/rest/pricing/v2/voice/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/v2/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/v2/voice/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/pricing/v2/voice/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.055782 twilio-8.1.0/twilio/rest/proxy/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/proxy/ProxyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.055782 twilio-8.1.0/twilio/rest/proxy/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/proxy/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.055782 twilio-8.1.0/twilio/rest/proxy/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    38044 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/proxy/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23754 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/proxy/v1/service/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.059782 twilio-8.1.0/twilio/rest/proxy/v1/service/session/
--rw-r--r--   0 runner    (1001) docker     (123)    27767 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/proxy/v1/service/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/proxy/v1/service/session/interaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.059782 twilio-8.1.0/twilio/rest/proxy/v1/service/session/participant/
--rw-r--r--   0 runner    (1001) docker     (123)    22765 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/proxy/v1/service/session/participant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23242 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    21333 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/proxy/v1/service/short_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.059782 twilio-8.1.0/twilio/rest/routes/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/routes/RoutesBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.059782 twilio-8.1.0/twilio/rest/routes/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/routes/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/routes/v2/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/routes/v2/sip_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/routes/v2/trunk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.059782 twilio-8.1.0/twilio/rest/serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/serverless/ServerlessBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.059782 twilio-8.1.0/twilio/rest/serverless/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/serverless/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.059782 twilio-8.1.0/twilio/rest/serverless/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/serverless/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.059782 twilio-8.1.0/twilio/rest/serverless/v1/service/asset/
--rw-r--r--   0 runner    (1001) docker     (123)    20582 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/serverless/v1/service/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/serverless/v1/service/asset/asset_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.059782 twilio-8.1.0/twilio/rest/serverless/v1/service/build/
--rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/serverless/v1/service/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/serverless/v1/service/build/build_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.059782 twilio-8.1.0/twilio/rest/serverless/v1/service/environment/
--rw-r--r--   0 runner    (1001) docker     (123)    21009 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/serverless/v1/service/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/serverless/v1/service/environment/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    20926 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/serverless/v1/service/environment/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/serverless/v1/service/environment/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.063783 twilio-8.1.0/twilio/rest/serverless/v1/service/function/
--rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/serverless/v1/service/function/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.063783 twilio-8.1.0/twilio/rest/serverless/v1/service/function/function_version/
--rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.063783 twilio-8.1.0/twilio/rest/studio/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/StudioBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.063783 twilio-8.1.0/twilio/rest/studio/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.063783 twilio-8.1.0/twilio/rest/studio/v1/flow/
--rw-r--r--   0 runner    (1001) docker     (123)    16404 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v1/flow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.063783 twilio-8.1.0/twilio/rest/studio/v1/flow/engagement/
--rw-r--r--   0 runner    (1001) docker     (123)    21366 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v1/flow/engagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.063783 twilio-8.1.0/twilio/rest/studio/v1/flow/engagement/step/
--rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.063783 twilio-8.1.0/twilio/rest/studio/v1/flow/execution/
--rw-r--r--   0 runner    (1001) docker     (123)    27270 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v1/flow/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v1/flow/execution/execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.063783 twilio-8.1.0/twilio/rest/studio/v1/flow/execution/execution_step/
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.063783 twilio-8.1.0/twilio/rest/studio/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.063783 twilio-8.1.0/twilio/rest/studio/v2/flow/
--rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v2/flow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.063783 twilio-8.1.0/twilio/rest/studio/v2/flow/execution/
--rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v2/flow/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v2/flow/execution/execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.067782 twilio-8.1.0/twilio/rest/studio/v2/flow/execution/execution_step/
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v2/flow/flow_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v2/flow/flow_test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/studio/v2/flow_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.067782 twilio-8.1.0/twilio/rest/supersim/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/supersim/SupersimBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/supersim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.067782 twilio-8.1.0/twilio/rest/supersim/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/supersim/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23623 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/supersim/v1/esim_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/supersim/v1/fleet.py
--rw-r--r--   0 runner    (1001) docker     (123)    26640 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/supersim/v1/ip_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/supersim/v1/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.067782 twilio-8.1.0/twilio/rest/supersim/v1/network_access_profile/
--rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/supersim/v1/network_access_profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19359 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/supersim/v1/settings_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.067782 twilio-8.1.0/twilio/rest/supersim/v1/sim/
--rw-r--r--   0 runner    (1001) docker     (123)    28732 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/supersim/v1/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/supersim/v1/sim/billing_period.py
--rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/supersim/v1/sim/sim_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/supersim/v1/sms_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    26841 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/supersim/v1/usage_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.067782 twilio-8.1.0/twilio/rest/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/sync/SyncBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.067782 twilio-8.1.0/twilio/rest/sync/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/sync/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.067782 twilio-8.1.0/twilio/rest/sync/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    36623 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/sync/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.071783 twilio-8.1.0/twilio/rest/sync/v1/service/document/
--rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/sync/v1/service/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/sync/v1/service/document/document_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.071783 twilio-8.1.0/twilio/rest/sync/v1/service/sync_list/
--rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/sync/v1/service/sync_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36671 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21826 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.071783 twilio-8.1.0/twilio/rest/sync/v1/service/sync_map/
--rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/sync/v1/service/sync_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37230 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21754 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.071783 twilio-8.1.0/twilio/rest/sync/v1/service/sync_stream/
--rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/sync/v1/service/sync_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.071783 twilio-8.1.0/twilio/rest/taskrouter/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/TaskrouterBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.071783 twilio-8.1.0/twilio/rest/taskrouter/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.071783 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)    44452 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25986 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    32776 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.075783 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task/
--rw-r--r--   0 runner    (1001) docker     (123)    51478 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79751 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23470 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.075783 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/
--rw-r--r--   0 runner    (1001) docker     (123)    39230 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21315 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.075783 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/worker/
--rw-r--r--   0 runner    (1001) docker     (123)    43462 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77533 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22091 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.075783 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    34579 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    14701 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.075783 twilio-8.1.0/twilio/rest/trunking/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trunking/TrunkingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trunking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.075783 twilio-8.1.0/twilio/rest/trunking/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trunking/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.079783 twilio-8.1.0/twilio/rest/trunking/v1/trunk/
--rw-r--r--   0 runner    (1001) docker     (123)    39976 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trunking/v1/trunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trunking/v1/trunk/credential_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trunking/v1/trunk/origination_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    22459 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trunking/v1/trunk/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trunking/v1/trunk/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.079783 twilio-8.1.0/twilio/rest/trusthub/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/TrusthubBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.079783 twilio-8.1.0/twilio/rest/trusthub/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.079783 twilio-8.1.0/twilio/rest/trusthub/v1/customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23437 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (123)    20560 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/v1/end_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/v1/end_user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/v1/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/v1/supporting_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/v1/supporting_document_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.079783 twilio-8.1.0/twilio/rest/trusthub/v1/trust_products/
--rw-r--r--   0 runner    (1001) docker     (123)    30206 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/v1/trust_products/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.083783 twilio-8.1.0/twilio/rest/verify/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/VerifyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.083783 twilio-8.1.0/twilio/rest/verify/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/safelist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.083783 twilio-8.1.0/twilio/rest/verify/v2/service/
--rw-r--r--   0 runner    (1001) docker     (123)    55315 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/service/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.083783 twilio-8.1.0/twilio/rest/verify/v2/service/entity/
--rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/service/entity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.083783 twilio-8.1.0/twilio/rest/verify/v2/service/entity/challenge/
--rw-r--r--   0 runner    (1001) docker     (123)    34458 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/service/entity/challenge/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/service/entity/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/service/entity/new_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/service/messaging_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.083783 twilio-8.1.0/twilio/rest/verify/v2/service/rate_limit/
--rw-r--r--   0 runner    (1001) docker     (123)    21507 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/service/rate_limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22242 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/service/rate_limit/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    21417 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/service/verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/service/verification_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/service/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    29432 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/verification_attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/verify/v2/verification_attempts_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.083783 twilio-8.1.0/twilio/rest/video/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/VideoBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.087783 twilio-8.1.0/twilio/rest/video/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/v1/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)    54707 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/v1/composition_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/v1/composition_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/v1/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/v1/recording_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.087783 twilio-8.1.0/twilio/rest/video/v1/room/
--rw-r--r--   0 runner    (1001) docker     (123)    38074 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/v1/room/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.087783 twilio-8.1.0/twilio/rest/video/v1/room/participant/
--rw-r--r--   0 runner    (1001) docker     (123)    28698 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/v1/room/participant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/v1/room/participant/anonymize.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/v1/room/participant/published_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/v1/room/participant/subscribe_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/v1/room/participant/subscribed_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/v1/room/recording_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    24746 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/video/v1/room/room_recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.087783 twilio-8.1.0/twilio/rest/voice/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/voice/VoiceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/voice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.087783 twilio-8.1.0/twilio/rest/voice/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/voice/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/voice/v1/archived_call.py
--rw-r--r--   0 runner    (1001) docker     (123)    37359 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/voice/v1/byoc_trunk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.087783 twilio-8.1.0/twilio/rest/voice/v1/connection_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    20484 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/voice/v1/connection_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29170 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.087783 twilio-8.1.0/twilio/rest/voice/v1/dialing_permissions/
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/voice/v1/dialing_permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.087783 twilio-8.1.0/twilio/rest/voice/v1/dialing_permissions/country/
--rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/voice/v1/dialing_permissions/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/voice/v1/ip_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    19429 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/voice/v1/source_ip_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.087783 twilio-8.1.0/twilio/rest/wireless/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/wireless/WirelessBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/wireless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.091783 twilio-8.1.0/twilio/rest/wireless/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/wireless/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27361 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/wireless/v1/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    29604 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/wireless/v1/rate_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.091783 twilio-8.1.0/twilio/rest/wireless/v1/sim/
--rw-r--r--   0 runner    (1001) docker     (123)    46125 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/wireless/v1/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/wireless/v1/sim/data_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/wireless/v1/sim/usage_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/rest/wireless/v1/usage_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:22.091783 twilio-8.1.0/twilio/twiml/
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/twiml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/twiml/fax_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/twiml/messaging_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    82958 2023-04-20 07:29:07.000000 twilio-8.1.0/twilio/twiml/voice_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:29:21.975781 twilio-8.1.0/twilio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-04-20 07:29:21.000000 twilio-8.1.0/twilio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30366 2023-04-20 07:29:21.000000 twilio-8.1.0/twilio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:29:21.000000 twilio-8.1.0/twilio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-20 07:29:21.000000 twilio-8.1.0/twilio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 07:29:21.000000 twilio-8.1.0/twilio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.332207 twilio-8.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-04 09:30:30.000000 twilio-8.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-04 09:30:30.000000 twilio-8.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-04 09:30:30.000000 twilio-8.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-05-04 09:30:45.332207 twilio-8.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-05-04 09:30:30.000000 twilio-8.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-04 09:30:45.332207 twilio-8.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1694 2023-05-04 09:30:30.000000 twilio-8.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.152205 twilio-8.2.0/twilio/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.156205 twilio-8.2.0/twilio/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/instance_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/instance_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/obsolete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.156205 twilio-8.2.0/twilio/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/http/async_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/http/validation_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.156205 twilio-8.2.0/twilio/jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/jwt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.156205 twilio-8.2.0/twilio/jwt/access_token/
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/jwt/access_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/jwt/access_token/grants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.156205 twilio-8.2.0/twilio/jwt/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/jwt/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.156205 twilio-8.2.0/twilio/jwt/taskrouter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/jwt/taskrouter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/jwt/taskrouter/capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.160205 twilio-8.2.0/twilio/jwt/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/jwt/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/request_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.160205 twilio-8.2.0/twilio/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.160205 twilio-8.2.0/twilio/rest/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/AccountsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.160205 twilio-8.2.0/twilio/rest/accounts/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/v1/auth_token_promotion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.160205 twilio-8.2.0/twilio/rest/accounts/v1/credential/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/v1/credential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19489 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/v1/credential/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20007 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/v1/credential/public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/v1/secondary_auth_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.160205 twilio-8.2.0/twilio/rest/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/ApiBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.160205 twilio-8.2.0/twilio/rest/api/v2010/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.164205 twilio-8.2.0/twilio/rest/api/v2010/account/
+-rw-r--r--   0 runner    (1001) docker     (123)    36206 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.164205 twilio-8.2.0/twilio/rest/api/v2010/account/address/
+-rw-r--r--   0 runner    (1001) docker     (123)    35858 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47553 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/authorized_connect_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.164205 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/
+-rw-r--r--   0 runner    (1001) docker     (123)    21427 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46239 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46210 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45860 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46000 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45790 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/balance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.168205 twilio-8.2.0/twilio/rest/api/v2010/account/call/
+-rw-r--r--   0 runner    (1001) docker     (123)    92392 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13986 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/feedback_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28363 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23472 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38495 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77226 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/siprec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77116 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/user_defined_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.168205 twilio-8.2.0/twilio/rest/api/v2010/account/conference/
+-rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/conference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74737 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/conference/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32729 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/conference/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26539 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/connect_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/
+-rw-r--r--   0 runner    (1001) docker     (123)    73374 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18341 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36935 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37019 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37103 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/message/
+-rw-r--r--   0 runner    (1001) docker     (123)    53984 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/message/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27246 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/message/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/new_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/new_signing_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27505 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22199 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/outgoing_caller_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19131 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/queue/member.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/recording/
+-rw-r--r--   0 runner    (1001) docker     (123)    37769 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/recording/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/recording/add_on_result/
+-rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19233 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/recording/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26406 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/short_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/signing_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/sip/
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/sip/credential_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    21278 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22757 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    45116 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.176205 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.176205 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.176205 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21048 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.176205 twilio-8.2.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26238 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/transcription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.176205 twilio-8.2.0/twilio/rest/api/v2010/account/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.180205 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/
+-rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/all_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/last_month.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/this_month.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/today.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38293 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/yearly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/yesterday.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49245 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/validation_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.180205 twilio-8.2.0/twilio/rest/autopilot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/AutopilotBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.180205 twilio-8.2.0/twilio/rest/autopilot/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.180205 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    35087 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/dialogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.180205 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/field_type/
+-rw-r--r--   0 runner    (1001) docker     (123)    23752 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/field_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/field_type/field_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22851 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/model_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29877 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/style_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.180205 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    28213 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27891 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/task_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/task_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24728 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/restore_assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.184205 twilio-8.2.0/twilio/rest/bulkexports/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/BulkexportsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.184205 twilio-8.2.0/twilio/rest/bulkexports/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.184205 twilio-8.2.0/twilio/rest/bulkexports/v1/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/v1/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/v1/export/day.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/v1/export/export_custom_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/v1/export/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/v1/export_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.184205 twilio-8.2.0/twilio/rest/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.184205 twilio-8.2.0/twilio/rest/chat/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27856 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.184205 twilio-8.2.0/twilio/rest/chat/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    92674 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.184205 twilio-8.2.0/twilio/rest/chat/v1/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    28967 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26356 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21831 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.188205 twilio-8.2.0/twilio/rest/chat/v1/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    26317 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.188205 twilio-8.2.0/twilio/rest/chat/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27486 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.188205 twilio-8.2.0/twilio/rest/chat/v2/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    66570 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22118 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.188205 twilio-8.2.0/twilio/rest/chat/v2/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    39123 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22292 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37545 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33770 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/channel/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.188205 twilio-8.2.0/twilio/rest/chat/v2/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    29035 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/user/user_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27050 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.188205 twilio-8.2.0/twilio/rest/chat/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v3/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.188205 twilio-8.2.0/twilio/rest/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/content/ContentBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/content/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.192205 twilio-8.2.0/twilio/rest/content/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/content/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.192205 twilio-8.2.0/twilio/rest/content/v1/content/
+-rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/content/v1/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/content/v1/content/approval_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/content/v1/content_and_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/content/v1/legacy_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.192205 twilio-8.2.0/twilio/rest/conversations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/ConversationsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.192205 twilio-8.2.0/twilio/rest/conversations/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36854 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/address_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.192205 twilio-8.2.0/twilio/rest/conversations/v1/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/configuration/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.192205 twilio-8.2.0/twilio/rest/conversations/v1/conversation/
+-rw-r--r--   0 runner    (1001) docker     (123)    37723 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/conversation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.196205 twilio-8.2.0/twilio/rest/conversations/v1/conversation/message/
+-rw-r--r--   0 runner    (1001) docker     (123)    34972 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/conversation/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40116 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/conversation/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27236 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/conversation/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27935 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/participant_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20943 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.196205 twilio-8.2.0/twilio/rest/conversations/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22289 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.196205 twilio-8.2.0/twilio/rest/conversations/v1/service/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24410 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/configuration/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/configuration/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.196205 twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/
+-rw-r--r--   0 runner    (1001) docker     (123)    39574 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.200205 twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/message/
+-rw-r--r--   0 runner    (1001) docker     (123)    36629 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28926 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/participant_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22534 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.200205 twilio-8.2.0/twilio/rest/conversations/v1/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    29682 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26510 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/user/user_conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.200205 twilio-8.2.0/twilio/rest/conversations/v1/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    28016 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25215 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/user/user_conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.200205 twilio-8.2.0/twilio/rest/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/EventsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.200205 twilio-8.2.0/twilio/rest/events/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15317 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/event_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.200205 twilio-8.2.0/twilio/rest/events/v1/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/schema/schema_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.204205 twilio-8.2.0/twilio/rest/events/v1/sink/
+-rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/sink/sink_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/sink/sink_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.204205 twilio-8.2.0/twilio/rest/events/v1/subscription/
+-rw-r--r--   0 runner    (1001) docker     (123)    22609 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/subscription/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/subscription/subscribed_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.204205 twilio-8.2.0/twilio/rest/flex_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/FlexApiBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.208206 twilio-8.2.0/twilio/rest/flex_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/assessments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19793 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46860 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/flex_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17501 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_assessments_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_conversations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27126 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_questionnaires.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15704 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_settings_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_user_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.208206 twilio-8.2.0/twilio/rest/flex_api/v1/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/interaction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.212206 twilio-8.2.0/twilio/rest/flex_api/v1/interaction/interaction_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/web_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.212206 twilio-8.2.0/twilio/rest/flex_api/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v2/web_channels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.212206 twilio-8.2.0/twilio/rest/frontline_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/frontline_api/FrontlineApiBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/frontline_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.212206 twilio-8.2.0/twilio/rest/frontline_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/frontline_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/frontline_api/v1/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.212206 twilio-8.2.0/twilio/rest/insights/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/InsightsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.212206 twilio-8.2.0/twilio/rest/insights/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.216206 twilio-8.2.0/twilio/rest/insights/v1/call/
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/call/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/call/call_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/call/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/call/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28813 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/call_summaries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.216206 twilio-8.2.0/twilio/rest/insights/v1/conference/
+-rw-r--r--   0 runner    (1001) docker     (123)    31370 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/conference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/conference/conference_participant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.216206 twilio-8.2.0/twilio/rest/insights/v1/room/
+-rw-r--r--   0 runner    (1001) docker     (123)    25243 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/room/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17908 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/room/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/setting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.216206 twilio-8.2.0/twilio/rest/ip_messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/IpMessagingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.216206 twilio-8.2.0/twilio/rest/ip_messaging/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.220206 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    62960 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.220206 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    24064 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21725 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.220206 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.220206 twilio-8.2.0/twilio/rest/ip_messaging/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.220206 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    45390 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.224206 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29520 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28798 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.224206 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    24051 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21476 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.224206 twilio-8.2.0/twilio/rest/lookups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/lookups/LookupsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/lookups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.224206 twilio-8.2.0/twilio/rest/lookups/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/lookups/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/lookups/v1/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.224206 twilio-8.2.0/twilio/rest/lookups/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/lookups/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20961 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/lookups/v2/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.228206 twilio-8.2.0/twilio/rest/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/media/MediaBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/media/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.228206 twilio-8.2.0/twilio/rest/media/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/media/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26533 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/media/v1/media_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/media/v1/media_recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.228206 twilio-8.2.0/twilio/rest/media/v1/player_streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)    25414 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/media/v1/player_streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/media/v1/player_streamer/playback_grant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.228206 twilio-8.2.0/twilio/rest/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/MessagingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.232206 twilio-8.2.0/twilio/rest/messaging/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.232206 twilio-8.2.0/twilio/rest/messaging/v1/brand_registration/
+-rw-r--r--   0 runner    (1001) docker     (123)    24289 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/brand_registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19914 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/deactivations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/domain_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/domain_config_messaging_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/external_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.232206 twilio-8.2.0/twilio/rest/messaging/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    54653 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/service/alpha_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/service/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/service/short_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33395 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/service/us_app_to_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/usecase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.236206 twilio-8.2.0/twilio/rest/microvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/MicrovisorBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.236206 twilio-8.2.0/twilio/rest/microvisor/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/account_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/account_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.236206 twilio-8.2.0/twilio/rest/microvisor/v1/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/app/app_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.236206 twilio-8.2.0/twilio/rest/microvisor/v1/device/
+-rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/device/device_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/device/device_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.236206 twilio-8.2.0/twilio/rest/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/monitor/MonitorBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.236206 twilio-8.2.0/twilio/rest/monitor/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/monitor/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22723 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/monitor/v1/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25437 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/monitor/v1/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.240206 twilio-8.2.0/twilio/rest/notify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/notify/NotifyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/notify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.240206 twilio-8.2.0/twilio/rest/notify/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/notify/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/notify/v1/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.240206 twilio-8.2.0/twilio/rest/notify/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    47060 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/notify/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/notify/v1/service/binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25490 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/notify/v1/service/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.240206 twilio-8.2.0/twilio/rest/numbers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/NumbersBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.240206 twilio-8.2.0/twilio/rest/numbers/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.244206 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.244206 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)    47502 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.244206 twilio-8.2.0/twilio/rest/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/OauthBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.248206 twilio-8.2.0/twilio/rest/oauth/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/v1/device_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/v1/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/v1/openid_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/v1/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/v1/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.248206 twilio-8.2.0/twilio/rest/preview/
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/PreviewBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.248206 twilio-8.2.0/twilio/rest/preview/deployed_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/deployed_devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.252206 twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/
+-rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24118 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22163 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26656 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.252206 twilio-8.2.0/twilio/rest/preview/hosted_numbers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/hosted_numbers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.252206 twilio-8.2.0/twilio/rest/preview/hosted_numbers/authorization_document/
+-rw-r--r--   0 runner    (1001) docker     (123)    32009 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24829 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48143 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.252206 twilio-8.2.0/twilio/rest/preview/marketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/marketplace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.252206 twilio-8.2.0/twilio/rest/preview/marketplace/available_add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)    15067 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/marketplace/available_add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.252206 twilio-8.2.0/twilio/rest/preview/marketplace/installed_add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)    23293 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.252206 twilio-8.2.0/twilio/rest/preview/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.256206 twilio-8.2.0/twilio/rest/preview/sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.256206 twilio-8.2.0/twilio/rest/preview/sync/service/document/
+-rw-r--r--   0 runner    (1001) docker     (123)    20547 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/document/document_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.256206 twilio-8.2.0/twilio/rest/preview/sync/service/sync_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/sync_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.256206 twilio-8.2.0/twilio/rest/preview/sync/service/sync_map/
+-rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/sync_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24063 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21250 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.256206 twilio-8.2.0/twilio/rest/preview/understand/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.260206 twilio-8.2.0/twilio/rest/preview/understand/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/dialogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.260206 twilio-8.2.0/twilio/rest/preview/understand/assistant/field_type/
+-rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/field_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20410 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/field_type/field_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/model_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/style_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.260206 twilio-8.2.0/twilio/rest/preview/understand/assistant/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    26813 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/task/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/task/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/task/task_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/task/task_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.264206 twilio-8.2.0/twilio/rest/preview/wireless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/wireless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/wireless/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/wireless/rate_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.264206 twilio-8.2.0/twilio/rest/preview/wireless/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/wireless/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/wireless/sim/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.264206 twilio-8.2.0/twilio/rest/pricing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/PricingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.264206 twilio-8.2.0/twilio/rest/pricing/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.264206 twilio-8.2.0/twilio/rest/pricing/v1/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/messaging/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.264206 twilio-8.2.0/twilio/rest/pricing/v1/phone_number/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/phone_number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/phone_number/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.264206 twilio-8.2.0/twilio/rest/pricing/v1/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/voice/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/voice/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.268206 twilio-8.2.0/twilio/rest/pricing/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v2/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v2/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.268206 twilio-8.2.0/twilio/rest/pricing/v2/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v2/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v2/voice/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v2/voice/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.268206 twilio-8.2.0/twilio/rest/proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/ProxyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.268206 twilio-8.2.0/twilio/rest/proxy/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.268206 twilio-8.2.0/twilio/rest/proxy/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    38044 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23754 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/service/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.268206 twilio-8.2.0/twilio/rest/proxy/v1/service/session/
+-rw-r--r--   0 runner    (1001) docker     (123)    27767 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/service/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/service/session/interaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.272206 twilio-8.2.0/twilio/rest/proxy/v1/service/session/participant/
+-rw-r--r--   0 runner    (1001) docker     (123)    22765 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/service/session/participant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23242 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21333 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/service/short_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.272206 twilio-8.2.0/twilio/rest/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/routes/RoutesBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.272206 twilio-8.2.0/twilio/rest/routes/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/routes/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/routes/v2/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/routes/v2/sip_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/routes/v2/trunk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.272206 twilio-8.2.0/twilio/rest/serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/ServerlessBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.272206 twilio-8.2.0/twilio/rest/serverless/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.272206 twilio-8.2.0/twilio/rest/serverless/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.276206 twilio-8.2.0/twilio/rest/serverless/v1/service/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)    20582 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/asset/asset_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.276206 twilio-8.2.0/twilio/rest/serverless/v1/service/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/build/build_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.276206 twilio-8.2.0/twilio/rest/serverless/v1/service/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)    21009 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/environment/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20926 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/environment/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/environment/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.276206 twilio-8.2.0/twilio/rest/serverless/v1/service/function/
+-rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/function/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.276206 twilio-8.2.0/twilio/rest/serverless/v1/service/function/function_version/
+-rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.280206 twilio-8.2.0/twilio/rest/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/StudioBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.280206 twilio-8.2.0/twilio/rest/studio/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.280206 twilio-8.2.0/twilio/rest/studio/v1/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)    16404 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.280206 twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/
+-rw-r--r--   0 runner    (1001) docker     (123)    21366 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.280206 twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/step/
+-rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.280206 twilio-8.2.0/twilio/rest/studio/v1/flow/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)    27270 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/execution/execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.280206 twilio-8.2.0/twilio/rest/studio/v1/flow/execution/execution_step/
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.284206 twilio-8.2.0/twilio/rest/studio/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.284206 twilio-8.2.0/twilio/rest/studio/v2/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.284206 twilio-8.2.0/twilio/rest/studio/v2/flow/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow/execution/execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.284206 twilio-8.2.0/twilio/rest/studio/v2/flow/execution/execution_step/
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow/flow_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow/flow_test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.284206 twilio-8.2.0/twilio/rest/supersim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/SupersimBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.288206 twilio-8.2.0/twilio/rest/supersim/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23623 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/esim_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/fleet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26640 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/ip_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.288206 twilio-8.2.0/twilio/rest/supersim/v1/network_access_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/network_access_profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19359 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/settings_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.288206 twilio-8.2.0/twilio/rest/supersim/v1/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)    28732 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/sim/billing_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/sim/sim_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/sms_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26841 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/usage_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.292207 twilio-8.2.0/twilio/rest/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/SyncBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.292207 twilio-8.2.0/twilio/rest/sync/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.292207 twilio-8.2.0/twilio/rest/sync/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    36623 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.292207 twilio-8.2.0/twilio/rest/sync/v1/service/document/
+-rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/document/document_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.292207 twilio-8.2.0/twilio/rest/sync/v1/service/sync_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36671 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21826 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.292207 twilio-8.2.0/twilio/rest/sync/v1/service/sync_map/
+-rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37230 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21754 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.296207 twilio-8.2.0/twilio/rest/sync/v1/service/sync_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.296207 twilio-8.2.0/twilio/rest/taskrouter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/TaskrouterBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.296207 twilio-8.2.0/twilio/rest/taskrouter/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.296207 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)    44452 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25986 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32776 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.300207 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    51478 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79751 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23470 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.300207 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)    39230 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21315 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.304207 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)    43462 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77533 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22091 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.304207 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    34579 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14701 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.304207 twilio-8.2.0/twilio/rest/trunking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/TrunkingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.304207 twilio-8.2.0/twilio/rest/trunking/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.304207 twilio-8.2.0/twilio/rest/trunking/v1/trunk/
+-rw-r--r--   0 runner    (1001) docker     (123)    39976 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/v1/trunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/v1/trunk/credential_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/v1/trunk/origination_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22459 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/v1/trunk/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/v1/trunk/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.308207 twilio-8.2.0/twilio/rest/trusthub/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/TrusthubBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.308207 twilio-8.2.0/twilio/rest/trusthub/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.308207 twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23437 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20560 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/end_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/end_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/supporting_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/supporting_document_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.312207 twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/
+-rw-r--r--   0 runner    (1001) docker     (123)    30206 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.312207 twilio-8.2.0/twilio/rest/verify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/VerifyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.312207 twilio-8.2.0/twilio/rest/verify/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/safelist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.316207 twilio-8.2.0/twilio/rest/verify/v2/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    55315 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.316207 twilio-8.2.0/twilio/rest/verify/v2/service/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/entity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.316207 twilio-8.2.0/twilio/rest/verify/v2/service/entity/challenge/
+-rw-r--r--   0 runner    (1001) docker     (123)    34458 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/entity/challenge/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/entity/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/entity/new_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/messaging_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.320207 twilio-8.2.0/twilio/rest/verify/v2/service/rate_limit/
+-rw-r--r--   0 runner    (1001) docker     (123)    21507 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/rate_limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22242 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/rate_limit/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21417 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/verification_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29432 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/verification_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/verification_attempts_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.320207 twilio-8.2.0/twilio/rest/video/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/VideoBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.320207 twilio-8.2.0/twilio/rest/video/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54707 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/composition_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/composition_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/recording_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.320207 twilio-8.2.0/twilio/rest/video/v1/room/
+-rw-r--r--   0 runner    (1001) docker     (123)    38074 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.324207 twilio-8.2.0/twilio/rest/video/v1/room/participant/
+-rw-r--r--   0 runner    (1001) docker     (123)    28698 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/participant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/participant/anonymize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/participant/published_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/participant/subscribe_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/participant/subscribed_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/recording_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24746 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/room_recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.324207 twilio-8.2.0/twilio/rest/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/VoiceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.324207 twilio-8.2.0/twilio/rest/voice/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/archived_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37359 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/byoc_trunk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.324207 twilio-8.2.0/twilio/rest/voice/v1/connection_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    20484 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/connection_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29170 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.328207 twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.328207 twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/country/
+-rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/ip_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19429 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/source_ip_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.328207 twilio-8.2.0/twilio/rest/wireless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/WirelessBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.328207 twilio-8.2.0/twilio/rest/wireless/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27361 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/v1/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29604 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/v1/rate_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.328207 twilio-8.2.0/twilio/rest/wireless/v1/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)    46125 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/v1/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/v1/sim/data_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/v1/sim/usage_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/v1/usage_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.332207 twilio-8.2.0/twilio/twiml/
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/twiml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/twiml/fax_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/twiml/messaging_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82958 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/twiml/voice_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.152205 twilio-8.2.0/twilio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-05-04 09:30:45.000000 twilio-8.2.0/twilio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30316 2023-05-04 09:30:45.000000 twilio-8.2.0/twilio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:45.000000 twilio-8.2.0/twilio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 09:30:45.000000 twilio-8.2.0/twilio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 09:30:45.000000 twilio-8.2.0/twilio.egg-info/top_level.txt
```

### Comparing `twilio-8.1.0/AUTHORS.md` & `twilio-8.2.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/LICENSE` & `twilio-8.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/PKG-INFO` & `twilio-8.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twilio
-Version: 8.1.0
+Version: 8.2.0
 Summary: Twilio API client and TwiML generator
 Home-page: https://github.com/twilio/twilio-python/
 Author: Twilio
 Author-email: help@twilio.com
 Keywords: twilio,twiml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `twilio-8.1.0/README.md` & `twilio-8.2.0/README.md`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/setup.py` & `twilio-8.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # python setup.py install
 #
 # You need to have the setuptools module installed. Try reading the setuptools
 # documentation: http://pypi.python.org/pypi/setuptools
 
 setup(
     name="twilio",
-    version="8.1.0",
+    version="8.2.0",
     description="Twilio API client and TwiML generator",
     author="Twilio",
     author_email="help@twilio.com",
     url="https://github.com/twilio/twilio-python/",
     keywords=["twilio", "twiml"],
     python_requires=">=3.7.0",
     install_requires=[
```

### Comparing `twilio-8.1.0/twilio/base/client_base.py` & `twilio-8.2.0/twilio/base/client_base.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/base/deserialize.py` & `twilio-8.2.0/twilio/base/deserialize.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/base/domain.py` & `twilio-8.2.0/twilio/base/domain.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/base/exceptions.py` & `twilio-8.2.0/twilio/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/base/obsolete.py` & `twilio-8.2.0/twilio/base/obsolete.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/base/page.py` & `twilio-8.2.0/twilio/base/page.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/base/serialize.py` & `twilio-8.2.0/twilio/base/serialize.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/base/version.py` & `twilio-8.2.0/twilio/base/version.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/http/__init__.py` & `twilio-8.2.0/twilio/http/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/http/async_http_client.py` & `twilio-8.2.0/twilio/http/async_http_client.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/http/http_client.py` & `twilio-8.2.0/twilio/http/http_client.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/http/request.py` & `twilio-8.2.0/twilio/http/request.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/http/response.py` & `twilio-8.2.0/twilio/http/response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/http/validation_client.py` & `twilio-8.2.0/twilio/http/validation_client.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/jwt/__init__.py` & `twilio-8.2.0/twilio/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/jwt/access_token/__init__.py` & `twilio-8.2.0/twilio/jwt/access_token/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/jwt/access_token/grants.py` & `twilio-8.2.0/twilio/jwt/access_token/grants.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/jwt/client/__init__.py` & `twilio-8.2.0/twilio/jwt/client/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/jwt/taskrouter/__init__.py` & `twilio-8.2.0/twilio/jwt/taskrouter/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/jwt/taskrouter/capabilities.py` & `twilio-8.2.0/twilio/jwt/taskrouter/capabilities.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/jwt/validation/__init__.py` & `twilio-8.2.0/twilio/jwt/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/request_validator.py` & `twilio-8.2.0/twilio/request_validator.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/__init__.py` & `twilio-8.2.0/twilio/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/accounts/AccountsBase.py` & `twilio-8.2.0/twilio/rest/accounts/AccountsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/accounts/__init__.py` & `twilio-8.2.0/twilio/rest/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/accounts/v1/__init__.py` & `twilio-8.2.0/twilio/rest/accounts/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/accounts/v1/auth_token_promotion.py` & `twilio-8.2.0/twilio/rest/accounts/v1/auth_token_promotion.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/accounts/v1/credential/__init__.py` & `twilio-8.2.0/twilio/rest/accounts/v1/credential/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/accounts/v1/credential/aws.py` & `twilio-8.2.0/twilio/rest/accounts/v1/credential/aws.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/accounts/v1/credential/public_key.py` & `twilio-8.2.0/twilio/rest/accounts/v1/credential/public_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/accounts/v1/secondary_auth_token.py` & `twilio-8.2.0/twilio/rest/accounts/v1/secondary_auth_token.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/ApiBase.py` & `twilio-8.2.0/twilio/rest/api/ApiBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/__init__.py` & `twilio-8.2.0/twilio/rest/api/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/address/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/address/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/application.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/application.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/authorized_connect_app.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/authorized_connect_app.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/balance.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/balance.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/call/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/call/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/call/event.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/call/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/call/feedback.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/call/feedback.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/call/feedback_summary.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/call/feedback_summary.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/call/notification.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/call/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/call/payment.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/call/payment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/call/recording.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/call/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/call/siprec.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/call/siprec.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/call/stream.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/call/stream.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/call/user_defined_message.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/call/user_defined_message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/conference/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/conference/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/conference/participant.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/conference/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/conference/recording.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/conference/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/connect_app.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/connect_app.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/key.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/message/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/message/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     class UpdateStatus(object):
         CANCELED = "canceled"
 
     """
     :ivar body: The message text. Can be up to 1,600 characters long.
     :ivar num_segments: The number of segments that make up the complete message. A message body that is too large to be sent in a single SMS message is segmented and charged as multiple messages. Inbound messages over 160 characters are reassembled when the message is received. Note: When using a Messaging Service to send messages, `num_segments` will always be 0 in Twilio's response to your API request.
     :ivar direction: 
-    :ivar _from: The phone number (in [E.164](https://en.wikipedia.org/wiki/E.164) format), [alphanumeric sender ID](https://www.twilio.com/docs/sms/send-messages#use-an-alphanumeric-sender-id), or [Wireless SIM](https://www.twilio.com/docs/wireless/tutorials/communications-guides/how-to-send-and-receive-text-messages) that initiated the message. For incoming messages, this will be the number of the sending phone. For outgoing messages, this value will be one of your Twilio phone numbers or the alphanumeric sender ID used.
+    :ivar from_: The phone number (in [E.164](https://en.wikipedia.org/wiki/E.164) format), [alphanumeric sender ID](https://www.twilio.com/docs/sms/send-messages#use-an-alphanumeric-sender-id), or [Wireless SIM](https://www.twilio.com/docs/wireless/tutorials/communications-guides/how-to-send-and-receive-text-messages) that initiated the message. For incoming messages, this will be the number of the sending phone. For outgoing messages, this value will be one of your Twilio phone numbers or the alphanumeric sender ID used.
     :ivar to: The phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format that received the message. For incoming messages, this will be one of your Twilio phone numbers. For outgoing messages, this will be the sending phone.
     :ivar date_updated: The date and time in GMT that the resource was last updated specified in [RFC 2822](https://www.ietf.org/rfc/rfc2822.txt) format.
     :ivar price: The amount billed for the message, in the currency specified by `price_unit`.  Note that your account is charged for each segment we send to the handset. Populated after the message has been sent. May not be immediately available.
     :ivar error_message: The description of the `error_code` if your message `status` is `failed` or `undelivered`. If the message was successful, this value is null.
     :ivar uri: The URI of the resource, relative to `https://api.twilio.com`.
     :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that sent the message that created the resource.
     :ivar num_media: The number of media files associated with the message. A message can send up to 10 media files.
@@ -90,15 +90,15 @@
         sid: Optional[str] = None,
     ):
         super().__init__(version)
 
         self.body: Optional[str] = payload.get("body")
         self.num_segments: Optional[str] = payload.get("num_segments")
         self.direction: Optional["MessageInstance.Direction"] = payload.get("direction")
-        self._from: Optional[str] = payload.get("from")
+        self.from_: Optional[str] = payload.get("from")
         self.to: Optional[str] = payload.get("to")
         self.date_updated: Optional[datetime] = deserialize.rfc2822_datetime(
             payload.get("date_updated")
         )
         self.price: Optional[str] = payload.get("price")
         self.error_message: Optional[str] = payload.get("error_message")
         self.uri: Optional[str] = payload.get("uri")
```

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/message/feedback.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/message/feedback.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/message/media.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/message/media.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/new_key.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/new_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/new_signing_key.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/new_signing_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/notification.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/outgoing_caller_id.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/outgoing_caller_id.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/queue/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/queue/member.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/queue/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/recording/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/recording/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/recording/transcription.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/recording/transcription.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/short_code.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/short_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/signing_key.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/signing_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/sip/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/sip/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/token.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/token.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/transcription.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/transcription.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/usage/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/usage/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/__init__.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/all_time.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/all_time.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/daily.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/daily.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/last_month.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/last_month.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/monthly.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/monthly.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/this_month.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/this_month.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/today.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/today.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/yearly.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/yearly.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/usage/record/yesterday.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/yesterday.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/usage/trigger.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/usage/trigger.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/api/v2010/account/validation_request.py` & `twilio-8.2.0/twilio/rest/api/v2010/account/validation_request.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/AutopilotBase.py` & `twilio-8.2.0/twilio/rest/autopilot/AutopilotBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/__init__.py` & `twilio-8.2.0/twilio/rest/autopilot/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/__init__.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/assistant/__init__.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/assistant/defaults.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/defaults.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/assistant/dialogue.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/dialogue.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/assistant/field_type/__init__.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/field_type/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/assistant/field_type/field_value.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/field_type/field_value.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/assistant/model_build.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/model_build.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/assistant/query.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/query.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/assistant/style_sheet.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/style_sheet.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/assistant/task/__init__.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/assistant/task/field.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/field.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/assistant/task/sample.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/sample.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/assistant/task/task_actions.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/task_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/assistant/task/task_statistics.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/task_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/assistant/webhook.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/autopilot/v1/restore_assistant.py` & `twilio-8.2.0/twilio/rest/autopilot/v1/restore_assistant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/bulkexports/BulkexportsBase.py` & `twilio-8.2.0/twilio/rest/bulkexports/BulkexportsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/bulkexports/__init__.py` & `twilio-8.2.0/twilio/rest/bulkexports/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/bulkexports/v1/__init__.py` & `twilio-8.2.0/twilio/rest/bulkexports/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/bulkexports/v1/export/__init__.py` & `twilio-8.2.0/twilio/rest/bulkexports/v1/export/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/bulkexports/v1/export/day.py` & `twilio-8.2.0/twilio/rest/bulkexports/v1/export/day.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/bulkexports/v1/export/export_custom_job.py` & `twilio-8.2.0/twilio/rest/bulkexports/v1/export/export_custom_job.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/bulkexports/v1/export/job.py` & `twilio-8.2.0/twilio/rest/bulkexports/v1/export/job.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/bulkexports/v1/export_configuration.py` & `twilio-8.2.0/twilio/rest/bulkexports/v1/export_configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/ChatBase.py` & `twilio-8.2.0/twilio/rest/chat/ChatBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/__init__.py` & `twilio-8.2.0/twilio/rest/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v1/__init__.py` & `twilio-8.2.0/twilio/rest/chat/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v1/credential.py` & `twilio-8.2.0/twilio/rest/chat/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v1/service/__init__.py` & `twilio-8.2.0/twilio/rest/chat/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v1/service/channel/__init__.py` & `twilio-8.2.0/twilio/rest/chat/v1/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v1/service/channel/invite.py` & `twilio-8.2.0/twilio/rest/chat/v1/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v1/service/channel/member.py` & `twilio-8.2.0/twilio/rest/chat/v1/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v1/service/channel/message.py` & `twilio-8.2.0/twilio/rest/chat/v1/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v1/service/role.py` & `twilio-8.2.0/twilio/rest/chat/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v1/service/user/__init__.py` & `twilio-8.2.0/twilio/rest/chat/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v1/service/user/user_channel.py` & `twilio-8.2.0/twilio/rest/chat/v1/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v2/__init__.py` & `twilio-8.2.0/twilio/rest/chat/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v2/credential.py` & `twilio-8.2.0/twilio/rest/chat/v2/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v2/service/__init__.py` & `twilio-8.2.0/twilio/rest/chat/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v2/service/binding.py` & `twilio-8.2.0/twilio/rest/chat/v2/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v2/service/channel/__init__.py` & `twilio-8.2.0/twilio/rest/chat/v2/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v2/service/channel/invite.py` & `twilio-8.2.0/twilio/rest/chat/v2/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v2/service/channel/member.py` & `twilio-8.2.0/twilio/rest/chat/v2/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v2/service/channel/message.py` & `twilio-8.2.0/twilio/rest/chat/v2/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v2/service/channel/webhook.py` & `twilio-8.2.0/twilio/rest/chat/v2/service/channel/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v2/service/role.py` & `twilio-8.2.0/twilio/rest/chat/v2/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v2/service/user/__init__.py` & `twilio-8.2.0/twilio/rest/chat/v2/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v2/service/user/user_binding.py` & `twilio-8.2.0/twilio/rest/chat/v2/service/user/user_binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v2/service/user/user_channel.py` & `twilio-8.2.0/twilio/rest/chat/v2/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v3/__init__.py` & `twilio-8.2.0/twilio/rest/chat/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/chat/v3/channel.py` & `twilio-8.2.0/twilio/rest/chat/v3/channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/content/ContentBase.py` & `twilio-8.2.0/twilio/rest/content/ContentBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/content/__init__.py` & `twilio-8.2.0/twilio/rest/content/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/content/v1/__init__.py` & `twilio-8.2.0/twilio/rest/content/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/content/v1/content/__init__.py` & `twilio-8.2.0/twilio/rest/content/v1/content/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/content/v1/content/approval_fetch.py` & `twilio-8.2.0/twilio/rest/content/v1/content/approval_fetch.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/content/v1/content_and_approvals.py` & `twilio-8.2.0/twilio/rest/content/v1/content_and_approvals.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/content/v1/legacy_content.py` & `twilio-8.2.0/twilio/rest/content/v1/legacy_content.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/ConversationsBase.py` & `twilio-8.2.0/twilio/rest/conversations/ConversationsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/__init__.py` & `twilio-8.2.0/twilio/rest/conversations/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/__init__.py` & `twilio-8.2.0/twilio/rest/conversations/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/address_configuration.py` & `twilio-8.2.0/twilio/rest/conversations/v1/address_configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/configuration/__init__.py` & `twilio-8.2.0/twilio/rest/conversations/v1/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/configuration/webhook.py` & `twilio-8.2.0/twilio/rest/conversations/v1/configuration/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/conversation/__init__.py` & `twilio-8.2.0/twilio/rest/conversations/v1/conversation/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -666,218 +666,160 @@
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return ConversationInstance(self._version, payload)
 
     def stream(
         self,
-        start_date: Union[str, object] = values.unset,
-        end_date: Union[str, object] = values.unset,
-        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[ConversationInstance]:
         """
         Streams ConversationInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
-        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
-        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
-        page = self.page(
-            start_date=start_date,
-            end_date=end_date,
-            state=state,
-            page_size=limits["page_size"],
-        )
+        page = self.page(page_size=limits["page_size"])
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
-        start_date: Union[str, object] = values.unset,
-        end_date: Union[str, object] = values.unset,
-        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[ConversationInstance]:
         """
         Asynchronously streams ConversationInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
-        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
-        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
-        page = await self.page_async(
-            start_date=start_date,
-            end_date=end_date,
-            state=state,
-            page_size=limits["page_size"],
-        )
+        page = await self.page_async(page_size=limits["page_size"])
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
-        start_date: Union[str, object] = values.unset,
-        end_date: Union[str, object] = values.unset,
-        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[ConversationInstance]:
         """
         Lists ConversationInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
-        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
-        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return list(
             self.stream(
-                start_date=start_date,
-                end_date=end_date,
-                state=state,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
-        start_date: Union[str, object] = values.unset,
-        end_date: Union[str, object] = values.unset,
-        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[ConversationInstance]:
         """
         Asynchronously lists ConversationInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
-        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
-        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return [
             record
             async for record in await self.stream_async(
-                start_date=start_date,
-                end_date=end_date,
-                state=state,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
-        start_date: Union[str, object] = values.unset,
-        end_date: Union[str, object] = values.unset,
-        state: Union["ConversationInstance.State", object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> ConversationPage:
         """
         Retrieve a single page of ConversationInstance records from the API.
         Request is executed immediately
 
-        :param start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
-        :param end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
-        :param state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of ConversationInstance
         """
         data = values.of(
             {
-                "StartDate": start_date,
-                "EndDate": end_date,
-                "State": state,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
         return ConversationPage(self._version, response)
 
     async def page_async(
         self,
-        start_date: Union[str, object] = values.unset,
-        end_date: Union[str, object] = values.unset,
-        state: Union["ConversationInstance.State", object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> ConversationPage:
         """
         Asynchronously retrieve a single page of ConversationInstance records from the API.
         Request is executed immediately
 
-        :param start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
-        :param end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
-        :param state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of ConversationInstance
         """
         data = values.of(
             {
-                "StartDate": start_date,
-                "EndDate": end_date,
-                "State": state,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = await self._version.page_async(
```

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/conversation/message/__init__.py` & `twilio-8.2.0/twilio/rest/conversations/v1/conversation/message/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py` & `twilio-8.2.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/conversation/participant.py` & `twilio-8.2.0/twilio/rest/conversations/v1/conversation/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/conversation/webhook.py` & `twilio-8.2.0/twilio/rest/conversations/v1/conversation/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/credential.py` & `twilio-8.2.0/twilio/rest/conversations/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/participant_conversation.py` & `twilio-8.2.0/twilio/rest/conversations/v1/participant_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/role.py` & `twilio-8.2.0/twilio/rest/conversations/v1/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/service/__init__.py` & `twilio-8.2.0/twilio/rest/conversations/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/service/binding.py` & `twilio-8.2.0/twilio/rest/conversations/v1/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/service/configuration/__init__.py` & `twilio-8.2.0/twilio/rest/conversations/v1/service/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/service/configuration/notification.py` & `twilio-8.2.0/twilio/rest/conversations/v1/service/configuration/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/service/configuration/webhook.py` & `twilio-8.2.0/twilio/rest/conversations/v1/service/configuration/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/service/conversation/__init__.py` & `twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -706,218 +706,160 @@
 
         return ConversationInstance(
             self._version, payload, chat_service_sid=self._solution["chat_service_sid"]
         )
 
     def stream(
         self,
-        start_date: Union[str, object] = values.unset,
-        end_date: Union[str, object] = values.unset,
-        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[ConversationInstance]:
         """
         Streams ConversationInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
-        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
-        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
-        page = self.page(
-            start_date=start_date,
-            end_date=end_date,
-            state=state,
-            page_size=limits["page_size"],
-        )
+        page = self.page(page_size=limits["page_size"])
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
-        start_date: Union[str, object] = values.unset,
-        end_date: Union[str, object] = values.unset,
-        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[ConversationInstance]:
         """
         Asynchronously streams ConversationInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
-        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
-        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
-        page = await self.page_async(
-            start_date=start_date,
-            end_date=end_date,
-            state=state,
-            page_size=limits["page_size"],
-        )
+        page = await self.page_async(page_size=limits["page_size"])
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
-        start_date: Union[str, object] = values.unset,
-        end_date: Union[str, object] = values.unset,
-        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[ConversationInstance]:
         """
         Lists ConversationInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
-        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
-        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return list(
             self.stream(
-                start_date=start_date,
-                end_date=end_date,
-                state=state,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
-        start_date: Union[str, object] = values.unset,
-        end_date: Union[str, object] = values.unset,
-        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[ConversationInstance]:
         """
         Asynchronously lists ConversationInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
-        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
-        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return [
             record
             async for record in await self.stream_async(
-                start_date=start_date,
-                end_date=end_date,
-                state=state,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
-        start_date: Union[str, object] = values.unset,
-        end_date: Union[str, object] = values.unset,
-        state: Union["ConversationInstance.State", object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> ConversationPage:
         """
         Retrieve a single page of ConversationInstance records from the API.
         Request is executed immediately
 
-        :param start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
-        :param end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
-        :param state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of ConversationInstance
         """
         data = values.of(
             {
-                "StartDate": start_date,
-                "EndDate": end_date,
-                "State": state,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
         return ConversationPage(self._version, response, self._solution)
 
     async def page_async(
         self,
-        start_date: Union[str, object] = values.unset,
-        end_date: Union[str, object] = values.unset,
-        state: Union["ConversationInstance.State", object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> ConversationPage:
         """
         Asynchronously retrieve a single page of ConversationInstance records from the API.
         Request is executed immediately
 
-        :param start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
-        :param end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
-        :param state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of ConversationInstance
         """
         data = values.of(
             {
-                "StartDate": start_date,
-                "EndDate": end_date,
-                "State": state,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = await self._version.page_async(
```

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py` & `twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py` & `twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/service/conversation/participant.py` & `twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/service/conversation/webhook.py` & `twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/service/participant_conversation.py` & `twilio-8.2.0/twilio/rest/conversations/v1/service/participant_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/service/role.py` & `twilio-8.2.0/twilio/rest/conversations/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/service/user/__init__.py` & `twilio-8.2.0/twilio/rest/conversations/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/service/user/user_conversation.py` & `twilio-8.2.0/twilio/rest/conversations/v1/service/user/user_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/user/__init__.py` & `twilio-8.2.0/twilio/rest/conversations/v1/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/conversations/v1/user/user_conversation.py` & `twilio-8.2.0/twilio/rest/conversations/v1/user/user_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/events/EventsBase.py` & `twilio-8.2.0/twilio/rest/events/EventsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/events/__init__.py` & `twilio-8.2.0/twilio/rest/events/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/events/v1/__init__.py` & `twilio-8.2.0/twilio/rest/events/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/events/v1/event_type.py` & `twilio-8.2.0/twilio/rest/events/v1/event_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/events/v1/schema/__init__.py` & `twilio-8.2.0/twilio/rest/events/v1/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/events/v1/schema/schema_version.py` & `twilio-8.2.0/twilio/rest/events/v1/schema/schema_version.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/events/v1/sink/__init__.py` & `twilio-8.2.0/twilio/rest/events/v1/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/events/v1/sink/sink_test.py` & `twilio-8.2.0/twilio/rest/events/v1/sink/sink_test.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/events/v1/sink/sink_validate.py` & `twilio-8.2.0/twilio/rest/events/v1/sink/sink_validate.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/events/v1/subscription/__init__.py` & `twilio-8.2.0/twilio/rest/events/v1/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/events/v1/subscription/subscribed_event.py` & `twilio-8.2.0/twilio/rest/events/v1/subscription/subscribed_event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/FlexApiBase.py` & `twilio-8.2.0/twilio/rest/flex_api/FlexApiBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/__init__.py` & `twilio-8.2.0/twilio/rest/flex_api/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/__init__.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/assessments.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/assessments.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from twilio.base.page import Page
 
 
 class AssessmentsInstance(InstanceResource):
 
     """
     :ivar account_sid: The unique SID identifier of the Account.
-    :ivar assessment_id: The unique id of the assessment
+    :ivar assessment_sid: The SID of the assessment
     :ivar offset: Offset of the conversation
     :ivar report: The flag indicating if this assessment is part of report
     :ivar weight: The weightage given to this comment
     :ivar agent_id: The id of the Agent
     :ivar segment_id: Segment Id of conversation
     :ivar user_name: The name of the user.
     :ivar user_email: The email id of the user.
@@ -41,50 +41,50 @@
     :ivar url:
     """
 
     def __init__(
         self,
         version: Version,
         payload: Dict[str, Any],
-        assessment_id: Optional[str] = None,
+        assessment_sid: Optional[str] = None,
     ):
         super().__init__(version)
 
         self.account_sid: Optional[str] = payload.get("account_sid")
-        self.assessment_id: Optional[str] = payload.get("assessment_id")
+        self.assessment_sid: Optional[str] = payload.get("assessment_sid")
         self.offset: Optional[float] = deserialize.decimal(payload.get("offset"))
         self.report: Optional[bool] = payload.get("report")
         self.weight: Optional[float] = deserialize.decimal(payload.get("weight"))
         self.agent_id: Optional[str] = payload.get("agent_id")
         self.segment_id: Optional[str] = payload.get("segment_id")
         self.user_name: Optional[str] = payload.get("user_name")
         self.user_email: Optional[str] = payload.get("user_email")
         self.answer_text: Optional[str] = payload.get("answer_text")
         self.answer_id: Optional[str] = payload.get("answer_id")
         self.assessment: Optional[Dict[str, object]] = payload.get("assessment")
         self.timestamp: Optional[float] = deserialize.decimal(payload.get("timestamp"))
         self.url: Optional[str] = payload.get("url")
 
         self._solution = {
-            "assessment_id": assessment_id or self.assessment_id,
+            "assessment_sid": assessment_sid or self.assessment_sid,
         }
         self._context: Optional[AssessmentsContext] = None
 
     @property
     def _proxy(self) -> "AssessmentsContext":
         """
         Generate an instance context for the instance, the context is capable of
         performing various actions. All instance actions are proxied to the context
 
         :returns: AssessmentsContext for this AssessmentsInstance
         """
         if self._context is None:
             self._context = AssessmentsContext(
                 self._version,
-                assessment_id=self._solution["assessment_id"],
+                assessment_sid=self._solution["assessment_sid"],
             )
         return self._context
 
     def update(
         self,
         offset: float,
         answer_text: str,
@@ -139,28 +139,30 @@
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
         return "<Twilio.FlexApi.V1.AssessmentsInstance {}>".format(context)
 
 
 class AssessmentsContext(InstanceContext):
-    def __init__(self, version: Version, assessment_id: str):
+    def __init__(self, version: Version, assessment_sid: str):
         """
         Initialize the AssessmentsContext
 
         :param version: Version that contains the resource
-        :param assessment_id: The id of the assessment to be modified
+        :param assessment_sid: The SID of the assessment to be modified
         """
         super().__init__(version)
 
         # Path Solution
         self._solution = {
-            "assessment_id": assessment_id,
+            "assessment_sid": assessment_sid,
         }
-        self._uri = "/Insights/QM/Assessments/{assessment_id}".format(**self._solution)
+        self._uri = "/Insights/QualityManagement/Assessments/{assessment_sid}".format(
+            **self._solution
+        )
 
     def update(
         self,
         offset: float,
         answer_text: str,
         answer_id: str,
         token: Union[str, object] = values.unset,
@@ -189,15 +191,15 @@
         )
 
         payload = self._version.update(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return AssessmentsInstance(
-            self._version, payload, assessment_id=self._solution["assessment_id"]
+            self._version, payload, assessment_sid=self._solution["assessment_sid"]
         )
 
     async def update_async(
         self,
         offset: float,
         answer_text: str,
         answer_id: str,
@@ -227,15 +229,15 @@
         )
 
         payload = await self._version.update_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return AssessmentsInstance(
-            self._version, payload, assessment_id=self._solution["assessment_id"]
+            self._version, payload, assessment_sid=self._solution["assessment_sid"]
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
@@ -268,65 +270,65 @@
         Initialize the AssessmentsList
 
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
-        self._uri = "/Insights/QM/Assessments"
+        self._uri = "/Insights/QualityManagement/Assessments"
 
     def create(
         self,
-        category_id: str,
+        category_sid: str,
         category_name: str,
         segment_id: str,
         user_name: str,
         user_email: str,
         agent_id: str,
         offset: float,
         metric_id: str,
         metric_name: str,
         answer_text: str,
         answer_id: str,
-        questionnaire_id: str,
+        questionnaire_sid: str,
         token: Union[str, object] = values.unset,
     ) -> AssessmentsInstance:
         """
         Create the AssessmentsInstance
 
-        :param category_id: The id of the category
+        :param category_sid: The SID of the category
         :param category_name: The name of the category
         :param segment_id: Segment Id of the conversation
         :param user_name: Name of the user assessing conversation
         :param user_email: Email of the user assessing conversation
         :param agent_id: The id of the Agent
         :param offset: The offset of the conversation.
-        :param metric_id: The question Id selected for assessment
+        :param metric_id: The question SID selected for assessment
         :param metric_name: The question name of the assessment
         :param answer_text: The answer text selected by user
         :param answer_id: The id of the answer selected by user
-        :param questionnaire_id: Questionnaire Id of the associated question
+        :param questionnaire_sid: Questionnaire SID of the associated question
         :param token: The Token HTTP request header
 
         :returns: The created AssessmentsInstance
         """
         data = values.of(
             {
-                "CategoryId": category_id,
+                "CategorySid": category_sid,
                 "CategoryName": category_name,
                 "SegmentId": segment_id,
                 "UserName": user_name,
                 "UserEmail": user_email,
                 "AgentId": agent_id,
                 "Offset": offset,
                 "MetricId": metric_id,
                 "MetricName": metric_name,
                 "AnswerText": answer_text,
                 "AnswerId": answer_id,
-                "QuestionnaireId": questionnaire_id,
+                "QuestionnaireSid": questionnaire_sid,
             }
         )
         headers = values.of(
             {
                 "Token": token,
             }
         )
@@ -334,61 +336,61 @@
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return AssessmentsInstance(self._version, payload)
 
     async def create_async(
         self,
-        category_id: str,
+        category_sid: str,
         category_name: str,
         segment_id: str,
         user_name: str,
         user_email: str,
         agent_id: str,
         offset: float,
         metric_id: str,
         metric_name: str,
         answer_text: str,
         answer_id: str,
-        questionnaire_id: str,
+        questionnaire_sid: str,
         token: Union[str, object] = values.unset,
     ) -> AssessmentsInstance:
         """
         Asynchronously create the AssessmentsInstance
 
-        :param category_id: The id of the category
+        :param category_sid: The SID of the category
         :param category_name: The name of the category
         :param segment_id: Segment Id of the conversation
         :param user_name: Name of the user assessing conversation
         :param user_email: Email of the user assessing conversation
         :param agent_id: The id of the Agent
         :param offset: The offset of the conversation.
-        :param metric_id: The question Id selected for assessment
+        :param metric_id: The question SID selected for assessment
         :param metric_name: The question name of the assessment
         :param answer_text: The answer text selected by user
         :param answer_id: The id of the answer selected by user
-        :param questionnaire_id: Questionnaire Id of the associated question
+        :param questionnaire_sid: Questionnaire SID of the associated question
         :param token: The Token HTTP request header
 
         :returns: The created AssessmentsInstance
         """
         data = values.of(
             {
-                "CategoryId": category_id,
+                "CategorySid": category_sid,
                 "CategoryName": category_name,
                 "SegmentId": segment_id,
                 "UserName": user_name,
                 "UserEmail": user_email,
                 "AgentId": agent_id,
                 "Offset": offset,
                 "MetricId": metric_id,
                 "MetricName": metric_name,
                 "AnswerText": answer_text,
                 "AnswerId": answer_id,
-                "QuestionnaireId": questionnaire_id,
+                "QuestionnaireSid": questionnaire_sid,
             }
         )
         headers = values.of(
             {
                 "Token": token,
             }
         )
@@ -613,29 +615,29 @@
         :param target_url: API-generated URL for the requested results page
 
         :returns: Page of AssessmentsInstance
         """
         response = await self._version.domain.twilio.request_async("GET", target_url)
         return AssessmentsPage(self._version, response)
 
-    def get(self, assessment_id: str) -> AssessmentsContext:
+    def get(self, assessment_sid: str) -> AssessmentsContext:
         """
         Constructs a AssessmentsContext
 
-        :param assessment_id: The id of the assessment to be modified
+        :param assessment_sid: The SID of the assessment to be modified
         """
-        return AssessmentsContext(self._version, assessment_id=assessment_id)
+        return AssessmentsContext(self._version, assessment_sid=assessment_sid)
 
-    def __call__(self, assessment_id: str) -> AssessmentsContext:
+    def __call__(self, assessment_sid: str) -> AssessmentsContext:
         """
         Constructs a AssessmentsContext
 
-        :param assessment_id: The id of the assessment to be modified
+        :param assessment_sid: The SID of the assessment to be modified
         """
-        return AssessmentsContext(self._version, assessment_id=assessment_id)
+        return AssessmentsContext(self._version, assessment_sid=assessment_sid)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
```

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/channel.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/configuration.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/flex_flow.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/flex_flow.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/insights_assessments_comment.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/insights_assessments_comment.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from twilio.base.page import Page
 
 
 class InsightsAssessmentsCommentInstance(InstanceResource):
 
     """
     :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Flex Insights resource and owns this resource.
-    :ivar assessment_id: The unique ID of the assessment.
+    :ivar assessment_sid: The SID of the assessment.
     :ivar comment: The comment added for assessment.
     :ivar offset: The offset
     :ivar report: The flag indicating if this assessment is part of report
     :ivar weight: The weightage given to this comment
     :ivar agent_id: The id of the agent.
     :ivar segment_id: The id of the segment.
     :ivar user_name: The name of the user.
@@ -39,15 +39,15 @@
     :ivar url:
     """
 
     def __init__(self, version: Version, payload: Dict[str, Any]):
         super().__init__(version)
 
         self.account_sid: Optional[str] = payload.get("account_sid")
-        self.assessment_id: Optional[str] = payload.get("assessment_id")
+        self.assessment_sid: Optional[str] = payload.get("assessment_sid")
         self.comment: Optional[Dict[str, object]] = payload.get("comment")
         self.offset: Optional[float] = deserialize.decimal(payload.get("offset"))
         self.report: Optional[bool] = payload.get("report")
         self.weight: Optional[float] = deserialize.decimal(payload.get("weight"))
         self.agent_id: Optional[str] = payload.get("agent_id")
         self.segment_id: Optional[str] = payload.get("segment_id")
         self.user_name: Optional[str] = payload.get("user_name")
@@ -91,15 +91,15 @@
         Initialize the InsightsAssessmentsCommentList
 
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
-        self._uri = "/Insights/QM/Assessments/Comments"
+        self._uri = "/Insights/QualityManagement/Assessments/Comments"
 
     def create(
         self,
         category_id: str,
         category_name: str,
         comment: str,
         segment_id: str,
```

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/insights_conversations.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/insights_conversations.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/insights_questionnaires.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/insights_questionnaires.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,52 +22,55 @@
 from twilio.base.page import Page
 
 
 class InsightsQuestionnairesInstance(InstanceResource):
 
     """
     :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Flex Insights resource and owns this resource.
-    :ivar id: The unique id of this questionnaire
+    :ivar questionnaire_sid: The sid of this questionnaire
     :ivar name: The name of this category.
     :ivar description: The description of this questionnaire
     :ivar active: The flag to enable or disable questionnaire
     :ivar questions: The list of questions with category for a questionnaire
     :ivar url:
     """
 
     def __init__(
-        self, version: Version, payload: Dict[str, Any], id: Optional[str] = None
+        self,
+        version: Version,
+        payload: Dict[str, Any],
+        questionnaire_sid: Optional[str] = None,
     ):
         super().__init__(version)
 
         self.account_sid: Optional[str] = payload.get("account_sid")
-        self.id: Optional[str] = payload.get("id")
+        self.questionnaire_sid: Optional[str] = payload.get("questionnaire_sid")
         self.name: Optional[str] = payload.get("name")
         self.description: Optional[str] = payload.get("description")
         self.active: Optional[bool] = payload.get("active")
         self.questions: Optional[List[object]] = payload.get("questions")
         self.url: Optional[str] = payload.get("url")
 
         self._solution = {
-            "id": id or self.id,
+            "questionnaire_sid": questionnaire_sid or self.questionnaire_sid,
         }
         self._context: Optional[InsightsQuestionnairesContext] = None
 
     @property
     def _proxy(self) -> "InsightsQuestionnairesContext":
         """
         Generate an instance context for the instance, the context is capable of
         performing various actions. All instance actions are proxied to the context
 
         :returns: InsightsQuestionnairesContext for this InsightsQuestionnairesInstance
         """
         if self._context is None:
             self._context = InsightsQuestionnairesContext(
                 self._version,
-                id=self._solution["id"],
+                questionnaire_sid=self._solution["questionnaire_sid"],
             )
         return self._context
 
     def delete(self, token: Union[str, object] = values.unset) -> bool:
         """
         Deletes the InsightsQuestionnairesInstance
 
@@ -121,87 +124,91 @@
 
     def update(
         self,
         active: bool,
         token: Union[str, object] = values.unset,
         name: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
-        question_ids: Union[List[str], object] = values.unset,
+        question_sids: Union[List[str], object] = values.unset,
     ) -> "InsightsQuestionnairesInstance":
         """
         Update the InsightsQuestionnairesInstance
 
         :param active: The flag to enable or disable questionnaire
         :param token: The Token HTTP request header
         :param name: The name of this questionnaire
         :param description: The description of this questionnaire
-        :param question_ids: The list of questions ids under a questionnaire
+        :param question_sids: The list of questions sids under a questionnaire
 
         :returns: The updated InsightsQuestionnairesInstance
         """
         return self._proxy.update(
             active=active,
             token=token,
             name=name,
             description=description,
-            question_ids=question_ids,
+            question_sids=question_sids,
         )
 
     async def update_async(
         self,
         active: bool,
         token: Union[str, object] = values.unset,
         name: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
-        question_ids: Union[List[str], object] = values.unset,
+        question_sids: Union[List[str], object] = values.unset,
     ) -> "InsightsQuestionnairesInstance":
         """
         Asynchronous coroutine to update the InsightsQuestionnairesInstance
 
         :param active: The flag to enable or disable questionnaire
         :param token: The Token HTTP request header
         :param name: The name of this questionnaire
         :param description: The description of this questionnaire
-        :param question_ids: The list of questions ids under a questionnaire
+        :param question_sids: The list of questions sids under a questionnaire
 
         :returns: The updated InsightsQuestionnairesInstance
         """
         return await self._proxy.update_async(
             active=active,
             token=token,
             name=name,
             description=description,
-            question_ids=question_ids,
+            question_sids=question_sids,
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
         return "<Twilio.FlexApi.V1.InsightsQuestionnairesInstance {}>".format(context)
 
 
 class InsightsQuestionnairesContext(InstanceContext):
-    def __init__(self, version: Version, id: str):
+    def __init__(self, version: Version, questionnaire_sid: str):
         """
         Initialize the InsightsQuestionnairesContext
 
         :param version: Version that contains the resource
-        :param id: The unique ID of the questionnaire
+        :param questionnaire_sid: The SID of the questionnaire
         """
         super().__init__(version)
 
         # Path Solution
         self._solution = {
-            "id": id,
+            "questionnaire_sid": questionnaire_sid,
         }
-        self._uri = "/Insights/QM/Questionnaires/{id}".format(**self._solution)
+        self._uri = (
+            "/Insights/QualityManagement/Questionnaires/{questionnaire_sid}".format(
+                **self._solution
+            )
+        )
 
     def delete(self, token: Union[str, object] = values.unset) -> bool:
         """
         Deletes the InsightsQuestionnairesInstance
 
         :param token: The Token HTTP request header
 
@@ -251,15 +258,15 @@
         )
 
         payload = self._version.fetch(method="GET", uri=self._uri, params=data)
 
         return InsightsQuestionnairesInstance(
             self._version,
             payload,
-            id=self._solution["id"],
+            questionnaire_sid=self._solution["questionnaire_sid"],
         )
 
     async def fetch_async(
         self, token: Union[str, object] = values.unset
     ) -> InsightsQuestionnairesInstance:
         """
         Asynchronous coroutine to fetch the InsightsQuestionnairesInstance
@@ -278,97 +285,101 @@
         payload = await self._version.fetch_async(
             method="GET", uri=self._uri, params=data
         )
 
         return InsightsQuestionnairesInstance(
             self._version,
             payload,
-            id=self._solution["id"],
+            questionnaire_sid=self._solution["questionnaire_sid"],
         )
 
     def update(
         self,
         active: bool,
         token: Union[str, object] = values.unset,
         name: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
-        question_ids: Union[List[str], object] = values.unset,
+        question_sids: Union[List[str], object] = values.unset,
     ) -> InsightsQuestionnairesInstance:
         """
         Update the InsightsQuestionnairesInstance
 
         :param active: The flag to enable or disable questionnaire
         :param token: The Token HTTP request header
         :param name: The name of this questionnaire
         :param description: The description of this questionnaire
-        :param question_ids: The list of questions ids under a questionnaire
+        :param question_sids: The list of questions sids under a questionnaire
 
         :returns: The updated InsightsQuestionnairesInstance
         """
         data = values.of(
             {
                 "Active": active,
                 "Name": name,
                 "Description": description,
-                "QuestionIds": serialize.map(question_ids, lambda e: e),
+                "QuestionSids": serialize.map(question_sids, lambda e: e),
             }
         )
         headers = values.of(
             {
                 "Token": token,
             }
         )
 
         payload = self._version.update(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsQuestionnairesInstance(
-            self._version, payload, id=self._solution["id"]
+            self._version,
+            payload,
+            questionnaire_sid=self._solution["questionnaire_sid"],
         )
 
     async def update_async(
         self,
         active: bool,
         token: Union[str, object] = values.unset,
         name: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
-        question_ids: Union[List[str], object] = values.unset,
+        question_sids: Union[List[str], object] = values.unset,
     ) -> InsightsQuestionnairesInstance:
         """
         Asynchronous coroutine to update the InsightsQuestionnairesInstance
 
         :param active: The flag to enable or disable questionnaire
         :param token: The Token HTTP request header
         :param name: The name of this questionnaire
         :param description: The description of this questionnaire
-        :param question_ids: The list of questions ids under a questionnaire
+        :param question_sids: The list of questions sids under a questionnaire
 
         :returns: The updated InsightsQuestionnairesInstance
         """
         data = values.of(
             {
                 "Active": active,
                 "Name": name,
                 "Description": description,
-                "QuestionIds": serialize.map(question_ids, lambda e: e),
+                "QuestionSids": serialize.map(question_sids, lambda e: e),
             }
         )
         headers = values.of(
             {
                 "Token": token,
             }
         )
 
         payload = await self._version.update_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsQuestionnairesInstance(
-            self._version, payload, id=self._solution["id"]
+            self._version,
+            payload,
+            questionnaire_sid=self._solution["questionnaire_sid"],
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
@@ -401,41 +412,41 @@
         Initialize the InsightsQuestionnairesList
 
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
-        self._uri = "/Insights/QM/Questionnaires"
+        self._uri = "/Insights/QualityManagement/Questionnaires"
 
     def create(
         self,
         name: str,
         token: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         active: Union[bool, object] = values.unset,
-        question_ids: Union[List[str], object] = values.unset,
+        question_sids: Union[List[str], object] = values.unset,
     ) -> InsightsQuestionnairesInstance:
         """
         Create the InsightsQuestionnairesInstance
 
         :param name: The name of this questionnaire
         :param token: The Token HTTP request header
         :param description: The description of this questionnaire
         :param active: The flag to enable or disable questionnaire
-        :param question_ids: The list of questions ids under a questionnaire
+        :param question_sids: The list of questions sids under a questionnaire
 
         :returns: The created InsightsQuestionnairesInstance
         """
         data = values.of(
             {
                 "Name": name,
                 "Description": description,
                 "Active": active,
-                "QuestionIds": serialize.map(question_ids, lambda e: e),
+                "QuestionSids": serialize.map(question_sids, lambda e: e),
             }
         )
         headers = values.of(
             {
                 "Token": token,
             }
         )
@@ -447,33 +458,33 @@
 
     async def create_async(
         self,
         name: str,
         token: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         active: Union[bool, object] = values.unset,
-        question_ids: Union[List[str], object] = values.unset,
+        question_sids: Union[List[str], object] = values.unset,
     ) -> InsightsQuestionnairesInstance:
         """
         Asynchronously create the InsightsQuestionnairesInstance
 
         :param name: The name of this questionnaire
         :param token: The Token HTTP request header
         :param description: The description of this questionnaire
         :param active: The flag to enable or disable questionnaire
-        :param question_ids: The list of questions ids under a questionnaire
+        :param question_sids: The list of questions sids under a questionnaire
 
         :returns: The created InsightsQuestionnairesInstance
         """
         data = values.of(
             {
                 "Name": name,
                 "Description": description,
                 "Active": active,
-                "QuestionIds": serialize.map(question_ids, lambda e: e),
+                "QuestionSids": serialize.map(question_sids, lambda e: e),
             }
         )
         headers = values.of(
             {
                 "Token": token,
             }
         )
@@ -702,29 +713,33 @@
         :param target_url: API-generated URL for the requested results page
 
         :returns: Page of InsightsQuestionnairesInstance
         """
         response = await self._version.domain.twilio.request_async("GET", target_url)
         return InsightsQuestionnairesPage(self._version, response)
 
-    def get(self, id: str) -> InsightsQuestionnairesContext:
+    def get(self, questionnaire_sid: str) -> InsightsQuestionnairesContext:
         """
         Constructs a InsightsQuestionnairesContext
 
-        :param id: The unique ID of the questionnaire
+        :param questionnaire_sid: The SID of the questionnaire
         """
-        return InsightsQuestionnairesContext(self._version, id=id)
+        return InsightsQuestionnairesContext(
+            self._version, questionnaire_sid=questionnaire_sid
+        )
 
-    def __call__(self, id: str) -> InsightsQuestionnairesContext:
+    def __call__(self, questionnaire_sid: str) -> InsightsQuestionnairesContext:
         """
         Constructs a InsightsQuestionnairesContext
 
-        :param id: The unique ID of the questionnaire
+        :param questionnaire_sid: The SID of the questionnaire
         """
-        return InsightsQuestionnairesContext(self._version, id=id)
+        return InsightsQuestionnairesContext(
+            self._version, questionnaire_sid=questionnaire_sid
+        )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
```

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,49 +22,49 @@
 from twilio.base.page import Page
 
 
 class InsightsQuestionnairesCategoryInstance(InstanceResource):
 
     """
     :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Flex Insights resource and owns this resource.
-    :ivar category_id: The unique ID for the category
+    :ivar category_sid: The SID of the category
     :ivar name: The name of this category.
     :ivar url:
     """
 
     def __init__(
         self,
         version: Version,
         payload: Dict[str, Any],
-        category_id: Optional[str] = None,
+        category_sid: Optional[str] = None,
     ):
         super().__init__(version)
 
         self.account_sid: Optional[str] = payload.get("account_sid")
-        self.category_id: Optional[str] = payload.get("category_id")
+        self.category_sid: Optional[str] = payload.get("category_sid")
         self.name: Optional[str] = payload.get("name")
         self.url: Optional[str] = payload.get("url")
 
         self._solution = {
-            "category_id": category_id or self.category_id,
+            "category_sid": category_sid or self.category_sid,
         }
         self._context: Optional[InsightsQuestionnairesCategoryContext] = None
 
     @property
     def _proxy(self) -> "InsightsQuestionnairesCategoryContext":
         """
         Generate an instance context for the instance, the context is capable of
         performing various actions. All instance actions are proxied to the context
 
         :returns: InsightsQuestionnairesCategoryContext for this InsightsQuestionnairesCategoryInstance
         """
         if self._context is None:
             self._context = InsightsQuestionnairesCategoryContext(
                 self._version,
-                category_id=self._solution["category_id"],
+                category_sid=self._solution["category_sid"],
             )
         return self._context
 
     def delete(self, token: Union[str, object] = values.unset) -> bool:
         """
         Deletes the InsightsQuestionnairesCategoryInstance
 
@@ -129,28 +129,30 @@
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
         return "<Twilio.FlexApi.V1.InsightsQuestionnairesCategoryInstance {}>".format(
             context
         )
 
 
 class InsightsQuestionnairesCategoryContext(InstanceContext):
-    def __init__(self, version: Version, category_id: str):
+    def __init__(self, version: Version, category_sid: str):
         """
         Initialize the InsightsQuestionnairesCategoryContext
 
         :param version: Version that contains the resource
-        :param category_id: The ID of the category to be update
+        :param category_sid: The SID of the category to be updated
         """
         super().__init__(version)
 
         # Path Solution
         self._solution = {
-            "category_id": category_id,
+            "category_sid": category_sid,
         }
-        self._uri = "/Insights/QM/Categories/{category_id}".format(**self._solution)
+        self._uri = "/Insights/QualityManagement/Categories/{category_sid}".format(
+            **self._solution
+        )
 
     def delete(self, token: Union[str, object] = values.unset) -> bool:
         """
         Deletes the InsightsQuestionnairesCategoryInstance
 
         :param token: The Token HTTP request header
 
@@ -205,15 +207,15 @@
         )
 
         payload = self._version.update(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsQuestionnairesCategoryInstance(
-            self._version, payload, category_id=self._solution["category_id"]
+            self._version, payload, category_sid=self._solution["category_sid"]
         )
 
     async def update_async(
         self, name: str, token: Union[str, object] = values.unset
     ) -> InsightsQuestionnairesCategoryInstance:
         """
         Asynchronous coroutine to update the InsightsQuestionnairesCategoryInstance
@@ -235,15 +237,15 @@
         )
 
         payload = await self._version.update_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsQuestionnairesCategoryInstance(
-            self._version, payload, category_id=self._solution["category_id"]
+            self._version, payload, category_sid=self._solution["category_sid"]
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
@@ -280,15 +282,15 @@
         Initialize the InsightsQuestionnairesCategoryList
 
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
-        self._uri = "/Insights/QM/Categories"
+        self._uri = "/Insights/QualityManagement/Categories"
 
     def create(
         self, name: str, token: Union[str, object] = values.unset
     ) -> InsightsQuestionnairesCategoryInstance:
         """
         Create the InsightsQuestionnairesCategoryInstance
 
@@ -537,32 +539,32 @@
         :param target_url: API-generated URL for the requested results page
 
         :returns: Page of InsightsQuestionnairesCategoryInstance
         """
         response = await self._version.domain.twilio.request_async("GET", target_url)
         return InsightsQuestionnairesCategoryPage(self._version, response)
 
-    def get(self, category_id: str) -> InsightsQuestionnairesCategoryContext:
+    def get(self, category_sid: str) -> InsightsQuestionnairesCategoryContext:
         """
         Constructs a InsightsQuestionnairesCategoryContext
 
-        :param category_id: The ID of the category to be update
+        :param category_sid: The SID of the category to be updated
         """
         return InsightsQuestionnairesCategoryContext(
-            self._version, category_id=category_id
+            self._version, category_sid=category_sid
         )
 
-    def __call__(self, category_id: str) -> InsightsQuestionnairesCategoryContext:
+    def __call__(self, category_sid: str) -> InsightsQuestionnairesCategoryContext:
         """
         Constructs a InsightsQuestionnairesCategoryContext
 
-        :param category_id: The ID of the category to be update
+        :param category_sid: The SID of the category to be updated
         """
         return InsightsQuestionnairesCategoryContext(
-            self._version, category_id=category_id
+            self._version, category_sid=category_sid
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
```

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,61 +22,61 @@
 from twilio.base.page import Page
 
 
 class InsightsQuestionnairesQuestionInstance(InstanceResource):
 
     """
     :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Flex Insights resource and owns this resource.
-    :ivar question_id: The unique ID of the question
+    :ivar question_sid: The SID of the question
     :ivar question: The question.
     :ivar description: The description for the question.
     :ivar category: The Category for the question.
     :ivar answer_set_id: The answer_set for the question.
     :ivar allow_na: The flag  to enable for disable NA for answer.
     :ivar usage: Integer value that tells a particular question is used by how many questionnaires
     :ivar answer_set: Set of answers for the question
     :ivar url:
     """
 
     def __init__(
         self,
         version: Version,
         payload: Dict[str, Any],
-        question_id: Optional[str] = None,
+        question_sid: Optional[str] = None,
     ):
         super().__init__(version)
 
         self.account_sid: Optional[str] = payload.get("account_sid")
-        self.question_id: Optional[str] = payload.get("question_id")
+        self.question_sid: Optional[str] = payload.get("question_sid")
         self.question: Optional[str] = payload.get("question")
         self.description: Optional[str] = payload.get("description")
         self.category: Optional[Dict[str, object]] = payload.get("category")
         self.answer_set_id: Optional[str] = payload.get("answer_set_id")
         self.allow_na: Optional[bool] = payload.get("allow_na")
         self.usage: Optional[int] = deserialize.integer(payload.get("usage"))
         self.answer_set: Optional[Dict[str, object]] = payload.get("answer_set")
         self.url: Optional[str] = payload.get("url")
 
         self._solution = {
-            "question_id": question_id or self.question_id,
+            "question_sid": question_sid or self.question_sid,
         }
         self._context: Optional[InsightsQuestionnairesQuestionContext] = None
 
     @property
     def _proxy(self) -> "InsightsQuestionnairesQuestionContext":
         """
         Generate an instance context for the instance, the context is capable of
         performing various actions. All instance actions are proxied to the context
 
         :returns: InsightsQuestionnairesQuestionContext for this InsightsQuestionnairesQuestionInstance
         """
         if self._context is None:
             self._context = InsightsQuestionnairesQuestionContext(
                 self._version,
-                question_id=self._solution["question_id"],
+                question_sid=self._solution["question_sid"],
             )
         return self._context
 
     def delete(self, token: Union[str, object] = values.unset) -> bool:
         """
         Deletes the InsightsQuestionnairesQuestionInstance
 
@@ -100,65 +100,65 @@
             token=token,
         )
 
     def update(
         self,
         allow_na: bool,
         token: Union[str, object] = values.unset,
-        category_id: Union[str, object] = values.unset,
+        category_sid: Union[str, object] = values.unset,
         question: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         answer_set_id: Union[str, object] = values.unset,
     ) -> "InsightsQuestionnairesQuestionInstance":
         """
         Update the InsightsQuestionnairesQuestionInstance
 
         :param allow_na: The flag to enable for disable NA for answer.
         :param token: The Token HTTP request header
-        :param category_id: The ID of the category
+        :param category_sid: The SID of the category
         :param question: The question.
         :param description: The description for the question.
         :param answer_set_id: The answer_set for the question.
 
         :returns: The updated InsightsQuestionnairesQuestionInstance
         """
         return self._proxy.update(
             allow_na=allow_na,
             token=token,
-            category_id=category_id,
+            category_sid=category_sid,
             question=question,
             description=description,
             answer_set_id=answer_set_id,
         )
 
     async def update_async(
         self,
         allow_na: bool,
         token: Union[str, object] = values.unset,
-        category_id: Union[str, object] = values.unset,
+        category_sid: Union[str, object] = values.unset,
         question: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         answer_set_id: Union[str, object] = values.unset,
     ) -> "InsightsQuestionnairesQuestionInstance":
         """
         Asynchronous coroutine to update the InsightsQuestionnairesQuestionInstance
 
         :param allow_na: The flag to enable for disable NA for answer.
         :param token: The Token HTTP request header
-        :param category_id: The ID of the category
+        :param category_sid: The SID of the category
         :param question: The question.
         :param description: The description for the question.
         :param answer_set_id: The answer_set for the question.
 
         :returns: The updated InsightsQuestionnairesQuestionInstance
         """
         return await self._proxy.update_async(
             allow_na=allow_na,
             token=token,
-            category_id=category_id,
+            category_sid=category_sid,
             question=question,
             description=description,
             answer_set_id=answer_set_id,
         )
 
     def __repr__(self) -> str:
         """
@@ -169,28 +169,30 @@
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
         return "<Twilio.FlexApi.V1.InsightsQuestionnairesQuestionInstance {}>".format(
             context
         )
 
 
 class InsightsQuestionnairesQuestionContext(InstanceContext):
-    def __init__(self, version: Version, question_id: str):
+    def __init__(self, version: Version, question_sid: str):
         """
         Initialize the InsightsQuestionnairesQuestionContext
 
         :param version: Version that contains the resource
-        :param question_id: The unique ID of the question
+        :param question_sid: The SID of the question
         """
         super().__init__(version)
 
         # Path Solution
         self._solution = {
-            "question_id": question_id,
+            "question_sid": question_sid,
         }
-        self._uri = "/Insights/QM/Questions/{question_id}".format(**self._solution)
+        self._uri = "/Insights/QualityManagement/Questions/{question_sid}".format(
+            **self._solution
+        )
 
     def delete(self, token: Union[str, object] = values.unset) -> bool:
         """
         Deletes the InsightsQuestionnairesQuestionInstance
 
         :param token: The Token HTTP request header
 
@@ -222,35 +224,35 @@
             method="DELETE", uri=self._uri, headers=headers
         )
 
     def update(
         self,
         allow_na: bool,
         token: Union[str, object] = values.unset,
-        category_id: Union[str, object] = values.unset,
+        category_sid: Union[str, object] = values.unset,
         question: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         answer_set_id: Union[str, object] = values.unset,
     ) -> InsightsQuestionnairesQuestionInstance:
         """
         Update the InsightsQuestionnairesQuestionInstance
 
         :param allow_na: The flag to enable for disable NA for answer.
         :param token: The Token HTTP request header
-        :param category_id: The ID of the category
+        :param category_sid: The SID of the category
         :param question: The question.
         :param description: The description for the question.
         :param answer_set_id: The answer_set for the question.
 
         :returns: The updated InsightsQuestionnairesQuestionInstance
         """
         data = values.of(
             {
                 "AllowNa": allow_na,
-                "CategoryId": category_id,
+                "CategorySid": category_sid,
                 "Question": question,
                 "Description": description,
                 "AnswerSetId": answer_set_id,
             }
         )
         headers = values.of(
             {
@@ -259,42 +261,42 @@
         )
 
         payload = self._version.update(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsQuestionnairesQuestionInstance(
-            self._version, payload, question_id=self._solution["question_id"]
+            self._version, payload, question_sid=self._solution["question_sid"]
         )
 
     async def update_async(
         self,
         allow_na: bool,
         token: Union[str, object] = values.unset,
-        category_id: Union[str, object] = values.unset,
+        category_sid: Union[str, object] = values.unset,
         question: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         answer_set_id: Union[str, object] = values.unset,
     ) -> InsightsQuestionnairesQuestionInstance:
         """
         Asynchronous coroutine to update the InsightsQuestionnairesQuestionInstance
 
         :param allow_na: The flag to enable for disable NA for answer.
         :param token: The Token HTTP request header
-        :param category_id: The ID of the category
+        :param category_sid: The SID of the category
         :param question: The question.
         :param description: The description for the question.
         :param answer_set_id: The answer_set for the question.
 
         :returns: The updated InsightsQuestionnairesQuestionInstance
         """
         data = values.of(
             {
                 "AllowNa": allow_na,
-                "CategoryId": category_id,
+                "CategorySid": category_sid,
                 "Question": question,
                 "Description": description,
                 "AnswerSetId": answer_set_id,
             }
         )
         headers = values.of(
             {
@@ -303,15 +305,15 @@
         )
 
         payload = await self._version.update_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsQuestionnairesQuestionInstance(
-            self._version, payload, question_id=self._solution["question_id"]
+            self._version, payload, question_sid=self._solution["question_sid"]
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
@@ -348,40 +350,40 @@
         Initialize the InsightsQuestionnairesQuestionList
 
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
-        self._uri = "/Insights/QM/Questions"
+        self._uri = "/Insights/QualityManagement/Questions"
 
     def create(
         self,
-        category_id: str,
+        category_sid: str,
         question: str,
         answer_set_id: str,
         allow_na: bool,
         token: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
     ) -> InsightsQuestionnairesQuestionInstance:
         """
         Create the InsightsQuestionnairesQuestionInstance
 
-        :param category_id: The ID of the category
+        :param category_sid: The SID of the category
         :param question: The question.
         :param answer_set_id: The answer_set for the question.
         :param allow_na: The flag to enable for disable NA for answer.
         :param token: The Token HTTP request header
         :param description: The description for the question.
 
         :returns: The created InsightsQuestionnairesQuestionInstance
         """
         data = values.of(
             {
-                "CategoryId": category_id,
+                "CategorySid": category_sid,
                 "Question": question,
                 "AnswerSetId": answer_set_id,
                 "AllowNa": allow_na,
                 "Description": description,
             }
         )
         headers = values.of(
@@ -393,36 +395,36 @@
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsQuestionnairesQuestionInstance(self._version, payload)
 
     async def create_async(
         self,
-        category_id: str,
+        category_sid: str,
         question: str,
         answer_set_id: str,
         allow_na: bool,
         token: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
     ) -> InsightsQuestionnairesQuestionInstance:
         """
         Asynchronously create the InsightsQuestionnairesQuestionInstance
 
-        :param category_id: The ID of the category
+        :param category_sid: The SID of the category
         :param question: The question.
         :param answer_set_id: The answer_set for the question.
         :param allow_na: The flag to enable for disable NA for answer.
         :param token: The Token HTTP request header
         :param description: The description for the question.
 
         :returns: The created InsightsQuestionnairesQuestionInstance
         """
         data = values.of(
             {
-                "CategoryId": category_id,
+                "CategorySid": category_sid,
                 "Question": question,
                 "AnswerSetId": answer_set_id,
                 "AllowNa": allow_na,
                 "Description": description,
             }
         )
         headers = values.of(
@@ -435,195 +437,195 @@
         )
 
         return InsightsQuestionnairesQuestionInstance(self._version, payload)
 
     def stream(
         self,
         token: Union[str, object] = values.unset,
-        category_id: Union[List[str], object] = values.unset,
+        category_sid: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[InsightsQuestionnairesQuestionInstance]:
         """
         Streams InsightsQuestionnairesQuestionInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
         :param str token: The Token HTTP request header
-        :param List[str] category_id: The list of category IDs
+        :param List[str] category_sid: The list of category SIDs
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = self.page(
-            token=token, category_id=category_id, page_size=limits["page_size"]
+            token=token, category_sid=category_sid, page_size=limits["page_size"]
         )
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
         token: Union[str, object] = values.unset,
-        category_id: Union[List[str], object] = values.unset,
+        category_sid: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[InsightsQuestionnairesQuestionInstance]:
         """
         Asynchronously streams InsightsQuestionnairesQuestionInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
         :param str token: The Token HTTP request header
-        :param List[str] category_id: The list of category IDs
+        :param List[str] category_sid: The list of category SIDs
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = await self.page_async(
-            token=token, category_id=category_id, page_size=limits["page_size"]
+            token=token, category_sid=category_sid, page_size=limits["page_size"]
         )
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
         token: Union[str, object] = values.unset,
-        category_id: Union[List[str], object] = values.unset,
+        category_sid: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsQuestionnairesQuestionInstance]:
         """
         Lists InsightsQuestionnairesQuestionInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
         :param str token: The Token HTTP request header
-        :param List[str] category_id: The list of category IDs
+        :param List[str] category_sid: The list of category SIDs
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return list(
             self.stream(
                 token=token,
-                category_id=category_id,
+                category_sid=category_sid,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
         token: Union[str, object] = values.unset,
-        category_id: Union[List[str], object] = values.unset,
+        category_sid: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsQuestionnairesQuestionInstance]:
         """
         Asynchronously lists InsightsQuestionnairesQuestionInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
         :param str token: The Token HTTP request header
-        :param List[str] category_id: The list of category IDs
+        :param List[str] category_sid: The list of category SIDs
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return [
             record
             async for record in await self.stream_async(
                 token=token,
-                category_id=category_id,
+                category_sid=category_sid,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
         token: Union[str, object] = values.unset,
-        category_id: Union[List[str], object] = values.unset,
+        category_sid: Union[List[str], object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsQuestionnairesQuestionPage:
         """
         Retrieve a single page of InsightsQuestionnairesQuestionInstance records from the API.
         Request is executed immediately
 
         :param token: The Token HTTP request header
-        :param category_id: The list of category IDs
+        :param category_sid: The list of category SIDs
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsQuestionnairesQuestionInstance
         """
         data = values.of(
             {
                 "Token": token,
-                "CategoryId": serialize.map(category_id, lambda e: e),
+                "CategorySid": serialize.map(category_sid, lambda e: e),
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
         return InsightsQuestionnairesQuestionPage(self._version, response)
 
     async def page_async(
         self,
         token: Union[str, object] = values.unset,
-        category_id: Union[List[str], object] = values.unset,
+        category_sid: Union[List[str], object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsQuestionnairesQuestionPage:
         """
         Asynchronously retrieve a single page of InsightsQuestionnairesQuestionInstance records from the API.
         Request is executed immediately
 
         :param token: The Token HTTP request header
-        :param category_id: The list of category IDs
+        :param category_sid: The list of category SIDs
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsQuestionnairesQuestionInstance
         """
         data = values.of(
             {
                 "Token": token,
-                "CategoryId": serialize.map(category_id, lambda e: e),
+                "CategorySid": serialize.map(category_sid, lambda e: e),
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = await self._version.page_async(
@@ -653,32 +655,32 @@
         :param target_url: API-generated URL for the requested results page
 
         :returns: Page of InsightsQuestionnairesQuestionInstance
         """
         response = await self._version.domain.twilio.request_async("GET", target_url)
         return InsightsQuestionnairesQuestionPage(self._version, response)
 
-    def get(self, question_id: str) -> InsightsQuestionnairesQuestionContext:
+    def get(self, question_sid: str) -> InsightsQuestionnairesQuestionContext:
         """
         Constructs a InsightsQuestionnairesQuestionContext
 
-        :param question_id: The unique ID of the question
+        :param question_sid: The SID of the question
         """
         return InsightsQuestionnairesQuestionContext(
-            self._version, question_id=question_id
+            self._version, question_sid=question_sid
         )
 
-    def __call__(self, question_id: str) -> InsightsQuestionnairesQuestionContext:
+    def __call__(self, question_sid: str) -> InsightsQuestionnairesQuestionContext:
         """
         Constructs a InsightsQuestionnairesQuestionContext
 
-        :param question_id: The unique ID of the question
+        :param question_sid: The SID of the question
         """
         return InsightsQuestionnairesQuestionContext(
-            self._version, question_id=question_id
+            self._version, question_sid=question_sid
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
```

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/insights_segments.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/insights_segments.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
 
 from typing import Any, Dict, List, Optional, Union, Iterator, AsyncIterator
 from twilio.base import serialize, values
-from twilio.base.instance_context import InstanceContext
+
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 from twilio.base.page import Page
 
 
 class InsightsSegmentsInstance(InstanceResource):
@@ -45,20 +45,15 @@
     :ivar segment_recording_offset: The offset value for the recording.
     :ivar media: The media identifiers of the conversation.
     :ivar assessment_type: The type of the assessment.
     :ivar assessment_percentage: The percentage scored on the Assessments.
     :ivar url:
     """
 
-    def __init__(
-        self,
-        version: Version,
-        payload: Dict[str, Any],
-        segment_id: Optional[str] = None,
-    ):
+    def __init__(self, version: Version, payload: Dict[str, Any]):
         super().__init__(version)
 
         self.segment_id: Optional[str] = payload.get("segment_id")
         self.external_id: Optional[str] = payload.get("external_id")
         self.queue: Optional[str] = payload.get("queue")
         self.external_contact: Optional[str] = payload.get("external_contact")
         self.external_segment_link_id: Optional[str] = payload.get(
@@ -86,148 +81,22 @@
             "assessment_type"
         )
         self.assessment_percentage: Optional[Dict[str, object]] = payload.get(
             "assessment_percentage"
         )
         self.url: Optional[str] = payload.get("url")
 
-        self._solution = {
-            "segment_id": segment_id or self.segment_id,
-        }
-        self._context: Optional[InsightsSegmentsContext] = None
-
-    @property
-    def _proxy(self) -> "InsightsSegmentsContext":
-        """
-        Generate an instance context for the instance, the context is capable of
-        performing various actions. All instance actions are proxied to the context
-
-        :returns: InsightsSegmentsContext for this InsightsSegmentsInstance
-        """
-        if self._context is None:
-            self._context = InsightsSegmentsContext(
-                self._version,
-                segment_id=self._solution["segment_id"],
-            )
-        return self._context
-
-    def fetch(
-        self, token: Union[str, object] = values.unset
-    ) -> "InsightsSegmentsInstance":
-        """
-        Fetch the InsightsSegmentsInstance
-
-        :param token: The Token HTTP request header
-
-        :returns: The fetched InsightsSegmentsInstance
-        """
-        return self._proxy.fetch(
-            token=token,
-        )
-
-    async def fetch_async(
-        self, token: Union[str, object] = values.unset
-    ) -> "InsightsSegmentsInstance":
-        """
-        Asynchronous coroutine to fetch the InsightsSegmentsInstance
-
-        :param token: The Token HTTP request header
-
-        :returns: The fetched InsightsSegmentsInstance
-        """
-        return await self._proxy.fetch_async(
-            token=token,
-        )
-
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.FlexApi.V1.InsightsSegmentsInstance {}>".format(context)
-
-
-class InsightsSegmentsContext(InstanceContext):
-    def __init__(self, version: Version, segment_id: str):
-        """
-        Initialize the InsightsSegmentsContext
-
-        :param version: Version that contains the resource
-        :param segment_id: To unique id of the segment
-        """
-        super().__init__(version)
-
-        # Path Solution
-        self._solution = {
-            "segment_id": segment_id,
-        }
-        self._uri = "/Insights/Segments/{segment_id}".format(**self._solution)
-
-    def fetch(
-        self, token: Union[str, object] = values.unset
-    ) -> InsightsSegmentsInstance:
-        """
-        Fetch the InsightsSegmentsInstance
-
-        :param token: The Token HTTP request header
-
-        :returns: The fetched InsightsSegmentsInstance
-        """
-
-        data = values.of(
-            {
-                "Token": token,
-            }
-        )
-
-        payload = self._version.fetch(method="GET", uri=self._uri, params=data)
-
-        return InsightsSegmentsInstance(
-            self._version,
-            payload,
-            segment_id=self._solution["segment_id"],
-        )
-
-    async def fetch_async(
-        self, token: Union[str, object] = values.unset
-    ) -> InsightsSegmentsInstance:
-        """
-        Asynchronous coroutine to fetch the InsightsSegmentsInstance
-
-        :param token: The Token HTTP request header
-
-        :returns: The fetched InsightsSegmentsInstance
-        """
-
-        data = values.of(
-            {
-                "Token": token,
-            }
-        )
-
-        payload = await self._version.fetch_async(
-            method="GET", uri=self._uri, params=data
-        )
-
-        return InsightsSegmentsInstance(
-            self._version,
-            payload,
-            segment_id=self._solution["segment_id"],
-        )
-
-    def __repr__(self) -> str:
-        """
-        Provide a friendly representation
 
-        :returns: Machine friendly representation
-        """
-        context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.FlexApi.V1.InsightsSegmentsContext {}>".format(context)
+        return "<Twilio.FlexApi.V1.InsightsSegmentsInstance>"
 
 
 class InsightsSegmentsPage(Page):
     def get_instance(self, payload: Dict[str, Any]) -> InsightsSegmentsInstance:
         """
         Build an instance of InsightsSegmentsInstance
 
@@ -255,194 +124,216 @@
         super().__init__(version)
 
         self._uri = "/Insights/Segments"
 
     def stream(
         self,
         token: Union[str, object] = values.unset,
+        segment_id: Union[str, object] = values.unset,
         reservation_id: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[InsightsSegmentsInstance]:
         """
         Streams InsightsSegmentsInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
         :param str token: The Token HTTP request header
+        :param str segment_id: To unique id of the segment
         :param List[str] reservation_id: The list of reservation Ids
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = self.page(
-            token=token, reservation_id=reservation_id, page_size=limits["page_size"]
+            token=token,
+            segment_id=segment_id,
+            reservation_id=reservation_id,
+            page_size=limits["page_size"],
         )
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
         token: Union[str, object] = values.unset,
+        segment_id: Union[str, object] = values.unset,
         reservation_id: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[InsightsSegmentsInstance]:
         """
         Asynchronously streams InsightsSegmentsInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
         :param str token: The Token HTTP request header
+        :param str segment_id: To unique id of the segment
         :param List[str] reservation_id: The list of reservation Ids
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = await self.page_async(
-            token=token, reservation_id=reservation_id, page_size=limits["page_size"]
+            token=token,
+            segment_id=segment_id,
+            reservation_id=reservation_id,
+            page_size=limits["page_size"],
         )
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
         token: Union[str, object] = values.unset,
+        segment_id: Union[str, object] = values.unset,
         reservation_id: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsSegmentsInstance]:
         """
         Lists InsightsSegmentsInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
         :param str token: The Token HTTP request header
+        :param str segment_id: To unique id of the segment
         :param List[str] reservation_id: The list of reservation Ids
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return list(
             self.stream(
                 token=token,
+                segment_id=segment_id,
                 reservation_id=reservation_id,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
         token: Union[str, object] = values.unset,
+        segment_id: Union[str, object] = values.unset,
         reservation_id: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsSegmentsInstance]:
         """
         Asynchronously lists InsightsSegmentsInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
         :param str token: The Token HTTP request header
+        :param str segment_id: To unique id of the segment
         :param List[str] reservation_id: The list of reservation Ids
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return [
             record
             async for record in await self.stream_async(
                 token=token,
+                segment_id=segment_id,
                 reservation_id=reservation_id,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
         token: Union[str, object] = values.unset,
+        segment_id: Union[str, object] = values.unset,
         reservation_id: Union[List[str], object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsSegmentsPage:
         """
         Retrieve a single page of InsightsSegmentsInstance records from the API.
         Request is executed immediately
 
         :param token: The Token HTTP request header
+        :param segment_id: To unique id of the segment
         :param reservation_id: The list of reservation Ids
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsSegmentsInstance
         """
         data = values.of(
             {
                 "Token": token,
+                "SegmentId": segment_id,
                 "ReservationId": serialize.map(reservation_id, lambda e: e),
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
         return InsightsSegmentsPage(self._version, response)
 
     async def page_async(
         self,
         token: Union[str, object] = values.unset,
+        segment_id: Union[str, object] = values.unset,
         reservation_id: Union[List[str], object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsSegmentsPage:
         """
         Asynchronously retrieve a single page of InsightsSegmentsInstance records from the API.
         Request is executed immediately
 
         :param token: The Token HTTP request header
+        :param segment_id: To unique id of the segment
         :param reservation_id: The list of reservation Ids
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsSegmentsInstance
         """
         data = values.of(
             {
                 "Token": token,
+                "SegmentId": segment_id,
                 "ReservationId": serialize.map(reservation_id, lambda e: e),
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
@@ -471,30 +362,14 @@
         :param target_url: API-generated URL for the requested results page
 
         :returns: Page of InsightsSegmentsInstance
         """
         response = await self._version.domain.twilio.request_async("GET", target_url)
         return InsightsSegmentsPage(self._version, response)
 
-    def get(self, segment_id: str) -> InsightsSegmentsContext:
-        """
-        Constructs a InsightsSegmentsContext
-
-        :param segment_id: To unique id of the segment
-        """
-        return InsightsSegmentsContext(self._version, segment_id=segment_id)
-
-    def __call__(self, segment_id: str) -> InsightsSegmentsContext:
-        """
-        Constructs a InsightsSegmentsContext
-
-        :param segment_id: To unique id of the segment
-        """
-        return InsightsSegmentsContext(self._version, segment_id=segment_id)
-
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         return "<Twilio.FlexApi.V1.InsightsSegmentsList>"
```

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/insights_session.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/insights_session.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         Initialize the InsightsSettingsAnswerSetsList
 
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
-        self._uri = "/Insights/QM/Settings/AnswerSets"
+        self._uri = "/Insights/QualityManagement/Settings/AnswerSets"
 
     def fetch(self) -> InsightsSettingsAnswerSetsInstance:
         """
         Asynchronously fetch the InsightsSettingsAnswerSetsInstance
 
         :returns: The fetched InsightsSettingsAnswerSetsInstance
         """
```

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/insights_settings_comment.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/insights_settings_comment.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         Initialize the InsightsSettingsCommentList
 
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
-        self._uri = "/Insights/QM/Settings/CommentTags"
+        self._uri = "/Insights/QualityManagement/Settings/CommentTags"
 
     def fetch(self) -> InsightsSettingsCommentInstance:
         """
         Asynchronously fetch the InsightsSettingsCommentInstance
 
         :returns: The fetched InsightsSettingsCommentInstance
         """
```

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/insights_user_roles.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/insights_user_roles.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/interaction/__init__.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/interaction/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v1/web_channel.py` & `twilio-8.2.0/twilio/rest/flex_api/v1/web_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v2/__init__.py` & `twilio-8.2.0/twilio/rest/flex_api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/flex_api/v2/web_channels.py` & `twilio-8.2.0/twilio/rest/flex_api/v2/web_channels.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/frontline_api/FrontlineApiBase.py` & `twilio-8.2.0/twilio/rest/frontline_api/FrontlineApiBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/frontline_api/v1/__init__.py` & `twilio-8.2.0/twilio/rest/frontline_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/frontline_api/v1/user.py` & `twilio-8.2.0/twilio/rest/frontline_api/v1/user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/insights/InsightsBase.py` & `twilio-8.2.0/twilio/rest/insights/InsightsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/insights/__init__.py` & `twilio-8.2.0/twilio/rest/insights/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/insights/v1/__init__.py` & `twilio-8.2.0/twilio/rest/insights/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/insights/v1/call/__init__.py` & `twilio-8.2.0/twilio/rest/insights/v1/call/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/insights/v1/call/annotation.py` & `twilio-8.2.0/twilio/rest/insights/v1/call/annotation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/insights/v1/call/call_summary.py` & `twilio-8.2.0/twilio/rest/insights/v1/call/call_summary.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/insights/v1/call/event.py` & `twilio-8.2.0/twilio/rest/insights/v1/call/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/insights/v1/call/metric.py` & `twilio-8.2.0/twilio/rest/insights/v1/call/metric.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/insights/v1/call_summaries.py` & `twilio-8.2.0/twilio/rest/insights/v1/call_summaries.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/insights/v1/conference/__init__.py` & `twilio-8.2.0/twilio/rest/insights/v1/conference/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/insights/v1/conference/conference_participant.py` & `twilio-8.2.0/twilio/rest/insights/v1/conference/conference_participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/insights/v1/room/__init__.py` & `twilio-8.2.0/twilio/rest/insights/v1/room/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/insights/v1/room/participant.py` & `twilio-8.2.0/twilio/rest/insights/v1/room/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/insights/v1/setting.py` & `twilio-8.2.0/twilio/rest/insights/v1/setting.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/IpMessagingBase.py` & `twilio-8.2.0/twilio/rest/ip_messaging/IpMessagingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/__init__.py` & `twilio-8.2.0/twilio/rest/ip_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v1/__init__.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v1/credential.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v1/service/__init__.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v1/service/channel/invite.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v1/service/channel/member.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v1/service/channel/message.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v1/service/role.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v1/service/user/__init__.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v2/__init__.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v2/credential.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v2/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v2/service/__init__.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v2/service/binding.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v2/service/channel/invite.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v2/service/channel/member.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v2/service/channel/message.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v2/service/role.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v2/service/user/__init__.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py` & `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/lookups/LookupsBase.py` & `twilio-8.2.0/twilio/rest/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/lookups/v1/__init__.py` & `twilio-8.2.0/twilio/rest/lookups/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/lookups/v1/phone_number.py` & `twilio-8.2.0/twilio/rest/lookups/v1/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/lookups/v2/__init__.py` & `twilio-8.2.0/twilio/rest/lookups/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/lookups/v2/phone_number.py` & `twilio-8.2.0/twilio/rest/lookups/v2/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/media/MediaBase.py` & `twilio-8.2.0/twilio/rest/media/MediaBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/media/__init__.py` & `twilio-8.2.0/twilio/rest/media/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/media/v1/__init__.py` & `twilio-8.2.0/twilio/rest/media/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/media/v1/media_processor.py` & `twilio-8.2.0/twilio/rest/media/v1/media_processor.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/media/v1/media_recording.py` & `twilio-8.2.0/twilio/rest/media/v1/media_recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/media/v1/player_streamer/__init__.py` & `twilio-8.2.0/twilio/rest/media/v1/player_streamer/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/media/v1/player_streamer/playback_grant.py` & `twilio-8.2.0/twilio/rest/media/v1/player_streamer/playback_grant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/MessagingBase.py` & `twilio-8.2.0/twilio/rest/messaging/MessagingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/__init__.py` & `twilio-8.2.0/twilio/rest/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/__init__.py` & `twilio-8.2.0/twilio/rest/messaging/v1/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     DomainConfigMessagingServiceList,
 )
 from twilio.rest.messaging.v1.external_campaign import ExternalCampaignList
 from twilio.rest.messaging.v1.linkshortening_messaging_service import (
     LinkshorteningMessagingServiceList,
 )
 from twilio.rest.messaging.v1.service import ServiceList
-from twilio.rest.messaging.v1.tollfree_verification import TollfreeVerificationList
 from twilio.rest.messaging.v1.usecase import UsecaseList
 
 
 class V1(Version):
     def __init__(self, domain: Domain):
         """
         Initialize the V1 version of Messaging
@@ -47,15 +46,14 @@
             DomainConfigMessagingServiceList
         ] = None
         self._external_campaign: Optional[ExternalCampaignList] = None
         self._linkshortening_messaging_service: Optional[
             LinkshorteningMessagingServiceList
         ] = None
         self._services: Optional[ServiceList] = None
-        self._tollfree_verifications: Optional[TollfreeVerificationList] = None
         self._usecases: Optional[UsecaseList] = None
 
     @property
     def brand_registrations(self) -> BrandRegistrationList:
         if self._brand_registrations is None:
             self._brand_registrations = BrandRegistrationList(self)
         return self._brand_registrations
@@ -103,20 +101,14 @@
     @property
     def services(self) -> ServiceList:
         if self._services is None:
             self._services = ServiceList(self)
         return self._services
 
     @property
-    def tollfree_verifications(self) -> TollfreeVerificationList:
-        if self._tollfree_verifications is None:
-            self._tollfree_verifications = TollfreeVerificationList(self)
-        return self._tollfree_verifications
-
-    @property
     def usecases(self) -> UsecaseList:
         if self._usecases is None:
             self._usecases = UsecaseList(self)
         return self._usecases
 
     def __repr__(self) -> str:
         """
```

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/brand_registration/__init__.py` & `twilio-8.2.0/twilio/rest/messaging/v1/brand_registration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py` & `twilio-8.2.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py` & `twilio-8.2.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/deactivations.py` & `twilio-8.2.0/twilio/rest/messaging/v1/deactivations.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/domain_certs.py` & `twilio-8.2.0/twilio/rest/messaging/v1/domain_certs.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/domain_config.py` & `twilio-8.2.0/twilio/rest/messaging/v1/domain_config.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/domain_config_messaging_service.py` & `twilio-8.2.0/twilio/rest/messaging/v1/domain_config_messaging_service.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/external_campaign.py` & `twilio-8.2.0/twilio/rest/messaging/v1/external_campaign.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py` & `twilio-8.2.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/service/__init__.py` & `twilio-8.2.0/twilio/rest/messaging/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/service/alpha_sender.py` & `twilio-8.2.0/twilio/rest/messaging/v1/service/alpha_sender.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/service/phone_number.py` & `twilio-8.2.0/twilio/rest/messaging/v1/service/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/service/short_code.py` & `twilio-8.2.0/twilio/rest/messaging/v1/service/short_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/service/us_app_to_person.py` & `twilio-8.2.0/twilio/rest/messaging/v1/service/us_app_to_person.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py` & `twilio-8.2.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/messaging/v1/usecase.py` & `twilio-8.2.0/twilio/rest/messaging/v1/usecase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/microvisor/MicrovisorBase.py` & `twilio-8.2.0/twilio/rest/microvisor/MicrovisorBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/microvisor/__init__.py` & `twilio-8.2.0/twilio/rest/microvisor/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/microvisor/v1/__init__.py` & `twilio-8.2.0/twilio/rest/microvisor/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/microvisor/v1/account_config.py` & `twilio-8.2.0/twilio/rest/microvisor/v1/account_config.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/microvisor/v1/account_secret.py` & `twilio-8.2.0/twilio/rest/microvisor/v1/account_secret.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/microvisor/v1/app/__init__.py` & `twilio-8.2.0/twilio/rest/microvisor/v1/app/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/microvisor/v1/app/app_manifest.py` & `twilio-8.2.0/twilio/rest/microvisor/v1/app/app_manifest.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/microvisor/v1/device/__init__.py` & `twilio-8.2.0/twilio/rest/microvisor/v1/device/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/microvisor/v1/device/device_config.py` & `twilio-8.2.0/twilio/rest/microvisor/v1/device/device_config.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/microvisor/v1/device/device_secret.py` & `twilio-8.2.0/twilio/rest/microvisor/v1/device/device_secret.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/monitor/MonitorBase.py` & `twilio-8.2.0/twilio/rest/monitor/MonitorBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/monitor/__init__.py` & `twilio-8.2.0/twilio/rest/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/monitor/v1/__init__.py` & `twilio-8.2.0/twilio/rest/monitor/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/monitor/v1/alert.py` & `twilio-8.2.0/twilio/rest/monitor/v1/alert.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/monitor/v1/event.py` & `twilio-8.2.0/twilio/rest/monitor/v1/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/notify/NotifyBase.py` & `twilio-8.2.0/twilio/rest/notify/NotifyBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/notify/__init__.py` & `twilio-8.2.0/twilio/rest/notify/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/notify/v1/__init__.py` & `twilio-8.2.0/twilio/rest/notify/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/notify/v1/credential.py` & `twilio-8.2.0/twilio/rest/notify/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/notify/v1/service/__init__.py` & `twilio-8.2.0/twilio/rest/notify/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/notify/v1/service/binding.py` & `twilio-8.2.0/twilio/rest/notify/v1/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/notify/v1/service/notification.py` & `twilio-8.2.0/twilio/rest/notify/v1/service/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/numbers/NumbersBase.py` & `twilio-8.2.0/twilio/rest/voice/VoiceBase.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,46 +9,35 @@
   Do not edit the class manually.
 """
 
 from typing import Optional
 
 from twilio.base.domain import Domain
 from twilio.rest import Client
-from twilio.rest.numbers.v1 import V1
-from twilio.rest.numbers.v2 import V2
+from twilio.rest.voice.v1 import V1
 
 
-class NumbersBase(Domain):
+class VoiceBase(Domain):
     def __init__(self, twilio: Client):
         """
-        Initialize the Numbers Domain
+        Initialize the Voice Domain
 
-        :returns: Domain for Numbers
+        :returns: Domain for Voice
         """
-        super().__init__(twilio, "https://numbers.twilio.com")
+        super().__init__(twilio, "https://voice.twilio.com")
         self._v1: Optional[V1] = None
-        self._v2: Optional[V2] = None
 
     @property
     def v1(self) -> V1:
         """
-        :returns: Versions v1 of Numbers
+        :returns: Versions v1 of Voice
         """
         if self._v1 is None:
             self._v1 = V1(self)
         return self._v1
 
-    @property
-    def v2(self) -> V2:
-        """
-        :returns: Versions v2 of Numbers
-        """
-        if self._v2 is None:
-            self._v2 = V2(self)
-        return self._v2
-
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.Numbers>"
+        return "<Twilio.Voice>"
```

### Comparing `twilio-8.1.0/twilio/rest/numbers/v2/__init__.py` & `twilio-8.2.0/twilio/rest/numbers/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py` & `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py` & `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py` & `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py` & `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py` & `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py` & `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py` & `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py` & `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py` & `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py` & `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py` & `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/oauth/OauthBase.py` & `twilio-8.2.0/twilio/rest/oauth/OauthBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/oauth/__init__.py` & `twilio-8.2.0/twilio/rest/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/oauth/v1/__init__.py` & `twilio-8.2.0/twilio/rest/oauth/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/oauth/v1/device_code.py` & `twilio-8.2.0/twilio/rest/oauth/v1/device_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/oauth/v1/oauth.py` & `twilio-8.2.0/twilio/rest/oauth/v1/oauth.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/oauth/v1/openid_discovery.py` & `twilio-8.2.0/twilio/rest/oauth/v1/openid_discovery.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/oauth/v1/token.py` & `twilio-8.2.0/twilio/rest/oauth/v1/token.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/oauth/v1/user_info.py` & `twilio-8.2.0/twilio/rest/oauth/v1/user_info.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/PreviewBase.py` & `twilio-8.2.0/twilio/rest/preview/PreviewBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/__init__.py` & `twilio-8.2.0/twilio/rest/preview/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/deployed_devices/__init__.py` & `twilio-8.2.0/twilio/rest/preview/deployed_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/deployed_devices/fleet/__init__.py` & `twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/deployed_devices/fleet/certificate.py` & `twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/certificate.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/deployed_devices/fleet/deployment.py` & `twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/deployment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/deployed_devices/fleet/device.py` & `twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/device.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/deployed_devices/fleet/key.py` & `twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/hosted_numbers/__init__.py` & `twilio-8.2.0/twilio/rest/preview/hosted_numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py` & `twilio-8.2.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py` & `twilio-8.2.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py` & `twilio-8.2.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/marketplace/__init__.py` & `twilio-8.2.0/twilio/rest/preview/marketplace/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/marketplace/available_add_on/__init__.py` & `twilio-8.2.0/twilio/rest/preview/marketplace/available_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py` & `twilio-8.2.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py` & `twilio-8.2.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py` & `twilio-8.2.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/sync/__init__.py` & `twilio-8.2.0/twilio/rest/preview/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/sync/service/__init__.py` & `twilio-8.2.0/twilio/rest/preview/sync/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/sync/service/document/__init__.py` & `twilio-8.2.0/twilio/rest/preview/sync/service/document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/sync/service/document/document_permission.py` & `twilio-8.2.0/twilio/rest/preview/sync/service/document/document_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/sync/service/sync_list/__init__.py` & `twilio-8.2.0/twilio/rest/preview/sync/service/sync_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py` & `twilio-8.2.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py` & `twilio-8.2.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/sync/service/sync_map/__init__.py` & `twilio-8.2.0/twilio/rest/preview/sync/service/sync_map/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py` & `twilio-8.2.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py` & `twilio-8.2.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/understand/__init__.py` & `twilio-8.2.0/twilio/rest/preview/understand/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/understand/assistant/__init__.py` & `twilio-8.2.0/twilio/rest/preview/understand/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py` & `twilio-8.2.0/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py` & `twilio-8.2.0/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/understand/assistant/dialogue.py` & `twilio-8.2.0/twilio/rest/preview/understand/assistant/dialogue.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/understand/assistant/field_type/__init__.py` & `twilio-8.2.0/twilio/rest/preview/understand/assistant/field_type/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/understand/assistant/field_type/field_value.py` & `twilio-8.2.0/twilio/rest/preview/understand/assistant/field_type/field_value.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/understand/assistant/model_build.py` & `twilio-8.2.0/twilio/rest/preview/understand/assistant/model_build.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/understand/assistant/query.py` & `twilio-8.2.0/twilio/rest/preview/understand/assistant/query.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/understand/assistant/style_sheet.py` & `twilio-8.2.0/twilio/rest/preview/understand/assistant/style_sheet.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/understand/assistant/task/__init__.py` & `twilio-8.2.0/twilio/rest/preview/understand/assistant/task/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/understand/assistant/task/field.py` & `twilio-8.2.0/twilio/rest/preview/understand/assistant/task/field.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/understand/assistant/task/sample.py` & `twilio-8.2.0/twilio/rest/preview/understand/assistant/task/sample.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/understand/assistant/task/task_actions.py` & `twilio-8.2.0/twilio/rest/preview/understand/assistant/task/task_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/understand/assistant/task/task_statistics.py` & `twilio-8.2.0/twilio/rest/preview/understand/assistant/task/task_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/wireless/__init__.py` & `twilio-8.2.0/twilio/rest/preview/wireless/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/wireless/command.py` & `twilio-8.2.0/twilio/rest/preview/wireless/command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/wireless/rate_plan.py` & `twilio-8.2.0/twilio/rest/preview/wireless/rate_plan.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/wireless/sim/__init__.py` & `twilio-8.2.0/twilio/rest/preview/wireless/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/preview/wireless/sim/usage.py` & `twilio-8.2.0/twilio/rest/preview/wireless/sim/usage.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/PricingBase.py` & `twilio-8.2.0/twilio/rest/pricing/PricingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/__init__.py` & `twilio-8.2.0/twilio/rest/pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/v1/__init__.py` & `twilio-8.2.0/twilio/rest/pricing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/v1/messaging/__init__.py` & `twilio-8.2.0/twilio/rest/pricing/v1/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/v1/messaging/country.py` & `twilio-8.2.0/twilio/rest/pricing/v1/messaging/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/v1/phone_number/__init__.py` & `twilio-8.2.0/twilio/rest/pricing/v1/phone_number/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/v1/phone_number/country.py` & `twilio-8.2.0/twilio/rest/pricing/v1/phone_number/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/v1/voice/__init__.py` & `twilio-8.2.0/twilio/rest/pricing/v1/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/v1/voice/country.py` & `twilio-8.2.0/twilio/rest/pricing/v1/voice/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/v1/voice/number.py` & `twilio-8.2.0/twilio/rest/pricing/v1/voice/number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/v2/__init__.py` & `twilio-8.2.0/twilio/rest/pricing/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/v2/country.py` & `twilio-8.2.0/twilio/rest/pricing/v2/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/v2/number.py` & `twilio-8.2.0/twilio/rest/pricing/v2/number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/v2/voice/__init__.py` & `twilio-8.2.0/twilio/rest/pricing/v2/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/v2/voice/country.py` & `twilio-8.2.0/twilio/rest/pricing/v2/voice/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/pricing/v2/voice/number.py` & `twilio-8.2.0/twilio/rest/pricing/v2/voice/number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/proxy/ProxyBase.py` & `twilio-8.2.0/twilio/rest/proxy/ProxyBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/proxy/v1/__init__.py` & `twilio-8.2.0/twilio/rest/proxy/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/proxy/v1/service/__init__.py` & `twilio-8.2.0/twilio/rest/proxy/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/proxy/v1/service/phone_number.py` & `twilio-8.2.0/twilio/rest/proxy/v1/service/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/proxy/v1/service/session/__init__.py` & `twilio-8.2.0/twilio/rest/proxy/v1/service/session/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/proxy/v1/service/session/interaction.py` & `twilio-8.2.0/twilio/rest/proxy/v1/service/session/interaction.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/proxy/v1/service/session/participant/__init__.py` & `twilio-8.2.0/twilio/rest/proxy/v1/service/session/participant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py` & `twilio-8.2.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/proxy/v1/service/short_code.py` & `twilio-8.2.0/twilio/rest/proxy/v1/service/short_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/routes/RoutesBase.py` & `twilio-8.2.0/twilio/rest/routes/RoutesBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/routes/__init__.py` & `twilio-8.2.0/twilio/rest/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/routes/v2/__init__.py` & `twilio-8.2.0/twilio/rest/routes/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/routes/v2/phone_number.py` & `twilio-8.2.0/twilio/rest/routes/v2/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/routes/v2/sip_domain.py` & `twilio-8.2.0/twilio/rest/routes/v2/sip_domain.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/routes/v2/trunk.py` & `twilio-8.2.0/twilio/rest/routes/v2/trunk.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/serverless/ServerlessBase.py` & `twilio-8.2.0/twilio/rest/serverless/ServerlessBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/serverless/v1/__init__.py` & `twilio-8.2.0/twilio/rest/serverless/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/serverless/v1/service/__init__.py` & `twilio-8.2.0/twilio/rest/serverless/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/serverless/v1/service/asset/__init__.py` & `twilio-8.2.0/twilio/rest/serverless/v1/service/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/serverless/v1/service/asset/asset_version.py` & `twilio-8.2.0/twilio/rest/serverless/v1/service/asset/asset_version.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/serverless/v1/service/build/__init__.py` & `twilio-8.2.0/twilio/rest/serverless/v1/service/build/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/serverless/v1/service/build/build_status.py` & `twilio-8.2.0/twilio/rest/serverless/v1/service/build/build_status.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/serverless/v1/service/environment/__init__.py` & `twilio-8.2.0/twilio/rest/serverless/v1/service/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/serverless/v1/service/environment/deployment.py` & `twilio-8.2.0/twilio/rest/serverless/v1/service/environment/deployment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/serverless/v1/service/environment/log.py` & `twilio-8.2.0/twilio/rest/serverless/v1/service/environment/log.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/serverless/v1/service/environment/variable.py` & `twilio-8.2.0/twilio/rest/serverless/v1/service/environment/variable.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/serverless/v1/service/function/__init__.py` & `twilio-8.2.0/twilio/rest/serverless/v1/service/function/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py` & `twilio-8.2.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py` & `twilio-8.2.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/StudioBase.py` & `twilio-8.2.0/twilio/rest/studio/StudioBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/__init__.py` & `twilio-8.2.0/twilio/rest/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v1/__init__.py` & `twilio-8.2.0/twilio/rest/studio/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v1/flow/__init__.py` & `twilio-8.2.0/twilio/rest/studio/v1/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v1/flow/engagement/__init__.py` & `twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py` & `twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py` & `twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py` & `twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v1/flow/execution/__init__.py` & `twilio-8.2.0/twilio/rest/studio/v1/flow/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v1/flow/execution/execution_context.py` & `twilio-8.2.0/twilio/rest/studio/v1/flow/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py` & `twilio-8.2.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py` & `twilio-8.2.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v2/__init__.py` & `twilio-8.2.0/twilio/rest/studio/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v2/flow/__init__.py` & `twilio-8.2.0/twilio/rest/studio/v2/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v2/flow/execution/__init__.py` & `twilio-8.2.0/twilio/rest/studio/v2/flow/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v2/flow/execution/execution_context.py` & `twilio-8.2.0/twilio/rest/studio/v2/flow/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py` & `twilio-8.2.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py` & `twilio-8.2.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v2/flow/flow_revision.py` & `twilio-8.2.0/twilio/rest/studio/v2/flow/flow_revision.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v2/flow/flow_test_user.py` & `twilio-8.2.0/twilio/rest/studio/v2/flow/flow_test_user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/studio/v2/flow_validate.py` & `twilio-8.2.0/twilio/rest/studio/v2/flow_validate.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/supersim/SupersimBase.py` & `twilio-8.2.0/twilio/rest/supersim/SupersimBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/supersim/__init__.py` & `twilio-8.2.0/twilio/rest/supersim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/supersim/v1/__init__.py` & `twilio-8.2.0/twilio/rest/supersim/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/supersim/v1/esim_profile.py` & `twilio-8.2.0/twilio/rest/supersim/v1/esim_profile.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/supersim/v1/fleet.py` & `twilio-8.2.0/twilio/rest/supersim/v1/fleet.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/supersim/v1/ip_command.py` & `twilio-8.2.0/twilio/rest/supersim/v1/ip_command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/supersim/v1/network.py` & `twilio-8.2.0/twilio/rest/supersim/v1/network.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/supersim/v1/network_access_profile/__init__.py` & `twilio-8.2.0/twilio/rest/supersim/v1/network_access_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py` & `twilio-8.2.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/supersim/v1/settings_update.py` & `twilio-8.2.0/twilio/rest/supersim/v1/settings_update.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/supersim/v1/sim/__init__.py` & `twilio-8.2.0/twilio/rest/supersim/v1/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/supersim/v1/sim/billing_period.py` & `twilio-8.2.0/twilio/rest/supersim/v1/sim/billing_period.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/supersim/v1/sim/sim_ip_address.py` & `twilio-8.2.0/twilio/rest/supersim/v1/sim/sim_ip_address.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/supersim/v1/sms_command.py` & `twilio-8.2.0/twilio/rest/supersim/v1/sms_command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/supersim/v1/usage_record.py` & `twilio-8.2.0/twilio/rest/supersim/v1/usage_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/sync/SyncBase.py` & `twilio-8.2.0/twilio/rest/sync/SyncBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/sync/v1/__init__.py` & `twilio-8.2.0/twilio/rest/sync/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/sync/v1/service/__init__.py` & `twilio-8.2.0/twilio/rest/sync/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/sync/v1/service/document/__init__.py` & `twilio-8.2.0/twilio/rest/sync/v1/service/document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/sync/v1/service/document/document_permission.py` & `twilio-8.2.0/twilio/rest/sync/v1/service/document/document_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/sync/v1/service/sync_list/__init__.py` & `twilio-8.2.0/twilio/rest/sync/v1/service/sync_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py` & `twilio-8.2.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py` & `twilio-8.2.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/sync/v1/service/sync_map/__init__.py` & `twilio-8.2.0/twilio/rest/sync/v1/service/sync_map/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py` & `twilio-8.2.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py` & `twilio-8.2.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/sync/v1/service/sync_stream/__init__.py` & `twilio-8.2.0/twilio/rest/sync/v1/service/sync_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py` & `twilio-8.2.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/TaskrouterBase.py` & `twilio-8.2.0/twilio/rest/taskrouter/TaskrouterBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/__init__.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/__init__.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/activity.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/activity.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/event.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task_channel.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py` & `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trunking/TrunkingBase.py` & `twilio-8.2.0/twilio/rest/trunking/TrunkingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trunking/v1/__init__.py` & `twilio-8.2.0/twilio/rest/trunking/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trunking/v1/trunk/__init__.py` & `twilio-8.2.0/twilio/rest/trunking/v1/trunk/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trunking/v1/trunk/credential_list.py` & `twilio-8.2.0/twilio/rest/trunking/v1/trunk/credential_list.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py` & `twilio-8.2.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trunking/v1/trunk/origination_url.py` & `twilio-8.2.0/twilio/rest/trunking/v1/trunk/origination_url.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trunking/v1/trunk/phone_number.py` & `twilio-8.2.0/twilio/rest/trunking/v1/trunk/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trunking/v1/trunk/recording.py` & `twilio-8.2.0/twilio/rest/trunking/v1/trunk/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/TrusthubBase.py` & `twilio-8.2.0/twilio/rest/trusthub/TrusthubBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/__init__.py` & `twilio-8.2.0/twilio/rest/trusthub/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/v1/__init__.py` & `twilio-8.2.0/twilio/rest/trusthub/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py` & `twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py` & `twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py` & `twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py` & `twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/v1/end_user.py` & `twilio-8.2.0/twilio/rest/trusthub/v1/end_user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/v1/end_user_type.py` & `twilio-8.2.0/twilio/rest/trusthub/v1/end_user_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/v1/policies.py` & `twilio-8.2.0/twilio/rest/trusthub/v1/policies.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/v1/supporting_document.py` & `twilio-8.2.0/twilio/rest/trusthub/v1/supporting_document.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/v1/supporting_document_type.py` & `twilio-8.2.0/twilio/rest/trusthub/v1/supporting_document_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/v1/trust_products/__init__.py` & `twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py` & `twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py` & `twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py` & `twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/VerifyBase.py` & `twilio-8.2.0/twilio/rest/verify/VerifyBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/__init__.py` & `twilio-8.2.0/twilio/rest/verify/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/__init__.py` & `twilio-8.2.0/twilio/rest/verify/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/form.py` & `twilio-8.2.0/twilio/rest/verify/v2/form.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/safelist.py` & `twilio-8.2.0/twilio/rest/verify/v2/safelist.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/service/__init__.py` & `twilio-8.2.0/twilio/rest/verify/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/service/access_token.py` & `twilio-8.2.0/twilio/rest/verify/v2/service/access_token.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/service/entity/__init__.py` & `twilio-8.2.0/twilio/rest/verify/v2/service/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py` & `twilio-8.2.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/service/entity/challenge/notification.py` & `twilio-8.2.0/twilio/rest/verify/v2/service/entity/challenge/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/service/entity/factor.py` & `twilio-8.2.0/twilio/rest/verify/v2/service/entity/factor.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/service/entity/new_factor.py` & `twilio-8.2.0/twilio/rest/verify/v2/service/entity/new_factor.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/service/messaging_configuration.py` & `twilio-8.2.0/twilio/rest/verify/v2/service/messaging_configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/service/rate_limit/__init__.py` & `twilio-8.2.0/twilio/rest/verify/v2/service/rate_limit/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/service/rate_limit/bucket.py` & `twilio-8.2.0/twilio/rest/verify/v2/service/rate_limit/bucket.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/service/verification.py` & `twilio-8.2.0/twilio/rest/verify/v2/service/verification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/service/verification_check.py` & `twilio-8.2.0/twilio/rest/verify/v2/service/verification_check.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/service/webhook.py` & `twilio-8.2.0/twilio/rest/verify/v2/service/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/template.py` & `twilio-8.2.0/twilio/rest/verify/v2/template.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/verification_attempt.py` & `twilio-8.2.0/twilio/rest/verify/v2/verification_attempt.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/verify/v2/verification_attempts_summary.py` & `twilio-8.2.0/twilio/rest/verify/v2/verification_attempts_summary.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/VideoBase.py` & `twilio-8.2.0/twilio/rest/video/VideoBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/__init__.py` & `twilio-8.2.0/twilio/rest/video/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/v1/__init__.py` & `twilio-8.2.0/twilio/rest/video/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/v1/composition.py` & `twilio-8.2.0/twilio/rest/video/v1/composition.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/v1/composition_hook.py` & `twilio-8.2.0/twilio/rest/video/v1/composition_hook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/v1/composition_settings.py` & `twilio-8.2.0/twilio/rest/video/v1/composition_settings.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/v1/recording.py` & `twilio-8.2.0/twilio/rest/video/v1/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/v1/recording_settings.py` & `twilio-8.2.0/twilio/rest/video/v1/recording_settings.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/v1/room/__init__.py` & `twilio-8.2.0/twilio/rest/video/v1/room/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/v1/room/participant/__init__.py` & `twilio-8.2.0/twilio/rest/video/v1/room/participant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/v1/room/participant/anonymize.py` & `twilio-8.2.0/twilio/rest/video/v1/room/participant/anonymize.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/v1/room/participant/published_track.py` & `twilio-8.2.0/twilio/rest/video/v1/room/participant/published_track.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/v1/room/participant/subscribe_rules.py` & `twilio-8.2.0/twilio/rest/video/v1/room/participant/subscribe_rules.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/v1/room/participant/subscribed_track.py` & `twilio-8.2.0/twilio/rest/video/v1/room/participant/subscribed_track.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/v1/room/recording_rules.py` & `twilio-8.2.0/twilio/rest/video/v1/room/recording_rules.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/video/v1/room/room_recording.py` & `twilio-8.2.0/twilio/rest/video/v1/room/room_recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/voice/VoiceBase.py` & `twilio-8.2.0/twilio/rest/wireless/WirelessBase.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,35 +9,35 @@
   Do not edit the class manually.
 """
 
 from typing import Optional
 
 from twilio.base.domain import Domain
 from twilio.rest import Client
-from twilio.rest.voice.v1 import V1
+from twilio.rest.wireless.v1 import V1
 
 
-class VoiceBase(Domain):
+class WirelessBase(Domain):
     def __init__(self, twilio: Client):
         """
-        Initialize the Voice Domain
+        Initialize the Wireless Domain
 
-        :returns: Domain for Voice
+        :returns: Domain for Wireless
         """
-        super().__init__(twilio, "https://voice.twilio.com")
+        super().__init__(twilio, "https://wireless.twilio.com")
         self._v1: Optional[V1] = None
 
     @property
     def v1(self) -> V1:
         """
-        :returns: Versions v1 of Voice
+        :returns: Versions v1 of Wireless
         """
         if self._v1 is None:
             self._v1 = V1(self)
         return self._v1
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.Voice>"
+        return "<Twilio.Wireless>"
```

### Comparing `twilio-8.1.0/twilio/rest/voice/__init__.py` & `twilio-8.2.0/twilio/rest/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/voice/v1/__init__.py` & `twilio-8.2.0/twilio/rest/voice/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/voice/v1/archived_call.py` & `twilio-8.2.0/twilio/rest/voice/v1/archived_call.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/voice/v1/byoc_trunk.py` & `twilio-8.2.0/twilio/rest/voice/v1/byoc_trunk.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/voice/v1/connection_policy/__init__.py` & `twilio-8.2.0/twilio/rest/voice/v1/connection_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py` & `twilio-8.2.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/voice/v1/dialing_permissions/__init__.py` & `twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py` & `twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py` & `twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py` & `twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/voice/v1/dialing_permissions/settings.py` & `twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/settings.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/voice/v1/ip_record.py` & `twilio-8.2.0/twilio/rest/voice/v1/ip_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/voice/v1/source_ip_mapping.py` & `twilio-8.2.0/twilio/rest/voice/v1/source_ip_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/wireless/WirelessBase.py` & `twilio-8.2.0/twilio/rest/numbers/NumbersBase.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,35 +9,35 @@
   Do not edit the class manually.
 """
 
 from typing import Optional
 
 from twilio.base.domain import Domain
 from twilio.rest import Client
-from twilio.rest.wireless.v1 import V1
+from twilio.rest.numbers.v2 import V2
 
 
-class WirelessBase(Domain):
+class NumbersBase(Domain):
     def __init__(self, twilio: Client):
         """
-        Initialize the Wireless Domain
+        Initialize the Numbers Domain
 
-        :returns: Domain for Wireless
+        :returns: Domain for Numbers
         """
-        super().__init__(twilio, "https://wireless.twilio.com")
-        self._v1: Optional[V1] = None
+        super().__init__(twilio, "https://numbers.twilio.com")
+        self._v2: Optional[V2] = None
 
     @property
-    def v1(self) -> V1:
+    def v2(self) -> V2:
         """
-        :returns: Versions v1 of Wireless
+        :returns: Versions v2 of Numbers
         """
-        if self._v1 is None:
-            self._v1 = V1(self)
-        return self._v1
+        if self._v2 is None:
+            self._v2 = V2(self)
+        return self._v2
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.Wireless>"
+        return "<Twilio.Numbers>"
```

### Comparing `twilio-8.1.0/twilio/rest/wireless/__init__.py` & `twilio-8.2.0/twilio/rest/wireless/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/wireless/v1/__init__.py` & `twilio-8.2.0/twilio/rest/wireless/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/wireless/v1/command.py` & `twilio-8.2.0/twilio/rest/wireless/v1/command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/wireless/v1/rate_plan.py` & `twilio-8.2.0/twilio/rest/wireless/v1/rate_plan.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/wireless/v1/sim/__init__.py` & `twilio-8.2.0/twilio/rest/wireless/v1/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/wireless/v1/sim/data_session.py` & `twilio-8.2.0/twilio/rest/wireless/v1/sim/data_session.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/wireless/v1/sim/usage_record.py` & `twilio-8.2.0/twilio/rest/wireless/v1/sim/usage_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/rest/wireless/v1/usage_record.py` & `twilio-8.2.0/twilio/rest/wireless/v1/usage_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/twiml/__init__.py` & `twilio-8.2.0/twilio/twiml/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/twiml/fax_response.py` & `twilio-8.2.0/twilio/twiml/fax_response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/twiml/messaging_response.py` & `twilio-8.2.0/twilio/twiml/messaging_response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio/twiml/voice_response.py` & `twilio-8.2.0/twilio/twiml/voice_response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.1.0/twilio.egg-info/PKG-INFO` & `twilio-8.2.0/twilio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twilio
-Version: 8.1.0
+Version: 8.2.0
 Summary: Twilio API client and TwiML generator
 Home-page: https://github.com/twilio/twilio-python/
 Author: Twilio
 Author-email: help@twilio.com
 Keywords: twilio,twiml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `twilio-8.1.0/twilio.egg-info/SOURCES.txt` & `twilio-8.2.0/twilio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

```diff
@@ -314,15 +314,14 @@
 twilio/rest/messaging/v1/__init__.py
 twilio/rest/messaging/v1/deactivations.py
 twilio/rest/messaging/v1/domain_certs.py
 twilio/rest/messaging/v1/domain_config.py
 twilio/rest/messaging/v1/domain_config_messaging_service.py
 twilio/rest/messaging/v1/external_campaign.py
 twilio/rest/messaging/v1/linkshortening_messaging_service.py
-twilio/rest/messaging/v1/tollfree_verification.py
 twilio/rest/messaging/v1/usecase.py
 twilio/rest/messaging/v1/brand_registration/__init__.py
 twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py
 twilio/rest/messaging/v1/brand_registration/brand_vetting.py
 twilio/rest/messaging/v1/service/__init__.py
 twilio/rest/messaging/v1/service/alpha_sender.py
 twilio/rest/messaging/v1/service/phone_number.py
```

