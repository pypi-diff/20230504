# Comparing `tmp/webauthn-1.8.0.tar.gz` & `tmp/webauthn-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webauthn-1.8.0.tar", last modified: Wed Mar 15 22:05:18 2023, max compression
+gzip compressed data, was "webauthn-1.8.1.tar", last modified: Thu May  4 18:56:46 2023, max compression
```

## Comparing `webauthn-1.8.0.tar` & `webauthn-1.8.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:05:18.386533 webauthn-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-15 22:05:08.000000 webauthn-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-03-15 22:05:18.386533 webauthn-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-03-15 22:05:08.000000 webauthn-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 22:05:18.386533 webauthn-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-15 22:05:08.000000 webauthn-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:05:18.382533 webauthn-1.8.0/webauthn/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:05:18.382533 webauthn-1.8.0/webauthn/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/authentication/generate_authentication_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/authentication/verify_authentication_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:05:18.386533 webauthn-1.8.0/webauthn/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/aaguid_to_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/algorithms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:05:18.386533 webauthn-1.8.0/webauthn/helpers/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/asn1/android_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/base64url_to_bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/bytes_to_base64url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/cose.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/decode_credential_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/decoded_public_key_to_cryptography.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/generate_challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/generate_user_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/hash_by_alg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/json_loads_base64url_to_bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/known_root_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/options_to_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/parse_attestation_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/parse_attestation_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/parse_authenticator_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/parse_backup_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/parse_client_data_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/pem_cert_bytes_to_open_ssl_x509.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/snake_case_to_camel_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    20861 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:05:18.386533 webauthn-1.8.0/webauthn/helpers/tpm/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/tpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/tpm/parse_cert_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/tpm/parse_pub_area.py
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/tpm/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/validate_certificate_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/verify_safetynet_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/helpers/verify_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:05:18.386533 webauthn-1.8.0/webauthn/registration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/registration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:05:18.386533 webauthn-1.8.0/webauthn/registration/formats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/registration/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/registration/formats/android_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/registration/formats/android_safetynet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/registration/formats/apple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/registration/formats/fido_u2f.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/registration/formats/packed.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/registration/formats/tpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/registration/generate_registration_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    11819 2023-03-15 22:05:08.000000 webauthn-1.8.0/webauthn/registration/verify_registration_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:05:18.382533 webauthn-1.8.0/webauthn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-03-15 22:05:18.000000 webauthn-1.8.0/webauthn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-15 22:05:18.000000 webauthn-1.8.0/webauthn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 22:05:18.000000 webauthn-1.8.0/webauthn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-15 22:05:18.000000 webauthn-1.8.0/webauthn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-15 22:05:18.000000 webauthn-1.8.0/webauthn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:56:46.108299 webauthn-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-04 18:56:32.000000 webauthn-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-04 18:56:46.108299 webauthn-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-04 18:56:32.000000 webauthn-1.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:56:46.108299 webauthn-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-04 18:56:32.000000 webauthn-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:56:46.104299 webauthn-1.8.1/webauthn/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:56:46.108299 webauthn-1.8.1/webauthn/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/authentication/generate_authentication_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/authentication/verify_authentication_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:56:46.108299 webauthn-1.8.1/webauthn/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/aaguid_to_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/algorithms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:56:46.108299 webauthn-1.8.1/webauthn/helpers/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/asn1/android_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/base64url_to_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/bytes_to_base64url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/cose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/decode_credential_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/decoded_public_key_to_cryptography.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/generate_challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/generate_user_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/hash_by_alg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/json_loads_base64url_to_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/known_root_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/options_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/parse_attestation_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/parse_attestation_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/parse_authenticator_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/parse_backup_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/parse_client_data_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/pem_cert_bytes_to_open_ssl_x509.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/snake_case_to_camel_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20861 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:56:46.108299 webauthn-1.8.1/webauthn/helpers/tpm/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/tpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/tpm/parse_cert_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/tpm/parse_pub_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/tpm/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/validate_certificate_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/verify_safetynet_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/helpers/verify_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:56:46.108299 webauthn-1.8.1/webauthn/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/registration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:56:46.108299 webauthn-1.8.1/webauthn/registration/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/registration/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/registration/formats/android_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/registration/formats/android_safetynet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/registration/formats/apple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/registration/formats/fido_u2f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/registration/formats/packed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/registration/formats/tpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/registration/generate_registration_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11819 2023-05-04 18:56:32.000000 webauthn-1.8.1/webauthn/registration/verify_registration_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:56:46.104299 webauthn-1.8.1/webauthn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-04 18:56:46.000000 webauthn-1.8.1/webauthn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-04 18:56:46.000000 webauthn-1.8.1/webauthn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:56:46.000000 webauthn-1.8.1/webauthn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-04 18:56:46.000000 webauthn-1.8.1/webauthn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 18:56:46.000000 webauthn-1.8.1/webauthn.egg-info/top_level.txt
```

### Comparing `webauthn-1.8.0/LICENSE` & `webauthn-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/PKG-INFO` & `webauthn-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: webauthn
-Version: 1.8.0
+Version: 1.8.1
 Summary: Pythonic WebAuthn
 Home-page: https://github.com/duo-labs/py_webauthn
-Download-URL: https://github.com/duo-labs/py_webauthn/archive/1.8.0.tar.gz
+Download-URL: https://github.com/duo-labs/py_webauthn/archive/1.8.1.tar.gz
 Author: Duo Labs
 Author-email: labs@duo.com
 License: BSD
 Keywords: webauthn fido2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `webauthn-1.8.0/README.md` & `webauthn-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/setup.py` & `webauthn-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,12 +46,12 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3'
     ],
     install_requires=[
         'asn1crypto>=1.4.0',
         'cbor2>=5.4.2.post1',
-        'cryptography>=36.0.1',
+        'cryptography>=39.0.1',
         'pydantic>=1.9.0',
-        'pyOpenSSL>=22.0.0',
+        'pyOpenSSL>=23.0.0',
     ]
 )
```

### Comparing `webauthn-1.8.0/webauthn/__init__.py` & `webauthn-1.8.1/webauthn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     generate_authentication_options,
 )
 from .authentication.verify_authentication_response import (
     verify_authentication_response,
 )
 from .helpers import base64url_to_bytes, options_to_json
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 
 __all__ = [
     "generate_registration_options",
     "verify_registration_response",
     "generate_authentication_options",
     "verify_authentication_response",
     "base64url_to_bytes",
```

### Comparing `webauthn-1.8.0/webauthn/authentication/generate_authentication_options.py` & `webauthn-1.8.1/webauthn/authentication/generate_authentication_options.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/authentication/verify_authentication_response.py` & `webauthn-1.8.1/webauthn/authentication/verify_authentication_response.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/__init__.py` & `webauthn-1.8.1/webauthn/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/aaguid_to_string.py` & `webauthn-1.8.1/webauthn/helpers/aaguid_to_string.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/algorithms.py` & `webauthn-1.8.1/webauthn/helpers/algorithms.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/asn1/android_key.py` & `webauthn-1.8.1/webauthn/helpers/asn1/android_key.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/cose.py` & `webauthn-1.8.1/webauthn/helpers/cose.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/decode_credential_public_key.py` & `webauthn-1.8.1/webauthn/helpers/decode_credential_public_key.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/decoded_public_key_to_cryptography.py` & `webauthn-1.8.1/webauthn/helpers/decoded_public_key_to_cryptography.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/exceptions.py` & `webauthn-1.8.1/webauthn/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/generate_user_handle.py` & `webauthn-1.8.1/webauthn/helpers/generate_user_handle.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/hash_by_alg.py` & `webauthn-1.8.1/webauthn/helpers/hash_by_alg.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/json_loads_base64url_to_bytes.py` & `webauthn-1.8.1/webauthn/helpers/json_loads_base64url_to_bytes.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/known_root_certs.py` & `webauthn-1.8.1/webauthn/helpers/known_root_certs.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/parse_attestation_object.py` & `webauthn-1.8.1/webauthn/helpers/parse_attestation_object.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/parse_attestation_statement.py` & `webauthn-1.8.1/webauthn/helpers/parse_attestation_statement.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/parse_authenticator_data.py` & `webauthn-1.8.1/webauthn/helpers/parse_authenticator_data.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/parse_backup_flags.py` & `webauthn-1.8.1/webauthn/helpers/parse_backup_flags.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/parse_client_data_json.py` & `webauthn-1.8.1/webauthn/helpers/parse_client_data_json.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/structs.py` & `webauthn-1.8.1/webauthn/helpers/structs.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/tpm/parse_cert_info.py` & `webauthn-1.8.1/webauthn/helpers/tpm/parse_cert_info.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/tpm/parse_pub_area.py` & `webauthn-1.8.1/webauthn/helpers/tpm/parse_pub_area.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/tpm/structs.py` & `webauthn-1.8.1/webauthn/helpers/tpm/structs.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/validate_certificate_chain.py` & `webauthn-1.8.1/webauthn/helpers/validate_certificate_chain.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/verify_safetynet_timestamp.py` & `webauthn-1.8.1/webauthn/helpers/verify_safetynet_timestamp.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/helpers/verify_signature.py` & `webauthn-1.8.1/webauthn/helpers/verify_signature.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/registration/formats/android_key.py` & `webauthn-1.8.1/webauthn/registration/formats/android_key.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/registration/formats/android_safetynet.py` & `webauthn-1.8.1/webauthn/registration/formats/android_safetynet.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/registration/formats/apple.py` & `webauthn-1.8.1/webauthn/registration/formats/apple.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/registration/formats/fido_u2f.py` & `webauthn-1.8.1/webauthn/registration/formats/fido_u2f.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/registration/formats/packed.py` & `webauthn-1.8.1/webauthn/registration/formats/packed.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/registration/formats/tpm.py` & `webauthn-1.8.1/webauthn/registration/formats/tpm.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/registration/generate_registration_options.py` & `webauthn-1.8.1/webauthn/registration/generate_registration_options.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn/registration/verify_registration_response.py` & `webauthn-1.8.1/webauthn/registration/verify_registration_response.py`

 * *Files identical despite different names*

### Comparing `webauthn-1.8.0/webauthn.egg-info/PKG-INFO` & `webauthn-1.8.1/webauthn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: webauthn
-Version: 1.8.0
+Version: 1.8.1
 Summary: Pythonic WebAuthn
 Home-page: https://github.com/duo-labs/py_webauthn
-Download-URL: https://github.com/duo-labs/py_webauthn/archive/1.8.0.tar.gz
+Download-URL: https://github.com/duo-labs/py_webauthn/archive/1.8.1.tar.gz
 Author: Duo Labs
 Author-email: labs@duo.com
 License: BSD
 Keywords: webauthn fido2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `webauthn-1.8.0/webauthn.egg-info/SOURCES.txt` & `webauthn-1.8.1/webauthn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

