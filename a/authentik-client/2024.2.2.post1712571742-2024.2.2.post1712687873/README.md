# Comparing `tmp/authentik_client-2024.2.2.post1712571742.tar.gz` & `tmp/authentik_client-2024.2.2.post1712687873.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authentik_client-2024.2.2.post1712571742.tar", max compression
+gzip compressed data, was "authentik_client-2024.2.2.post1712687873.tar", max compression
```

## Comparing `authentik_client-2024.2.2.post1712571742.tar` & `authentik_client-2024.2.2.post1712687873.tar`

### file list

```diff
@@ -1,583 +1,583 @@
--rw-r--r--   0        0        0   140605 2024-04-08 10:22:33.843093 authentik_client-2024.2.2.post1712571742/README.md
--rw-r--r--   0        0        0    47475 2024-04-08 10:22:33.851093 authentik_client-2024.2.2.post1712571742/authentik_client/__init__.py
--rw-r--r--   0        0        0     1170 2024-04-08 10:22:33.855093 authentik_client-2024.2.2.post1712571742/authentik_client/api/__init__.py
--rw-r--r--   0        0        0    97518 2024-04-08 10:22:33.599094 authentik_client-2024.2.2.post1712571742/authentik_client/api/admin_api.py
--rw-r--r--   0        0        0   700271 2024-04-08 10:22:33.619094 authentik_client-2024.2.2.post1712571742/authentik_client/api/authenticators_api.py
--rw-r--r--   0        0        0   699928 2024-04-08 10:22:33.655094 authentik_client-2024.2.2.post1712571742/authentik_client/api/core_api.py
--rw-r--r--   0        0        0   116805 2024-04-08 10:22:33.671094 authentik_client-2024.2.2.post1712571742/authentik_client/api/crypto_api.py
--rw-r--r--   0        0        0   107946 2024-04-08 10:22:33.679094 authentik_client-2024.2.2.post1712571742/authentik_client/api/enterprise_api.py
--rw-r--r--   0        0        0   408008 2024-04-08 10:22:33.691094 authentik_client-2024.2.2.post1712571742/authentik_client/api/events_api.py
--rw-r--r--   0        0        0   280806 2024-04-08 10:22:33.703094 authentik_client-2024.2.2.post1712571742/authentik_client/api/flows_api.py
--rw-r--r--   0        0        0   101134 2024-04-08 10:22:33.711094 authentik_client-2024.2.2.post1712571742/authentik_client/api/managed_api.py
--rw-r--r--   0        0        0   135649 2024-04-08 10:22:33.719094 authentik_client-2024.2.2.post1712571742/authentik_client/api/oauth2_api.py
--rw-r--r--   0        0        0   413301 2024-04-08 10:22:33.727094 authentik_client-2024.2.2.post1712571742/authentik_client/api/outposts_api.py
--rw-r--r--   0        0        0   725201 2024-04-08 10:22:33.739094 authentik_client-2024.2.2.post1712571742/authentik_client/api/policies_api.py
--rw-r--r--   0        0        0   552586 2024-04-08 10:22:33.751093 authentik_client-2024.2.2.post1712571742/authentik_client/api/propertymappings_api.py
--rw-r--r--   0        0        0   718066 2024-04-08 10:22:33.763094 authentik_client-2024.2.2.post1712571742/authentik_client/api/providers_api.py
--rw-r--r--   0        0        0   150485 2024-04-08 10:22:33.771093 authentik_client-2024.2.2.post1712571742/authentik_client/api/rac_api.py
--rw-r--r--   0        0        0   207550 2024-04-08 10:22:33.779093 authentik_client-2024.2.2.post1712571742/authentik_client/api/rbac_api.py
--rw-r--r--   0        0        0    10391 2024-04-08 10:22:33.783093 authentik_client-2024.2.2.post1712571742/authentik_client/api/root_api.py
--rw-r--r--   0        0        0    11845 2024-04-08 10:22:33.791093 authentik_client-2024.2.2.post1712571742/authentik_client/api/schema_api.py
--rw-r--r--   0        0        0   802117 2024-04-08 10:22:33.799093 authentik_client-2024.2.2.post1712571742/authentik_client/api/sources_api.py
--rw-r--r--   0        0        0  1945986 2024-04-08 10:22:33.823093 authentik_client-2024.2.2.post1712571742/authentik_client/api/stages_api.py
--rw-r--r--   0        0        0   157909 2024-04-08 10:22:33.835093 authentik_client-2024.2.2.post1712571742/authentik_client/api/tenants_api.py
--rw-r--r--   0        0        0    25779 2024-04-08 10:22:33.855093 authentik_client-2024.2.2.post1712571742/authentik_client/api_client.py
--rw-r--r--   0        0        0      652 2024-04-08 10:22:33.855093 authentik_client-2024.2.2.post1712571742/authentik_client/api_response.py
--rw-r--r--   0        0        0    15345 2024-04-08 10:22:33.851093 authentik_client-2024.2.2.post1712571742/authentik_client/configuration.py
--rw-r--r--   0        0        0     5934 2024-04-08 10:22:33.855093 authentik_client-2024.2.2.post1712571742/authentik_client/exceptions.py
--rw-r--r--   0        0        0    45777 2024-04-08 10:22:33.851093 authentik_client-2024.2.2.post1712571742/authentik_client/models/__init__.py
--rw-r--r--   0        0        0     4513 2024-04-08 10:22:30.991111 authentik_client-2024.2.2.post1712571742/authentik_client/models/access_denied_challenge.py
--rw-r--r--   0        0        0     2482 2024-04-08 10:22:31.007111 authentik_client-2024.2.2.post1712571742/authentik_client/models/app.py
--rw-r--r--   0        0        0     4168 2024-04-08 10:22:31.011111 authentik_client-2024.2.2.post1712571742/authentik_client/models/app_enum.py
--rw-r--r--   0        0        0     2702 2024-04-08 10:22:31.023111 authentik_client-2024.2.2.post1712571742/authentik_client/models/apple_challenge_response_request.py
--rw-r--r--   0        0        0     4508 2024-04-08 10:22:31.035111 authentik_client-2024.2.2.post1712571742/authentik_client/models/apple_login_challenge.py
--rw-r--r--   0        0        0     6686 2024-04-08 10:22:31.043111 authentik_client-2024.2.2.post1712571742/authentik_client/models/application.py
--rw-r--r--   0        0        0     4473 2024-04-08 10:22:31.051111 authentik_client-2024.2.2.post1712571742/authentik_client/models/application_request.py
--rw-r--r--   0        0        0      711 2024-04-08 10:22:31.055111 authentik_client-2024.2.2.post1712571742/authentik_client/models/auth_mode_enum.py
--rw-r--r--   0        0        0      709 2024-04-08 10:22:31.059111 authentik_client-2024.2.2.post1712571742/authentik_client/models/auth_type_enum.py
--rw-r--r--   0        0        0     4984 2024-04-08 10:22:31.067111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session.py
--rw-r--r--   0        0        0     3064 2024-04-08 10:22:31.071111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_asn.py
--rw-r--r--   0        0        0     2826 2024-04-08 10:22:31.075111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_geo_ip.py
--rw-r--r--   0        0        0     3865 2024-04-08 10:22:31.083111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent.py
--rw-r--r--   0        0        0     2646 2024-04-08 10:22:31.087111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent_device.py
--rw-r--r--   0        0        0     2792 2024-04-08 10:22:31.095111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent_os.py
--rw-r--r--   0        0        0     2725 2024-04-08 10:22:31.099110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent_user_agent.py
--rw-r--r--   0        0        0      895 2024-04-08 10:22:31.103111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authentication_enum.py
--rw-r--r--   0        0        0      782 2024-04-08 10:22:31.103111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_attachment_enum.py
--rw-r--r--   0        0        0     4686 2024-04-08 10:22:31.111111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_challenge.py
--rw-r--r--   0        0        0     2743 2024-04-08 10:22:31.115110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_challenge_response_request.py
--rw-r--r--   0        0        0     5327 2024-04-08 10:22:31.123110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage.py
--rw-r--r--   0        0        0     2768 2024-04-08 10:22:31.127110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage_device_import_response.py
--rw-r--r--   0        0        0     2785 2024-04-08 10:22:31.135110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
--rw-r--r--   0        0        0     4744 2024-04-08 10:22:31.139110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     4594 2024-04-08 10:22:31.143110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_challenge.py
--rw-r--r--   0        0        0     3022 2024-04-08 10:22:31.151110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_challenge_response_request.py
--rw-r--r--   0        0        0     6409 2024-04-08 10:22:31.155110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_stage.py
--rw-r--r--   0        0        0     5595 2024-04-08 10:22:31.163110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4474 2024-04-08 10:22:31.167110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_challenge.py
--rw-r--r--   0        0        0     2761 2024-04-08 10:22:31.175110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_challenge_response_request.py
--rw-r--r--   0        0        0     5363 2024-04-08 10:22:31.179110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_stage.py
--rw-r--r--   0        0        0     4392 2024-04-08 10:22:31.183110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4468 2024-04-08 10:22:31.191110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_challenge.py
--rw-r--r--   0        0        0     2858 2024-04-08 10:22:31.195110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_challenge_response_request.py
--rw-r--r--   0        0        0     5132 2024-04-08 10:22:31.199110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_stage.py
--rw-r--r--   0        0        0     4201 2024-04-08 10:22:31.207110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     5636 2024-04-08 10:22:31.211110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validate_stage.py
--rw-r--r--   0        0        0     4705 2024-04-08 10:22:31.215110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5717 2024-04-08 10:22:31.223110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validation_challenge.py
--rw-r--r--   0        0        0     3805 2024-04-08 10:22:31.227110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validation_challenge_response_request.py
--rw-r--r--   0        0        0     4499 2024-04-08 10:22:31.231110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_web_authn_challenge.py
--rw-r--r--   0        0        0     2852 2024-04-08 10:22:31.239110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_web_authn_challenge_response_request.py
--rw-r--r--   0        0        0     7081 2024-04-08 10:22:31.243110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_web_authn_stage.py
--rw-r--r--   0        0        0     5302 2024-04-08 10:22:31.247110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     2718 2024-04-08 10:22:31.251110 authentik_client-2024.2.2.post1712571742/authentik_client/models/auto_submit_challenge_response_request.py
--rw-r--r--   0        0        0     4388 2024-04-08 10:22:31.259110 authentik_client-2024.2.2.post1712571742/authentik_client/models/autosubmit_challenge.py
--rw-r--r--   0        0        0      950 2024-04-08 10:22:31.263110 authentik_client-2024.2.2.post1712571742/authentik_client/models/backends_enum.py
--rw-r--r--   0        0        0      748 2024-04-08 10:22:31.263110 authentik_client-2024.2.2.post1712571742/authentik_client/models/binding_type_enum.py
--rw-r--r--   0        0        0     2995 2024-04-08 10:22:31.267109 authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_file.py
--rw-r--r--   0        0        0     4453 2024-04-08 10:22:31.271109 authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_instance.py
--rw-r--r--   0        0        0     3208 2024-04-08 10:22:31.279109 authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_instance_request.py
--rw-r--r--   0        0        0      836 2024-04-08 10:22:31.279109 authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_instance_status_enum.py
--rw-r--r--   0        0        0     6255 2024-04-08 10:22:31.283109 authentik_client-2024.2.2.post1712571742/authentik_client/models/brand.py
--rw-r--r--   0        0        0     6307 2024-04-08 10:22:31.291109 authentik_client-2024.2.2.post1712571742/authentik_client/models/brand_request.py
--rw-r--r--   0        0        0     2501 2024-04-08 10:22:31.295109 authentik_client-2024.2.2.post1712571742/authentik_client/models/cache.py
--rw-r--r--   0        0        0      875 2024-04-08 10:22:31.299109 authentik_client-2024.2.2.post1712571742/authentik_client/models/capabilities_enum.py
--rw-r--r--   0        0        0     4476 2024-04-08 10:22:31.303109 authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_challenge.py
--rw-r--r--   0        0        0     2797 2024-04-08 10:22:31.307109 authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_challenge_response_request.py
--rw-r--r--   0        0        0     4438 2024-04-08 10:22:31.311109 authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_stage.py
--rw-r--r--   0        0        0     3774 2024-04-08 10:22:31.315109 authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_stage_request.py
--rw-r--r--   0        0        0     2522 2024-04-08 10:22:31.319109 authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_data.py
--rw-r--r--   0        0        0     2861 2024-04-08 10:22:31.323109 authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_generation_request.py
--rw-r--r--   0        0        0     6655 2024-04-08 10:22:31.327109 authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_key_pair.py
--rw-r--r--   0        0        0     2989 2024-04-08 10:22:31.331109 authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_key_pair_request.py
--rw-r--r--   0        0        0      747 2024-04-08 10:22:31.335109 authentik_client-2024.2.2.post1712571742/authentik_client/models/challenge_choices.py
--rw-r--r--   0        0        0    24236 2024-04-08 10:22:31.343109 authentik_client-2024.2.2.post1712571742/authentik_client/models/challenge_types.py
--rw-r--r--   0        0        0      729 2024-04-08 10:22:31.347109 authentik_client-2024.2.2.post1712571742/authentik_client/models/client_type_enum.py
--rw-r--r--   0        0        0     3539 2024-04-08 10:22:31.359109 authentik_client-2024.2.2.post1712571742/authentik_client/models/config.py
--rw-r--r--   0        0        0     4021 2024-04-08 10:22:31.363109 authentik_client-2024.2.2.post1712571742/authentik_client/models/connection_token.py
--rw-r--r--   0        0        0     2662 2024-04-08 10:22:31.367109 authentik_client-2024.2.2.post1712571742/authentik_client/models/connection_token_request.py
--rw-r--r--   0        0        0     5736 2024-04-08 10:22:31.375109 authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_challenge.py
--rw-r--r--   0        0        0     2838 2024-04-08 10:22:31.379109 authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_challenge_response_request.py
--rw-r--r--   0        0        0     2513 2024-04-08 10:22:31.383109 authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_permission.py
--rw-r--r--   0        0        0     4511 2024-04-08 10:22:31.387109 authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_stage.py
--rw-r--r--   0        0        0      783 2024-04-08 10:22:31.391109 authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_stage_mode_enum.py
--rw-r--r--   0        0        0     3569 2024-04-08 10:22:31.395109 authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_stage_request.py
--rw-r--r--   0        0        0     2891 2024-04-08 10:22:31.399109 authentik_client-2024.2.2.post1712571742/authentik_client/models/contextual_flow_info.py
--rw-r--r--   0        0        0      879 2024-04-08 10:22:31.403109 authentik_client-2024.2.2.post1712571742/authentik_client/models/contextual_flow_info_layout_enum.py
--rw-r--r--   0        0        0     2657 2024-04-08 10:22:31.407109 authentik_client-2024.2.2.post1712571742/authentik_client/models/coordinate.py
--rw-r--r--   0        0        0     4704 2024-04-08 10:22:31.411109 authentik_client-2024.2.2.post1712571742/authentik_client/models/current_brand.py
--rw-r--r--   0        0        0      771 2024-04-08 10:22:31.415109 authentik_client-2024.2.2.post1712571742/authentik_client/models/denied_action_enum.py
--rw-r--r--   0        0        0     4200 2024-04-08 10:22:31.419108 authentik_client-2024.2.2.post1712571742/authentik_client/models/deny_stage.py
--rw-r--r--   0        0        0     3230 2024-04-08 10:22:31.423108 authentik_client-2024.2.2.post1712571742/authentik_client/models/deny_stage_request.py
--rw-r--r--   0        0        0     3522 2024-04-08 10:22:31.431108 authentik_client-2024.2.2.post1712571742/authentik_client/models/device.py
--rw-r--r--   0        0        0     2657 2024-04-08 10:22:31.435109 authentik_client-2024.2.2.post1712571742/authentik_client/models/device_challenge.py
--rw-r--r--   0        0        0     2792 2024-04-08 10:22:31.439108 authentik_client-2024.2.2.post1712571742/authentik_client/models/device_challenge_request.py
--rw-r--r--   0        0        0      780 2024-04-08 10:22:31.443108 authentik_client-2024.2.2.post1712571742/authentik_client/models/device_classes_enum.py
--rw-r--r--   0        0        0     1244 2024-04-08 10:22:31.447108 authentik_client-2024.2.2.post1712571742/authentik_client/models/digest_algorithm_enum.py
--rw-r--r--   0        0        0      695 2024-04-08 10:22:31.447108 authentik_client-2024.2.2.post1712571742/authentik_client/models/digits_enum.py
--rw-r--r--   0        0        0     4969 2024-04-08 10:22:31.451108 authentik_client-2024.2.2.post1712571742/authentik_client/models/docker_service_connection.py
--rw-r--r--   0        0        0     4087 2024-04-08 10:22:31.455108 authentik_client-2024.2.2.post1712571742/authentik_client/models/docker_service_connection_request.py
--rw-r--r--   0        0        0     2847 2024-04-08 10:22:31.459108 authentik_client-2024.2.2.post1712571742/authentik_client/models/domain.py
--rw-r--r--   0        0        0     2746 2024-04-08 10:22:31.467108 authentik_client-2024.2.2.post1712571742/authentik_client/models/domain_request.py
--rw-r--r--   0        0        0     4155 2024-04-08 10:22:31.471108 authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_challenge.py
--rw-r--r--   0        0        0     2681 2024-04-08 10:22:31.475108 authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_challenge_response_request.py
--rw-r--r--   0        0        0     4515 2024-04-08 10:22:31.483108 authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_policy.py
--rw-r--r--   0        0        0     3237 2024-04-08 10:22:31.487108 authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_policy_request.py
--rw-r--r--   0        0        0     4213 2024-04-08 10:22:31.491108 authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_stage.py
--rw-r--r--   0        0        0     3232 2024-04-08 10:22:31.495108 authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_stage_request.py
--rw-r--r--   0        0        0     2720 2024-04-08 10:22:31.499108 authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_device.py
--rw-r--r--   0        0        0     2575 2024-04-08 10:22:31.503108 authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_device_enrollment_status.py
--rw-r--r--   0        0        0     2619 2024-04-08 10:22:31.507108 authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_device_request.py
--rw-r--r--   0        0        0      748 2024-04-08 10:22:31.511108 authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_response_enum.py
--rw-r--r--   0        0        0     4090 2024-04-08 10:22:31.515108 authentik_client-2024.2.2.post1712571742/authentik_client/models/email_challenge.py
--rw-r--r--   0        0        0     2770 2024-04-08 10:22:31.523108 authentik_client-2024.2.2.post1712571742/authentik_client/models/email_challenge_response_request.py
--rw-r--r--   0        0        0     5902 2024-04-08 10:22:31.531108 authentik_client-2024.2.2.post1712571742/authentik_client/models/email_stage.py
--rw-r--r--   0        0        0     5121 2024-04-08 10:22:31.535108 authentik_client-2024.2.2.post1712571742/authentik_client/models/email_stage_request.py
--rw-r--r--   0        0        0     4707 2024-04-08 10:22:31.543108 authentik_client-2024.2.2.post1712571742/authentik_client/models/endpoint.py
--rw-r--r--   0        0        0     3678 2024-04-08 10:22:31.547108 authentik_client-2024.2.2.post1712571742/authentik_client/models/endpoint_request.py
--rw-r--r--   0        0        0     2530 2024-04-08 10:22:31.551108 authentik_client-2024.2.2.post1712571742/authentik_client/models/error_detail.py
--rw-r--r--   0        0        0     3309 2024-04-08 10:22:31.555108 authentik_client-2024.2.2.post1712571742/authentik_client/models/error_reporting_config.py
--rw-r--r--   0        0        0     4129 2024-04-08 10:22:31.559108 authentik_client-2024.2.2.post1712571742/authentik_client/models/event.py
--rw-r--r--   0        0        0     1730 2024-04-08 10:22:31.563108 authentik_client-2024.2.2.post1712571742/authentik_client/models/event_actions.py
--rw-r--r--   0        0        0     6006 2024-04-08 10:22:31.567108 authentik_client-2024.2.2.post1712571742/authentik_client/models/event_matcher_policy.py
--rw-r--r--   0        0        0     4807 2024-04-08 10:22:31.575107 authentik_client-2024.2.2.post1712571742/authentik_client/models/event_matcher_policy_request.py
--rw-r--r--   0        0        0     3990 2024-04-08 10:22:31.579107 authentik_client-2024.2.2.post1712571742/authentik_client/models/event_request.py
--rw-r--r--   0        0        0     2697 2024-04-08 10:22:31.583108 authentik_client-2024.2.2.post1712571742/authentik_client/models/event_top_per_user.py
--rw-r--r--   0        0        0     3715 2024-04-08 10:22:31.591107 authentik_client-2024.2.2.post1712571742/authentik_client/models/expiring_base_grant_model.py
--rw-r--r--   0        0        0     4191 2024-04-08 10:22:31.595107 authentik_client-2024.2.2.post1712571742/authentik_client/models/expression_policy.py
--rw-r--r--   0        0        0     2992 2024-04-08 10:22:31.603107 authentik_client-2024.2.2.post1712571742/authentik_client/models/expression_policy_request.py
--rw-r--r--   0        0        0     4524 2024-04-08 10:22:31.603107 authentik_client-2024.2.2.post1712571742/authentik_client/models/extra_role_object_permission.py
--rw-r--r--   0        0        0     4524 2024-04-08 10:22:31.607107 authentik_client-2024.2.2.post1712571742/authentik_client/models/extra_user_object_permission.py
--rw-r--r--   0        0        0     2519 2024-04-08 10:22:31.611107 authentik_client-2024.2.2.post1712571742/authentik_client/models/file_path_request.py
--rw-r--r--   0        0        0     6047 2024-04-08 10:22:31.615107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow.py
--rw-r--r--   0        0        0    25850 2024-04-08 10:22:31.623107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_challenge_response_request.py
--rw-r--r--   0        0        0      934 2024-04-08 10:22:31.623107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_designation_enum.py
--rw-r--r--   0        0        0     2533 2024-04-08 10:22:31.627107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_diagram.py
--rw-r--r--   0        0        0     4505 2024-04-08 10:22:31.631107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_error_challenge.py
--rw-r--r--   0        0        0     3111 2024-04-08 10:22:31.635107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_import_result.py
--rw-r--r--   0        0        0     3418 2024-04-08 10:22:31.639107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_inspection.py
--rw-r--r--   0        0        0     3875 2024-04-08 10:22:31.643107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_inspector_plan.py
--rw-r--r--   0        0        0      837 2024-04-08 10:22:31.647107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_layout_enum.py
--rw-r--r--   0        0        0     4741 2024-04-08 10:22:31.651107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_request.py
--rw-r--r--   0        0        0     5223 2024-04-08 10:22:31.655107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_set.py
--rw-r--r--   0        0        0     4459 2024-04-08 10:22:31.659107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_set_request.py
--rw-r--r--   0        0        0     4763 2024-04-08 10:22:31.663107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_stage_binding.py
--rw-r--r--   0        0        0     3983 2024-04-08 10:22:31.667107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_stage_binding_request.py
--rw-r--r--   0        0        0     2641 2024-04-08 10:22:31.667107 authentik_client-2024.2.2.post1712571742/authentik_client/models/footer_link.py
--rw-r--r--   0        0        0     2531 2024-04-08 10:22:31.671107 authentik_client-2024.2.2.post1712571742/authentik_client/models/generic_error.py
--rw-r--r--   0        0        0      865 2024-04-08 10:22:31.671107 authentik_client-2024.2.2.post1712571742/authentik_client/models/geoip_binding_enum.py
--rw-r--r--   0        0        0     5216 2024-04-08 10:22:31.675107 authentik_client-2024.2.2.post1712571742/authentik_client/models/group.py
--rw-r--r--   0        0        0     4209 2024-04-08 10:22:31.679107 authentik_client-2024.2.2.post1712571742/authentik_client/models/group_member.py
--rw-r--r--   0        0        0     4006 2024-04-08 10:22:31.683107 authentik_client-2024.2.2.post1712571742/authentik_client/models/group_member_request.py
--rw-r--r--   0        0        0     3347 2024-04-08 10:22:31.687107 authentik_client-2024.2.2.post1712571742/authentik_client/models/group_request.py
--rw-r--r--   0        0        0     6080 2024-04-08 10:22:31.691107 authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_challenge.py
--rw-r--r--   0        0        0     3174 2024-04-08 10:22:31.695107 authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_challenge_response_request.py
--rw-r--r--   0        0        0     7503 2024-04-08 10:22:31.699107 authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_stage.py
--rw-r--r--   0        0        0     6533 2024-04-08 10:22:31.703107 authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_stage_request.py
--rw-r--r--   0        0        0     2438 2024-04-08 10:22:31.707107 authentik_client-2024.2.2.post1712571742/authentik_client/models/install_id.py
--rw-r--r--   0        0        0      771 2024-04-08 10:22:31.707107 authentik_client-2024.2.2.post1712571742/authentik_client/models/intent_enum.py
--rw-r--r--   0        0        0      800 2024-04-08 10:22:31.711107 authentik_client-2024.2.2.post1712571742/authentik_client/models/invalid_response_action_enum.py
--rw-r--r--   0        0        0     4667 2024-04-08 10:22:31.715107 authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation.py
--rw-r--r--   0        0        0     3684 2024-04-08 10:22:31.719107 authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation_request.py
--rw-r--r--   0        0        0     4508 2024-04-08 10:22:31.719107 authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation_stage.py
--rw-r--r--   0        0        0     3527 2024-04-08 10:22:31.723106 authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation_stage_request.py
--rw-r--r--   0        0        0      729 2024-04-08 10:22:31.727106 authentik_client-2024.2.2.post1712571742/authentik_client/models/issuer_mode_enum.py
--rw-r--r--   0        0        0     4386 2024-04-08 10:22:31.727106 authentik_client-2024.2.2.post1712571742/authentik_client/models/kubernetes_service_connection.py
--rw-r--r--   0        0        0     3454 2024-04-08 10:22:31.731107 authentik_client-2024.2.2.post1712571742/authentik_client/models/kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     2811 2024-04-08 10:22:31.735107 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_debug.py
--rw-r--r--   0        0        0     5765 2024-04-08 10:22:31.739107 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_outpost_config.py
--rw-r--r--   0        0        0     4378 2024-04-08 10:22:31.739107 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_property_mapping.py
--rw-r--r--   0        0        0     3478 2024-04-08 10:22:31.743106 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_property_mapping_request.py
--rw-r--r--   0        0        0     8694 2024-04-08 10:22:31.747106 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_provider.py
--rw-r--r--   0        0        0     6192 2024-04-08 10:22:31.747106 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_provider_request.py
--rw-r--r--   0        0        0    11791 2024-04-08 10:22:31.751106 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_source.py
--rw-r--r--   0        0        0     9542 2024-04-08 10:22:31.755106 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_source_request.py
--rw-r--r--   0        0        0     3129 2024-04-08 10:22:31.759106 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_sync_status.py
--rw-r--r--   0        0        0      726 2024-04-08 10:22:31.731107 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldapapi_access_mode.py
--rw-r--r--   0        0        0     3278 2024-04-08 10:22:31.763106 authentik_client-2024.2.2.post1712571742/authentik_client/models/license.py
--rw-r--r--   0        0        0     2897 2024-04-08 10:22:31.767106 authentik_client-2024.2.2.post1712571742/authentik_client/models/license_forecast.py
--rw-r--r--   0        0        0     2509 2024-04-08 10:22:31.775106 authentik_client-2024.2.2.post1712571742/authentik_client/models/license_request.py
--rw-r--r--   0        0        0     3222 2024-04-08 10:22:31.779106 authentik_client-2024.2.2.post1712571742/authentik_client/models/license_summary.py
--rw-r--r--   0        0        0     2411 2024-04-08 10:22:31.779106 authentik_client-2024.2.2.post1712571742/authentik_client/models/link.py
--rw-r--r--   0        0        0     2882 2024-04-08 10:22:31.787106 authentik_client-2024.2.2.post1712571742/authentik_client/models/log_event.py
--rw-r--r--   0        0        0      843 2024-04-08 10:22:31.787106 authentik_client-2024.2.2.post1712571742/authentik_client/models/log_level_enum.py
--rw-r--r--   0        0        0     6520 2024-04-08 10:22:31.795106 authentik_client-2024.2.2.post1712571742/authentik_client/models/login_challenge_types.py
--rw-r--r--   0        0        0     4171 2024-04-08 10:22:31.799106 authentik_client-2024.2.2.post1712571742/authentik_client/models/login_metrics.py
--rw-r--r--   0        0        0     3192 2024-04-08 10:22:31.803106 authentik_client-2024.2.2.post1712571742/authentik_client/models/login_source.py
--rw-r--r--   0        0        0     2513 2024-04-08 10:22:31.811106 authentik_client-2024.2.2.post1712571742/authentik_client/models/metadata.py
--rw-r--r--   0        0        0     7524 2024-04-08 10:22:31.815106 authentik_client-2024.2.2.post1712571742/authentik_client/models/model_enum.py
--rw-r--r--   0        0        0     9828 2024-04-08 10:22:31.819106 authentik_client-2024.2.2.post1712571742/authentik_client/models/model_request.py
--rw-r--r--   0        0        0     1559 2024-04-08 10:22:31.823106 authentik_client-2024.2.2.post1712571742/authentik_client/models/name_id_policy_enum.py
--rw-r--r--   0        0        0      831 2024-04-08 10:22:31.823106 authentik_client-2024.2.2.post1712571742/authentik_client/models/network_binding_enum.py
--rw-r--r--   0        0        0      764 2024-04-08 10:22:31.827106 authentik_client-2024.2.2.post1712571742/authentik_client/models/not_configured_action_enum.py
--rw-r--r--   0        0        0     3479 2024-04-08 10:22:31.827106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification.py
--rw-r--r--   0        0        0     2858 2024-04-08 10:22:31.831106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_request.py
--rw-r--r--   0        0        0     4010 2024-04-08 10:22:31.835106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_rule.py
--rw-r--r--   0        0        0     3549 2024-04-08 10:22:31.839106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_rule_request.py
--rw-r--r--   0        0        0     3760 2024-04-08 10:22:31.839106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport.py
--rw-r--r--   0        0        0      818 2024-04-08 10:22:31.843106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport_mode_enum.py
--rw-r--r--   0        0        0     3500 2024-04-08 10:22:31.843106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport_request.py
--rw-r--r--   0        0        0     2503 2024-04-08 10:22:31.847106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport_test.py
--rw-r--r--   0        0        0     2707 2024-04-08 10:22:31.851106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_webhook_mapping.py
--rw-r--r--   0        0        0     2717 2024-04-08 10:22:31.855106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     8888 2024-04-08 10:22:31.859106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth2_provider.py
--rw-r--r--   0        0        0     6654 2024-04-08 10:22:31.863106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth2_provider_request.py
--rw-r--r--   0        0        0     3482 2024-04-08 10:22:31.867106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth2_provider_setup_urls.py
--rw-r--r--   0        0        0     4164 2024-04-08 10:22:31.871106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_challenge.py
--rw-r--r--   0        0        0     2846 2024-04-08 10:22:31.875106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_challenge_response_request.py
--rw-r--r--   0        0        0     4213 2024-04-08 10:22:31.879106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_finish_challenge.py
--rw-r--r--   0        0        0     2816 2024-04-08 10:22:31.879106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
--rw-r--r--   0        0        0    10563 2024-04-08 10:22:31.883106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_source.py
--rw-r--r--   0        0        0     8069 2024-04-08 10:22:31.887106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_source_request.py
--rw-r--r--   0        0        0     3922 2024-04-08 10:22:31.891106 authentik_client-2024.2.2.post1712571742/authentik_client/models/open_id_connect_configuration.py
--rw-r--r--   0        0        0     5545 2024-04-08 10:22:31.895105 authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost.py
--rw-r--r--   0        0        0     2541 2024-04-08 10:22:31.899105 authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_default_config.py
--rw-r--r--   0        0        0     3755 2024-04-08 10:22:31.899105 authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_health.py
--rw-r--r--   0        0        0     4050 2024-04-08 10:22:31.903105 authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_request.py
--rw-r--r--   0        0        0      752 2024-04-08 10:22:31.907105 authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_type_enum.py
--rw-r--r--   0        0        0     3322 2024-04-08 10:22:31.907105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_application_list.py
--rw-r--r--   0        0        0     3395 2024-04-08 10:22:31.911105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticated_session_list.py
--rw-r--r--   0        0        0     3404 2024-04-08 10:22:31.915105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_duo_stage_list.py
--rw-r--r--   0        0        0     3404 2024-04-08 10:22:31.919105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_sms_stage_list.py
--rw-r--r--   0        0        0     3428 2024-04-08 10:22:31.923105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_static_stage_list.py
--rw-r--r--   0        0        0     3412 2024-04-08 10:22:31.923105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_totp_stage_list.py
--rw-r--r--   0        0        0     3444 2024-04-08 10:22:31.927105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_validate_stage_list.py
--rw-r--r--   0        0        0     3445 2024-04-08 10:22:31.931105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
--rw-r--r--   0        0        0     3371 2024-04-08 10:22:31.935105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_blueprint_instance_list.py
--rw-r--r--   0        0        0     3274 2024-04-08 10:22:31.935105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_brand_list.py
--rw-r--r--   0        0        0     3331 2024-04-08 10:22:31.939105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_captcha_stage_list.py
--rw-r--r--   0        0        0     3380 2024-04-08 10:22:31.943105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_certificate_key_pair_list.py
--rw-r--r--   0        0        0     3355 2024-04-08 10:22:31.947105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_connection_token_list.py
--rw-r--r--   0        0        0     3331 2024-04-08 10:22:31.947105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_consent_stage_list.py
--rw-r--r--   0        0        0     3307 2024-04-08 10:22:31.951105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_deny_stage_list.py
--rw-r--r--   0        0        0     3420 2024-04-08 10:22:31.955105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_docker_service_connection_list.py
--rw-r--r--   0        0        0     3282 2024-04-08 10:22:31.959105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_domain_list.py
--rw-r--r--   0        0        0     3323 2024-04-08 10:22:31.963105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_dummy_policy_list.py
--rw-r--r--   0        0        0     3315 2024-04-08 10:22:31.967105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_dummy_stage_list.py
--rw-r--r--   0        0        0     3307 2024-04-08 10:22:31.967105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_duo_device_list.py
--rw-r--r--   0        0        0     3315 2024-04-08 10:22:31.971105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_email_stage_list.py
--rw-r--r--   0        0        0     3298 2024-04-08 10:22:31.975105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_endpoint_list.py
--rw-r--r--   0        0        0     3274 2024-04-08 10:22:31.979105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_event_list.py
--rw-r--r--   0        0        0     3380 2024-04-08 10:22:31.979105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_event_matcher_policy_list.py
--rw-r--r--   0        0        0     3413 2024-04-08 10:22:31.983105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_expiring_base_grant_model_list.py
--rw-r--r--   0        0        0     3363 2024-04-08 10:22:31.987105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_expression_policy_list.py
--rw-r--r--   0        0        0     3437 2024-04-08 10:22:31.987105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_extra_role_object_permission_list.py
--rw-r--r--   0        0        0     3437 2024-04-08 10:22:31.991105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_extra_user_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-04-08 10:22:31.995105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_flow_list.py
--rw-r--r--   0        0        0     3364 2024-04-08 10:22:31.995105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_flow_stage_binding_list.py
--rw-r--r--   0        0        0     3274 2024-04-08 10:22:31.999105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_group_list.py
--rw-r--r--   0        0        0     3387 2024-04-08 10:22:32.003105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_identification_stage_list.py
--rw-r--r--   0        0        0     3314 2024-04-08 10:22:32.007105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_invitation_list.py
--rw-r--r--   0        0        0     3355 2024-04-08 10:22:32.007105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_invitation_stage_list.py
--rw-r--r--   0        0        0     3452 2024-04-08 10:22:32.011105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_kubernetes_service_connection_list.py
--rw-r--r--   0        0        0     3372 2024-04-08 10:22:32.015105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_outpost_config_list.py
--rw-r--r--   0        0        0     3388 2024-04-08 10:22:32.015105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-08 10:22:32.019105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_provider_list.py
--rw-r--r--   0        0        0     3315 2024-04-08 10:22:32.023105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_source_list.py
--rw-r--r--   0        0        0     3290 2024-04-08 10:22:32.023105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_license_list.py
--rw-r--r--   0        0        0     3330 2024-04-08 10:22:32.027105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_list.py
--rw-r--r--   0        0        0     3363 2024-04-08 10:22:32.031105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_rule_list.py
--rw-r--r--   0        0        0     3403 2024-04-08 10:22:32.035105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_transport_list.py
--rw-r--r--   0        0        0     3444 2024-04-08 10:22:32.039105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_webhook_mapping_list.py
--rw-r--r--   0        0        0     3348 2024-04-08 10:22:32.039105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_o_auth2_provider_list.py
--rw-r--r--   0        0        0     3324 2024-04-08 10:22:32.043105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_o_auth_source_list.py
--rw-r--r--   0        0        0     3290 2024-04-08 10:22:32.047104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_outpost_list.py
--rw-r--r--   0        0        0     3396 2024-04-08 10:22:32.051104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_password_expiry_policy_list.py
--rw-r--r--   0        0        0     3347 2024-04-08 10:22:32.055104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_password_policy_list.py
--rw-r--r--   0        0        0     3339 2024-04-08 10:22:32.059104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_password_stage_list.py
--rw-r--r--   0        0        0     3314 2024-04-08 10:22:32.059104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_permission_list.py
--rw-r--r--   0        0        0     3396 2024-04-08 10:22:32.063104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_plex_source_connection_list.py
--rw-r--r--   0        0        0     3315 2024-04-08 10:22:32.067104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_plex_source_list.py
--rw-r--r--   0        0        0     3339 2024-04-08 10:22:32.071104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_policy_binding_list.py
--rw-r--r--   0        0        0     3282 2024-04-08 10:22:32.075104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_policy_list.py
--rw-r--r--   0        0        0     3282 2024-04-08 10:22:32.075104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_prompt_list.py
--rw-r--r--   0        0        0     3323 2024-04-08 10:22:32.079104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_prompt_stage_list.py
--rw-r--r--   0        0        0     3355 2024-04-08 10:22:32.083104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_property_mapping_list.py
--rw-r--r--   0        0        0     3298 2024-04-08 10:22:32.083104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_provider_list.py
--rw-r--r--   0        0        0     3380 2024-04-08 10:22:32.087104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_proxy_outpost_config_list.py
--rw-r--r--   0        0        0     3339 2024-04-08 10:22:32.087104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_proxy_provider_list.py
--rw-r--r--   0        0        0     3380 2024-04-08 10:22:32.091104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_rac_property_mapping_list.py
--rw-r--r--   0        0        0     3323 2024-04-08 10:22:32.091104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_rac_provider_list.py
--rw-r--r--   0        0        0     3388 2024-04-08 10:22:32.095104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_radius_outpost_config_list.py
--rw-r--r--   0        0        0     3347 2024-04-08 10:22:32.099104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_radius_provider_list.py
--rw-r--r--   0        0        0     3314 2024-04-08 10:22:32.099104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_reputation_list.py
--rw-r--r--   0        0        0     3363 2024-04-08 10:22:32.103104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_reputation_policy_list.py
--rw-r--r--   0        0        0     3461 2024-04-08 10:22:32.103104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_role_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-04-08 10:22:32.107104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_role_list.py
--rw-r--r--   0        0        0     3388 2024-04-08 10:22:32.111104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_saml_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-08 10:22:32.111104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_saml_provider_list.py
--rw-r--r--   0        0        0     3315 2024-04-08 10:22:32.115104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_saml_source_list.py
--rw-r--r--   0        0        0     3323 2024-04-08 10:22:32.115104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_scim_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-08 10:22:32.119104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_scim_provider_list.py
--rw-r--r--   0        0        0     3331 2024-04-08 10:22:32.123104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_scope_mapping_list.py
--rw-r--r--   0        0        0     3371 2024-04-08 10:22:32.123104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_service_connection_list.py
--rw-r--r--   0        0        0     3307 2024-04-08 10:22:32.119104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_sms_device_list.py
--rw-r--r--   0        0        0     3282 2024-04-08 10:22:32.127104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_source_list.py
--rw-r--r--   0        0        0     3323 2024-04-08 10:22:32.127104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_source_stage_list.py
--rw-r--r--   0        0        0     3274 2024-04-08 10:22:32.131104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_stage_list.py
--rw-r--r--   0        0        0     3331 2024-04-08 10:22:32.135104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_static_device_list.py
--rw-r--r--   0        0        0     3315 2024-04-08 10:22:32.135104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_system_task_list.py
--rw-r--r--   0        0        0     3282 2024-04-08 10:22:32.143104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_tenant_list.py
--rw-r--r--   0        0        0     3274 2024-04-08 10:22:32.147104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_token_list.py
--rw-r--r--   0        0        0     3315 2024-04-08 10:22:32.147104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_token_model_list.py
--rw-r--r--   0        0        0     3315 2024-04-08 10:22:32.139104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_totp_device_list.py
--rw-r--r--   0        0        0     3461 2024-04-08 10:22:32.151104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3323 2024-04-08 10:22:32.151104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_consent_list.py
--rw-r--r--   0        0        0     3356 2024-04-08 10:22:32.155104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_delete_stage_list.py
--rw-r--r--   0        0        0     3266 2024-04-08 10:22:32.155104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_list.py
--rw-r--r--   0        0        0     3348 2024-04-08 10:22:32.159104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_login_stage_list.py
--rw-r--r--   0        0        0     3356 2024-04-08 10:22:32.159104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_logout_stage_list.py
--rw-r--r--   0        0        0     3438 2024-04-08 10:22:32.163104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_o_auth_source_connection_list.py
--rw-r--r--   0        0        0     3429 2024-04-08 10:22:32.163104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_saml_source_connection_list.py
--rw-r--r--   0        0        0     3396 2024-04-08 10:22:32.167104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_source_connection_list.py
--rw-r--r--   0        0        0     3348 2024-04-08 10:22:32.171104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_write_stage_list.py
--rw-r--r--   0        0        0     3348 2024-04-08 10:22:32.171104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_web_authn_device_list.py
--rw-r--r--   0        0        0     3381 2024-04-08 10:22:32.175104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_web_authn_device_type_list.py
--rw-r--r--   0        0        0     3076 2024-04-08 10:22:32.175104 authentik_client-2024.2.2.post1712571742/authentik_client/models/pagination.py
--rw-r--r--   0        0        0     4454 2024-04-08 10:22:32.179104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_challenge.py
--rw-r--r--   0        0        0     2819 2024-04-08 10:22:32.179104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_challenge_response_request.py
--rw-r--r--   0        0        0     4377 2024-04-08 10:22:32.183104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_expiry_policy.py
--rw-r--r--   0        0        0     3099 2024-04-08 10:22:32.183104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_expiry_policy_request.py
--rw-r--r--   0        0        0     6428 2024-04-08 10:22:32.187104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_policy.py
--rw-r--r--   0        0        0     5239 2024-04-08 10:22:32.187104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_policy_request.py
--rw-r--r--   0        0        0     5274 2024-04-08 10:22:32.191104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_stage.py
--rw-r--r--   0        0        0     4264 2024-04-08 10:22:32.195104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_stage_request.py
--rw-r--r--   0        0        0     4594 2024-04-08 10:22:32.195104 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_application_request.py
--rw-r--r--   0        0        0     4833 2024-04-08 10:22:32.199103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     5701 2024-04-08 10:22:32.199103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4430 2024-04-08 10:22:32.203103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4256 2024-04-08 10:22:32.207104 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     4743 2024-04-08 10:22:32.207104 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5340 2024-04-08 10:22:32.211104 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     3246 2024-04-08 10:22:32.211104 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_blueprint_instance_request.py
--rw-r--r--   0        0        0     6352 2024-04-08 10:22:32.215103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_brand_request.py
--rw-r--r--   0        0        0     3860 2024-04-08 10:22:32.219103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_captcha_stage_request.py
--rw-r--r--   0        0        0     3051 2024-04-08 10:22:32.219103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_certificate_key_pair_request.py
--rw-r--r--   0        0        0     2717 2024-04-08 10:22:32.223103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_connection_token_request.py
--rw-r--r--   0        0        0     3607 2024-04-08 10:22:32.223103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_consent_stage_request.py
--rw-r--r--   0        0        0     3268 2024-04-08 10:22:32.227103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_deny_stage_request.py
--rw-r--r--   0        0        0     4149 2024-04-08 10:22:32.227103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_docker_service_connection_request.py
--rw-r--r--   0        0        0     2801 2024-04-08 10:22:32.231103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_domain_request.py
--rw-r--r--   0        0        0     3275 2024-04-08 10:22:32.231103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_dummy_policy_request.py
--rw-r--r--   0        0        0     3270 2024-04-08 10:22:32.235103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_dummy_stage_request.py
--rw-r--r--   0        0        0     2674 2024-04-08 10:22:32.235103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_duo_device_request.py
--rw-r--r--   0        0        0     5159 2024-04-08 10:22:32.239103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_email_stage_request.py
--rw-r--r--   0        0        0     3784 2024-04-08 10:22:32.239103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_endpoint_request.py
--rw-r--r--   0        0        0     4845 2024-04-08 10:22:32.243103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_event_matcher_policy_request.py
--rw-r--r--   0        0        0     4045 2024-04-08 10:22:32.243103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_event_request.py
--rw-r--r--   0        0        0     3047 2024-04-08 10:22:32.247103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_expression_policy_request.py
--rw-r--r--   0        0        0     4903 2024-04-08 10:22:32.251103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_flow_request.py
--rw-r--r--   0        0        0     4055 2024-04-08 10:22:32.251103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_flow_stage_binding_request.py
--rw-r--r--   0        0        0     3385 2024-04-08 10:22:32.255103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_group_request.py
--rw-r--r--   0        0        0     6571 2024-04-08 10:22:32.259103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_identification_stage_request.py
--rw-r--r--   0        0        0     3774 2024-04-08 10:22:32.263103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_invitation_request.py
--rw-r--r--   0        0        0     3565 2024-04-08 10:22:32.267103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_invitation_stage_request.py
--rw-r--r--   0        0        0     3492 2024-04-08 10:22:32.267103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     3550 2024-04-08 10:22:32.271103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_ldap_property_mapping_request.py
--rw-r--r--   0        0        0     6254 2024-04-08 10:22:32.275103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_ldap_provider_request.py
--rw-r--r--   0        0        0     9697 2024-04-08 10:22:32.275103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_ldap_source_request.py
--rw-r--r--   0        0        0     2557 2024-04-08 10:22:32.279103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_license_request.py
--rw-r--r--   0        0        0     2879 2024-04-08 10:22:32.279103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_request.py
--rw-r--r--   0        0        0     3587 2024-04-08 10:22:32.283103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_rule_request.py
--rw-r--r--   0        0        0     3538 2024-04-08 10:22:32.283103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_transport_request.py
--rw-r--r--   0        0        0     2782 2024-04-08 10:22:32.287103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     6716 2024-04-08 10:22:32.291103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_o_auth2_provider_request.py
--rw-r--r--   0        0        0     8241 2024-04-08 10:22:32.291103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_o_auth_source_request.py
--rw-r--r--   0        0        0     4139 2024-04-08 10:22:32.295103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_outpost_request.py
--rw-r--r--   0        0        0     3154 2024-04-08 10:22:32.295103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_password_expiry_policy_request.py
--rw-r--r--   0        0        0     5277 2024-04-08 10:22:32.299103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_password_policy_request.py
--rw-r--r--   0        0        0     4326 2024-04-08 10:22:32.303103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_password_stage_request.py
--rw-r--r--   0        0        0     2922 2024-04-08 10:22:32.303103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_permission_assign_request.py
--rw-r--r--   0        0        0     2784 2024-04-08 10:22:32.307103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_plex_source_connection_request.py
--rw-r--r--   0        0        0     5905 2024-04-08 10:22:32.311103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_plex_source_request.py
--rw-r--r--   0        0        0     4286 2024-04-08 10:22:32.315103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_policy_binding_request.py
--rw-r--r--   0        0        0     5023 2024-04-08 10:22:32.315103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_prompt_request.py
--rw-r--r--   0        0        0     3406 2024-04-08 10:22:32.319103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_prompt_stage_request.py
--rw-r--r--   0        0        0     6907 2024-04-08 10:22:32.323103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_proxy_provider_request.py
--rw-r--r--   0        0        0     3495 2024-04-08 10:22:32.323103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_rac_property_mapping_request.py
--rw-r--r--   0        0        0     4413 2024-04-08 10:22:32.327103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_rac_provider_request.py
--rw-r--r--   0        0        0     4563 2024-04-08 10:22:32.331103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_radius_provider_request.py
--rw-r--r--   0        0        0     3276 2024-04-08 10:22:32.331103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_reputation_policy_request.py
--rw-r--r--   0        0        0     2565 2024-04-08 10:22:32.335103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_role_request.py
--rw-r--r--   0        0        0     3901 2024-04-08 10:22:32.339103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_saml_property_mapping_request.py
--rw-r--r--   0        0        0     7539 2024-04-08 10:22:32.339103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_saml_provider_request.py
--rw-r--r--   0        0        0     8676 2024-04-08 10:22:32.343103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_saml_source_request.py
--rw-r--r--   0        0        0     3364 2024-04-08 10:22:32.347102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_scim_mapping_request.py
--rw-r--r--   0        0        0     3888 2024-04-08 10:22:32.347102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_scim_provider_request.py
--rw-r--r--   0        0        0     3819 2024-04-08 10:22:32.355103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_scope_mapping_request.py
--rw-r--r--   0        0        0     4590 2024-04-08 10:22:32.355103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_settings_request.py
--rw-r--r--   0        0        0     2674 2024-04-08 10:22:32.351102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_sms_device_request.py
--rw-r--r--   0        0        0     3562 2024-04-08 10:22:32.359103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_source_stage_request.py
--rw-r--r--   0        0        0     2686 2024-04-08 10:22:32.359103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_static_device_request.py
--rw-r--r--   0        0        0     2820 2024-04-08 10:22:32.367102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_tenant_request.py
--rw-r--r--   0        0        0     4208 2024-04-08 10:22:32.367102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_token_request.py
--rw-r--r--   0        0        0     2678 2024-04-08 10:22:32.363103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_totp_device_request.py
--rw-r--r--   0        0        0     3167 2024-04-08 10:22:32.371102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_delete_stage_request.py
--rw-r--r--   0        0        0     4766 2024-04-08 10:22:32.371102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_login_stage_request.py
--rw-r--r--   0        0        0     3167 2024-04-08 10:22:32.375102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_logout_stage_request.py
--rw-r--r--   0        0        0     3109 2024-04-08 10:22:32.379102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3934 2024-04-08 10:22:32.379102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_request.py
--rw-r--r--   0        0        0     2733 2024-04-08 10:22:32.383102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_saml_source_connection_request.py
--rw-r--r--   0        0        0     4450 2024-04-08 10:22:32.383102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_write_stage_request.py
--rw-r--r--   0        0        0     2625 2024-04-08 10:22:32.387102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_web_authn_device_request.py
--rw-r--r--   0        0        0     3548 2024-04-08 10:22:32.387102 authentik_client-2024.2.2.post1712571742/authentik_client/models/permission.py
--rw-r--r--   0        0        0     2884 2024-04-08 10:22:32.391102 authentik_client-2024.2.2.post1712571742/authentik_client/models/permission_assign_request.py
--rw-r--r--   0        0        0     4315 2024-04-08 10:22:32.395102 authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_authentication_challenge.py
--rw-r--r--   0        0        0     2726 2024-04-08 10:22:32.395102 authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_authentication_challenge_response_request.py
--rw-r--r--   0        0        0     7752 2024-04-08 10:22:32.399102 authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source.py
--rw-r--r--   0        0        0     3265 2024-04-08 10:22:32.403102 authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source_connection.py
--rw-r--r--   0        0        0     2719 2024-04-08 10:22:32.403102 authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source_connection_request.py
--rw-r--r--   0        0        0     5760 2024-04-08 10:22:32.407102 authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source_request.py
--rw-r--r--   0        0        0     2576 2024-04-08 10:22:32.411102 authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_token_redeem_request.py
--rw-r--r--   0        0        0     4055 2024-04-08 10:22:32.415102 authentik_client-2024.2.2.post1712571742/authentik_client/models/policy.py
--rw-r--r--   0        0        0     5643 2024-04-08 10:22:32.415102 authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_binding.py
--rw-r--r--   0        0        0     4231 2024-04-08 10:22:32.419102 authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_binding_request.py
--rw-r--r--   0        0        0      711 2024-04-08 10:22:32.419102 authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_engine_mode.py
--rw-r--r--   0        0        0     2817 2024-04-08 10:22:32.423102 authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_request.py
--rw-r--r--   0        0        0     2583 2024-04-08 10:22:32.427102 authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_test_request.py
--rw-r--r--   0        0        0     3281 2024-04-08 10:22:32.427102 authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_test_result.py
--rw-r--r--   0        0        0     4885 2024-04-08 10:22:32.431102 authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt.py
--rw-r--r--   0        0        0     4649 2024-04-08 10:22:32.435102 authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_challenge.py
--rw-r--r--   0        0        0     3325 2024-04-08 10:22:32.435102 authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_challenge_response_request.py
--rw-r--r--   0        0        0     4927 2024-04-08 10:22:32.439102 authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_request.py
--rw-r--r--   0        0        0     4321 2024-04-08 10:22:32.439102 authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_stage.py
--rw-r--r--   0        0        0     3351 2024-04-08 10:22:32.443102 authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_stage_request.py
--rw-r--r--   0        0        0     1185 2024-04-08 10:22:32.443102 authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_type_enum.py
--rw-r--r--   0        0        0     4264 2024-04-08 10:22:32.443102 authentik_client-2024.2.2.post1712571742/authentik_client/models/property_mapping.py
--rw-r--r--   0        0        0     2610 2024-04-08 10:22:32.447102 authentik_client-2024.2.2.post1712571742/authentik_client/models/property_mapping_preview.py
--rw-r--r--   0        0        0     2744 2024-04-08 10:22:32.447102 authentik_client-2024.2.2.post1712571742/authentik_client/models/property_mapping_test_result.py
--rw-r--r--   0        0        0      715 2024-04-08 10:22:32.451102 authentik_client-2024.2.2.post1712571742/authentik_client/models/protocol_enum.py
--rw-r--r--   0        0        0     5722 2024-04-08 10:22:32.451102 authentik_client-2024.2.2.post1712571742/authentik_client/models/provider.py
--rw-r--r--   0        0        0      713 2024-04-08 10:22:32.455102 authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_enum.py
--rw-r--r--   0        0        0     1314 2024-04-08 10:22:32.455102 authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_model_enum.py
--rw-r--r--   0        0        0     3397 2024-04-08 10:22:32.455102 authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_request.py
--rw-r--r--   0        0        0     1009 2024-04-08 10:22:32.455102 authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_type_enum.py
--rw-r--r--   0        0        0      754 2024-04-08 10:22:32.459102 authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_mode.py
--rw-r--r--   0        0        0     7819 2024-04-08 10:22:32.459102 authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_outpost_config.py
--rw-r--r--   0        0        0     9552 2024-04-08 10:22:32.463102 authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_provider.py
--rw-r--r--   0        0        0     6828 2024-04-08 10:22:32.463102 authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_provider_request.py
--rw-r--r--   0        0        0     4407 2024-04-08 10:22:32.463102 authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_property_mapping.py
--rw-r--r--   0        0        0     3440 2024-04-08 10:22:32.467102 authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_property_mapping_request.py
--rw-r--r--   0        0        0     6813 2024-04-08 10:22:32.467102 authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_provider.py
--rw-r--r--   0        0        0     4351 2024-04-08 10:22:32.471102 authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_provider_request.py
--rw-r--r--   0        0        0     3833 2024-04-08 10:22:32.471102 authentik_client-2024.2.2.post1712571742/authentik_client/models/radius_outpost_config.py
--rw-r--r--   0        0        0     6924 2024-04-08 10:22:32.475102 authentik_client-2024.2.2.post1712571742/authentik_client/models/radius_provider.py
--rw-r--r--   0        0        0     4501 2024-04-08 10:22:32.475102 authentik_client-2024.2.2.post1712571742/authentik_client/models/radius_provider_request.py
--rw-r--r--   0        0        0     4184 2024-04-08 10:22:32.479102 authentik_client-2024.2.2.post1712571742/authentik_client/models/redirect_challenge.py
--rw-r--r--   0        0        0     3642 2024-04-08 10:22:32.483102 authentik_client-2024.2.2.post1712571742/authentik_client/models/reputation.py
--rw-r--r--   0        0        0     4516 2024-04-08 10:22:32.483102 authentik_client-2024.2.2.post1712571742/authentik_client/models/reputation_policy.py
--rw-r--r--   0        0        0     3238 2024-04-08 10:22:32.487102 authentik_client-2024.2.2.post1712571742/authentik_client/models/reputation_policy_request.py
--rw-r--r--   0        0        0      795 2024-04-08 10:22:32.487102 authentik_client-2024.2.2.post1712571742/authentik_client/models/resident_key_requirement_enum.py
--rw-r--r--   0        0        0     2618 2024-04-08 10:22:32.487102 authentik_client-2024.2.2.post1712571742/authentik_client/models/role.py
--rw-r--r--   0        0        0     3333 2024-04-08 10:22:32.491102 authentik_client-2024.2.2.post1712571742/authentik_client/models/role_assigned_object_permission.py
--rw-r--r--   0        0        0     3293 2024-04-08 10:22:32.491102 authentik_client-2024.2.2.post1712571742/authentik_client/models/role_object_permission.py
--rw-r--r--   0        0        0     2517 2024-04-08 10:22:32.495102 authentik_client-2024.2.2.post1712571742/authentik_client/models/role_request.py
--rw-r--r--   0        0        0     2712 2024-04-08 10:22:32.495102 authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_metadata.py
--rw-r--r--   0        0        0     4718 2024-04-08 10:22:32.503102 authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_property_mapping.py
--rw-r--r--   0        0        0     3829 2024-04-08 10:22:32.503102 authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_property_mapping_request.py
--rw-r--r--   0        0        0    11056 2024-04-08 10:22:32.507102 authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_provider.py
--rw-r--r--   0        0        0     7460 2024-04-08 10:22:32.511102 authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_provider_request.py
--rw-r--r--   0        0        0    10563 2024-04-08 10:22:32.511102 authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_source.py
--rw-r--r--   0        0        0     8507 2024-04-08 10:22:32.515102 authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_source_request.py
--rw-r--r--   0        0        0     4248 2024-04-08 10:22:32.519101 authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_mapping.py
--rw-r--r--   0        0        0     3309 2024-04-08 10:22:32.523101 authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_mapping_request.py
--rw-r--r--   0        0        0     5454 2024-04-08 10:22:32.523101 authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_provider.py
--rw-r--r--   0        0        0     3802 2024-04-08 10:22:32.527101 authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_provider_request.py
--rw-r--r--   0        0        0     3131 2024-04-08 10:22:32.531101 authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_sync_status.py
--rw-r--r--   0        0        0     4629 2024-04-08 10:22:32.535101 authentik_client-2024.2.2.post1712571742/authentik_client/models/scope_mapping.py
--rw-r--r--   0        0        0     3740 2024-04-08 10:22:32.539101 authentik_client-2024.2.2.post1712571742/authentik_client/models/scope_mapping_request.py
--rw-r--r--   0        0        0     2738 2024-04-08 10:22:32.543101 authentik_client-2024.2.2.post1712571742/authentik_client/models/selectable_stage.py
--rw-r--r--   0        0        0     3773 2024-04-08 10:22:32.543101 authentik_client-2024.2.2.post1712571742/authentik_client/models/service_connection.py
--rw-r--r--   0        0        0     2776 2024-04-08 10:22:32.547101 authentik_client-2024.2.2.post1712571742/authentik_client/models/service_connection_request.py
--rw-r--r--   0        0        0     2731 2024-04-08 10:22:32.551101 authentik_client-2024.2.2.post1712571742/authentik_client/models/service_connection_state.py
--rw-r--r--   0        0        0     3178 2024-04-08 10:22:32.551101 authentik_client-2024.2.2.post1712571742/authentik_client/models/session_user.py
--rw-r--r--   0        0        0     4441 2024-04-08 10:22:32.555101 authentik_client-2024.2.2.post1712571742/authentik_client/models/settings.py
--rw-r--r--   0        0        0     4569 2024-04-08 10:22:32.559101 authentik_client-2024.2.2.post1712571742/authentik_client/models/settings_request.py
--rw-r--r--   0        0        0      733 2024-04-08 10:22:32.559101 authentik_client-2024.2.2.post1712571742/authentik_client/models/severity_enum.py
--rw-r--r--   0        0        0     4175 2024-04-08 10:22:32.563101 authentik_client-2024.2.2.post1712571742/authentik_client/models/shell_challenge.py
--rw-r--r--   0        0        0     1492 2024-04-08 10:22:32.563101 authentik_client-2024.2.2.post1712571742/authentik_client/models/signature_algorithm_enum.py
--rw-r--r--   0        0        0     2906 2024-04-08 10:22:32.531101 authentik_client-2024.2.2.post1712571742/authentik_client/models/sms_device.py
--rw-r--r--   0        0        0     2619 2024-04-08 10:22:32.535101 authentik_client-2024.2.2.post1712571742/authentik_client/models/sms_device_request.py
--rw-r--r--   0        0        0     6945 2024-04-08 10:22:32.567101 authentik_client-2024.2.2.post1712571742/authentik_client/models/source.py
--rw-r--r--   0        0        0     4836 2024-04-08 10:22:32.571101 authentik_client-2024.2.2.post1712571742/authentik_client/models/source_request.py
--rw-r--r--   0        0        0     4438 2024-04-08 10:22:32.575101 authentik_client-2024.2.2.post1712571742/authentik_client/models/source_stage.py
--rw-r--r--   0        0        0     3507 2024-04-08 10:22:32.579101 authentik_client-2024.2.2.post1712571742/authentik_client/models/source_stage_request.py
--rw-r--r--   0        0        0     5355 2024-04-08 10:22:32.579101 authentik_client-2024.2.2.post1712571742/authentik_client/models/source_type.py
--rw-r--r--   0        0        0      714 2024-04-08 10:22:32.583101 authentik_client-2024.2.2.post1712571742/authentik_client/models/sp_binding_enum.py
--rw-r--r--   0        0        0     4070 2024-04-08 10:22:32.583101 authentik_client-2024.2.2.post1712571742/authentik_client/models/stage.py
--rw-r--r--   0        0        0     3437 2024-04-08 10:22:32.587101 authentik_client-2024.2.2.post1712571742/authentik_client/models/stage_prompt.py
--rw-r--r--   0        0        0     3089 2024-04-08 10:22:32.591101 authentik_client-2024.2.2.post1712571742/authentik_client/models/stage_request.py
--rw-r--r--   0        0        0     3385 2024-04-08 10:22:32.591101 authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device.py
--rw-r--r--   0        0        0     2631 2024-04-08 10:22:32.595101 authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device_request.py
--rw-r--r--   0        0        0     2546 2024-04-08 10:22:32.599101 authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device_token.py
--rw-r--r--   0        0        0     2581 2024-04-08 10:22:32.603101 authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device_token_request.py
--rw-r--r--   0        0        0      846 2024-04-08 10:22:32.603101 authentik_client-2024.2.2.post1712571742/authentik_client/models/sub_mode_enum.py
--rw-r--r--   0        0        0     4463 2024-04-08 10:22:32.607101 authentik_client-2024.2.2.post1712571742/authentik_client/models/system_info.py
--rw-r--r--   0        0        0     2934 2024-04-08 10:22:32.607101 authentik_client-2024.2.2.post1712571742/authentik_client/models/system_info_runtime.py
--rw-r--r--   0        0        0     4286 2024-04-08 10:22:32.611101 authentik_client-2024.2.2.post1712571742/authentik_client/models/system_task.py
--rw-r--r--   0        0        0      789 2024-04-08 10:22:32.611101 authentik_client-2024.2.2.post1712571742/authentik_client/models/system_task_status_enum.py
--rw-r--r--   0        0        0     2872 2024-04-08 10:22:32.619101 authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant.py
--rw-r--r--   0        0        0     2589 2024-04-08 10:22:32.623101 authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_admin_group_request_request.py
--rw-r--r--   0        0        0     2705 2024-04-08 10:22:32.627101 authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_recovery_key_request_request.py
--rw-r--r--   0        0        0     2599 2024-04-08 10:22:32.631101 authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_recovery_key_response.py
--rw-r--r--   0        0        0     2765 2024-04-08 10:22:32.631101 authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_request.py
--rw-r--r--   0        0        0     4591 2024-04-08 10:22:32.635101 authentik_client-2024.2.2.post1712571742/authentik_client/models/token.py
--rw-r--r--   0        0        0     3987 2024-04-08 10:22:32.639101 authentik_client-2024.2.2.post1712571742/authentik_client/models/token_model.py
--rw-r--r--   0        0        0     4118 2024-04-08 10:22:32.643101 authentik_client-2024.2.2.post1712571742/authentik_client/models/token_request.py
--rw-r--r--   0        0        0     2521 2024-04-08 10:22:32.643101 authentik_client-2024.2.2.post1712571742/authentik_client/models/token_set_key_request.py
--rw-r--r--   0        0        0     2494 2024-04-08 10:22:32.647101 authentik_client-2024.2.2.post1712571742/authentik_client/models/token_view.py
--rw-r--r--   0        0        0     2724 2024-04-08 10:22:32.615101 authentik_client-2024.2.2.post1712571742/authentik_client/models/totp_device.py
--rw-r--r--   0        0        0     2623 2024-04-08 10:22:32.619101 authentik_client-2024.2.2.post1712571742/authentik_client/models/totp_device_request.py
--rw-r--r--   0        0        0     3389 2024-04-08 10:22:32.651101 authentik_client-2024.2.2.post1712571742/authentik_client/models/transaction_application_request.py
--rw-r--r--   0        0        0     2595 2024-04-08 10:22:32.651101 authentik_client-2024.2.2.post1712571742/authentik_client/models/transaction_application_response.py
--rw-r--r--   0        0        0     2936 2024-04-08 10:22:32.655101 authentik_client-2024.2.2.post1712571742/authentik_client/models/type_create.py
--rw-r--r--   0        0        0      730 2024-04-08 10:22:32.655101 authentik_client-2024.2.2.post1712571742/authentik_client/models/ui_theme_enum.py
--rw-r--r--   0        0        0     2808 2024-04-08 10:22:32.659101 authentik_client-2024.2.2.post1712571742/authentik_client/models/used_by.py
--rw-r--r--   0        0        0      795 2024-04-08 10:22:32.659101 authentik_client-2024.2.2.post1712571742/authentik_client/models/used_by_action_enum.py
--rw-r--r--   0        0        0     5226 2024-04-08 10:22:32.663101 authentik_client-2024.2.2.post1712571742/authentik_client/models/user.py
--rw-r--r--   0        0        0     2458 2024-04-08 10:22:32.667101 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_account_request.py
--rw-r--r--   0        0        0     4946 2024-04-08 10:22:32.671100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_assigned_object_permission.py
--rw-r--r--   0        0        0     3617 2024-04-08 10:22:32.675100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_consent.py
--rw-r--r--   0        0        0      811 2024-04-08 10:22:32.675100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_creation_mode_enum.py
--rw-r--r--   0        0        0     4110 2024-04-08 10:22:32.679100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_delete_stage.py
--rw-r--r--   0        0        0     3129 2024-04-08 10:22:32.683100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_delete_stage_request.py
--rw-r--r--   0        0        0      735 2024-04-08 10:22:32.683100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_fields_enum.py
--rw-r--r--   0        0        0     3909 2024-04-08 10:22:32.687101 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_group.py
--rw-r--r--   0        0        0     3193 2024-04-08 10:22:32.687101 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_group_request.py
--rw-r--r--   0        0        0     4334 2024-04-08 10:22:32.691100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_challenge.py
--rw-r--r--   0        0        0     2805 2024-04-08 10:22:32.695100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_challenge_response_request.py
--rw-r--r--   0        0        0     5631 2024-04-08 10:22:32.699100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_stage.py
--rw-r--r--   0        0        0     4728 2024-04-08 10:22:32.703100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_stage_request.py
--rw-r--r--   0        0        0     4110 2024-04-08 10:22:32.703100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_logout_stage.py
--rw-r--r--   0        0        0     3129 2024-04-08 10:22:32.707100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_logout_stage_request.py
--rw-r--r--   0        0        0      853 2024-04-08 10:22:32.711100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_matching_mode_enum.py
--rw-r--r--   0        0        0     4160 2024-04-08 10:22:32.711100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_metrics.py
--rw-r--r--   0        0        0     3188 2024-04-08 10:22:32.715100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_o_auth_source_connection.py
--rw-r--r--   0        0        0     3054 2024-04-08 10:22:32.715100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3293 2024-04-08 10:22:32.719100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_object_permission.py
--rw-r--r--   0        0        0     2557 2024-04-08 10:22:32.719100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_password_set_request.py
--rw-r--r--   0        0        0     2491 2024-04-08 10:22:32.723100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_path.py
--rw-r--r--   0        0        0     3872 2024-04-08 10:22:32.723100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_request.py
--rw-r--r--   0        0        0     3107 2024-04-08 10:22:32.727100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_saml_source_connection.py
--rw-r--r--   0        0        0     2668 2024-04-08 10:22:32.727100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_saml_source_connection_request.py
--rw-r--r--   0        0        0     5465 2024-04-08 10:22:32.731100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_self.py
--rw-r--r--   0        0        0     2629 2024-04-08 10:22:32.731100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_self_groups.py
--rw-r--r--   0        0        0     3074 2024-04-08 10:22:32.731100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_service_account_request.py
--rw-r--r--   0        0        0     2844 2024-04-08 10:22:32.735100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_service_account_response.py
--rw-r--r--   0        0        0     2866 2024-04-08 10:22:32.735100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_setting.py
--rw-r--r--   0        0        0     3245 2024-04-08 10:22:32.739100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_source_connection.py
--rw-r--r--   0        0        0      817 2024-04-08 10:22:32.739100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_type_enum.py
--rw-r--r--   0        0        0      777 2024-04-08 10:22:32.739100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_verification_enum.py
--rw-r--r--   0        0        0     5382 2024-04-08 10:22:32.743100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_write_stage.py
--rw-r--r--   0        0        0     4412 2024-04-08 10:22:32.743100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_write_stage_request.py
--rw-r--r--   0        0        0     3197 2024-04-08 10:22:32.747100 authentik_client-2024.2.2.post1712571742/authentik_client/models/validation_error.py
--rw-r--r--   0        0        0     3589 2024-04-08 10:22:32.751100 authentik_client-2024.2.2.post1712571742/authentik_client/models/version.py
--rw-r--r--   0        0        0     3630 2024-04-08 10:22:32.751100 authentik_client-2024.2.2.post1712571742/authentik_client/models/web_authn_device.py
--rw-r--r--   0        0        0     2577 2024-04-08 10:22:32.755100 authentik_client-2024.2.2.post1712571742/authentik_client/models/web_authn_device_request.py
--rw-r--r--   0        0        0     2562 2024-04-08 10:22:32.755100 authentik_client-2024.2.2.post1712571742/authentik_client/models/web_authn_device_type.py
--rw-r--r--   0        0        0     2669 2024-04-08 10:22:32.759100 authentik_client-2024.2.2.post1712571742/authentik_client/models/web_authn_device_type_request.py
--rw-r--r--   0        0        0     2410 2024-04-08 10:22:32.759100 authentik_client-2024.2.2.post1712571742/authentik_client/models/workers.py
--rw-r--r--   0        0        0        0 2024-04-08 10:22:33.847093 authentik_client-2024.2.2.post1712571742/authentik_client/py.typed
--rw-r--r--   0        0        0     9196 2024-04-08 10:22:33.855093 authentik_client-2024.2.2.post1712571742/authentik_client/rest.py
--rw-r--r--   0        0        0     1936 2024-04-08 10:22:33.847093 authentik_client-2024.2.2.post1712571742/pyproject.toml
--rw-r--r--   0        0        0   141557 1970-01-01 00:00:00.000000 authentik_client-2024.2.2.post1712571742/PKG-INFO
+-rw-r--r--   0        0        0   140605 2024-04-09 18:38:05.623901 authentik_client-2024.2.2.post1712687873/README.md
+-rw-r--r--   0        0        0    47475 2024-04-09 18:38:05.631902 authentik_client-2024.2.2.post1712687873/authentik_client/__init__.py
+-rw-r--r--   0        0        0     1170 2024-04-09 18:38:05.635902 authentik_client-2024.2.2.post1712687873/authentik_client/api/__init__.py
+-rw-r--r--   0        0        0    97518 2024-04-09 18:38:05.315901 authentik_client-2024.2.2.post1712687873/authentik_client/api/admin_api.py
+-rw-r--r--   0        0        0   700271 2024-04-09 18:38:05.335901 authentik_client-2024.2.2.post1712687873/authentik_client/api/authenticators_api.py
+-rw-r--r--   0        0        0   699928 2024-04-09 18:38:05.367901 authentik_client-2024.2.2.post1712687873/authentik_client/api/core_api.py
+-rw-r--r--   0        0        0   116805 2024-04-09 18:38:05.379901 authentik_client-2024.2.2.post1712687873/authentik_client/api/crypto_api.py
+-rw-r--r--   0        0        0   107946 2024-04-09 18:38:05.387901 authentik_client-2024.2.2.post1712687873/authentik_client/api/enterprise_api.py
+-rw-r--r--   0        0        0   408008 2024-04-09 18:38:05.399901 authentik_client-2024.2.2.post1712687873/authentik_client/api/events_api.py
+-rw-r--r--   0        0        0   280806 2024-04-09 18:38:05.415901 authentik_client-2024.2.2.post1712687873/authentik_client/api/flows_api.py
+-rw-r--r--   0        0        0   101134 2024-04-09 18:38:05.423901 authentik_client-2024.2.2.post1712687873/authentik_client/api/managed_api.py
+-rw-r--r--   0        0        0   135649 2024-04-09 18:38:05.435901 authentik_client-2024.2.2.post1712687873/authentik_client/api/oauth2_api.py
+-rw-r--r--   0        0        0   413301 2024-04-09 18:38:05.447901 authentik_client-2024.2.2.post1712687873/authentik_client/api/outposts_api.py
+-rw-r--r--   0        0        0   725201 2024-04-09 18:38:05.467901 authentik_client-2024.2.2.post1712687873/authentik_client/api/policies_api.py
+-rw-r--r--   0        0        0   552586 2024-04-09 18:38:05.483901 authentik_client-2024.2.2.post1712687873/authentik_client/api/propertymappings_api.py
+-rw-r--r--   0        0        0   718066 2024-04-09 18:38:05.499901 authentik_client-2024.2.2.post1712687873/authentik_client/api/providers_api.py
+-rw-r--r--   0        0        0   150485 2024-04-09 18:38:05.511901 authentik_client-2024.2.2.post1712687873/authentik_client/api/rac_api.py
+-rw-r--r--   0        0        0   207550 2024-04-09 18:38:05.519901 authentik_client-2024.2.2.post1712687873/authentik_client/api/rbac_api.py
+-rw-r--r--   0        0        0    10391 2024-04-09 18:38:05.527902 authentik_client-2024.2.2.post1712687873/authentik_client/api/root_api.py
+-rw-r--r--   0        0        0    11845 2024-04-09 18:38:05.531901 authentik_client-2024.2.2.post1712687873/authentik_client/api/schema_api.py
+-rw-r--r--   0        0        0   802117 2024-04-09 18:38:05.551901 authentik_client-2024.2.2.post1712687873/authentik_client/api/sources_api.py
+-rw-r--r--   0        0        0  1945986 2024-04-09 18:38:05.595902 authentik_client-2024.2.2.post1712687873/authentik_client/api/stages_api.py
+-rw-r--r--   0        0        0   157909 2024-04-09 18:38:05.611901 authentik_client-2024.2.2.post1712687873/authentik_client/api/tenants_api.py
+-rw-r--r--   0        0        0    25779 2024-04-09 18:38:05.635902 authentik_client-2024.2.2.post1712687873/authentik_client/api_client.py
+-rw-r--r--   0        0        0      652 2024-04-09 18:38:05.635902 authentik_client-2024.2.2.post1712687873/authentik_client/api_response.py
+-rw-r--r--   0        0        0    15345 2024-04-09 18:38:05.631902 authentik_client-2024.2.2.post1712687873/authentik_client/configuration.py
+-rw-r--r--   0        0        0     5934 2024-04-09 18:38:05.635902 authentik_client-2024.2.2.post1712687873/authentik_client/exceptions.py
+-rw-r--r--   0        0        0    45777 2024-04-09 18:38:05.631902 authentik_client-2024.2.2.post1712687873/authentik_client/models/__init__.py
+-rw-r--r--   0        0        0     4513 2024-04-09 18:38:02.647900 authentik_client-2024.2.2.post1712687873/authentik_client/models/access_denied_challenge.py
+-rw-r--r--   0        0        0     2482 2024-04-09 18:38:02.659900 authentik_client-2024.2.2.post1712687873/authentik_client/models/app.py
+-rw-r--r--   0        0        0     4168 2024-04-09 18:38:02.667900 authentik_client-2024.2.2.post1712687873/authentik_client/models/app_enum.py
+-rw-r--r--   0        0        0     2702 2024-04-09 18:38:02.683900 authentik_client-2024.2.2.post1712687873/authentik_client/models/apple_challenge_response_request.py
+-rw-r--r--   0        0        0     4508 2024-04-09 18:38:02.695900 authentik_client-2024.2.2.post1712687873/authentik_client/models/apple_login_challenge.py
+-rw-r--r--   0        0        0     6686 2024-04-09 18:38:02.703900 authentik_client-2024.2.2.post1712687873/authentik_client/models/application.py
+-rw-r--r--   0        0        0     4473 2024-04-09 18:38:02.711900 authentik_client-2024.2.2.post1712687873/authentik_client/models/application_request.py
+-rw-r--r--   0        0        0      711 2024-04-09 18:38:02.715900 authentik_client-2024.2.2.post1712687873/authentik_client/models/auth_mode_enum.py
+-rw-r--r--   0        0        0      709 2024-04-09 18:38:02.719900 authentik_client-2024.2.2.post1712687873/authentik_client/models/auth_type_enum.py
+-rw-r--r--   0        0        0     4984 2024-04-09 18:38:02.723900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticated_session.py
+-rw-r--r--   0        0        0     3064 2024-04-09 18:38:02.731900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticated_session_asn.py
+-rw-r--r--   0        0        0     2826 2024-04-09 18:38:02.735900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticated_session_geo_ip.py
+-rw-r--r--   0        0        0     3865 2024-04-09 18:38:02.739900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticated_session_user_agent.py
+-rw-r--r--   0        0        0     2646 2024-04-09 18:38:02.747900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticated_session_user_agent_device.py
+-rw-r--r--   0        0        0     2792 2024-04-09 18:38:02.751900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticated_session_user_agent_os.py
+-rw-r--r--   0        0        0     2725 2024-04-09 18:38:02.755900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticated_session_user_agent_user_agent.py
+-rw-r--r--   0        0        0      895 2024-04-09 18:38:02.759900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authentication_enum.py
+-rw-r--r--   0        0        0      782 2024-04-09 18:38:02.763900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_attachment_enum.py
+-rw-r--r--   0        0        0     4686 2024-04-09 18:38:02.767900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_duo_challenge.py
+-rw-r--r--   0        0        0     2743 2024-04-09 18:38:02.771900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_duo_challenge_response_request.py
+-rw-r--r--   0        0        0     5327 2024-04-09 18:38:02.779900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_duo_stage.py
+-rw-r--r--   0        0        0     2768 2024-04-09 18:38:02.783900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_duo_stage_device_import_response.py
+-rw-r--r--   0        0        0     2785 2024-04-09 18:38:02.787900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
+-rw-r--r--   0        0        0     4744 2024-04-09 18:38:02.795900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-04-09 18:38:02.799900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_sms_challenge.py
+-rw-r--r--   0        0        0     3022 2024-04-09 18:38:02.803900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_sms_challenge_response_request.py
+-rw-r--r--   0        0        0     6409 2024-04-09 18:38:02.811900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_sms_stage.py
+-rw-r--r--   0        0        0     5595 2024-04-09 18:38:02.815900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4474 2024-04-09 18:38:02.819900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_static_challenge.py
+-rw-r--r--   0        0        0     2761 2024-04-09 18:38:02.823900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_static_challenge_response_request.py
+-rw-r--r--   0        0        0     5363 2024-04-09 18:38:02.831900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_static_stage.py
+-rw-r--r--   0        0        0     4392 2024-04-09 18:38:02.835900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4468 2024-04-09 18:38:02.843900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_totp_challenge.py
+-rw-r--r--   0        0        0     2858 2024-04-09 18:38:02.847900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_totp_challenge_response_request.py
+-rw-r--r--   0        0        0     5132 2024-04-09 18:38:02.851900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_totp_stage.py
+-rw-r--r--   0        0        0     4201 2024-04-09 18:38:02.855900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     5636 2024-04-09 18:38:02.863900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_validate_stage.py
+-rw-r--r--   0        0        0     4705 2024-04-09 18:38:02.867900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5717 2024-04-09 18:38:02.871900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_validation_challenge.py
+-rw-r--r--   0        0        0     3805 2024-04-09 18:38:02.879900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_validation_challenge_response_request.py
+-rw-r--r--   0        0        0     4499 2024-04-09 18:38:02.883900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_web_authn_challenge.py
+-rw-r--r--   0        0        0     2852 2024-04-09 18:38:02.891900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_web_authn_challenge_response_request.py
+-rw-r--r--   0        0        0     7081 2024-04-09 18:38:02.895900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_web_authn_stage.py
+-rw-r--r--   0        0        0     5302 2024-04-09 18:38:02.899900 authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     2718 2024-04-09 18:38:02.903900 authentik_client-2024.2.2.post1712687873/authentik_client/models/auto_submit_challenge_response_request.py
+-rw-r--r--   0        0        0     4388 2024-04-09 18:38:02.911900 authentik_client-2024.2.2.post1712687873/authentik_client/models/autosubmit_challenge.py
+-rw-r--r--   0        0        0      950 2024-04-09 18:38:02.911900 authentik_client-2024.2.2.post1712687873/authentik_client/models/backends_enum.py
+-rw-r--r--   0        0        0      748 2024-04-09 18:38:02.915900 authentik_client-2024.2.2.post1712687873/authentik_client/models/binding_type_enum.py
+-rw-r--r--   0        0        0     2995 2024-04-09 18:38:02.919900 authentik_client-2024.2.2.post1712687873/authentik_client/models/blueprint_file.py
+-rw-r--r--   0        0        0     4453 2024-04-09 18:38:02.923900 authentik_client-2024.2.2.post1712687873/authentik_client/models/blueprint_instance.py
+-rw-r--r--   0        0        0     3208 2024-04-09 18:38:02.927900 authentik_client-2024.2.2.post1712687873/authentik_client/models/blueprint_instance_request.py
+-rw-r--r--   0        0        0      836 2024-04-09 18:38:02.927900 authentik_client-2024.2.2.post1712687873/authentik_client/models/blueprint_instance_status_enum.py
+-rw-r--r--   0        0        0     6255 2024-04-09 18:38:02.931900 authentik_client-2024.2.2.post1712687873/authentik_client/models/brand.py
+-rw-r--r--   0        0        0     6307 2024-04-09 18:38:02.935900 authentik_client-2024.2.2.post1712687873/authentik_client/models/brand_request.py
+-rw-r--r--   0        0        0     2501 2024-04-09 18:38:02.939900 authentik_client-2024.2.2.post1712687873/authentik_client/models/cache.py
+-rw-r--r--   0        0        0      875 2024-04-09 18:38:02.943900 authentik_client-2024.2.2.post1712687873/authentik_client/models/capabilities_enum.py
+-rw-r--r--   0        0        0     4476 2024-04-09 18:38:02.947900 authentik_client-2024.2.2.post1712687873/authentik_client/models/captcha_challenge.py
+-rw-r--r--   0        0        0     2797 2024-04-09 18:38:02.955900 authentik_client-2024.2.2.post1712687873/authentik_client/models/captcha_challenge_response_request.py
+-rw-r--r--   0        0        0     4438 2024-04-09 18:38:02.963900 authentik_client-2024.2.2.post1712687873/authentik_client/models/captcha_stage.py
+-rw-r--r--   0        0        0     3774 2024-04-09 18:38:02.967900 authentik_client-2024.2.2.post1712687873/authentik_client/models/captcha_stage_request.py
+-rw-r--r--   0        0        0     2522 2024-04-09 18:38:02.971900 authentik_client-2024.2.2.post1712687873/authentik_client/models/certificate_data.py
+-rw-r--r--   0        0        0     2861 2024-04-09 18:38:02.975901 authentik_client-2024.2.2.post1712687873/authentik_client/models/certificate_generation_request.py
+-rw-r--r--   0        0        0     6655 2024-04-09 18:38:02.979900 authentik_client-2024.2.2.post1712687873/authentik_client/models/certificate_key_pair.py
+-rw-r--r--   0        0        0     2989 2024-04-09 18:38:02.983900 authentik_client-2024.2.2.post1712687873/authentik_client/models/certificate_key_pair_request.py
+-rw-r--r--   0        0        0      747 2024-04-09 18:38:02.987900 authentik_client-2024.2.2.post1712687873/authentik_client/models/challenge_choices.py
+-rw-r--r--   0        0        0    24236 2024-04-09 18:38:02.995900 authentik_client-2024.2.2.post1712687873/authentik_client/models/challenge_types.py
+-rw-r--r--   0        0        0      729 2024-04-09 18:38:02.999900 authentik_client-2024.2.2.post1712687873/authentik_client/models/client_type_enum.py
+-rw-r--r--   0        0        0     3539 2024-04-09 18:38:03.003900 authentik_client-2024.2.2.post1712687873/authentik_client/models/config.py
+-rw-r--r--   0        0        0     4021 2024-04-09 18:38:03.007900 authentik_client-2024.2.2.post1712687873/authentik_client/models/connection_token.py
+-rw-r--r--   0        0        0     2662 2024-04-09 18:38:03.011901 authentik_client-2024.2.2.post1712687873/authentik_client/models/connection_token_request.py
+-rw-r--r--   0        0        0     5736 2024-04-09 18:38:03.015900 authentik_client-2024.2.2.post1712687873/authentik_client/models/consent_challenge.py
+-rw-r--r--   0        0        0     2838 2024-04-09 18:38:03.019900 authentik_client-2024.2.2.post1712687873/authentik_client/models/consent_challenge_response_request.py
+-rw-r--r--   0        0        0     2513 2024-04-09 18:38:03.023900 authentik_client-2024.2.2.post1712687873/authentik_client/models/consent_permission.py
+-rw-r--r--   0        0        0     4511 2024-04-09 18:38:03.031901 authentik_client-2024.2.2.post1712687873/authentik_client/models/consent_stage.py
+-rw-r--r--   0        0        0      783 2024-04-09 18:38:03.031901 authentik_client-2024.2.2.post1712687873/authentik_client/models/consent_stage_mode_enum.py
+-rw-r--r--   0        0        0     3569 2024-04-09 18:38:03.035900 authentik_client-2024.2.2.post1712687873/authentik_client/models/consent_stage_request.py
+-rw-r--r--   0        0        0     2891 2024-04-09 18:38:03.039900 authentik_client-2024.2.2.post1712687873/authentik_client/models/contextual_flow_info.py
+-rw-r--r--   0        0        0      879 2024-04-09 18:38:03.043900 authentik_client-2024.2.2.post1712687873/authentik_client/models/contextual_flow_info_layout_enum.py
+-rw-r--r--   0        0        0     2657 2024-04-09 18:38:03.047901 authentik_client-2024.2.2.post1712687873/authentik_client/models/coordinate.py
+-rw-r--r--   0        0        0     4704 2024-04-09 18:38:03.051900 authentik_client-2024.2.2.post1712687873/authentik_client/models/current_brand.py
+-rw-r--r--   0        0        0      771 2024-04-09 18:38:03.055900 authentik_client-2024.2.2.post1712687873/authentik_client/models/denied_action_enum.py
+-rw-r--r--   0        0        0     4200 2024-04-09 18:38:03.059900 authentik_client-2024.2.2.post1712687873/authentik_client/models/deny_stage.py
+-rw-r--r--   0        0        0     3230 2024-04-09 18:38:03.063900 authentik_client-2024.2.2.post1712687873/authentik_client/models/deny_stage_request.py
+-rw-r--r--   0        0        0     3522 2024-04-09 18:38:03.071900 authentik_client-2024.2.2.post1712687873/authentik_client/models/device.py
+-rw-r--r--   0        0        0     2657 2024-04-09 18:38:03.075900 authentik_client-2024.2.2.post1712687873/authentik_client/models/device_challenge.py
+-rw-r--r--   0        0        0     2792 2024-04-09 18:38:03.079900 authentik_client-2024.2.2.post1712687873/authentik_client/models/device_challenge_request.py
+-rw-r--r--   0        0        0      780 2024-04-09 18:38:03.083901 authentik_client-2024.2.2.post1712687873/authentik_client/models/device_classes_enum.py
+-rw-r--r--   0        0        0     1244 2024-04-09 18:38:03.087900 authentik_client-2024.2.2.post1712687873/authentik_client/models/digest_algorithm_enum.py
+-rw-r--r--   0        0        0      695 2024-04-09 18:38:03.087900 authentik_client-2024.2.2.post1712687873/authentik_client/models/digits_enum.py
+-rw-r--r--   0        0        0     4969 2024-04-09 18:38:03.091900 authentik_client-2024.2.2.post1712687873/authentik_client/models/docker_service_connection.py
+-rw-r--r--   0        0        0     4087 2024-04-09 18:38:03.095900 authentik_client-2024.2.2.post1712687873/authentik_client/models/docker_service_connection_request.py
+-rw-r--r--   0        0        0     2847 2024-04-09 18:38:03.099900 authentik_client-2024.2.2.post1712687873/authentik_client/models/domain.py
+-rw-r--r--   0        0        0     2746 2024-04-09 18:38:03.103901 authentik_client-2024.2.2.post1712687873/authentik_client/models/domain_request.py
+-rw-r--r--   0        0        0     4155 2024-04-09 18:38:03.111900 authentik_client-2024.2.2.post1712687873/authentik_client/models/dummy_challenge.py
+-rw-r--r--   0        0        0     2681 2024-04-09 18:38:03.115900 authentik_client-2024.2.2.post1712687873/authentik_client/models/dummy_challenge_response_request.py
+-rw-r--r--   0        0        0     4515 2024-04-09 18:38:03.119901 authentik_client-2024.2.2.post1712687873/authentik_client/models/dummy_policy.py
+-rw-r--r--   0        0        0     3237 2024-04-09 18:38:03.123901 authentik_client-2024.2.2.post1712687873/authentik_client/models/dummy_policy_request.py
+-rw-r--r--   0        0        0     4213 2024-04-09 18:38:03.127900 authentik_client-2024.2.2.post1712687873/authentik_client/models/dummy_stage.py
+-rw-r--r--   0        0        0     3232 2024-04-09 18:38:03.131900 authentik_client-2024.2.2.post1712687873/authentik_client/models/dummy_stage_request.py
+-rw-r--r--   0        0        0     2720 2024-04-09 18:38:03.135900 authentik_client-2024.2.2.post1712687873/authentik_client/models/duo_device.py
+-rw-r--r--   0        0        0     2575 2024-04-09 18:38:03.139901 authentik_client-2024.2.2.post1712687873/authentik_client/models/duo_device_enrollment_status.py
+-rw-r--r--   0        0        0     2619 2024-04-09 18:38:03.143900 authentik_client-2024.2.2.post1712687873/authentik_client/models/duo_device_request.py
+-rw-r--r--   0        0        0      748 2024-04-09 18:38:03.147900 authentik_client-2024.2.2.post1712687873/authentik_client/models/duo_response_enum.py
+-rw-r--r--   0        0        0     4090 2024-04-09 18:38:03.151900 authentik_client-2024.2.2.post1712687873/authentik_client/models/email_challenge.py
+-rw-r--r--   0        0        0     2770 2024-04-09 18:38:03.155901 authentik_client-2024.2.2.post1712687873/authentik_client/models/email_challenge_response_request.py
+-rw-r--r--   0        0        0     5902 2024-04-09 18:38:03.159901 authentik_client-2024.2.2.post1712687873/authentik_client/models/email_stage.py
+-rw-r--r--   0        0        0     5121 2024-04-09 18:38:03.167900 authentik_client-2024.2.2.post1712687873/authentik_client/models/email_stage_request.py
+-rw-r--r--   0        0        0     4707 2024-04-09 18:38:03.171900 authentik_client-2024.2.2.post1712687873/authentik_client/models/endpoint.py
+-rw-r--r--   0        0        0     3678 2024-04-09 18:38:03.175901 authentik_client-2024.2.2.post1712687873/authentik_client/models/endpoint_request.py
+-rw-r--r--   0        0        0     2530 2024-04-09 18:38:03.179901 authentik_client-2024.2.2.post1712687873/authentik_client/models/error_detail.py
+-rw-r--r--   0        0        0     3309 2024-04-09 18:38:03.183900 authentik_client-2024.2.2.post1712687873/authentik_client/models/error_reporting_config.py
+-rw-r--r--   0        0        0     4129 2024-04-09 18:38:03.187900 authentik_client-2024.2.2.post1712687873/authentik_client/models/event.py
+-rw-r--r--   0        0        0     1730 2024-04-09 18:38:03.191901 authentik_client-2024.2.2.post1712687873/authentik_client/models/event_actions.py
+-rw-r--r--   0        0        0     6006 2024-04-09 18:38:03.195901 authentik_client-2024.2.2.post1712687873/authentik_client/models/event_matcher_policy.py
+-rw-r--r--   0        0        0     4807 2024-04-09 18:38:03.199900 authentik_client-2024.2.2.post1712687873/authentik_client/models/event_matcher_policy_request.py
+-rw-r--r--   0        0        0     3990 2024-04-09 18:38:03.203900 authentik_client-2024.2.2.post1712687873/authentik_client/models/event_request.py
+-rw-r--r--   0        0        0     2697 2024-04-09 18:38:03.207900 authentik_client-2024.2.2.post1712687873/authentik_client/models/event_top_per_user.py
+-rw-r--r--   0        0        0     3715 2024-04-09 18:38:03.211901 authentik_client-2024.2.2.post1712687873/authentik_client/models/expiring_base_grant_model.py
+-rw-r--r--   0        0        0     4191 2024-04-09 18:38:03.215901 authentik_client-2024.2.2.post1712687873/authentik_client/models/expression_policy.py
+-rw-r--r--   0        0        0     2992 2024-04-09 18:38:03.215901 authentik_client-2024.2.2.post1712687873/authentik_client/models/expression_policy_request.py
+-rw-r--r--   0        0        0     4524 2024-04-09 18:38:03.219900 authentik_client-2024.2.2.post1712687873/authentik_client/models/extra_role_object_permission.py
+-rw-r--r--   0        0        0     4524 2024-04-09 18:38:03.223900 authentik_client-2024.2.2.post1712687873/authentik_client/models/extra_user_object_permission.py
+-rw-r--r--   0        0        0     2519 2024-04-09 18:38:03.227901 authentik_client-2024.2.2.post1712687873/authentik_client/models/file_path_request.py
+-rw-r--r--   0        0        0     6047 2024-04-09 18:38:03.231901 authentik_client-2024.2.2.post1712687873/authentik_client/models/flow.py
+-rw-r--r--   0        0        0    25850 2024-04-09 18:38:03.239900 authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_challenge_response_request.py
+-rw-r--r--   0        0        0      934 2024-04-09 18:38:03.239900 authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_designation_enum.py
+-rw-r--r--   0        0        0     2533 2024-04-09 18:38:03.243900 authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_diagram.py
+-rw-r--r--   0        0        0     4505 2024-04-09 18:38:03.247901 authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_error_challenge.py
+-rw-r--r--   0        0        0     3111 2024-04-09 18:38:03.251901 authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_import_result.py
+-rw-r--r--   0        0        0     3418 2024-04-09 18:38:03.255900 authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_inspection.py
+-rw-r--r--   0        0        0     3875 2024-04-09 18:38:03.259900 authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_inspector_plan.py
+-rw-r--r--   0        0        0      837 2024-04-09 18:38:03.263901 authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_layout_enum.py
+-rw-r--r--   0        0        0     4741 2024-04-09 18:38:03.267901 authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_request.py
+-rw-r--r--   0        0        0     5223 2024-04-09 18:38:03.271901 authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_set.py
+-rw-r--r--   0        0        0     4459 2024-04-09 18:38:03.275900 authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_set_request.py
+-rw-r--r--   0        0        0     4763 2024-04-09 18:38:03.279900 authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_stage_binding.py
+-rw-r--r--   0        0        0     3983 2024-04-09 18:38:03.283901 authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_stage_binding_request.py
+-rw-r--r--   0        0        0     2641 2024-04-09 18:38:03.287901 authentik_client-2024.2.2.post1712687873/authentik_client/models/footer_link.py
+-rw-r--r--   0        0        0     2531 2024-04-09 18:38:03.287901 authentik_client-2024.2.2.post1712687873/authentik_client/models/generic_error.py
+-rw-r--r--   0        0        0      865 2024-04-09 18:38:03.291900 authentik_client-2024.2.2.post1712687873/authentik_client/models/geoip_binding_enum.py
+-rw-r--r--   0        0        0     5216 2024-04-09 18:38:03.295900 authentik_client-2024.2.2.post1712687873/authentik_client/models/group.py
+-rw-r--r--   0        0        0     4209 2024-04-09 18:38:03.303901 authentik_client-2024.2.2.post1712687873/authentik_client/models/group_member.py
+-rw-r--r--   0        0        0     4006 2024-04-09 18:38:03.307901 authentik_client-2024.2.2.post1712687873/authentik_client/models/group_member_request.py
+-rw-r--r--   0        0        0     3347 2024-04-09 18:38:03.311900 authentik_client-2024.2.2.post1712687873/authentik_client/models/group_request.py
+-rw-r--r--   0        0        0     6080 2024-04-09 18:38:03.315900 authentik_client-2024.2.2.post1712687873/authentik_client/models/identification_challenge.py
+-rw-r--r--   0        0        0     3174 2024-04-09 18:38:03.319901 authentik_client-2024.2.2.post1712687873/authentik_client/models/identification_challenge_response_request.py
+-rw-r--r--   0        0        0     7503 2024-04-09 18:38:03.323901 authentik_client-2024.2.2.post1712687873/authentik_client/models/identification_stage.py
+-rw-r--r--   0        0        0     6533 2024-04-09 18:38:03.327901 authentik_client-2024.2.2.post1712687873/authentik_client/models/identification_stage_request.py
+-rw-r--r--   0        0        0     2438 2024-04-09 18:38:03.331900 authentik_client-2024.2.2.post1712687873/authentik_client/models/install_id.py
+-rw-r--r--   0        0        0      771 2024-04-09 18:38:03.331900 authentik_client-2024.2.2.post1712687873/authentik_client/models/intent_enum.py
+-rw-r--r--   0        0        0      800 2024-04-09 18:38:03.335901 authentik_client-2024.2.2.post1712687873/authentik_client/models/invalid_response_action_enum.py
+-rw-r--r--   0        0        0     4667 2024-04-09 18:38:03.339901 authentik_client-2024.2.2.post1712687873/authentik_client/models/invitation.py
+-rw-r--r--   0        0        0     3684 2024-04-09 18:38:03.343901 authentik_client-2024.2.2.post1712687873/authentik_client/models/invitation_request.py
+-rw-r--r--   0        0        0     4508 2024-04-09 18:38:03.347900 authentik_client-2024.2.2.post1712687873/authentik_client/models/invitation_stage.py
+-rw-r--r--   0        0        0     3527 2024-04-09 18:38:03.351900 authentik_client-2024.2.2.post1712687873/authentik_client/models/invitation_stage_request.py
+-rw-r--r--   0        0        0      729 2024-04-09 18:38:03.351900 authentik_client-2024.2.2.post1712687873/authentik_client/models/issuer_mode_enum.py
+-rw-r--r--   0        0        0     4386 2024-04-09 18:38:03.355901 authentik_client-2024.2.2.post1712687873/authentik_client/models/kubernetes_service_connection.py
+-rw-r--r--   0        0        0     3454 2024-04-09 18:38:03.359901 authentik_client-2024.2.2.post1712687873/authentik_client/models/kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     2811 2024-04-09 18:38:03.363901 authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_debug.py
+-rw-r--r--   0        0        0     5765 2024-04-09 18:38:03.367900 authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_outpost_config.py
+-rw-r--r--   0        0        0     4378 2024-04-09 18:38:03.371901 authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_property_mapping.py
+-rw-r--r--   0        0        0     3478 2024-04-09 18:38:03.371901 authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     8694 2024-04-09 18:38:03.375901 authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_provider.py
+-rw-r--r--   0        0        0     6192 2024-04-09 18:38:03.379901 authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_provider_request.py
+-rw-r--r--   0        0        0    11791 2024-04-09 18:38:03.383901 authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_source.py
+-rw-r--r--   0        0        0     9542 2024-04-09 18:38:03.387900 authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_source_request.py
+-rw-r--r--   0        0        0     3129 2024-04-09 18:38:03.391901 authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_sync_status.py
+-rw-r--r--   0        0        0      726 2024-04-09 18:38:03.359901 authentik_client-2024.2.2.post1712687873/authentik_client/models/ldapapi_access_mode.py
+-rw-r--r--   0        0        0     3278 2024-04-09 18:38:03.395901 authentik_client-2024.2.2.post1712687873/authentik_client/models/license.py
+-rw-r--r--   0        0        0     2897 2024-04-09 18:38:03.395901 authentik_client-2024.2.2.post1712687873/authentik_client/models/license_forecast.py
+-rw-r--r--   0        0        0     2509 2024-04-09 18:38:03.399901 authentik_client-2024.2.2.post1712687873/authentik_client/models/license_request.py
+-rw-r--r--   0        0        0     3222 2024-04-09 18:38:03.403900 authentik_client-2024.2.2.post1712687873/authentik_client/models/license_summary.py
+-rw-r--r--   0        0        0     2411 2024-04-09 18:38:03.407901 authentik_client-2024.2.2.post1712687873/authentik_client/models/link.py
+-rw-r--r--   0        0        0     2882 2024-04-09 18:38:03.407901 authentik_client-2024.2.2.post1712687873/authentik_client/models/log_event.py
+-rw-r--r--   0        0        0      843 2024-04-09 18:38:03.411901 authentik_client-2024.2.2.post1712687873/authentik_client/models/log_level_enum.py
+-rw-r--r--   0        0        0     6520 2024-04-09 18:38:03.415901 authentik_client-2024.2.2.post1712687873/authentik_client/models/login_challenge_types.py
+-rw-r--r--   0        0        0     4171 2024-04-09 18:38:03.415901 authentik_client-2024.2.2.post1712687873/authentik_client/models/login_metrics.py
+-rw-r--r--   0        0        0     3192 2024-04-09 18:38:03.419901 authentik_client-2024.2.2.post1712687873/authentik_client/models/login_source.py
+-rw-r--r--   0        0        0     2513 2024-04-09 18:38:03.419901 authentik_client-2024.2.2.post1712687873/authentik_client/models/metadata.py
+-rw-r--r--   0        0        0     7524 2024-04-09 18:38:03.423901 authentik_client-2024.2.2.post1712687873/authentik_client/models/model_enum.py
+-rw-r--r--   0        0        0     9828 2024-04-09 18:38:03.427901 authentik_client-2024.2.2.post1712687873/authentik_client/models/model_request.py
+-rw-r--r--   0        0        0     1559 2024-04-09 18:38:03.427901 authentik_client-2024.2.2.post1712687873/authentik_client/models/name_id_policy_enum.py
+-rw-r--r--   0        0        0      831 2024-04-09 18:38:03.427901 authentik_client-2024.2.2.post1712687873/authentik_client/models/network_binding_enum.py
+-rw-r--r--   0        0        0      764 2024-04-09 18:38:03.431901 authentik_client-2024.2.2.post1712687873/authentik_client/models/not_configured_action_enum.py
+-rw-r--r--   0        0        0     3479 2024-04-09 18:38:03.431901 authentik_client-2024.2.2.post1712687873/authentik_client/models/notification.py
+-rw-r--r--   0        0        0     2858 2024-04-09 18:38:03.435901 authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_request.py
+-rw-r--r--   0        0        0     4010 2024-04-09 18:38:03.439900 authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_rule.py
+-rw-r--r--   0        0        0     3549 2024-04-09 18:38:03.439900 authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_rule_request.py
+-rw-r--r--   0        0        0     3760 2024-04-09 18:38:03.443901 authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_transport.py
+-rw-r--r--   0        0        0      818 2024-04-09 18:38:03.443901 authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_transport_mode_enum.py
+-rw-r--r--   0        0        0     3500 2024-04-09 18:38:03.447901 authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_transport_request.py
+-rw-r--r--   0        0        0     2503 2024-04-09 18:38:03.451901 authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_transport_test.py
+-rw-r--r--   0        0        0     2707 2024-04-09 18:38:03.455901 authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_webhook_mapping.py
+-rw-r--r--   0        0        0     2717 2024-04-09 18:38:03.459901 authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     8888 2024-04-09 18:38:03.463901 authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth2_provider.py
+-rw-r--r--   0        0        0     6654 2024-04-09 18:38:03.467901 authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth2_provider_request.py
+-rw-r--r--   0        0        0     3482 2024-04-09 18:38:03.467901 authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth2_provider_setup_urls.py
+-rw-r--r--   0        0        0     4164 2024-04-09 18:38:03.471901 authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth_device_code_challenge.py
+-rw-r--r--   0        0        0     2846 2024-04-09 18:38:03.475901 authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth_device_code_challenge_response_request.py
+-rw-r--r--   0        0        0     4213 2024-04-09 18:38:03.479901 authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth_device_code_finish_challenge.py
+-rw-r--r--   0        0        0     2816 2024-04-09 18:38:03.483901 authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
+-rw-r--r--   0        0        0    10563 2024-04-09 18:38:03.487901 authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth_source.py
+-rw-r--r--   0        0        0     8013 2024-04-09 18:38:03.491901 authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth_source_request.py
+-rw-r--r--   0        0        0     3922 2024-04-09 18:38:03.495901 authentik_client-2024.2.2.post1712687873/authentik_client/models/open_id_connect_configuration.py
+-rw-r--r--   0        0        0     5545 2024-04-09 18:38:03.499901 authentik_client-2024.2.2.post1712687873/authentik_client/models/outpost.py
+-rw-r--r--   0        0        0     2541 2024-04-09 18:38:03.503901 authentik_client-2024.2.2.post1712687873/authentik_client/models/outpost_default_config.py
+-rw-r--r--   0        0        0     3755 2024-04-09 18:38:03.507901 authentik_client-2024.2.2.post1712687873/authentik_client/models/outpost_health.py
+-rw-r--r--   0        0        0     4050 2024-04-09 18:38:03.511901 authentik_client-2024.2.2.post1712687873/authentik_client/models/outpost_request.py
+-rw-r--r--   0        0        0      752 2024-04-09 18:38:03.515901 authentik_client-2024.2.2.post1712687873/authentik_client/models/outpost_type_enum.py
+-rw-r--r--   0        0        0     3322 2024-04-09 18:38:03.519901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_application_list.py
+-rw-r--r--   0        0        0     3395 2024-04-09 18:38:03.523901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_authenticated_session_list.py
+-rw-r--r--   0        0        0     3404 2024-04-09 18:38:03.527901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_authenticator_duo_stage_list.py
+-rw-r--r--   0        0        0     3404 2024-04-09 18:38:03.531901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_authenticator_sms_stage_list.py
+-rw-r--r--   0        0        0     3428 2024-04-09 18:38:03.535901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_authenticator_static_stage_list.py
+-rw-r--r--   0        0        0     3412 2024-04-09 18:38:03.539901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_authenticator_totp_stage_list.py
+-rw-r--r--   0        0        0     3444 2024-04-09 18:38:03.539901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_authenticator_validate_stage_list.py
+-rw-r--r--   0        0        0     3445 2024-04-09 18:38:03.543901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
+-rw-r--r--   0        0        0     3371 2024-04-09 18:38:03.547901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_blueprint_instance_list.py
+-rw-r--r--   0        0        0     3274 2024-04-09 18:38:03.551901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_brand_list.py
+-rw-r--r--   0        0        0     3331 2024-04-09 18:38:03.551901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_captcha_stage_list.py
+-rw-r--r--   0        0        0     3380 2024-04-09 18:38:03.555901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_certificate_key_pair_list.py
+-rw-r--r--   0        0        0     3355 2024-04-09 18:38:03.559901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_connection_token_list.py
+-rw-r--r--   0        0        0     3331 2024-04-09 18:38:03.563901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_consent_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-04-09 18:38:03.567901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_deny_stage_list.py
+-rw-r--r--   0        0        0     3420 2024-04-09 18:38:03.571901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_docker_service_connection_list.py
+-rw-r--r--   0        0        0     3282 2024-04-09 18:38:03.571901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_domain_list.py
+-rw-r--r--   0        0        0     3323 2024-04-09 18:38:03.579901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_dummy_policy_list.py
+-rw-r--r--   0        0        0     3315 2024-04-09 18:38:03.579901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_dummy_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-04-09 18:38:03.583901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_duo_device_list.py
+-rw-r--r--   0        0        0     3315 2024-04-09 18:38:03.587901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_email_stage_list.py
+-rw-r--r--   0        0        0     3298 2024-04-09 18:38:03.591901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_endpoint_list.py
+-rw-r--r--   0        0        0     3274 2024-04-09 18:38:03.595901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_event_list.py
+-rw-r--r--   0        0        0     3380 2024-04-09 18:38:03.595901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_event_matcher_policy_list.py
+-rw-r--r--   0        0        0     3413 2024-04-09 18:38:03.599901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_expiring_base_grant_model_list.py
+-rw-r--r--   0        0        0     3363 2024-04-09 18:38:03.603901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_expression_policy_list.py
+-rw-r--r--   0        0        0     3437 2024-04-09 18:38:03.607901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_extra_role_object_permission_list.py
+-rw-r--r--   0        0        0     3437 2024-04-09 18:38:03.611901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_extra_user_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-04-09 18:38:03.611901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_flow_list.py
+-rw-r--r--   0        0        0     3364 2024-04-09 18:38:03.615901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_flow_stage_binding_list.py
+-rw-r--r--   0        0        0     3274 2024-04-09 18:38:03.619901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_group_list.py
+-rw-r--r--   0        0        0     3387 2024-04-09 18:38:03.623901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_identification_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-04-09 18:38:03.627901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_invitation_list.py
+-rw-r--r--   0        0        0     3355 2024-04-09 18:38:03.627901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_invitation_stage_list.py
+-rw-r--r--   0        0        0     3452 2024-04-09 18:38:03.631901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_kubernetes_service_connection_list.py
+-rw-r--r--   0        0        0     3372 2024-04-09 18:38:03.635901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_ldap_outpost_config_list.py
+-rw-r--r--   0        0        0     3388 2024-04-09 18:38:03.639901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_ldap_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-09 18:38:03.639901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_ldap_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-04-09 18:38:03.643901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_ldap_source_list.py
+-rw-r--r--   0        0        0     3290 2024-04-09 18:38:03.647901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_license_list.py
+-rw-r--r--   0        0        0     3330 2024-04-09 18:38:03.651901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_notification_list.py
+-rw-r--r--   0        0        0     3363 2024-04-09 18:38:03.651901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_notification_rule_list.py
+-rw-r--r--   0        0        0     3403 2024-04-09 18:38:03.655901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_notification_transport_list.py
+-rw-r--r--   0        0        0     3444 2024-04-09 18:38:03.659901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_notification_webhook_mapping_list.py
+-rw-r--r--   0        0        0     3348 2024-04-09 18:38:03.663901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_o_auth2_provider_list.py
+-rw-r--r--   0        0        0     3324 2024-04-09 18:38:03.663901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_o_auth_source_list.py
+-rw-r--r--   0        0        0     3290 2024-04-09 18:38:03.667901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_outpost_list.py
+-rw-r--r--   0        0        0     3396 2024-04-09 18:38:03.671901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_password_expiry_policy_list.py
+-rw-r--r--   0        0        0     3347 2024-04-09 18:38:03.675901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_password_policy_list.py
+-rw-r--r--   0        0        0     3339 2024-04-09 18:38:03.679901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_password_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-04-09 18:38:03.683901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_permission_list.py
+-rw-r--r--   0        0        0     3396 2024-04-09 18:38:03.683901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_plex_source_connection_list.py
+-rw-r--r--   0        0        0     3315 2024-04-09 18:38:03.687901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_plex_source_list.py
+-rw-r--r--   0        0        0     3339 2024-04-09 18:38:03.691901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_policy_binding_list.py
+-rw-r--r--   0        0        0     3282 2024-04-09 18:38:03.695901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_policy_list.py
+-rw-r--r--   0        0        0     3282 2024-04-09 18:38:03.699901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_prompt_list.py
+-rw-r--r--   0        0        0     3323 2024-04-09 18:38:03.703901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_prompt_stage_list.py
+-rw-r--r--   0        0        0     3355 2024-04-09 18:38:03.703901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_property_mapping_list.py
+-rw-r--r--   0        0        0     3298 2024-04-09 18:38:03.707901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-04-09 18:38:03.711901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_proxy_outpost_config_list.py
+-rw-r--r--   0        0        0     3339 2024-04-09 18:38:03.711901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_proxy_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-04-09 18:38:03.715901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_rac_property_mapping_list.py
+-rw-r--r--   0        0        0     3323 2024-04-09 18:38:03.719901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_rac_provider_list.py
+-rw-r--r--   0        0        0     3388 2024-04-09 18:38:03.723901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_radius_outpost_config_list.py
+-rw-r--r--   0        0        0     3347 2024-04-09 18:38:03.723901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_radius_provider_list.py
+-rw-r--r--   0        0        0     3314 2024-04-09 18:38:03.727901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_reputation_list.py
+-rw-r--r--   0        0        0     3363 2024-04-09 18:38:03.731901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_reputation_policy_list.py
+-rw-r--r--   0        0        0     3461 2024-04-09 18:38:03.735901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_role_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-04-09 18:38:03.735901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_role_list.py
+-rw-r--r--   0        0        0     3388 2024-04-09 18:38:03.739901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_saml_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-09 18:38:03.743901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_saml_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-04-09 18:38:03.747901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_saml_source_list.py
+-rw-r--r--   0        0        0     3323 2024-04-09 18:38:03.747901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_scim_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-09 18:38:03.751901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_scim_provider_list.py
+-rw-r--r--   0        0        0     3331 2024-04-09 18:38:03.759901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_scope_mapping_list.py
+-rw-r--r--   0        0        0     3371 2024-04-09 18:38:03.763901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_service_connection_list.py
+-rw-r--r--   0        0        0     3307 2024-04-09 18:38:03.755901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_sms_device_list.py
+-rw-r--r--   0        0        0     3282 2024-04-09 18:38:03.763901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_source_list.py
+-rw-r--r--   0        0        0     3323 2024-04-09 18:38:03.767901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_source_stage_list.py
+-rw-r--r--   0        0        0     3274 2024-04-09 18:38:03.771901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_stage_list.py
+-rw-r--r--   0        0        0     3331 2024-04-09 18:38:03.775901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_static_device_list.py
+-rw-r--r--   0        0        0     3315 2024-04-09 18:38:03.775901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_system_task_list.py
+-rw-r--r--   0        0        0     3282 2024-04-09 18:38:03.783901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_tenant_list.py
+-rw-r--r--   0        0        0     3274 2024-04-09 18:38:03.783901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_token_list.py
+-rw-r--r--   0        0        0     3315 2024-04-09 18:38:03.787901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_token_model_list.py
+-rw-r--r--   0        0        0     3315 2024-04-09 18:38:03.779901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_totp_device_list.py
+-rw-r--r--   0        0        0     3461 2024-04-09 18:38:03.791901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3323 2024-04-09 18:38:03.795901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_consent_list.py
+-rw-r--r--   0        0        0     3356 2024-04-09 18:38:03.795901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_delete_stage_list.py
+-rw-r--r--   0        0        0     3266 2024-04-09 18:38:03.799901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_list.py
+-rw-r--r--   0        0        0     3348 2024-04-09 18:38:03.803901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_login_stage_list.py
+-rw-r--r--   0        0        0     3356 2024-04-09 18:38:03.803901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_logout_stage_list.py
+-rw-r--r--   0        0        0     3438 2024-04-09 18:38:03.807901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_o_auth_source_connection_list.py
+-rw-r--r--   0        0        0     3429 2024-04-09 18:38:03.807901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_saml_source_connection_list.py
+-rw-r--r--   0        0        0     3396 2024-04-09 18:38:03.811901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_source_connection_list.py
+-rw-r--r--   0        0        0     3348 2024-04-09 18:38:03.815901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_write_stage_list.py
+-rw-r--r--   0        0        0     3348 2024-04-09 18:38:03.815901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_web_authn_device_list.py
+-rw-r--r--   0        0        0     3381 2024-04-09 18:38:03.819901 authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_web_authn_device_type_list.py
+-rw-r--r--   0        0        0     3076 2024-04-09 18:38:03.819901 authentik_client-2024.2.2.post1712687873/authentik_client/models/pagination.py
+-rw-r--r--   0        0        0     4454 2024-04-09 18:38:03.823901 authentik_client-2024.2.2.post1712687873/authentik_client/models/password_challenge.py
+-rw-r--r--   0        0        0     2819 2024-04-09 18:38:03.827901 authentik_client-2024.2.2.post1712687873/authentik_client/models/password_challenge_response_request.py
+-rw-r--r--   0        0        0     4377 2024-04-09 18:38:03.827901 authentik_client-2024.2.2.post1712687873/authentik_client/models/password_expiry_policy.py
+-rw-r--r--   0        0        0     3099 2024-04-09 18:38:03.831901 authentik_client-2024.2.2.post1712687873/authentik_client/models/password_expiry_policy_request.py
+-rw-r--r--   0        0        0     6428 2024-04-09 18:38:03.835901 authentik_client-2024.2.2.post1712687873/authentik_client/models/password_policy.py
+-rw-r--r--   0        0        0     5239 2024-04-09 18:38:03.839901 authentik_client-2024.2.2.post1712687873/authentik_client/models/password_policy_request.py
+-rw-r--r--   0        0        0     5274 2024-04-09 18:38:03.839901 authentik_client-2024.2.2.post1712687873/authentik_client/models/password_stage.py
+-rw-r--r--   0        0        0     4264 2024-04-09 18:38:03.843901 authentik_client-2024.2.2.post1712687873/authentik_client/models/password_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-04-09 18:38:03.847901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_application_request.py
+-rw-r--r--   0        0        0     4833 2024-04-09 18:38:03.851901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     5701 2024-04-09 18:38:03.851901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4430 2024-04-09 18:38:03.855901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4256 2024-04-09 18:38:03.855901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     4743 2024-04-09 18:38:03.859901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5340 2024-04-09 18:38:03.863901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     3246 2024-04-09 18:38:03.867901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_blueprint_instance_request.py
+-rw-r--r--   0        0        0     6352 2024-04-09 18:38:03.867901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_brand_request.py
+-rw-r--r--   0        0        0     3860 2024-04-09 18:38:03.871901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_captcha_stage_request.py
+-rw-r--r--   0        0        0     3051 2024-04-09 18:38:03.871901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_certificate_key_pair_request.py
+-rw-r--r--   0        0        0     2717 2024-04-09 18:38:03.875901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_connection_token_request.py
+-rw-r--r--   0        0        0     3607 2024-04-09 18:38:03.879901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_consent_stage_request.py
+-rw-r--r--   0        0        0     3268 2024-04-09 18:38:03.879901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_deny_stage_request.py
+-rw-r--r--   0        0        0     4149 2024-04-09 18:38:03.883901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_docker_service_connection_request.py
+-rw-r--r--   0        0        0     2801 2024-04-09 18:38:03.887901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_domain_request.py
+-rw-r--r--   0        0        0     3275 2024-04-09 18:38:03.887901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_dummy_policy_request.py
+-rw-r--r--   0        0        0     3270 2024-04-09 18:38:03.891901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_dummy_stage_request.py
+-rw-r--r--   0        0        0     2674 2024-04-09 18:38:03.895901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_duo_device_request.py
+-rw-r--r--   0        0        0     5159 2024-04-09 18:38:03.895901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_email_stage_request.py
+-rw-r--r--   0        0        0     3784 2024-04-09 18:38:03.899901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_endpoint_request.py
+-rw-r--r--   0        0        0     4845 2024-04-09 18:38:03.903901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_event_matcher_policy_request.py
+-rw-r--r--   0        0        0     4045 2024-04-09 18:38:03.903901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_event_request.py
+-rw-r--r--   0        0        0     3047 2024-04-09 18:38:03.907901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_expression_policy_request.py
+-rw-r--r--   0        0        0     4903 2024-04-09 18:38:03.911901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_flow_request.py
+-rw-r--r--   0        0        0     4055 2024-04-09 18:38:03.915901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_flow_stage_binding_request.py
+-rw-r--r--   0        0        0     3385 2024-04-09 18:38:03.915901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_group_request.py
+-rw-r--r--   0        0        0     6571 2024-04-09 18:38:03.919901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_identification_stage_request.py
+-rw-r--r--   0        0        0     3774 2024-04-09 18:38:03.923901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_invitation_request.py
+-rw-r--r--   0        0        0     3565 2024-04-09 18:38:03.923901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_invitation_stage_request.py
+-rw-r--r--   0        0        0     3492 2024-04-09 18:38:03.927901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     3550 2024-04-09 18:38:03.931901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     6254 2024-04-09 18:38:03.931901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_ldap_provider_request.py
+-rw-r--r--   0        0        0     9697 2024-04-09 18:38:03.935901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_ldap_source_request.py
+-rw-r--r--   0        0        0     2557 2024-04-09 18:38:03.939901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_license_request.py
+-rw-r--r--   0        0        0     2879 2024-04-09 18:38:03.939901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_notification_request.py
+-rw-r--r--   0        0        0     3587 2024-04-09 18:38:03.943901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_notification_rule_request.py
+-rw-r--r--   0        0        0     3538 2024-04-09 18:38:03.943901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_notification_transport_request.py
+-rw-r--r--   0        0        0     2782 2024-04-09 18:38:03.947901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     6716 2024-04-09 18:38:03.951901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_o_auth2_provider_request.py
+-rw-r--r--   0        0        0     8185 2024-04-09 18:38:03.955901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_o_auth_source_request.py
+-rw-r--r--   0        0        0     4139 2024-04-09 18:38:03.955901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_outpost_request.py
+-rw-r--r--   0        0        0     3154 2024-04-09 18:38:03.959901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_password_expiry_policy_request.py
+-rw-r--r--   0        0        0     5277 2024-04-09 18:38:03.959901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_password_policy_request.py
+-rw-r--r--   0        0        0     4326 2024-04-09 18:38:03.963901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_password_stage_request.py
+-rw-r--r--   0        0        0     2922 2024-04-09 18:38:03.967901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_permission_assign_request.py
+-rw-r--r--   0        0        0     2784 2024-04-09 18:38:03.971901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_plex_source_connection_request.py
+-rw-r--r--   0        0        0     5905 2024-04-09 18:38:03.975901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_plex_source_request.py
+-rw-r--r--   0        0        0     4286 2024-04-09 18:38:03.979901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_policy_binding_request.py
+-rw-r--r--   0        0        0     5023 2024-04-09 18:38:03.983901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_prompt_request.py
+-rw-r--r--   0        0        0     3406 2024-04-09 18:38:03.987901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_prompt_stage_request.py
+-rw-r--r--   0        0        0     6907 2024-04-09 18:38:03.991901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_proxy_provider_request.py
+-rw-r--r--   0        0        0     3495 2024-04-09 18:38:03.991901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_rac_property_mapping_request.py
+-rw-r--r--   0        0        0     4413 2024-04-09 18:38:03.995901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_rac_provider_request.py
+-rw-r--r--   0        0        0     4563 2024-04-09 18:38:03.999901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_radius_provider_request.py
+-rw-r--r--   0        0        0     3276 2024-04-09 18:38:03.999901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_reputation_policy_request.py
+-rw-r--r--   0        0        0     2565 2024-04-09 18:38:04.003901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_role_request.py
+-rw-r--r--   0        0        0     3901 2024-04-09 18:38:04.003901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_saml_property_mapping_request.py
+-rw-r--r--   0        0        0     7539 2024-04-09 18:38:04.007901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_saml_provider_request.py
+-rw-r--r--   0        0        0     8676 2024-04-09 18:38:04.011901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_saml_source_request.py
+-rw-r--r--   0        0        0     3364 2024-04-09 18:38:04.011901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_scim_mapping_request.py
+-rw-r--r--   0        0        0     3888 2024-04-09 18:38:04.015901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_scim_provider_request.py
+-rw-r--r--   0        0        0     3819 2024-04-09 18:38:04.019901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_scope_mapping_request.py
+-rw-r--r--   0        0        0     4590 2024-04-09 18:38:04.019901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_settings_request.py
+-rw-r--r--   0        0        0     2674 2024-04-09 18:38:04.015901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_sms_device_request.py
+-rw-r--r--   0        0        0     3562 2024-04-09 18:38:04.023901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_source_stage_request.py
+-rw-r--r--   0        0        0     2686 2024-04-09 18:38:04.023901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_static_device_request.py
+-rw-r--r--   0        0        0     2820 2024-04-09 18:38:04.027901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_tenant_request.py
+-rw-r--r--   0        0        0     4208 2024-04-09 18:38:04.031901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_token_request.py
+-rw-r--r--   0        0        0     2678 2024-04-09 18:38:04.027901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_totp_device_request.py
+-rw-r--r--   0        0        0     3167 2024-04-09 18:38:04.031901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_user_delete_stage_request.py
+-rw-r--r--   0        0        0     4766 2024-04-09 18:38:04.035901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_user_login_stage_request.py
+-rw-r--r--   0        0        0     3167 2024-04-09 18:38:04.035901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_user_logout_stage_request.py
+-rw-r--r--   0        0        0     3109 2024-04-09 18:38:04.039901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3934 2024-04-09 18:38:04.039901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_user_request.py
+-rw-r--r--   0        0        0     2733 2024-04-09 18:38:04.043901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     4450 2024-04-09 18:38:04.043901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_user_write_stage_request.py
+-rw-r--r--   0        0        0     2625 2024-04-09 18:38:04.047901 authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_web_authn_device_request.py
+-rw-r--r--   0        0        0     3548 2024-04-09 18:38:04.047901 authentik_client-2024.2.2.post1712687873/authentik_client/models/permission.py
+-rw-r--r--   0        0        0     2884 2024-04-09 18:38:04.051901 authentik_client-2024.2.2.post1712687873/authentik_client/models/permission_assign_request.py
+-rw-r--r--   0        0        0     4315 2024-04-09 18:38:04.051901 authentik_client-2024.2.2.post1712687873/authentik_client/models/plex_authentication_challenge.py
+-rw-r--r--   0        0        0     2726 2024-04-09 18:38:04.055901 authentik_client-2024.2.2.post1712687873/authentik_client/models/plex_authentication_challenge_response_request.py
+-rw-r--r--   0        0        0     7752 2024-04-09 18:38:04.059901 authentik_client-2024.2.2.post1712687873/authentik_client/models/plex_source.py
+-rw-r--r--   0        0        0     3265 2024-04-09 18:38:04.063901 authentik_client-2024.2.2.post1712687873/authentik_client/models/plex_source_connection.py
+-rw-r--r--   0        0        0     2719 2024-04-09 18:38:04.067901 authentik_client-2024.2.2.post1712687873/authentik_client/models/plex_source_connection_request.py
+-rw-r--r--   0        0        0     5760 2024-04-09 18:38:04.067901 authentik_client-2024.2.2.post1712687873/authentik_client/models/plex_source_request.py
+-rw-r--r--   0        0        0     2576 2024-04-09 18:38:04.071901 authentik_client-2024.2.2.post1712687873/authentik_client/models/plex_token_redeem_request.py
+-rw-r--r--   0        0        0     4055 2024-04-09 18:38:04.075901 authentik_client-2024.2.2.post1712687873/authentik_client/models/policy.py
+-rw-r--r--   0        0        0     5643 2024-04-09 18:38:04.075901 authentik_client-2024.2.2.post1712687873/authentik_client/models/policy_binding.py
+-rw-r--r--   0        0        0     4231 2024-04-09 18:38:04.079901 authentik_client-2024.2.2.post1712687873/authentik_client/models/policy_binding_request.py
+-rw-r--r--   0        0        0      711 2024-04-09 18:38:04.079901 authentik_client-2024.2.2.post1712687873/authentik_client/models/policy_engine_mode.py
+-rw-r--r--   0        0        0     2817 2024-04-09 18:38:04.083901 authentik_client-2024.2.2.post1712687873/authentik_client/models/policy_request.py
+-rw-r--r--   0        0        0     2583 2024-04-09 18:38:04.083901 authentik_client-2024.2.2.post1712687873/authentik_client/models/policy_test_request.py
+-rw-r--r--   0        0        0     3281 2024-04-09 18:38:04.087901 authentik_client-2024.2.2.post1712687873/authentik_client/models/policy_test_result.py
+-rw-r--r--   0        0        0     4885 2024-04-09 18:38:04.087901 authentik_client-2024.2.2.post1712687873/authentik_client/models/prompt.py
+-rw-r--r--   0        0        0     4649 2024-04-09 18:38:04.091901 authentik_client-2024.2.2.post1712687873/authentik_client/models/prompt_challenge.py
+-rw-r--r--   0        0        0     3325 2024-04-09 18:38:04.091901 authentik_client-2024.2.2.post1712687873/authentik_client/models/prompt_challenge_response_request.py
+-rw-r--r--   0        0        0     4927 2024-04-09 18:38:04.095901 authentik_client-2024.2.2.post1712687873/authentik_client/models/prompt_request.py
+-rw-r--r--   0        0        0     4321 2024-04-09 18:38:04.095901 authentik_client-2024.2.2.post1712687873/authentik_client/models/prompt_stage.py
+-rw-r--r--   0        0        0     3351 2024-04-09 18:38:04.099901 authentik_client-2024.2.2.post1712687873/authentik_client/models/prompt_stage_request.py
+-rw-r--r--   0        0        0     1185 2024-04-09 18:38:04.099901 authentik_client-2024.2.2.post1712687873/authentik_client/models/prompt_type_enum.py
+-rw-r--r--   0        0        0     4264 2024-04-09 18:38:04.103901 authentik_client-2024.2.2.post1712687873/authentik_client/models/property_mapping.py
+-rw-r--r--   0        0        0     2610 2024-04-09 18:38:04.103901 authentik_client-2024.2.2.post1712687873/authentik_client/models/property_mapping_preview.py
+-rw-r--r--   0        0        0     2744 2024-04-09 18:38:04.107901 authentik_client-2024.2.2.post1712687873/authentik_client/models/property_mapping_test_result.py
+-rw-r--r--   0        0        0      715 2024-04-09 18:38:04.107901 authentik_client-2024.2.2.post1712687873/authentik_client/models/protocol_enum.py
+-rw-r--r--   0        0        0     5722 2024-04-09 18:38:04.107901 authentik_client-2024.2.2.post1712687873/authentik_client/models/provider.py
+-rw-r--r--   0        0        0      713 2024-04-09 18:38:04.111901 authentik_client-2024.2.2.post1712687873/authentik_client/models/provider_enum.py
+-rw-r--r--   0        0        0     1314 2024-04-09 18:38:04.111901 authentik_client-2024.2.2.post1712687873/authentik_client/models/provider_model_enum.py
+-rw-r--r--   0        0        0     3397 2024-04-09 18:38:04.111901 authentik_client-2024.2.2.post1712687873/authentik_client/models/provider_request.py
+-rw-r--r--   0        0        0     1009 2024-04-09 18:38:04.115901 authentik_client-2024.2.2.post1712687873/authentik_client/models/provider_type_enum.py
+-rw-r--r--   0        0        0      754 2024-04-09 18:38:04.115901 authentik_client-2024.2.2.post1712687873/authentik_client/models/proxy_mode.py
+-rw-r--r--   0        0        0     7819 2024-04-09 18:38:04.115901 authentik_client-2024.2.2.post1712687873/authentik_client/models/proxy_outpost_config.py
+-rw-r--r--   0        0        0     9552 2024-04-09 18:38:04.119901 authentik_client-2024.2.2.post1712687873/authentik_client/models/proxy_provider.py
+-rw-r--r--   0        0        0     6828 2024-04-09 18:38:04.123901 authentik_client-2024.2.2.post1712687873/authentik_client/models/proxy_provider_request.py
+-rw-r--r--   0        0        0     4407 2024-04-09 18:38:04.123901 authentik_client-2024.2.2.post1712687873/authentik_client/models/rac_property_mapping.py
+-rw-r--r--   0        0        0     3440 2024-04-09 18:38:04.127901 authentik_client-2024.2.2.post1712687873/authentik_client/models/rac_property_mapping_request.py
+-rw-r--r--   0        0        0     6813 2024-04-09 18:38:04.127901 authentik_client-2024.2.2.post1712687873/authentik_client/models/rac_provider.py
+-rw-r--r--   0        0        0     4351 2024-04-09 18:38:04.131901 authentik_client-2024.2.2.post1712687873/authentik_client/models/rac_provider_request.py
+-rw-r--r--   0        0        0     3833 2024-04-09 18:38:04.131901 authentik_client-2024.2.2.post1712687873/authentik_client/models/radius_outpost_config.py
+-rw-r--r--   0        0        0     6924 2024-04-09 18:38:04.135901 authentik_client-2024.2.2.post1712687873/authentik_client/models/radius_provider.py
+-rw-r--r--   0        0        0     4501 2024-04-09 18:38:04.135901 authentik_client-2024.2.2.post1712687873/authentik_client/models/radius_provider_request.py
+-rw-r--r--   0        0        0     4184 2024-04-09 18:38:04.139901 authentik_client-2024.2.2.post1712687873/authentik_client/models/redirect_challenge.py
+-rw-r--r--   0        0        0     3642 2024-04-09 18:38:04.143901 authentik_client-2024.2.2.post1712687873/authentik_client/models/reputation.py
+-rw-r--r--   0        0        0     4516 2024-04-09 18:38:04.143901 authentik_client-2024.2.2.post1712687873/authentik_client/models/reputation_policy.py
+-rw-r--r--   0        0        0     3238 2024-04-09 18:38:04.143901 authentik_client-2024.2.2.post1712687873/authentik_client/models/reputation_policy_request.py
+-rw-r--r--   0        0        0      795 2024-04-09 18:38:04.147901 authentik_client-2024.2.2.post1712687873/authentik_client/models/resident_key_requirement_enum.py
+-rw-r--r--   0        0        0     2618 2024-04-09 18:38:04.147901 authentik_client-2024.2.2.post1712687873/authentik_client/models/role.py
+-rw-r--r--   0        0        0     3333 2024-04-09 18:38:04.151901 authentik_client-2024.2.2.post1712687873/authentik_client/models/role_assigned_object_permission.py
+-rw-r--r--   0        0        0     3293 2024-04-09 18:38:04.151901 authentik_client-2024.2.2.post1712687873/authentik_client/models/role_object_permission.py
+-rw-r--r--   0        0        0     2517 2024-04-09 18:38:04.155901 authentik_client-2024.2.2.post1712687873/authentik_client/models/role_request.py
+-rw-r--r--   0        0        0     2712 2024-04-09 18:38:04.155901 authentik_client-2024.2.2.post1712687873/authentik_client/models/saml_metadata.py
+-rw-r--r--   0        0        0     4718 2024-04-09 18:38:04.159901 authentik_client-2024.2.2.post1712687873/authentik_client/models/saml_property_mapping.py
+-rw-r--r--   0        0        0     3829 2024-04-09 18:38:04.159901 authentik_client-2024.2.2.post1712687873/authentik_client/models/saml_property_mapping_request.py
+-rw-r--r--   0        0        0    11056 2024-04-09 18:38:04.163901 authentik_client-2024.2.2.post1712687873/authentik_client/models/saml_provider.py
+-rw-r--r--   0        0        0     7460 2024-04-09 18:38:04.163901 authentik_client-2024.2.2.post1712687873/authentik_client/models/saml_provider_request.py
+-rw-r--r--   0        0        0    10563 2024-04-09 18:38:04.167901 authentik_client-2024.2.2.post1712687873/authentik_client/models/saml_source.py
+-rw-r--r--   0        0        0     8507 2024-04-09 18:38:04.167901 authentik_client-2024.2.2.post1712687873/authentik_client/models/saml_source_request.py
+-rw-r--r--   0        0        0     4248 2024-04-09 18:38:04.171901 authentik_client-2024.2.2.post1712687873/authentik_client/models/scim_mapping.py
+-rw-r--r--   0        0        0     3309 2024-04-09 18:38:04.171901 authentik_client-2024.2.2.post1712687873/authentik_client/models/scim_mapping_request.py
+-rw-r--r--   0        0        0     5454 2024-04-09 18:38:04.175901 authentik_client-2024.2.2.post1712687873/authentik_client/models/scim_provider.py
+-rw-r--r--   0        0        0     3802 2024-04-09 18:38:04.179901 authentik_client-2024.2.2.post1712687873/authentik_client/models/scim_provider_request.py
+-rw-r--r--   0        0        0     3131 2024-04-09 18:38:04.183901 authentik_client-2024.2.2.post1712687873/authentik_client/models/scim_sync_status.py
+-rw-r--r--   0        0        0     4629 2024-04-09 18:38:04.187901 authentik_client-2024.2.2.post1712687873/authentik_client/models/scope_mapping.py
+-rw-r--r--   0        0        0     3740 2024-04-09 18:38:04.191901 authentik_client-2024.2.2.post1712687873/authentik_client/models/scope_mapping_request.py
+-rw-r--r--   0        0        0     2738 2024-04-09 18:38:04.195901 authentik_client-2024.2.2.post1712687873/authentik_client/models/selectable_stage.py
+-rw-r--r--   0        0        0     3773 2024-04-09 18:38:04.199901 authentik_client-2024.2.2.post1712687873/authentik_client/models/service_connection.py
+-rw-r--r--   0        0        0     2776 2024-04-09 18:38:04.203901 authentik_client-2024.2.2.post1712687873/authentik_client/models/service_connection_request.py
+-rw-r--r--   0        0        0     2731 2024-04-09 18:38:04.203901 authentik_client-2024.2.2.post1712687873/authentik_client/models/service_connection_state.py
+-rw-r--r--   0        0        0     3178 2024-04-09 18:38:04.207901 authentik_client-2024.2.2.post1712687873/authentik_client/models/session_user.py
+-rw-r--r--   0        0        0     4441 2024-04-09 18:38:04.211901 authentik_client-2024.2.2.post1712687873/authentik_client/models/settings.py
+-rw-r--r--   0        0        0     4569 2024-04-09 18:38:04.215901 authentik_client-2024.2.2.post1712687873/authentik_client/models/settings_request.py
+-rw-r--r--   0        0        0      733 2024-04-09 18:38:04.215901 authentik_client-2024.2.2.post1712687873/authentik_client/models/severity_enum.py
+-rw-r--r--   0        0        0     4175 2024-04-09 18:38:04.219901 authentik_client-2024.2.2.post1712687873/authentik_client/models/shell_challenge.py
+-rw-r--r--   0        0        0     1492 2024-04-09 18:38:04.219901 authentik_client-2024.2.2.post1712687873/authentik_client/models/signature_algorithm_enum.py
+-rw-r--r--   0        0        0     2906 2024-04-09 18:38:04.183901 authentik_client-2024.2.2.post1712687873/authentik_client/models/sms_device.py
+-rw-r--r--   0        0        0     2619 2024-04-09 18:38:04.187901 authentik_client-2024.2.2.post1712687873/authentik_client/models/sms_device_request.py
+-rw-r--r--   0        0        0     6945 2024-04-09 18:38:04.223901 authentik_client-2024.2.2.post1712687873/authentik_client/models/source.py
+-rw-r--r--   0        0        0     4836 2024-04-09 18:38:04.227901 authentik_client-2024.2.2.post1712687873/authentik_client/models/source_request.py
+-rw-r--r--   0        0        0     4438 2024-04-09 18:38:04.231901 authentik_client-2024.2.2.post1712687873/authentik_client/models/source_stage.py
+-rw-r--r--   0        0        0     3507 2024-04-09 18:38:04.235901 authentik_client-2024.2.2.post1712687873/authentik_client/models/source_stage_request.py
+-rw-r--r--   0        0        0     5355 2024-04-09 18:38:04.235901 authentik_client-2024.2.2.post1712687873/authentik_client/models/source_type.py
+-rw-r--r--   0        0        0      714 2024-04-09 18:38:04.239901 authentik_client-2024.2.2.post1712687873/authentik_client/models/sp_binding_enum.py
+-rw-r--r--   0        0        0     4070 2024-04-09 18:38:04.239901 authentik_client-2024.2.2.post1712687873/authentik_client/models/stage.py
+-rw-r--r--   0        0        0     3437 2024-04-09 18:38:04.243901 authentik_client-2024.2.2.post1712687873/authentik_client/models/stage_prompt.py
+-rw-r--r--   0        0        0     3089 2024-04-09 18:38:04.247901 authentik_client-2024.2.2.post1712687873/authentik_client/models/stage_request.py
+-rw-r--r--   0        0        0     3385 2024-04-09 18:38:04.251901 authentik_client-2024.2.2.post1712687873/authentik_client/models/static_device.py
+-rw-r--r--   0        0        0     2631 2024-04-09 18:38:04.251901 authentik_client-2024.2.2.post1712687873/authentik_client/models/static_device_request.py
+-rw-r--r--   0        0        0     2546 2024-04-09 18:38:04.255901 authentik_client-2024.2.2.post1712687873/authentik_client/models/static_device_token.py
+-rw-r--r--   0        0        0     2581 2024-04-09 18:38:04.259901 authentik_client-2024.2.2.post1712687873/authentik_client/models/static_device_token_request.py
+-rw-r--r--   0        0        0      846 2024-04-09 18:38:04.259901 authentik_client-2024.2.2.post1712687873/authentik_client/models/sub_mode_enum.py
+-rw-r--r--   0        0        0     4463 2024-04-09 18:38:04.263901 authentik_client-2024.2.2.post1712687873/authentik_client/models/system_info.py
+-rw-r--r--   0        0        0     2934 2024-04-09 18:38:04.267901 authentik_client-2024.2.2.post1712687873/authentik_client/models/system_info_runtime.py
+-rw-r--r--   0        0        0     4286 2024-04-09 18:38:04.267901 authentik_client-2024.2.2.post1712687873/authentik_client/models/system_task.py
+-rw-r--r--   0        0        0      789 2024-04-09 18:38:04.271901 authentik_client-2024.2.2.post1712687873/authentik_client/models/system_task_status_enum.py
+-rw-r--r--   0        0        0     2872 2024-04-09 18:38:04.279901 authentik_client-2024.2.2.post1712687873/authentik_client/models/tenant.py
+-rw-r--r--   0        0        0     2589 2024-04-09 18:38:04.279901 authentik_client-2024.2.2.post1712687873/authentik_client/models/tenant_admin_group_request_request.py
+-rw-r--r--   0        0        0     2705 2024-04-09 18:38:04.283901 authentik_client-2024.2.2.post1712687873/authentik_client/models/tenant_recovery_key_request_request.py
+-rw-r--r--   0        0        0     2599 2024-04-09 18:38:04.287901 authentik_client-2024.2.2.post1712687873/authentik_client/models/tenant_recovery_key_response.py
+-rw-r--r--   0        0        0     2765 2024-04-09 18:38:04.291901 authentik_client-2024.2.2.post1712687873/authentik_client/models/tenant_request.py
+-rw-r--r--   0        0        0     4591 2024-04-09 18:38:04.291901 authentik_client-2024.2.2.post1712687873/authentik_client/models/token.py
+-rw-r--r--   0        0        0     3987 2024-04-09 18:38:04.295901 authentik_client-2024.2.2.post1712687873/authentik_client/models/token_model.py
+-rw-r--r--   0        0        0     4118 2024-04-09 18:38:04.303901 authentik_client-2024.2.2.post1712687873/authentik_client/models/token_request.py
+-rw-r--r--   0        0        0     2521 2024-04-09 18:38:04.303901 authentik_client-2024.2.2.post1712687873/authentik_client/models/token_set_key_request.py
+-rw-r--r--   0        0        0     2494 2024-04-09 18:38:04.307901 authentik_client-2024.2.2.post1712687873/authentik_client/models/token_view.py
+-rw-r--r--   0        0        0     2724 2024-04-09 18:38:04.271901 authentik_client-2024.2.2.post1712687873/authentik_client/models/totp_device.py
+-rw-r--r--   0        0        0     2623 2024-04-09 18:38:04.275901 authentik_client-2024.2.2.post1712687873/authentik_client/models/totp_device_request.py
+-rw-r--r--   0        0        0     3389 2024-04-09 18:38:04.311901 authentik_client-2024.2.2.post1712687873/authentik_client/models/transaction_application_request.py
+-rw-r--r--   0        0        0     2595 2024-04-09 18:38:04.311901 authentik_client-2024.2.2.post1712687873/authentik_client/models/transaction_application_response.py
+-rw-r--r--   0        0        0     2936 2024-04-09 18:38:04.315901 authentik_client-2024.2.2.post1712687873/authentik_client/models/type_create.py
+-rw-r--r--   0        0        0      730 2024-04-09 18:38:04.319901 authentik_client-2024.2.2.post1712687873/authentik_client/models/ui_theme_enum.py
+-rw-r--r--   0        0        0     2808 2024-04-09 18:38:04.319901 authentik_client-2024.2.2.post1712687873/authentik_client/models/used_by.py
+-rw-r--r--   0        0        0      795 2024-04-09 18:38:04.323901 authentik_client-2024.2.2.post1712687873/authentik_client/models/used_by_action_enum.py
+-rw-r--r--   0        0        0     5226 2024-04-09 18:38:04.323901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user.py
+-rw-r--r--   0        0        0     2458 2024-04-09 18:38:04.327901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_account_request.py
+-rw-r--r--   0        0        0     4946 2024-04-09 18:38:04.331901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_assigned_object_permission.py
+-rw-r--r--   0        0        0     3617 2024-04-09 18:38:04.335901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_consent.py
+-rw-r--r--   0        0        0      811 2024-04-09 18:38:04.335901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_creation_mode_enum.py
+-rw-r--r--   0        0        0     4110 2024-04-09 18:38:04.339901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_delete_stage.py
+-rw-r--r--   0        0        0     3129 2024-04-09 18:38:04.343901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_delete_stage_request.py
+-rw-r--r--   0        0        0      735 2024-04-09 18:38:04.343901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_fields_enum.py
+-rw-r--r--   0        0        0     3909 2024-04-09 18:38:04.347901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_group.py
+-rw-r--r--   0        0        0     3193 2024-04-09 18:38:04.351901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_group_request.py
+-rw-r--r--   0        0        0     4334 2024-04-09 18:38:04.355901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_login_challenge.py
+-rw-r--r--   0        0        0     2805 2024-04-09 18:38:04.355901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_login_challenge_response_request.py
+-rw-r--r--   0        0        0     5631 2024-04-09 18:38:04.359901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_login_stage.py
+-rw-r--r--   0        0        0     4728 2024-04-09 18:38:04.363901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_login_stage_request.py
+-rw-r--r--   0        0        0     4110 2024-04-09 18:38:04.367901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_logout_stage.py
+-rw-r--r--   0        0        0     3129 2024-04-09 18:38:04.367901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_logout_stage_request.py
+-rw-r--r--   0        0        0      853 2024-04-09 18:38:04.371901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_matching_mode_enum.py
+-rw-r--r--   0        0        0     4160 2024-04-09 18:38:04.371901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_metrics.py
+-rw-r--r--   0        0        0     3188 2024-04-09 18:38:04.375901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_o_auth_source_connection.py
+-rw-r--r--   0        0        0     3054 2024-04-09 18:38:04.375901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3293 2024-04-09 18:38:04.379901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_object_permission.py
+-rw-r--r--   0        0        0     2557 2024-04-09 18:38:04.379901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_password_set_request.py
+-rw-r--r--   0        0        0     2491 2024-04-09 18:38:04.383901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_path.py
+-rw-r--r--   0        0        0     3872 2024-04-09 18:38:04.383901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_request.py
+-rw-r--r--   0        0        0     3107 2024-04-09 18:38:04.387901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_saml_source_connection.py
+-rw-r--r--   0        0        0     2668 2024-04-09 18:38:04.391901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     5465 2024-04-09 18:38:04.391901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_self.py
+-rw-r--r--   0        0        0     2629 2024-04-09 18:38:04.395901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_self_groups.py
+-rw-r--r--   0        0        0     3074 2024-04-09 18:38:04.395901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_service_account_request.py
+-rw-r--r--   0        0        0     2844 2024-04-09 18:38:04.399901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_service_account_response.py
+-rw-r--r--   0        0        0     2866 2024-04-09 18:38:04.399901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_setting.py
+-rw-r--r--   0        0        0     3245 2024-04-09 18:38:04.403901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_source_connection.py
+-rw-r--r--   0        0        0      817 2024-04-09 18:38:04.403901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_type_enum.py
+-rw-r--r--   0        0        0      777 2024-04-09 18:38:04.403901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_verification_enum.py
+-rw-r--r--   0        0        0     5382 2024-04-09 18:38:04.407901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_write_stage.py
+-rw-r--r--   0        0        0     4412 2024-04-09 18:38:04.411901 authentik_client-2024.2.2.post1712687873/authentik_client/models/user_write_stage_request.py
+-rw-r--r--   0        0        0     3197 2024-04-09 18:38:04.411901 authentik_client-2024.2.2.post1712687873/authentik_client/models/validation_error.py
+-rw-r--r--   0        0        0     3589 2024-04-09 18:38:04.415901 authentik_client-2024.2.2.post1712687873/authentik_client/models/version.py
+-rw-r--r--   0        0        0     3630 2024-04-09 18:38:04.415901 authentik_client-2024.2.2.post1712687873/authentik_client/models/web_authn_device.py
+-rw-r--r--   0        0        0     2577 2024-04-09 18:38:04.419901 authentik_client-2024.2.2.post1712687873/authentik_client/models/web_authn_device_request.py
+-rw-r--r--   0        0        0     2562 2024-04-09 18:38:04.419901 authentik_client-2024.2.2.post1712687873/authentik_client/models/web_authn_device_type.py
+-rw-r--r--   0        0        0     2669 2024-04-09 18:38:04.423901 authentik_client-2024.2.2.post1712687873/authentik_client/models/web_authn_device_type_request.py
+-rw-r--r--   0        0        0     2410 2024-04-09 18:38:04.423901 authentik_client-2024.2.2.post1712687873/authentik_client/models/workers.py
+-rw-r--r--   0        0        0        0 2024-04-09 18:38:05.627901 authentik_client-2024.2.2.post1712687873/authentik_client/py.typed
+-rw-r--r--   0        0        0     9196 2024-04-09 18:38:05.639901 authentik_client-2024.2.2.post1712687873/authentik_client/rest.py
+-rw-r--r--   0        0        0     1936 2024-04-09 18:38:05.627901 authentik_client-2024.2.2.post1712687873/pyproject.toml
+-rw-r--r--   0        0        0   141557 1970-01-01 00:00:00.000000 authentik_client-2024.2.2.post1712687873/PKG-INFO
```

### Comparing `authentik_client-2024.2.2.post1712571742/README.md` & `authentik_client-2024.2.2.post1712687873/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2024.2.2
-- Package version: 2024.2.2-1712571742
+- Package version: 2024.2.2-1712687873
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/__init__.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "2024.2.2-1712571742"
+__version__ = "2024.2.2-1712687873"
 
 # import apis into sdk package
 from authentik_client.api.admin_api import AdminApi
 from authentik_client.api.authenticators_api import AuthenticatorsApi
 from authentik_client.api.core_api import CoreApi
 from authentik_client.api.crypto_api import CryptoApi
 from authentik_client.api.enterprise_api import EnterpriseApi
```

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/__init__.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/admin_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/authenticators_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/authenticators_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/core_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/crypto_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/crypto_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/enterprise_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/enterprise_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/events_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/events_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/flows_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/flows_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/managed_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/managed_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/oauth2_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/oauth2_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/outposts_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/outposts_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/policies_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/policies_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/propertymappings_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/propertymappings_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/providers_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/providers_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/rac_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/rac_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/rbac_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/rbac_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/root_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/root_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/schema_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/sources_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/sources_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/stages_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/stages_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api/tenants_api.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api/tenants_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api_client.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2024.2.2-1712571742/python'
+        self.user_agent = 'OpenAPI-Generator/2024.2.2-1712687873/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/api_response.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/api_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/configuration.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2024.2.2\n"\
-               "SDK Package Version: 2024.2.2-1712571742".\
+               "SDK Package Version: 2024.2.2-1712687873".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/exceptions.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/__init__.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/access_denied_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/access_denied_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/app.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/app.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/app_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/app_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/apple_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/apple_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/apple_login_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/apple_login_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/application.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/application.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/application_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/auth_mode_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/auth_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/auth_type_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/auth_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticated_session.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_asn.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticated_session_asn.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_geo_ip.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticated_session_geo_ip.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticated_session_user_agent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent_device.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticated_session_user_agent_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent_os.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticated_session_user_agent_os.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent_user_agent.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticated_session_user_agent_user_agent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authentication_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authentication_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_attachment_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_attachment_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_duo_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_duo_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_duo_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage_device_import_response.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_duo_stage_device_import_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_duo_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_sms_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_sms_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_sms_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_sms_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_static_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_static_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_static_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_static_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_totp_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_totp_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_totp_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_totp_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validate_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_validate_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validate_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_validate_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validation_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_validation_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validation_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_validation_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_web_authn_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_web_authn_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_web_authn_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_web_authn_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_web_authn_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_web_authn_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_web_authn_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/authenticator_web_authn_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/auto_submit_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/auto_submit_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/autosubmit_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/autosubmit_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/backends_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/backends_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/binding_type_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/binding_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_file.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/blueprint_file.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_instance.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/blueprint_instance.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_instance_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/blueprint_instance_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_instance_status_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/blueprint_instance_status_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/brand.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/brand.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/brand_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/brand_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/cache.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/cache.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/capabilities_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/capabilities_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/captcha_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/captcha_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/captcha_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/captcha_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_data.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/certificate_data.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_generation_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/certificate_generation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_key_pair.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/certificate_key_pair.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_key_pair_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/certificate_key_pair_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/challenge_choices.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/challenge_choices.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/challenge_types.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/challenge_types.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/client_type_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/client_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/config.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/connection_token.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/connection_token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/connection_token_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/connection_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/consent_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/consent_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_permission.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/consent_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/consent_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_stage_mode_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/consent_stage_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/consent_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/contextual_flow_info.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/contextual_flow_info.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/contextual_flow_info_layout_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/contextual_flow_info_layout_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/coordinate.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/coordinate.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/current_brand.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/current_brand.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/denied_action_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/denied_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/deny_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/deny_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/deny_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/deny_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/device.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/device_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/device_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/device_challenge_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/device_challenge_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/device_classes_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/device_classes_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/digest_algorithm_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/digest_algorithm_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/digits_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/digits_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/docker_service_connection.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/docker_service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/docker_service_connection_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/docker_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/domain.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/domain.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/domain_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/domain_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/dummy_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/dummy_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_policy.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/dummy_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_policy_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/dummy_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/dummy_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/dummy_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_device.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/duo_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_device_enrollment_status.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/duo_device_enrollment_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_device_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/duo_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_response_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/duo_response_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/email_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/email_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/email_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/email_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/email_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/email_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/email_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/email_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/endpoint.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/endpoint_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/endpoint_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/error_detail.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/error_detail.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/error_reporting_config.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/error_reporting_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/event.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/event.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/event_actions.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/event_actions.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/event_matcher_policy.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/event_matcher_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/event_matcher_policy_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/event_matcher_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/event_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/event_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/event_top_per_user.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/event_top_per_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/expiring_base_grant_model.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/expiring_base_grant_model.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/expression_policy.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/expression_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/expression_policy_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/expression_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/extra_role_object_permission.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/extra_role_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/extra_user_object_permission.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/extra_user_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/file_path_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/file_path_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/flow.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_designation_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_designation_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_diagram.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_diagram.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_error_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_error_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_import_result.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_import_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_inspection.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_inspection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_inspector_plan.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_inspector_plan.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_layout_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_layout_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_set.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_set.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_set_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_set_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_stage_binding.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_stage_binding.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_stage_binding_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/flow_stage_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/footer_link.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/footer_link.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/generic_error.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/generic_error.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/geoip_binding_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/geoip_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/group.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/group_member.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/group_member.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/group_member_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/group_member_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/group_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/identification_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/identification_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/identification_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/identification_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/install_id.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/install_id.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/intent_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/intent_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/invalid_response_action_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/invalid_response_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/invitation.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/invitation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/invitation_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/invitation_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/issuer_mode_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/issuer_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/kubernetes_service_connection.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/kubernetes_service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/kubernetes_service_connection_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/kubernetes_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_debug.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_debug.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_outpost_config.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_property_mapping.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_property_mapping_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_provider.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_provider_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_source.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_source_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_sync_status.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/ldap_sync_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldapapi_access_mode.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/ldapapi_access_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/license.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/license.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/license_forecast.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/license_forecast.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/license_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/license_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/license_summary.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/license_summary.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/link.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/link.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/log_event.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/log_event.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/log_level_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/log_level_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/login_challenge_types.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/login_challenge_types.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/login_metrics.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/login_metrics.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/login_source.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/login_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/metadata.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/metadata.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/model_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/model_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/model_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/model_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/name_id_policy_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/name_id_policy_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/network_binding_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/network_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/not_configured_action_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/not_configured_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/notification.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_rule.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_rule.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_rule_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_rule_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_transport.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport_mode_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_transport_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_transport_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport_test.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_transport_test.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_webhook_mapping.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_webhook_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_webhook_mapping_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/notification_webhook_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth2_provider.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth2_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth2_provider_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth2_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth2_provider_setup_urls.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth2_provider_setup_urls.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth_device_code_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth_device_code_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_finish_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth_device_code_finish_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_source.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_source_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/o_auth_source_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,18 @@
     enabled: Optional[StrictBool] = None
     authentication_flow: Optional[StrictStr] = Field(default=None, description="Flow to use when authenticating existing users.")
     enrollment_flow: Optional[StrictStr] = Field(default=None, description="Flow to use when enrolling new users.")
     policy_engine_mode: Optional[PolicyEngineMode] = None
     user_matching_mode: Optional[UserMatchingModeEnum] = Field(default=None, description="How the source determines if an existing user should be authenticated or a new user enrolled.")
     user_path_template: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
     provider_type: ProviderTypeEnum
-    request_token_url: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=255)]] = Field(default=None, description="URL used to request the initial token. This URL is only required for OAuth 1.")
-    authorization_url: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=255)]] = Field(default=None, description="URL the user is redirect to to conest the flow.")
-    access_token_url: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=255)]] = Field(default=None, description="URL used by authentik to retrieve tokens.")
-    profile_url: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=255)]] = Field(default=None, description="URL used by authentik to get user information.")
+    request_token_url: Optional[Annotated[str, Field(strict=True, max_length=255)]] = Field(default=None, description="URL used to request the initial token. This URL is only required for OAuth 1.")
+    authorization_url: Optional[Annotated[str, Field(strict=True, max_length=255)]] = Field(default=None, description="URL the user is redirect to to conest the flow.")
+    access_token_url: Optional[Annotated[str, Field(strict=True, max_length=255)]] = Field(default=None, description="URL used by authentik to retrieve tokens.")
+    profile_url: Optional[Annotated[str, Field(strict=True, max_length=255)]] = Field(default=None, description="URL used by authentik to get user information.")
     consumer_key: Annotated[str, Field(min_length=1, strict=True)]
     consumer_secret: Annotated[str, Field(min_length=1, strict=True)]
     additional_scopes: Optional[StrictStr] = None
     oidc_well_known_url: Optional[StrictStr] = None
     oidc_jwks_url: Optional[StrictStr] = None
     oidc_jwks: Optional[Any] = None
     __properties: ClassVar[List[str]] = ["name", "slug", "enabled", "authentication_flow", "enrollment_flow", "policy_engine_mode", "user_matching_mode", "user_path_template", "provider_type", "request_token_url", "authorization_url", "access_token_url", "profile_url", "consumer_key", "consumer_secret", "additional_scopes", "oidc_well_known_url", "oidc_jwks_url", "oidc_jwks"]
```

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/open_id_connect_configuration.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/open_id_connect_configuration.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/outpost.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_default_config.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/outpost_default_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_health.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/outpost_health.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/outpost_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_type_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/outpost_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_application_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_application_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticated_session_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_authenticated_session_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_duo_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_authenticator_duo_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_sms_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_authenticator_sms_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_static_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_authenticator_static_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_totp_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_authenticator_totp_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_validate_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_authenticator_validate_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_web_authn_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_authenticator_web_authn_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_blueprint_instance_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_blueprint_instance_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_brand_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_brand_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_captcha_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_captcha_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_certificate_key_pair_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_certificate_key_pair_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_connection_token_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_connection_token_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_consent_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_consent_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_deny_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_deny_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_docker_service_connection_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_docker_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_domain_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_domain_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_dummy_policy_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_dummy_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_dummy_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_dummy_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_duo_device_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_duo_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_email_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_email_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_endpoint_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_endpoint_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_event_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_event_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_event_matcher_policy_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_event_matcher_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_expiring_base_grant_model_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_expiring_base_grant_model_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_expression_policy_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_expression_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_extra_role_object_permission_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_extra_role_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_extra_user_object_permission_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_extra_user_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_flow_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_flow_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_flow_stage_binding_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_flow_stage_binding_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_group_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_group_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_identification_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_identification_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_invitation_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_invitation_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_invitation_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_invitation_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_kubernetes_service_connection_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_kubernetes_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_outpost_config_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_ldap_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_property_mapping_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_ldap_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_provider_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_ldap_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_source_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_ldap_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_license_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_license_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_notification_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_rule_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_notification_rule_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_transport_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_notification_transport_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_webhook_mapping_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_notification_webhook_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_o_auth2_provider_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_o_auth2_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_o_auth_source_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_o_auth_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_outpost_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_outpost_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_password_expiry_policy_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_password_expiry_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_password_policy_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_password_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_password_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_password_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_permission_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_plex_source_connection_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_plex_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_plex_source_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_plex_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_policy_binding_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_policy_binding_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_policy_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_prompt_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_prompt_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_prompt_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_prompt_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_property_mapping_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_provider_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_proxy_outpost_config_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_proxy_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_proxy_provider_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_proxy_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_rac_property_mapping_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_rac_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_rac_provider_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_rac_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_radius_outpost_config_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_radius_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_radius_provider_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_radius_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_reputation_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_reputation_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_reputation_policy_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_reputation_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_role_assigned_object_permission_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_role_assigned_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_role_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_role_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_saml_property_mapping_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_saml_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_saml_provider_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_saml_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_saml_source_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_saml_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_scim_mapping_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_scim_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_scim_provider_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_scim_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_scope_mapping_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_scope_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_service_connection_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_sms_device_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_sms_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_source_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_source_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_source_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_static_device_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_static_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_system_task_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_system_task_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_tenant_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_tenant_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_token_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_token_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_token_model_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_token_model_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_totp_device_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_totp_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_assigned_object_permission_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_assigned_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_consent_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_consent_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_delete_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_delete_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_login_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_login_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_logout_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_logout_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_o_auth_source_connection_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_o_auth_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_saml_source_connection_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_saml_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_source_connection_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_write_stage_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_user_write_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_web_authn_device_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_web_authn_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_web_authn_device_type_list.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/paginated_web_authn_device_type_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/pagination.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/pagination.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/password_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/password_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_expiry_policy.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/password_expiry_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_expiry_policy_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/password_expiry_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_policy.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/password_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_policy_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/password_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/password_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/password_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_application_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_duo_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_authenticator_duo_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_sms_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_authenticator_sms_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_static_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_authenticator_static_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_totp_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_authenticator_totp_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_validate_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_authenticator_validate_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_web_authn_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_authenticator_web_authn_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_blueprint_instance_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_blueprint_instance_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_brand_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_brand_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_captcha_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_captcha_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_certificate_key_pair_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_certificate_key_pair_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_connection_token_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_connection_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_consent_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_consent_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_deny_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_deny_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_docker_service_connection_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_docker_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_domain_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_domain_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_dummy_policy_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_dummy_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_dummy_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_dummy_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_duo_device_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_duo_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_email_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_email_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_endpoint_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_event_matcher_policy_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_event_matcher_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_event_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_event_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_expression_policy_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_expression_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_flow_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_flow_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_flow_stage_binding_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_flow_stage_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_group_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_identification_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_identification_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_invitation_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_invitation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_invitation_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_invitation_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_kubernetes_service_connection_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_kubernetes_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_ldap_property_mapping_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_ldap_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_ldap_provider_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_ldap_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_ldap_source_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_ldap_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_license_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_license_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_notification_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_rule_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_notification_rule_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_transport_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_notification_transport_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_webhook_mapping_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_notification_webhook_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_o_auth2_provider_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_o_auth2_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_o_auth_source_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_o_auth_source_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,18 +36,18 @@
     enabled: Optional[StrictBool] = None
     authentication_flow: Optional[StrictStr] = Field(default=None, description="Flow to use when authenticating existing users.")
     enrollment_flow: Optional[StrictStr] = Field(default=None, description="Flow to use when enrolling new users.")
     policy_engine_mode: Optional[PolicyEngineMode] = None
     user_matching_mode: Optional[UserMatchingModeEnum] = Field(default=None, description="How the source determines if an existing user should be authenticated or a new user enrolled.")
     user_path_template: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
     provider_type: Optional[ProviderTypeEnum] = None
-    request_token_url: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=255)]] = Field(default=None, description="URL used to request the initial token. This URL is only required for OAuth 1.")
-    authorization_url: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=255)]] = Field(default=None, description="URL the user is redirect to to conest the flow.")
-    access_token_url: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=255)]] = Field(default=None, description="URL used by authentik to retrieve tokens.")
-    profile_url: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=255)]] = Field(default=None, description="URL used by authentik to get user information.")
+    request_token_url: Optional[Annotated[str, Field(strict=True, max_length=255)]] = Field(default=None, description="URL used to request the initial token. This URL is only required for OAuth 1.")
+    authorization_url: Optional[Annotated[str, Field(strict=True, max_length=255)]] = Field(default=None, description="URL the user is redirect to to conest the flow.")
+    access_token_url: Optional[Annotated[str, Field(strict=True, max_length=255)]] = Field(default=None, description="URL used by authentik to retrieve tokens.")
+    profile_url: Optional[Annotated[str, Field(strict=True, max_length=255)]] = Field(default=None, description="URL used by authentik to get user information.")
     consumer_key: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
     consumer_secret: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
     additional_scopes: Optional[StrictStr] = None
     oidc_well_known_url: Optional[StrictStr] = None
     oidc_jwks_url: Optional[StrictStr] = None
     oidc_jwks: Optional[Any] = None
     __properties: ClassVar[List[str]] = ["name", "slug", "enabled", "authentication_flow", "enrollment_flow", "policy_engine_mode", "user_matching_mode", "user_path_template", "provider_type", "request_token_url", "authorization_url", "access_token_url", "profile_url", "consumer_key", "consumer_secret", "additional_scopes", "oidc_well_known_url", "oidc_jwks_url", "oidc_jwks"]
```

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_outpost_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_outpost_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_password_expiry_policy_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_password_expiry_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_password_policy_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_password_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_password_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_password_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_permission_assign_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_permission_assign_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_plex_source_connection_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_plex_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_plex_source_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_plex_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_policy_binding_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_policy_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_prompt_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_prompt_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_prompt_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_prompt_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_proxy_provider_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_proxy_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_rac_property_mapping_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_rac_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_rac_provider_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_rac_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_radius_provider_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_radius_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_reputation_policy_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_reputation_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_role_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_role_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_saml_property_mapping_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_saml_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_saml_provider_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_saml_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_saml_source_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_saml_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_scim_mapping_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_scim_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_scim_provider_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_scim_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_scope_mapping_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_scope_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_settings_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_settings_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_sms_device_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_sms_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_source_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_source_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_static_device_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_static_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_tenant_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_tenant_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_token_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_totp_device_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_totp_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_delete_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_user_delete_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_login_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_user_login_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_logout_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_user_logout_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_o_auth_source_connection_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_user_o_auth_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_saml_source_connection_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_user_saml_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_write_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_user_write_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_web_authn_device_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/patched_web_authn_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/permission.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/permission_assign_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/permission_assign_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_authentication_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/plex_authentication_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_authentication_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/plex_authentication_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/plex_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source_connection.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/plex_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source_connection_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/plex_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/plex_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_token_redeem_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/plex_token_redeem_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/policy.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_binding.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/policy_binding.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_binding_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/policy_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_engine_mode.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/policy_engine_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_test_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/policy_test_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_test_result.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/policy_test_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/prompt.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/prompt_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/prompt_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/prompt_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/prompt_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/prompt_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_type_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/prompt_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/property_mapping.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/property_mapping_preview.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/property_mapping_preview.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/property_mapping_test_result.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/property_mapping_test_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/protocol_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/protocol_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/provider.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/provider_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_model_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/provider_model_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_type_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/provider_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_mode.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/proxy_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_outpost_config.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/proxy_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_provider.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/proxy_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_provider_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/proxy_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_property_mapping.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/rac_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_property_mapping_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/rac_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_provider.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/rac_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_provider_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/rac_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/radius_outpost_config.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/radius_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/radius_provider.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/radius_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/radius_provider_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/radius_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/redirect_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/redirect_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/reputation.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/reputation.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/reputation_policy.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/reputation_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/reputation_policy_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/reputation_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/resident_key_requirement_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/resident_key_requirement_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/role.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/role.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/role_assigned_object_permission.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/role_assigned_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/role_object_permission.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/role_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/role_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/role_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_metadata.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/saml_metadata.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_property_mapping.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/saml_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_property_mapping_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/saml_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_provider.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/saml_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_provider_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/saml_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_source.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/saml_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_source_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/saml_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_mapping.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/scim_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_mapping_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/scim_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_provider.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/scim_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_provider_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/scim_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_sync_status.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/scim_sync_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/scope_mapping.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/scope_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/scope_mapping_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/scope_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/selectable_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/selectable_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/service_connection.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/service_connection_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/service_connection_state.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/service_connection_state.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/session_user.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/session_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/settings.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/settings.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/settings_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/settings_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/severity_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/severity_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/shell_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/shell_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/signature_algorithm_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/signature_algorithm_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/sms_device.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/sms_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/sms_device_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/sms_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/source.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/source_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/source_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/source_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/source_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/source_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/source_type.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/source_type.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/sp_binding_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/sp_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/stage_prompt.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/stage_prompt.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/static_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/static_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device_token.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/static_device_token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device_token_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/static_device_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/sub_mode_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/sub_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/system_info.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/system_info.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/system_info_runtime.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/system_info_runtime.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/system_task.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/system_task.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/system_task_status_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/system_task_status_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/tenant.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_admin_group_request_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/tenant_admin_group_request_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_recovery_key_request_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/tenant_recovery_key_request_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_recovery_key_response.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/tenant_recovery_key_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/tenant_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/token.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/token_model.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/token_model.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/token_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/token_set_key_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/token_set_key_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/token_view.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/token_view.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/totp_device.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/totp_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/totp_device_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/totp_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/transaction_application_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/transaction_application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/transaction_application_response.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/transaction_application_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/type_create.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/type_create.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/ui_theme_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/ui_theme_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/used_by.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/used_by.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/used_by_action_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/used_by_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_account_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_account_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_assigned_object_permission.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_assigned_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_consent.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_consent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_creation_mode_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_creation_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_delete_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_delete_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_delete_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_delete_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_fields_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_fields_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_group.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_group_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_challenge.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_login_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_challenge_response_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_login_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_login_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_login_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_logout_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_logout_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_logout_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_logout_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_matching_mode_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_matching_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_metrics.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_metrics.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_o_auth_source_connection.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_o_auth_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_o_auth_source_connection_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_o_auth_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_object_permission.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_password_set_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_password_set_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_path.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_path.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_saml_source_connection.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_saml_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_saml_source_connection_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_saml_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_self.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_self.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_self_groups.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_self_groups.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_service_account_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_service_account_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_service_account_response.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_service_account_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_setting.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_setting.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_source_connection.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_type_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_verification_enum.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_verification_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_write_stage.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_write_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_write_stage_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/user_write_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/validation_error.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/version.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/version.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/web_authn_device.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/web_authn_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/web_authn_device_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/web_authn_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/web_authn_device_type.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/web_authn_device_type.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/web_authn_device_type_request.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/web_authn_device_type_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/models/workers.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/models/workers.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/authentik_client/rest.py` & `authentik_client-2024.2.2.post1712687873/authentik_client/rest.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712571742/pyproject.toml` & `authentik_client-2024.2.2.post1712687873/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "authentik_client"
-version = "2024.2.2-1712571742"
+version = "2024.2.2-1712687873"
 description = "authentik"
 authors = ["authentik Team <hello@goauthentik.io>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/goauthentik/authentik"
 keywords = ["OpenAPI", "OpenAPI-Generator", "authentik"]
 include = ["authentik_client/py.typed"]
```

### Comparing `authentik_client-2024.2.2.post1712571742/PKG-INFO` & `authentik_client-2024.2.2.post1712687873/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authentik_client
-Version: 2024.2.2.post1712571742
+Version: 2024.2.2.post1712687873
 Summary: authentik
 Home-page: https://github.com/goauthentik/authentik
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,authentik
 Author: authentik Team
 Author-email: hello@goauthentik.io
 Requires-Python: >=3.7,<4.0
@@ -25,15 +25,15 @@
 
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2024.2.2
-- Package version: 2024.2.2-1712571742
+- Package version: 2024.2.2-1712687873
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

