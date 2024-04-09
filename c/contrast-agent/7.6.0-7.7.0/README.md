# Comparing `tmp/contrast-agent-7.6.0.tar.gz` & `tmp/contrast-agent-7.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contrast-agent-7.6.0.tar", last modified: Wed Mar 20 18:34:26 2024, max compression
+gzip compressed data, was "contrast-agent-7.7.0.tar", last modified: Tue Apr  9 18:16:43 2024, max compression
```

## Comparing `contrast-agent-7.6.0.tar` & `contrast-agent-7.7.0.tar`

### file list

```diff
@@ -1,780 +1,781 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.547761 contrast-agent-7.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-03-20 18:34:26.547761 contrast-agent-7.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.455759 contrast-agent-7.6.0/hookspy/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/hookspy/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/hookspy/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.455759 contrast-agent-7.6.0/hookspy/ext/
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/hookspy/ext/hookspy.c
--rwxr-xr-x   0 runner    (1001) docker     (127)      952 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/hookspy/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.443759 contrast-agent-7.6.0/hookspy/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.455759 contrast-agent-7.6.0/hookspy/src/hookspy/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/hookspy/src/hookspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/hookspy/src/hookspy/autogen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/hookspy/src/hookspy/body.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/hookspy/src/hookspy/signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/hookspy/src/hookspy/spy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 18:34:26.547761 contrast-agent-7.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.451759 contrast-agent-7.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.455759 contrast-agent-7.6.0/src/contrast/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.459759 contrast-agent-7.6.0/src/contrast/agent/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.459759 contrast-agent-7.6.0/src/contrast/agent/agent_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/agent_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/agent_lib/input_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/agent_lib/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/agent_lib/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/agent_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.463759 contrast-agent-7.6.0/src/contrast/agent/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/adjusted_span.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/apply_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/assess_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15343 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/contrast_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.463759 contrast-agent-7.6.0/src/contrast/agent/assess/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/deadzone_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/preshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagation_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagation_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.467759 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/append_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/base_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/center_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/codecs_splat_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/format_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/join_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/json_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/keep_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/split_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/tagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/source_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/source_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/string_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.467759 contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/preflight.py
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.467759 contrast-agent-7.6.0/src/contrast/agent/assess/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/base_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.471759 contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/base_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/django_httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/django_secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/django_session_age_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/flask_httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/flask_secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/flask_session_age_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/session_age_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/dataflow_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/non_dataflow_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.471759 contrast-agent-7.6.0/src/contrast/agent/assess/rules/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/providers/enable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.471759 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/base_response_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/xss.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/static_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/trigger_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.475759 contrast-agent-7.6.0/src/contrast/agent/assess/rules/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/string_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/truncate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/assess/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/disable_reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14252 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/exclusions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/heartbeat_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.475759 contrast-agent-7.6.0/src/contrast/agent/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/app_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13877 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/base_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/environ_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.475759 contrast-agent-7.6.0/src/contrast/agent/middlewares/response_wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/response_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.475759 contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/django_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/patch_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.475759 contrast-agent-7.6.0/src/contrast/agent/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/policy/applicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/policy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/policy/patch_location_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/policy/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/policy/policy_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/policy/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/policy/rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/policy/trigger_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/policy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.479760 contrast-agent-7.6.0/src/contrast/agent/protect/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/input_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.479760 contrast-agent-7.6.0/src/contrast/agent/protect/policy/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.479760 contrast-agent-7.6.0/src/contrast/agent/protect/rule/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/base_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/bot_blocker_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/cmdi_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.479760 contrast-agent-7.6.0/src/contrast/agent/protect/rule/deserialization/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/deserialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/deserialization_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/http_method_tampering.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/malformed_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.479760 contrast-agent-7.6.0/src/contrast/agent/protect/rule/nosql_injection/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/nosql_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/nosqli_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/path_traversal_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/protection_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/rules_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/sqli_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/ssrf_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/unsafe_file_upload_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/xss_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.479760 contrast-agent-7.6.0/src/contrast/agent/protect/rule/xxe/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/xxe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/protect/rule/xxe_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/reaction_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/request_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/request_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/scope.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/server_settings_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)    27611 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/sys_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/thread_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/agent/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.479760 contrast-agent-7.6.0/src/contrast/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/aiohttp/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/aiohttp/sources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.483759 contrast-agent-7.6.0/src/contrast/api/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/api/architecture_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/api/attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/api/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/api/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/api/route_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/api/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/api/trace_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/api/type_checked_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/api/user_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.483759 contrast-agent-7.6.0/src/contrast/applies/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/applies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.483759 contrast-agent-7.6.0/src/contrast/applies/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/applies/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/applies/assess/unsafe_code_execution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.483759 contrast-agent-7.6.0/src/contrast/applies/common/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/applies/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.483759 contrast-agent-7.6.0/src/contrast/applies/protect/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/applies/protect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/applies/sqli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.483759 contrast-agent-7.6.0/src/contrast/asgi/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/asgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.483759 contrast-agent-7.6.0/src/contrast/assess_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/build_funchook.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.487760 contrast-agent-7.6.0/src/contrast/assess_extensions/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/common/cast.c
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/common/format.c
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/common/intern.c
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/common/logging.c
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/common/patches.c
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/common/propagate.c
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/common/repeat.c
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/common/repr.c
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/common/scope.c
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/common/streams.c
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/common/subscript.c
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/common/trace.c
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/cs_str.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.487760 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/.git
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/.gitmodules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.487760 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/.travis/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/.travis/Dockerfile-alpine-test
--rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/.travis/run-test.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/appveyor.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/autogen.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    44826 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/config.guess
--rwxr-xr-x   0 runner    (1001) docker     (127)    35454 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/config.sub
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/configure.ac
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.487760 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/.git
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.487760 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/include/
--rw-r--r--   0 runner    (1001) docker     (127)    19536 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h
--rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.447759 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.487760 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.491760 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/mac/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.491760 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/win32/
--rw-r--r--   0 runner    (1001) docker     (127)    12995 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.h
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.491760 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/config.h
--rw-r--r--   0 runner    (1001) docker     (127)    25059 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c
--rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c
--rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h
--rw-r--r--   0 runner    (1001) docker     (127)   209309 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h
--rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c
--rw-r--r--   0 runner    (1001) docker     (127)    45685 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h
--rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-20 18:34:14.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.491760 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/include/
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/include/funchook.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    13998 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/install-sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.495760 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/__strerror.h
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook.c
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook_io.c
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook_io.h
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S
--rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c
--rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c
--rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/os_func.c
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/os_func.h
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c
--rw-r--r--   0 runner    (1001) docker     (127)    43872 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/printf_base.c
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/printf_base.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.495760 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/test/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/test/libfunchook_test.c
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/test/libfunchook_test2.c
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/test/suffix.list
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/test/test_main.c
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/test/x86_64_test.S
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/test/x86_test.S
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.499760 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/funchook.sln
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-20 18:34:13.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/funchook_test_exe.def
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.447759 contrast-agent-7.6.0/src/contrast/assess_extensions/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.447759 contrast-agent-7.6.0/src/contrast/assess_extensions/include/contrast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.499760 contrast-agent-7.6.0/src/contrast/assess_extensions/include/contrast/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/include/contrast/assess/intern.h
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/include/contrast/assess/logging.h
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/include/contrast/assess/patches.h
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/include/contrast/assess/scope.h
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/include/contrast/assess/trace.h
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/include/contrast/assess/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.499760 contrast-agent-7.6.0/src/contrast/assess_extensions/py3/
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py3/patches.c
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py3/str_concat.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.499760 contrast-agent-7.6.0/src/contrast/assess_extensions/py310/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py310/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py310/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py310/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py310/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py310/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py310/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.499760 contrast-agent-7.6.0/src/contrast/assess_extensions/py311/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py311/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py311/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py311/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py311/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py311/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py311/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.499760 contrast-agent-7.6.0/src/contrast/assess_extensions/py312/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py312/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py312/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py312/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py312/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py312/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py312/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.503760 contrast-agent-7.6.0/src/contrast/assess_extensions/py35/
--rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py35/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py35/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py35/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py35/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py35/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py35/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.503760 contrast-agent-7.6.0/src/contrast/assess_extensions/py36/
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py36/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py36/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py36/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py36/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py36/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py36/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.503760 contrast-agent-7.6.0/src/contrast/assess_extensions/py37/
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py37/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py37/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py37/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py37/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py37/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py37/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.503760 contrast-agent-7.6.0/src/contrast/assess_extensions/py38/
--rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py38/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py38/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py38/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py38/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py38/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py38/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.503760 contrast-agent-7.6.0/src/contrast/assess_extensions/py39/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py39/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py39/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py39/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py39/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py39/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/assess_extensions/py39/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.507760 contrast-agent-7.6.0/src/contrast/bottle/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/bottle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/bottle/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.507760 contrast-agent-7.6.0/src/contrast/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/configuration/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/configuration/agent_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/configuration/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/configuration/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/configuration/assess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/configuration/config_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/configuration/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/configuration/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/configuration/protect.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/configuration/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/configuration/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.507760 contrast-agent-7.6.0/src/contrast/django/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/django/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.507760 contrast-agent-7.6.0/src/contrast/django_asgi/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/django_asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/django_asgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.507760 contrast-agent-7.6.0/src/contrast/falcon/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/falcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/falcon/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.507760 contrast-agent-7.6.0/src/contrast/falcon_asgi/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/falcon_asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/falcon_asgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.507760 contrast-agent-7.6.0/src/contrast/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/fastapi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.507760 contrast-agent-7.6.0/src/contrast/flask/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/flask/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.507760 contrast-agent-7.6.0/src/contrast/loader/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/loader/sitecustomize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.511760 contrast-agent-7.6.0/src/contrast/patches/
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/cgi_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/concurrent_futures_thread_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/cs_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/cs_str.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.511760 contrast-agent-7.6.0/src/contrast/patches/databases/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/databases/dbapi2.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/databases/mysql_connector_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/databases/psycopg2_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/databases/pymysql_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/databases/sqlalchemy_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/databases/sqlite3_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/encodings_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/exec_and_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.511760 contrast-agent-7.6.0/src/contrast/patches/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/frameworks/bottle_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/frameworks/django_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/frameworks/drf_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/frameworks/falcon_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/frameworks/flask_and_quart_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/frameworks/pyramid_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/frameworks/starlette_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/genshi_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/import_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/lxml_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.515760 contrast-agent-7.6.0/src/contrast/patches/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/middleware/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/middleware/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/middleware/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/middleware/mod_wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/pathlib_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11140 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/re_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/str_new.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/sys_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/threading_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/urllib_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/patches/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.515760 contrast-agent-7.6.0/src/contrast/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/deadzones.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.515760 contrast-agent-7.6.0/src/contrast/policy/propagators/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/propagators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/propagators/codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/propagators/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/propagators/frameworks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/propagators/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/propagators/re.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/propagators/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/propagators/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.515760 contrast-agent-7.6.0/src/contrast/policy/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/sources/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/sources/cgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/sources/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/sources/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/sources/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/sources/quart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/sources/webob.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.519760 contrast-agent-7.6.0/src/contrast/policy/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/cmd_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/httponly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/nosql_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/path_traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/prompt_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/redos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/reflected_xss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/secure_flag_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/session_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/session_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/sql_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/ssrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/trust_boundary_violation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/unsafe_code_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/untrusted_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/unvalidated_redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/xpath_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/policy/triggers/xxe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.519760 contrast-agent-7.6.0/src/contrast/pyramid/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/pyramid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/pyramid/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.519760 contrast-agent-7.6.0/src/contrast/quart/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/quart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/quart/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.519760 contrast-agent-7.6.0/src/contrast/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/activity_masker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/reporting_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/request_audit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.523760 contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/_traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/application_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/application_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/application_startup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/application_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/base_ts_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/effective_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/library_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/observed_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/preflight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/server_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/server_startup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.523760 contrast-agent-7.6.0/src/contrast/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/scripts/fix_interpreter_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/scripts/propagator_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/scripts/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/scripts/validate_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.527760 contrast-agent-7.6.0/src/contrast/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.527760 contrast-agent-7.6.0/src/contrast/utils/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/assess/duck_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.527760 contrast-agent-7.6.0/src/contrast/utils/assess/formatting/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/assess/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/assess/formatting/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/assess/formatting/tokenize_cformat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/assess/formatting/tokenize_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/assess/stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/assess/tag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/assess/tracking_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/base64_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/configuration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/context_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/deprecated_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/digest_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/environ.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.527760 contrast-agent-7.6.0/src/contrast/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/exceptions/deprecation_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/exceptions/wsgi_compliance_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/ignored_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.527760 contrast-agent-7.6.0/src/contrast/utils/library_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/library_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/library_reader/library_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7655 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/library_reader/patched_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/library_reader/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/locale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.527760 contrast-agent-7.6.0/src/contrast/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/loggers/structlog.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/module_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/patch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/pattern_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/safe_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/stack_trace_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/stdlib_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-20 18:34:26.000000 contrast-agent-7.6.0/src/contrast/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.527760 contrast-agent-7.6.0/src/contrast/wsgi/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/wsgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast/wsgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.547761 contrast-agent-7.6.0/src/contrast_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    31815 2024-03-20 18:34:26.000000 contrast-agent-7.6.0/src/contrast_agent.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.527760 contrast-agent-7.6.0/src/contrast_rewriter/
--rw-r--r--   0 runner    (1001) docker     (127)    15302 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_rewriter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.527760 contrast-agent-7.6.0/src/contrast_vendor/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.531760 contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    34150 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/diagnose.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.531760 contrast-agent-7.6.0/src/contrast_vendor/isort/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/isort/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/isort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.531760 contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/all.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py27.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py311.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py312.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py36.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py37.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py39.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.531760 contrast-agent-7.6.0/src/contrast_vendor/ported_cpython_code/
--rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ported_cpython_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ported_cpython_code/import_functionality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.455759 contrast-agent-7.6.0/src/contrast_vendor/ruamel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.539760 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/anchor.py
--rw-r--r--   0 runner    (1001) docker     (127)    37673 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/composer.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/configobjwalker.py
--rw-r--r--   0 runner    (1001) docker     (127)    70392 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/cyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)    67960 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    59457 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    36019 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/representer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/scalarbool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/scalarint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/scalarstring.py
--rw-r--r--   0 runner    (1001) docker     (127)    87945 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.543760 contrast-agent-7.6.0/src/contrast_vendor/structlog/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/_greenlets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/_log_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/_native.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (127)    23428 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    37555 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/threadlocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/tracebacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/twisted.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/structlog/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/vendor-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.547761 contrast-agent-7.6.0/src/contrast_vendor/webob/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   210210 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/acceptparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/byterange.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/cachecontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    32879 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/dec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/etag.py
--rw-r--r--   0 runner    (1001) docker     (127)    38268 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/exc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/license.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/multidict.py
--rw-r--r--   0 runner    (1001) docker     (127)    59141 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    55423 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/static.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/webob/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.547761 contrast-agent-7.6.0/src/contrast_vendor/wrapt/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/wrapt/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/wrapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/wrapt/__wrapt__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/wrapt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/wrapt/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/wrapt/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/wrapt/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/wrapt/weakrefs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27137 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/wrapt/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.547761 contrast-agent-7.6.0/src/contrast_vendor/zipp/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/zipp/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/zipp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:26.547761 contrast-agent-7.6.0/src/contrast_vendor/zipp/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/zipp/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/zipp/compat/py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-03-20 18:34:11.000000 contrast-agent-7.6.0/src/contrast_vendor/zipp/glob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.821122 contrast-agent-7.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-09 18:16:43.821122 contrast-agent-7.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.665119 contrast-agent-7.7.0/hookspy/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.665119 contrast-agent-7.7.0/hookspy/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/ext/hookspy.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)      952 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.649119 contrast-agent-7.7.0/hookspy/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.665119 contrast-agent-7.7.0/hookspy/src/hookspy/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/src/hookspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/src/hookspy/autogen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/src/hookspy/body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/src/hookspy/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/src/hookspy/spy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:16:43.821122 contrast-agent-7.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.661119 contrast-agent-7.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.665119 contrast-agent-7.7.0/src/contrast/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.669119 contrast-agent-7.7.0/src/contrast/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.669119 contrast-agent-7.7.0/src/contrast/agent/agent_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/agent_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/agent_lib/input_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/agent_lib/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/agent_lib/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/agent_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.673119 contrast-agent-7.7.0/src/contrast/agent/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/adjusted_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/apply_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/assess_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15343 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/contrast_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.677119 contrast-agent-7.7.0/src/contrast/agent/assess/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/deadzone_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/preshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagation_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagation_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.689119 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/append_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/base_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/center_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/codecs_splat_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/format_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/join_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/json_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/keep_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/split_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/tagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/source_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/source_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/string_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.693120 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.697120 contrast-agent-7.7.0/src/contrast/agent/assess/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/base_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.705120 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/base_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/django_httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/django_secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/django_session_age_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/flask_httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/flask_secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/flask_session_age_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/session_age_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/dataflow_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/non_dataflow_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.705120 contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.713120 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/base_response_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/xss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/static_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/trigger_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.717120 contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/string_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/disable_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14252 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/heartbeat_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.721120 contrast-agent-7.7.0/src/contrast/agent/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/app_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14335 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/base_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/environ_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.721120 contrast-agent-7.7.0/src/contrast/agent/middlewares/response_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/response_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.725120 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/django_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/patch_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.725120 contrast-agent-7.7.0/src/contrast/agent/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/applicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/patch_location_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/policy_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/trigger_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.725120 contrast-agent-7.7.0/src/contrast/agent/protect/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/input_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.725120 contrast-agent-7.7.0/src/contrast/agent/protect/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.729120 contrast-agent-7.7.0/src/contrast/agent/protect/rule/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/base_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/bot_blocker_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/cmdi_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.729120 contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/http_method_tampering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/malformed_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.729120 contrast-agent-7.7.0/src/contrast/agent/protect/rule/nosql_injection/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/nosql_injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/nosqli_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/path_traversal_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/protection_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/rules_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/sqli_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/ssrf_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/unsafe_file_upload_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/xss_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.729120 contrast-agent-7.7.0/src/contrast/agent/protect/rule/xxe/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/xxe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/xxe_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/reaction_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/request_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/request_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/server_settings_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27611 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/sys_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/thread_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.729120 contrast-agent-7.7.0/src/contrast/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/aiohttp/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/aiohttp/sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.733120 contrast-agent-7.7.0/src/contrast/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/architecture_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/route_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/trace_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/type_checked_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/user_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.733120 contrast-agent-7.7.0/src/contrast/applies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/applies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.733120 contrast-agent-7.7.0/src/contrast/applies/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/applies/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/applies/assess/unsafe_code_execution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.733120 contrast-agent-7.7.0/src/contrast/applies/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/applies/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.733120 contrast-agent-7.7.0/src/contrast/applies/protect/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/applies/protect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/applies/sqli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.733120 contrast-agent-7.7.0/src/contrast/asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/asgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.733120 contrast-agent-7.7.0/src/contrast/assess_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/build_funchook.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.737120 contrast-agent-7.7.0/src/contrast/assess_extensions/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/cast.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/format.c
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/intern.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/logging.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/patches.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/propagate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/repeat.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/repr.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/scope.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/streams.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/subscript.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/trace.c
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/cs_str.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.741120 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.git
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.gitmodules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.741120 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.travis/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.travis/Dockerfile-alpine-test
+-rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.travis/run-test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/appveyor.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/autogen.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44826 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/config.guess
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35454 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/config.sub
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/configure.ac
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.741120 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/.git
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.741120 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    19536 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.653119 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.741120 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.741120 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/mac/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.741120 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)    12995 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.749121 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25059 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c
+-rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h
+-rw-r--r--   0 runner    (1001) docker     (127)   209309 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c
+-rw-r--r--   0 runner    (1001) docker     (127)    45685 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.749121 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/include/funchook.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13998 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/install-sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.749121 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/__strerror.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_io.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_io.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S
+-rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c
+-rw-r--r--   0 runner    (1001) docker     (127)    43872 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/printf_base.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/printf_base.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.753121 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/libfunchook_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/libfunchook_test2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/suffix.list
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/test_main.c
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/x86_64_test.S
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/x86_test.S
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.753121 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook.sln
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test_exe.def
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.657119 contrast-agent-7.7.0/src/contrast/assess_extensions/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.657119 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.753121 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/intern.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/logging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/patches.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/scope.h
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/trace.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.757121 contrast-agent-7.7.0/src/contrast/assess_extensions/py3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py3/patches.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py3/str_concat.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.757121 contrast-agent-7.7.0/src/contrast/assess_extensions/py310/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py310/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py310/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py310/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py310/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py310/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py310/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.757121 contrast-agent-7.7.0/src/contrast/assess_extensions/py311/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py311/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py311/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py311/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py311/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py311/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py311/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.757121 contrast-agent-7.7.0/src/contrast/assess_extensions/py312/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py312/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py312/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py312/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py312/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py312/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py312/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.761121 contrast-agent-7.7.0/src/contrast/assess_extensions/py35/
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py35/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py35/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py35/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py35/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py35/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py35/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.761121 contrast-agent-7.7.0/src/contrast/assess_extensions/py36/
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py36/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py36/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py36/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py36/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py36/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py36/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.761121 contrast-agent-7.7.0/src/contrast/assess_extensions/py37/
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py37/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py37/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py37/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py37/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py37/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py37/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.761121 contrast-agent-7.7.0/src/contrast/assess_extensions/py38/
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py38/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py38/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py38/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py38/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py38/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py38/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.765121 contrast-agent-7.7.0/src/contrast/assess_extensions/py39/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py39/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py39/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py39/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py39/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py39/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py39/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.765121 contrast-agent-7.7.0/src/contrast/bottle/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/bottle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/bottle/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.765121 contrast-agent-7.7.0/src/contrast/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/agent_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/assess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/protect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.769121 contrast-agent-7.7.0/src/contrast/django/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/django/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.769121 contrast-agent-7.7.0/src/contrast/django_asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/django_asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/django_asgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.769121 contrast-agent-7.7.0/src/contrast/falcon/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/falcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/falcon/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.769121 contrast-agent-7.7.0/src/contrast/falcon_asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/falcon_asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/falcon_asgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.769121 contrast-agent-7.7.0/src/contrast/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/fastapi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.769121 contrast-agent-7.7.0/src/contrast/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/flask/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.769121 contrast-agent-7.7.0/src/contrast/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/loader/sitecustomize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.773121 contrast-agent-7.7.0/src/contrast/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/cgi_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/concurrent_futures_thread_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/cs_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/cs_str.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.773121 contrast-agent-7.7.0/src/contrast/patches/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/databases/dbapi2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/databases/mysql_connector_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/databases/psycopg2_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/databases/pymysql_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/databases/sqlalchemy_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/databases/sqlite3_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/encodings_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/exec_and_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.777121 contrast-agent-7.7.0/src/contrast/patches/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/bottle_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/django_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/drf_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/falcon_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/flask_and_quart_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/pyramid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/starlette_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/genshi_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/import_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/lxml_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.777121 contrast-agent-7.7.0/src/contrast/patches/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/middleware/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/middleware/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/middleware/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/middleware/mod_wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/pathlib_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/re_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/str_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/sys_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/threading_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/urllib_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.777121 contrast-agent-7.7.0/src/contrast/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/deadzones.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.777121 contrast-agent-7.7.0/src/contrast/policy/propagators/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/frameworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.781121 contrast-agent-7.7.0/src/contrast/policy/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/cgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/quart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/webob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.785121 contrast-agent-7.7.0/src/contrast/policy/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/cmd_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/httponly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/nosql_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/path_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/prompt_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/redos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/reflected_xss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/secure_flag_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/session_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/session_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/sql_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/ssrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/trust_boundary_violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/unsafe_code_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/untrusted_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/unvalidated_redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/xpath_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/xxe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.785121 contrast-agent-7.7.0/src/contrast/pyramid/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/pyramid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/pyramid/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.785121 contrast-agent-7.7.0/src/contrast/quart/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/quart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/quart/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.785121 contrast-agent-7.7.0/src/contrast/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/activity_masker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/reporting_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/request_audit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.789121 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/application_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/application_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/application_startup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/application_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/base_ts_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/effective_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/library_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/observed_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/server_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/server_startup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.789121 contrast-agent-7.7.0/src/contrast/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/scripts/fix_interpreter_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/scripts/propagator_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/scripts/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/scripts/validate_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.793121 contrast-agent-7.7.0/src/contrast/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.793121 contrast-agent-7.7.0/src/contrast/utils/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/duck_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.793121 contrast-agent-7.7.0/src/contrast/utils/assess/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/formatting/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/formatting/tokenize_cformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/formatting/tokenize_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/tag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/tracking_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/base64_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/configuration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/context_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/deprecated_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/digest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/environ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.793121 contrast-agent-7.7.0/src/contrast/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/exceptions/deprecation_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/exceptions/wsgi_compliance_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/ignored_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.797121 contrast-agent-7.7.0/src/contrast/utils/library_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/library_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/library_reader/library_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/library_reader/patched_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/library_reader/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/locale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.797121 contrast-agent-7.7.0/src/contrast/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/loggers/structlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/module_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/patch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/pattern_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/safe_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/stack_trace_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/stdlib_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 18:16:43.000000 contrast-agent-7.7.0/src/contrast/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.797121 contrast-agent-7.7.0/src/contrast/wsgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/wsgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/wsgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.821122 contrast-agent-7.7.0/src/contrast_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    31844 2024-04-09 18:16:43.000000 contrast-agent-7.7.0/src/contrast_agent.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.797121 contrast-agent-7.7.0/src/contrast_rewriter/
+-rw-r--r--   0 runner    (1001) docker     (127)    15359 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_rewriter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.797121 contrast-agent-7.7.0/src/contrast_vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.801121 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    34323 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.801121 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/compat/py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/diagnose.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.801121 contrast-agent-7.7.0/src/contrast_vendor/isort/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.801121 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py27.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py311.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py36.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py39.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.805121 contrast-agent-7.7.0/src/contrast_vendor/ported_cpython_code/
+-rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ported_cpython_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ported_cpython_code/import_functionality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.661119 contrast-agent-7.7.0/src/contrast_vendor/ruamel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.809121 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37673 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/configobjwalker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70392 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/cyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67960 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59457 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36019 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/representer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarbool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87945 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.813121 contrast-agent-7.7.0/src/contrast_vendor/structlog/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_greenlets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23428 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    37555 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/threadlocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/tracebacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/twisted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/vendor-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.817122 contrast-agent-7.7.0/src/contrast_vendor/webob/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   210210 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/acceptparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/byterange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/cachecontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32879 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/etag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38268 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/multidict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59159 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55423 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.821122 contrast-agent-7.7.0/src/contrast_vendor/wrapt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/__wrapt__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/weakrefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27137 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.821122 contrast-agent-7.7.0/src/contrast_vendor/zipp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/zipp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/zipp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.821122 contrast-agent-7.7.0/src/contrast_vendor/zipp/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/zipp/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/zipp/compat/py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/zipp/glob.py
```

### Comparing `contrast-agent-7.6.0/LICENSE.txt` & `contrast-agent-7.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/MANIFEST.in` & `contrast-agent-7.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/PKG-INFO` & `contrast-agent-7.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contrast-agent
-Version: 7.6.0
+Version: 7.7.0
 Summary: Contrast Security's agent for Python web frameworks
 Author-email: "Contrast Security, Inc." <python@contrastsecurity.com>
 License: Copyright: 2024 Contrast Security, Inc
         Contact: support@contrastsecurity.com
         License: Commercial
         
         NOTICE: This Software and the patented inventions embodied within may only be used as
```

### Comparing `contrast-agent-7.6.0/hookspy/README.md` & `contrast-agent-7.7.0/hookspy/README.md`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/hookspy/ext/hookspy.c` & `contrast-agent-7.7.0/hookspy/ext/hookspy.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/hookspy/setup.py` & `contrast-agent-7.7.0/hookspy/setup.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/hookspy/src/hookspy/autogen.py` & `contrast-agent-7.7.0/hookspy/src/hookspy/autogen.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/hookspy/src/hookspy/body.py` & `contrast-agent-7.7.0/hookspy/src/hookspy/body.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/hookspy/src/hookspy/signatures.py` & `contrast-agent-7.7.0/hookspy/src/hookspy/signatures.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/hookspy/src/hookspy/spy.py` & `contrast-agent-7.7.0/hookspy/src/hookspy/spy.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/pyproject.toml` & `contrast-agent-7.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/setup.py` & `contrast-agent-7.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/__init__.py` & `contrast-agent-7.7.0/src/contrast/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/agent_lib/__init__.py` & `contrast-agent-7.7.0/src/contrast/agent/agent_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/agent_lib/input_tracing.py` & `contrast-agent-7.7.0/src/contrast/agent/agent_lib/input_tracing.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/agent_lib/main.py` & `contrast-agent-7.7.0/src/contrast/agent/agent_lib/main.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/agent_state.py` & `contrast-agent-7.7.0/src/contrast/agent/agent_state.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/asgi.py` & `contrast-agent-7.7.0/src/contrast/agent/asgi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 from io import BytesIO
 
-from contrast.agent import scope as scope_
-from contrast.agent.assess.policy.analysis import skip_analysis
+from contrast.agent import agent_state
 from contrast.agent.assess.policy.source_policy import (
     cs__apply_source,
     build_source_node,
 )
 from contrast.utils.decorators import cached_property, fail_quietly
 from contrast_vendor.webob.headers import ResponseHeaders
 
@@ -259,29 +258,28 @@
     and clear all of the places where starlette might save these variables. This could
     be avoided by going for an approach that's closer to pure ASGI instead of relying as
     much on starlette.
 
     @param context: the current request context
     @param scope: the ASGI scope dict
     """
-    if skip_analysis(context):
+    if (settings := agent_state.get_settings()) and not settings.is_assess_enabled():
         return
 
-    with scope_.contrast_scope():
-        for key, value in scope.items():
-            if key in ["client", "server"]:
-                for elem in value or []:
-                    _track_scope_item(context, scope, key, elem)
-            elif key == "headers":
-                for header_key, header_value in value or []:
-                    key = "cookie" if header_key == b"cookie" else "headers"
-                    _track_scope_item(context, scope, key, header_key)
-                    _track_scope_item(context, scope, key, header_value)
-            else:
-                _track_scope_item(context, scope, key, value)
+    for key, value in scope.items():
+        if key in ["client", "server"]:
+            for elem in value or []:
+                _track_scope_item(context, scope, key, elem)
+        elif key == "headers":
+            for header_key, header_value in value or []:
+                key = "cookie" if header_key == b"cookie" else "headers"
+                _track_scope_item(context, scope, key, header_key)
+                _track_scope_item(context, scope, key, header_value)
+        else:
+            _track_scope_item(context, scope, key, value)
 
 
 def _track_scope_item(context, scope, key, value):
     # there are other elements in `scope`, but only those in SCOPE_SOURCES matter to us
     if key in SCOPE_SOURCES:
         node = build_source_node(SOURCE_DICT, key, SCOPE_SOURCES[key])
         cs__apply_source(context, node, value, scope, value, (), {}, source_name=key)
```

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/adjusted_span.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/adjusted_span.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/apply_trigger.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/apply_trigger.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/contrast_event.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/contrast_event.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/analysis.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/analysis.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/deadzone_node.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/deadzone_node.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/patches.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/patches.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/preshift.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/preshift.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagation_node.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagation_node.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagation_policy.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagation_policy.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/__init__.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/append_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/append_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/base_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/base_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/format_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/format_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/join_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/join_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/json_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/json_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/split_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/split_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/source_node.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/source_node.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/source_policy.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/source_policy.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/string_propagation.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/string_propagation.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Custom trigger action that implements ReDos rule logic.
 
     A ReDOS vulnerability is triggered when the user input is untrusted (as
     with other rules) but unlike other rules, when the regex passed in to the re
     method matches a specific pattern. This rule deviates from other Assess rules in
     that the value provided may change the outcome of the vulnerability detection.
 
-    https://bitbucket.org/contrastsecurity/assess-specifications/src/master/rules/dataflow/redos.md
+    https://github.com/Contrast-Security-Inc/assess-specifications/blob/master/rules/dataflow/redos.md
     """
 
     def is_violated(
         self, source_properties, required_tags, disallowed_tags, orig_args=None
     ):
         # 1) Check that user input is untrusted.
         violated = super().is_violated(
```

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class SsrfAction(DefaultAction):
     """
     Custom trigger action that implements SSRF rule logic.
 
     For SSRF, only tag ranges within specific regions of the URL are considered
     to be vulnerable. For a more detailed description, see the dataflow rule
-    for SSRF in https://bitbucket.org/contrastsecurity/assess-specifications.
+    for SSRF in https://github.com/Contrast-Security-Inc/assess-specifications.
     """
 
     # Used to parse URLs into components for SSRF post-trigger analysis.
     # This follows the specification, linked above.
     SSRF_REGEX = (
         r"(?P<protocol>http|https|ftp|sftp|telnet|gopher|rtsp|rtsps|ssh|svn):\/\/"
         r"(?P<host>[^\/?]+)(?P<path>\/?[^?]*)(?P<querystring>\?.*)?"
```

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/policy/trigger_policy.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_policy.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/preflight.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/preflight.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/properties.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/properties.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/base_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/base_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/base_config_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/base_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/config/session_age_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/session_age_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/dataflow_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/dataflow_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/non_dataflow_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/non_dataflow_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/providers/enable.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/enable.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/analyze.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/analyze.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/base_response_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/base_response_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/response/xss.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/xss.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/static_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/static_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/trigger_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/trigger_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/sampling.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/sampling.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/string_tracker.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/string_tracker.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/tag.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/tag.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/truncate.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/truncate.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/assess/utils.py` & `contrast-agent-7.7.0/src/contrast/agent/assess/utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/disable_reaction.py` & `contrast-agent-7.7.0/src/contrast/agent/disable_reaction.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/events.py` & `contrast-agent-7.7.0/src/contrast/agent/events.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/exceptions.py` & `contrast-agent-7.7.0/src/contrast/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/exclusions.py` & `contrast-agent-7.7.0/src/contrast/agent/exclusions.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/framework.py` & `contrast-agent-7.7.0/src/contrast/agent/framework.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/heartbeat_thread.py` & `contrast-agent-7.7.0/src/contrast/agent/heartbeat_thread.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/metrics.py` & `contrast-agent-7.7.0/src/contrast/agent/metrics.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/middlewares/app_finder.py` & `contrast-agent-7.7.0/src/contrast/agent/middlewares/app_finder.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/middlewares/base_middleware.py` & `contrast-agent-7.7.0/src/contrast/agent/middlewares/base_middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,42 +12,65 @@
 )
 from contrast.agent.protect import input_analysis
 from contrast.agent.request_context import RequestContext
 from contrast.agent.assess.rules.response.xss import analyze_xss
 from contrast.agent.assess.rules.response.analyze import analyze_response_rules
 from contrast.agent.assess.preflight import update_preflight_hashes
 from contrast.agent.middlewares.route_coverage.routes_mixin import RoutesMixin
+from contrast.agent.middlewares.response_wrappers.base_response_wrapper import (
+    BaseResponseWrapper,
+)
 from contrast.api.attack import ProtectResponse
 from contrast.utils.decorators import cached_property
 from contrast.utils.loggers.logger import (
     setup_basic_agent_logger,
 )
 from contrast.reporting import get_reporting_client
 from contrast.utils.decorators import fail_loudly, fail_quietly
 from contrast.utils import timer
 
 # initialize a basic logger until config is parsed
 logger = setup_basic_agent_logger()
 
 
 @contextlib.contextmanager
-def log_request_start_and_end(request_path):
+def log_request_start_and_end(request_method, request_path):
     start_time = timer.now_ms()
-    logger.debug("Beginning request analysis", request_path=request_path)
+    logger.debug(
+        "Beginning request analysis",
+        request_method=request_method,
+        request_path=request_path,
+    )
     try:
         yield
     finally:
-        logger.debug("Ending request analysis", request_path=request_path)
+        logger.debug(
+            "Ending request analysis",
+            request_method=request_method,
+            request_path=request_path,
+        )
         logger.debug(
             "elapsed time request analysis ms",
             elapsed_time=timer.now_ms() - start_time,
+            request_method=request_method,
             request_path=request_path,
         )
 
 
+def _log_response_info(response: BaseResponseWrapper):
+    if response is None:
+        logger.debug("No response info for this request")
+        return
+    logger.debug(
+        "Response summary",
+        status_code=response.status_code,
+        content_length=response.headers.get("content-length", ""),
+    )
+
+
 class BaseMiddleware(RoutesMixin):
     """
     BaseMiddleware contains all the initial setup for the framework middlewares
 
     Requirements:
 
         1. It's callable
@@ -168,28 +191,29 @@
         """
         Method that should run for all middlewares AFTER every request is made.
         """
         if context is None:
             logger.error("Context not defined in middleware ensure")
             return
 
-        with scope.contrast_scope():
-            thread_watcher.ensure_running(self)
+        thread_watcher.ensure_running(self)
+
+        if self.settings.is_assess_enabled():
+            # route discovery and storage needs to occur before sending messages
+            self.handle_routes(context, request)
 
-            if self.settings.is_assess_enabled():
-                # route discovery and storage needs to occur before sending messages
-                self.handle_routes(context, request)
+            logger.debug("Updating preflight hashes with route info")
+            update_preflight_hashes(context)
 
-                logger.debug("Updating preflight hashes with route info")
-                update_preflight_hashes(context)
+        logger.debug("Sending final messages for reporting.")
 
-            logger.debug("Sending final messages for reporting.")
+        for msg in self.final_ts_messages(context):
+            self.reporting_client.add_message(msg)
 
-            for msg in self.final_ts_messages(context):
-                self.reporting_client.add_message(msg)
+        _log_response_info(context.response)
 
         agent_state.set_first_request(False)
 
     def final_ts_messages(self, context):
         if context is None:
             return []
 
@@ -230,19 +254,16 @@
         return messages
 
     @fail_loudly("Failed to run prefilter.")
     def prefilter(self):
         """
         Run all of our prefilter, those that happen before handing execution to the application code, here.
         """
-
-        # We check for protect here to avoid the unnecessary scope call for those processes where protect is disabled.
         if self.settings.is_protect_enabled():
-            with scope.contrast_scope():
-                self.prefilter_protect()
+            self.prefilter_protect()
 
     @fail_quietly("Failed to run prefilter protect.")
     def prefilter_protect(self):
         """
         Prefilter - AKA input analysis - is performed mostly with agent-lib but partly in the agent.
 
         In this method we call on agent-lib to do input analysis, which can result in:
@@ -263,20 +284,18 @@
 
     @fail_loudly("Unable to do postfilter")
     def postfilter(self, context):
         """
         For all postfilter enabled rules.
         """
         if self.settings.is_protect_enabled():
-            with scope.contrast_scope():
-                self.postfilter_protect(context)
+            self.postfilter_protect(context)
 
         if self.settings.is_assess_enabled():
-            with scope.contrast_scope():
-                self.response_analysis(context)
+            self.response_analysis(context)
 
     def _process_trigger_handler(self, handler):
         """
         Gather metadata about response handler callback for xss trigger node
 
         We need to check whether the response handler callback is an instance method or
         not. This affects the way that our policy machinery works, and it also affects
@@ -329,14 +348,17 @@
 
     @fail_quietly("Failed to run postfilter protect.")
     def postfilter_protect(self, context):
         logger.debug("PROTECT: Running Agent postfilter.")
 
         input_analysis.get_input_analysis(prefer_worth_watching=False)
 
+        # TODO: PYT-3255 this second call to get_input_analysis discards previous data
+        # about attack_count
+
         for rule in self.settings.protect_rules.values():
             if rule.is_postfilter():
                 rule.postfilter()
 
     @fail_loudly("Unable to do check_for_blocked")
     def check_for_blocked(self, context: RequestContext):
         """
```

### Comparing `contrast-agent-7.6.0/src/contrast/agent/middlewares/environ_tracker.py` & `contrast-agent-7.7.0/src/contrast/agent/middlewares/environ_tracker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
-from contrast.agent import scope
-from contrast.agent.assess.policy.analysis import skip_analysis
+from contrast.agent import agent_state
 from contrast.agent.assess.policy.source_node import SourceNode
 from contrast.agent.assess.policy.source_policy import cs__apply_source
 from contrast.utils.assess.stream_utils import ContrastWsgiStreamProxy
 from contrast.utils.decorators import fail_loudly
 
 # a best effort at translating the types in this document:
-# https://bitbucket.org/contrastsecurity/teamserver/src/
-# 862d499227e8eac42b6eb7c6b03f10b7f1556218/teamserver-agent-messages/src/main/java/
-# contrast/agent/messages/finding/trace/EventSourceTypeDTM.java#lines-8
+# https://github.com/Contrast-Security-Inc/teamserver/blob/341fc7545a1bc85b2f42157227b281b2c11b2050/teamserver-app/src/main/java/contrast/agent/messages/finding/trace/EventSourceTypeDTM.java#L27
 ENVIRON_SOURCES = {
     "CONTENT_LENGTH": "HEADER",
     "CONTENT_TYPE": "HEADER",
     "PATH_INFO": "URI",
     "QUERY_STRING": "QUERYSTRING",
     "REMOTE_ADDR": "URI",
     "REMOTE_HOST": "URI",
@@ -36,49 +33,36 @@
     "webob._parsed_post_vars",
     "webob._body_file",
     "webob._parsed_cookies",
     "webob._cache_control",
 }
 
 
-@fail_loudly("failed to track cookie sources")
-def track_cookie_sources(framework, context, cookies):
-    """track cookie keys and values"""
-    if skip_analysis(context):
-        return
-
-    with scope.contrast_scope():
-        _track_keys_and_values(
-            framework, context, cookies, "COOKIE_KEY", "COOKIE", no_cross_site=True
-        )
-
-
 @fail_loudly("Failed to track environ sources")
 def track_environ_sources(framework, context, environ):
     """
     This method will track necessary information in the environ
 
     For wsgi frameworks, this is the one true source of (stateless) untrusted data
 
     :param framework: current application's framework
     :param context: current request context
     :param environ: WSGI environ dict
 
     :return: None
     """
-    if skip_analysis(context):
+    if (settings := agent_state.get_settings()) and not settings.is_assess_enabled():
         return
 
-    with scope.contrast_scope():
-        for key, value in environ.items():
-            _track_environ_item(framework, context, environ, key, value)
-
-        _make_request_body_seekable(context.request)
-        _track_wsgi_input(environ)
-        _remove_webob_environ_vars(environ)
+    for key, value in environ.items():
+        _track_environ_item(framework, context, environ, key, value)
+
+    _make_request_body_seekable(context.request)
+    _track_wsgi_input(environ)
+    _remove_webob_environ_vars(environ)
 
 
 def _build_source_node(framework, method_name, source_type, no_cross_site=False):
     """
     Builds a new SourceNode based on the method name and source type
 
     Since cookie sources are not tagged with CROSS_SITE, callers must indicate whether
@@ -102,31 +86,14 @@
         **source_dict,
     )
     node.skip_stacktrace = True
 
     return node
 
 
-def _track_keys_and_values(
-    framework, context, mapping, key_type, value_type, no_cross_site=False
-):
-    for key, value in mapping.items():
-        if key:
-            key_node = _build_source_node(framework, key, key_type, no_cross_site)
-            cs__apply_source(
-                context, key_node, key, mapping, key, (), {}, source_name=key
-            )
-
-        if value:
-            value_node = _build_source_node(framework, value, value_type, no_cross_site)
-            cs__apply_source(
-                context, value_node, value, mapping, value, (), {}, source_name=key
-            )
-
-
 def _track_environ_item(framework, context, environ, key, value):
     source_type = ""
     if key in ENVIRON_SOURCES:
         source_type = ENVIRON_SOURCES[key]
 
         node = _build_source_node(framework, key, source_type, False)
```

### Comparing `contrast-agent-7.6.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py` & `contrast-agent-7.7.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py` & `contrast-agent-7.7.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py` & `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py` & `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/common.py` & `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/common.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/django_routes.py` & `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/django_routes.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py` & `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py` & `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py` & `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py` & `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py` & `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/patch_controller.py` & `contrast-agent-7.7.0/src/contrast/agent/patch_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 from contrast_vendor import structlog as logging
 
 logger = logging.getLogger("contrast")
 
-from contrast.agent import scope
 from contrast.agent.assess.policy import string_propagation
 from contrast.agent.policy import registry
 from contrast.agent.policy.applicator import register_import_hooks
 from contrast.agent.policy.rewriter import apply_rewrite_policy
 from contrast.agent.settings import Settings
 from contrast.assess_extensions import cs_str
 from contrast.patches import (
@@ -98,15 +97,14 @@
 
             cs_str_patches.patch_strtype_method(strtype, real_method_name)
             logger.debug(
                 "Applied pure Python patch for %s.%s", strtype.__name__, method_name
             )
 
 
-@scope.with_contrast_scope
 def enable_assess_patches(use_extension_hooks=True):
     """
     Enables extension hooks and other string patches.
 
     Has no effect if these patches are already enabled.
     """
     if module.assess_patches_enabled:
@@ -207,32 +205,21 @@
     # the runner, this has no effect (other than to log a message).
     # Eventually once the runner is fully supported we might feel comfortable
     # removing this code.
     if settings.is_rewriter_enabled:
         register_rewriter(override_config=True)
 
 
-def _enable_patches():
+def enable_patches():
     settings = Settings()
 
     if settings.is_analyze_libs_enabled():
         register_library_patches()
 
     if settings.is_protect_enabled():
         _enable_protect_patches()
 
     if settings.is_assess_enabled():
         _enable_assess_patches(settings)
 
     logger.debug("revisiting imported modules to apply patches")
     repatch_imported_modules()
-
-
-def enable_patches():
-    """
-    Enable all patches for agent based on current settings
-    """
-    # Being in scope here prevents us from inadvertently propagating while we are
-    # applying patches and navigating policy. This has a fairly significant performance
-    # impact for assess initialization, and also promotes correctness/safety.
-    with scope.contrast_scope():
-        _enable_patches()
```

### Comparing `contrast-agent-7.6.0/src/contrast/agent/policy/applicator.py` & `contrast-agent-7.7.0/src/contrast/agent/policy/applicator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/policy/constants.py` & `contrast-agent-7.7.0/src/contrast/agent/policy/constants.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/policy/patch_location_policy.py` & `contrast-agent-7.7.0/src/contrast/agent/policy/patch_location_policy.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/policy/patch_manager.py` & `contrast-agent-7.7.0/src/contrast/agent/policy/patch_manager.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/policy/policy_node.py` & `contrast-agent-7.7.0/src/contrast/agent/policy/policy_node.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/policy/registry.py` & `contrast-agent-7.7.0/src/contrast/agent/policy/registry.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/policy/rewriter.py` & `contrast-agent-7.7.0/src/contrast/agent/policy/rewriter.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/policy/trigger_node.py` & `contrast-agent-7.7.0/src/contrast/agent/policy/trigger_node.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/policy/utils.py` & `contrast-agent-7.7.0/src/contrast/agent/policy/utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/input_analysis.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/input_analysis.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/policy/__init__.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/base_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/base_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         Appends attacker to the context if a positive evaluation is found
         """
         logger.debug("PROTECT: Postfilter for %s", self.name)
 
         if self.mode in [ProtectionRule.OFF, ProtectionRule.PERMIT]:
             return
 
-        attack = self.find_attack(analysis_state=POSTFILTER)
+        attack = self.find_attack(analysis_stage=POSTFILTER)
         if attack is None or len(attack.samples) == 0:
             return
 
         self._append_to_context(attack)
 
         if self.should_block(attack):
             raise contrast.SecurityException(rule_name=self.name)
```

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/cmdi_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/cmdi_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/deserialization_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/http_method_tampering.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/http_method_tampering.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/nosqli_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/nosqli_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/path_traversal_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/path_traversal_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/rules_builder.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/rules_builder.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/sqli_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/sqli_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/ssrf_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/ssrf_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/xss_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/xss_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/protect/rule/xxe_rule.py` & `contrast-agent-7.7.0/src/contrast/agent/protect/rule/xxe_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/reaction_processor.py` & `contrast-agent-7.7.0/src/contrast/agent/reaction_processor.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/request.py` & `contrast-agent-7.7.0/src/contrast/agent/request.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/request_context.py` & `contrast-agent-7.7.0/src/contrast/agent/request_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,18 @@
             self.max_propagators_logged = True
 
         return threshold_reached
 
     @property
     def propagate_assess(self):
         # TODO: PYT-644 move this property of out this class?
-        return Settings().is_assess_enabled() and not scope.in_scope()
+        return (
+            Settings().is_assess_enabled()
+            and not scope.in_contrast_or_propagation_scope()
+        )
 
     def source_created(self):
         """
         Increase the running count of sources created in this request
         """
         self.source_count += 1
```

### Comparing `contrast-agent-7.6.0/src/contrast/agent/request_state.py` & `contrast-agent-7.7.0/src/contrast/agent/request_state.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/runner.py` & `contrast-agent-7.7.0/src/contrast/agent/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import os
 
 from contrast_rewriter import rewrite_for_pytest
+from contrast.agent import scope
 from contrast.agent.patch_controller import enable_assess_patches
 from contrast.agent.policy.rewriter import apply_rewrite_policy
 from contrast.configuration.agent_config import AgentConfig
 from contrast.patches import register_middleware_patches
 from contrast_vendor import structlog as logging
 
 from contrast.scripts.runner import USING_RUNNER_ENV_VAR, USING_REWRITE_WHILE_TESTING
@@ -18,14 +19,15 @@
     """
     We could probably check PYTHONPATH or see if our sitecustomize.py is in sys.modules,
     but using our own totally isolated env var is very safe
     """
     return os.environ.get(USING_RUNNER_ENV_VAR, "false") == "true"
 
 
+@scope.with_contrast_scope
 def start_runner():
     if rewrite_for_pytest():
         if bool(os.environ.get(USING_REWRITE_WHILE_TESTING, False)):
             apply_rewrite_policy(override_config=True)
         return
 
     config = AgentConfig()
```

### Comparing `contrast-agent-7.6.0/src/contrast/agent/server_settings_poll.py` & `contrast-agent-7.7.0/src/contrast/agent/server_settings_poll.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/settings.py` & `contrast-agent-7.7.0/src/contrast/agent/settings.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/sys_monitoring.py` & `contrast-agent-7.7.0/src/contrast/agent/sys_monitoring.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/telemetry.py` & `contrast-agent-7.7.0/src/contrast/agent/telemetry.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/thread_watcher.py` & `contrast-agent-7.7.0/src/contrast/agent/thread_watcher.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/agent/validator.py` & `contrast-agent-7.7.0/src/contrast/agent/validator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/aiohttp/middleware.py` & `contrast-agent-7.7.0/src/contrast/aiohttp/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,47 +50,48 @@
 
         self.app = request.app
         self.request_path = request.path
 
         # the request_id context manager must come first!
         with request_state.request_id_context(), Profiler(
             self.request_path
-        ), log_request_start_and_end(self.request_path):
+        ), log_request_start_and_end(request.method, self.request_path):
             with scope.contrast_scope():
                 environ = await sources.aiohttp_request_to_environ(request)
 
             context = self.should_analyze_request(environ)
             if context:
                 with contrast.CS__CONTEXT_TRACKER.lifespan(context):
                     return await self.call_with_agent(context, request, handler)
 
             return await self.call_without_agent_async(request, handler)
 
     async def call_with_agent(self, context, request, handler) -> StreamResponse:
-        sources.track_aiohttp_request_sources(context, request)
+        with scope.contrast_scope():
+            sources.track_aiohttp_request_sources(context, request)
 
-        try:
-            self.prefilter()
+            try:
+                self.prefilter()
 
-            response = await handler(request)
+                with scope.pop_contrast_scope():
+                    response = await handler(request)
 
-            with scope.contrast_scope():
                 wrapped_response = AioHttpResponseWrapper(response)
 
-            context.extract_response_to_context(wrapped_response)
+                context.extract_response_to_context(wrapped_response)
 
-            self.postfilter(context)
-            self.check_for_blocked(context)
+                self.postfilter(context)
+                self.check_for_blocked(context)
 
-            return response
+                return response
 
-        finally:
-            self.handle_ensure(context, request)
-            if self.settings.is_assess_enabled():
-                contrast.STRING_TRACKER.ageoff()
+            finally:
+                self.handle_ensure(context, request)
+                if self.settings.is_assess_enabled():
+                    contrast.STRING_TRACKER.ageoff()
 
     async def call_without_agent_async(self, request, handler) -> StreamResponse:
         super().call_without_agent()
         with scope.contrast_scope():
             return await handler(request)
 
     @fail_quietly("Unable to get route coverage", return_value={})
```

### Comparing `contrast-agent-7.6.0/src/contrast/aiohttp/sources.py` & `contrast-agent-7.7.0/src/contrast/aiohttp/sources.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import io
 
-from contrast.agent import scope
-from contrast.agent.assess.policy.analysis import skip_analysis
+from contrast.agent import agent_state
 from contrast.agent.assess.policy.source_policy import (
     cs__apply_source,
     build_source_node,
 )
 from contrast.utils.decorators import fail_loudly
 
 
@@ -105,22 +104,21 @@
     """
     Explicitly tracks all relevant attributes of an aiohttp.web.BaseRequest object. This
     is similar to the environ/scope trackers.
 
     @param context: the current request context
     @param request: the aiohttp request object
     """
-    if skip_analysis(context):
+    if (settings := agent_state.get_settings()) and not settings.is_assess_enabled():
         return
 
-    with scope.contrast_scope():
-        for attr_name in AIOHTTP_REQUEST_SOURCES:
-            if hasattr(request, attr_name):
-                node = build_source_node(
-                    SOURCE_DICT,
-                    attr_name,
-                    AIOHTTP_REQUEST_SOURCES[attr_name],
-                )
-                attr = getattr(request, attr_name)
-                cs__apply_source(
-                    context, node, attr, request, attr, (), {}, source_name=attr_name
-                )
+    for attr_name in AIOHTTP_REQUEST_SOURCES:
+        if hasattr(request, attr_name):
+            node = build_source_node(
+                SOURCE_DICT,
+                attr_name,
+                AIOHTTP_REQUEST_SOURCES[attr_name],
+            )
+            attr = getattr(request, attr_name)
+            cs__apply_source(
+                context, node, attr, request, attr, (), {}, source_name=attr_name
+            )
```

### Comparing `contrast-agent-7.6.0/src/contrast/api/architecture_component.py` & `contrast-agent-7.7.0/src/contrast/api/architecture_component.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/api/attack.py` & `contrast-agent-7.7.0/src/contrast/api/attack.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/api/finding.py` & `contrast-agent-7.7.0/src/contrast/api/finding.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/api/library.py` & `contrast-agent-7.7.0/src/contrast/api/library.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/api/route_coverage.py` & `contrast-agent-7.7.0/src/contrast/api/route_coverage.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/api/trace_event.py` & `contrast-agent-7.7.0/src/contrast/api/trace_event.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/api/type_checked_property.py` & `contrast-agent-7.7.0/src/contrast/api/type_checked_property.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/api/user_input.py` & `contrast-agent-7.7.0/src/contrast/api/user_input.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/applies/__init__.py` & `contrast-agent-7.7.0/src/contrast/applies/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/applies/assess/unsafe_code_execution.py` & `contrast-agent-7.7.0/src/contrast/applies/assess/unsafe_code_execution.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/applies/sqli.py` & `contrast-agent-7.7.0/src/contrast/applies/sqli.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/asgi/middleware.py` & `contrast-agent-7.7.0/src/contrast/asgi/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             return
 
         self.request_path = scope.get("path", "")
 
         # the request_id context manager must come first!
         with request_state.request_id_context(), Profiler(
             self.request_path
-        ), log_request_start_and_end(self.request_path):
+        ), log_request_start_and_end(scope.get("method", ""), self.request_path):
             if scope.get("type") != "http":
                 logger.debug("Detected non-http request - cannot analyze", scope=scope)
                 await self.call_without_agent_async(scope, receive, send)
                 return
 
             request = ASGIRequest(scope, receive)
             environ = await request.to_wsgi_environ()
@@ -98,35 +98,39 @@
                 with contrast.CS__CONTEXT_TRACKER.lifespan(context):
                     await self.call_with_agent(context, request, send)
                     return
 
             await self.call_without_agent_async(scope, receive, send)
 
     async def call_with_agent(self, context, request, send) -> None:
-        track_scope_sources(context, request.scope)
-
-        try:
-            self.prefilter()
-
-            response = ASGIResponse(send)
-            await self.asgi_app(
-                request.scope, request.contrast__receive, response.contrast__send
-            )
-
-            context.extract_response_to_context(response)
-
-            self.postfilter(context)
-            self.check_for_blocked(context)
+        with scope_.contrast_scope():
+            track_scope_sources(context, request.scope)
 
-            await response.call_send()
+            try:
+                self.prefilter()
 
-        finally:
-            self.handle_ensure(context, context.request)
-            if self.settings.is_assess_enabled():
-                contrast.STRING_TRACKER.ageoff()
+                response = ASGIResponse(send)
+                with scope_.pop_contrast_scope():
+                    await self.asgi_app(
+                        request.scope,
+                        request.contrast__receive,
+                        response.contrast__send,
+                    )
+
+                context.extract_response_to_context(response)
+
+                self.postfilter(context)
+                self.check_for_blocked(context)
+
+                await response.call_send()
+
+            finally:
+                self.handle_ensure(context, context.request)
+                if self.settings.is_assess_enabled():
+                    contrast.STRING_TRACKER.ageoff()
 
     async def call_without_agent_async(self, scope, receive, send) -> None:
         super().call_without_agent()
         with scope_.contrast_scope():
             await self.asgi_app(scope, receive, send)
 
     @cached_property
```

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/__init__.py` & `contrast-agent-7.7.0/src/contrast/assess_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/common/cast.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/common/cast.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/common/format.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/common/format.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/common/logging.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/common/logging.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/common/patches.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/common/patches.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/common/propagate.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/common/propagate.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/common/repeat.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/common/repeat.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/common/repr.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/common/repr.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/common/scope.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/common/scope.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/common/streams.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/common/streams.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/common/subscript.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/common/subscript.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/common/trace.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/common/trace.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/.travis.yml` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.travis.yml`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/LICENSE` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/Makefile.in` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/Makefile.in`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/README.md` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/README.md`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/appveyor.yml` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/appveyor.yml`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/config.guess` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/config.guess`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/config.sub` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/config.sub`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/configure.ac` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/configure.ac`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/COPYING` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/COPYING`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/README.md` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/README.md`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/setup.py` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/setup.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/config.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/config.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/include/funchook.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/include/funchook.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/install-sh` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/install-sh`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/Makefile.in` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/Makefile.in`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/__strerror.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/__strerror.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook_io.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_io.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook_io.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_io.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/os_func.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/os_func.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/printf_base.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/printf_base.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/src/printf_base.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/printf_base.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/test/Makefile.in` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/Makefile.in`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/test/suffix.list` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/suffix.list`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/test/test_main.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/test_main.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/test/x86_test.S` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/x86_test.S`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/funchook.sln` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook.sln`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters` & `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/include/contrast/assess/logging.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/logging.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/include/contrast/assess/patches.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/patches.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/include/contrast/assess/scope.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/scope.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/include/contrast/assess/utils.h` & `contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/utils.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py3/patches.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py3/patches.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py3/str_concat.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py3/str_concat.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py310/bytearray.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py310/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py310/bytes.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py310/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py310/bytesio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py310/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py310/iobase.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py310/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py310/stringio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py310/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py310/unicode.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py310/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py311/bytearray.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py311/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py311/bytes.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py311/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py311/bytesio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py311/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py311/iobase.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py311/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py311/stringio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py311/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py311/unicode.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py311/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py312/bytearray.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py312/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py312/bytes.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py312/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py312/bytesio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py312/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py312/iobase.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py312/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py312/stringio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py312/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py312/unicode.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py312/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py35/bytearray.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py35/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py35/bytes.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py35/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py35/bytesio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py35/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py35/iobase.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py35/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py35/stringio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py35/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py35/unicode.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py35/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py36/bytearray.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py36/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py36/bytes.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py36/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py36/bytesio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py36/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py36/iobase.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py36/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py36/stringio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py36/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py36/unicode.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py36/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py37/bytearray.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py37/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py37/bytes.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py37/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py37/bytesio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py37/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py37/iobase.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py37/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py37/stringio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py37/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py37/unicode.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py37/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py38/bytearray.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py38/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py38/bytes.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py38/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py38/bytesio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py38/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py38/iobase.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py38/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py38/stringio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py38/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py38/unicode.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py38/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py39/bytearray.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py39/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py39/bytes.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py39/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py39/bytesio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py39/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py39/iobase.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py39/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py39/stringio.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py39/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/assess_extensions/py39/unicode.c` & `contrast-agent-7.7.0/src/contrast/assess_extensions/py39/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/configuration/agent.py` & `contrast-agent-7.7.0/src/contrast/configuration/agent.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/configuration/agent_config.py` & `contrast-agent-7.7.0/src/contrast/configuration/agent_config.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/configuration/api.py` & `contrast-agent-7.7.0/src/contrast/configuration/api.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/configuration/application.py` & `contrast-agent-7.7.0/src/contrast/configuration/application.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/configuration/assess.py` & `contrast-agent-7.7.0/src/contrast/configuration/assess.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/configuration/config_builder.py` & `contrast-agent-7.7.0/src/contrast/configuration/config_builder.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/configuration/config_option.py` & `contrast-agent-7.7.0/src/contrast/configuration/config_option.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/configuration/inventory.py` & `contrast-agent-7.7.0/src/contrast/configuration/inventory.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/configuration/protect.py` & `contrast-agent-7.7.0/src/contrast/configuration/protect.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/configuration/server.py` & `contrast-agent-7.7.0/src/contrast/configuration/server.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/loader/sitecustomize.py` & `contrast-agent-7.7.0/src/contrast/loader/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/__init__.py` & `contrast-agent-7.7.0/src/contrast/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/cgi_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/cgi_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/concurrent_futures_thread_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/concurrent_futures_thread_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/cs_io.py` & `contrast-agent-7.7.0/src/contrast/patches/cs_io.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/cs_str.py` & `contrast-agent-7.7.0/src/contrast/patches/cs_str.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/databases/dbapi2.py` & `contrast-agent-7.7.0/src/contrast/patches/databases/dbapi2.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/databases/mysql_connector_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/databases/mysql_connector_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/databases/psycopg2_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/databases/psycopg2_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/databases/sqlalchemy_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/databases/sqlalchemy_patch.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import sys
 
 from contrast_vendor import wrapt
 from contrast.patches.databases import dbapi2
 from contrast.utils import Namespace
 
+from contrast_vendor import structlog as logging
+
+logger = logging.getLogger("contrast")
+
+
 ENGINE_DEFAULT_MODULE = "sqlalchemy.engine.default"
 
 
 class module(Namespace):
     # saved version of the original (unpatched) method
     # this value is None iff the method is currently unpatched
     unpatched_method = None
@@ -43,16 +48,31 @@
     """
     Wrapt decides to separate `instance` from `args`. Don't worry that `instance`
     isn't passed back in to `wrapped` at call-time! This is already handled internally
     by wrapt.
 
     See https://wrapt.readthedocs.io/en/latest/wrappers.html#function-wrappers.
     """
-    if "dbapi" in kwargs:
+    if getattr(instance, "is_async", False):
+        logger.debug(
+            "WARNING: Detected async sqlalchemy dialect - will not instrument",
+            instance=instance,
+            args=args,
+            kwargs=kwargs,
+        )
+    elif "dbapi" in kwargs:
         dbapi2.instrument_adapter(kwargs["dbapi"], "sqlalchemy")
+    else:
+        logger.debug(
+            "WARNING: couldn't extract dbapi adapter from dialect",
+            instance=instance,
+            args=args,
+            kwargs=kwargs,
+        )
+
     return wrapped(*args, **kwargs)
 
 
 def patch_sqlalchemy(sqlalchemy_engine_default):
     """
     SQLAlchemy performs some downright demonic introspection on the __init__ methods
     for DefaultDialect and subclasses (see sqlalchemy.util.langhelpers.get_cls_kwargs).
```

### Comparing `contrast-agent-7.6.0/src/contrast/patches/databases/sqlite3_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/databases/sqlite3_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/encodings_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/encodings_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/exec_and_eval.py` & `contrast-agent-7.7.0/src/contrast/patches/frameworks/bottle_patches.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,178 +1,149 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
-"""
-Instrumentation for exec/eval.
-
-This was defined outside of policy.json because we need to pass globals/locals from the
-frame in which function was originally called
-"""
-import ast
-import copy
-from sys import _getframe as getframe
-
+import sys
 from contrast_vendor.wrapt import register_post_import_hook
 
-import builtins
 import contrast
 from contrast.agent import scope
-from contrast.agent.policy import registry
-from contrast.agent.assess.policy import trigger_policy
-from contrast.utils.patch_utils import build_and_apply_patch
-from contrast.applies.assess.unsafe_code_execution import (
-    apply_rule as apply_unsafe_code_exec_rule,
-)
+from contrast.agent.policy.applicator import apply_module_patches
+from contrast.agent.middlewares.route_coverage.common import build_route
+from contrast.agent.middlewares.route_coverage.bottle_routes import create_bottle_routes
+from contrast.agent.policy import patch_manager
+from contrast.utils.patch_utils import build_and_apply_patch, wrap_and_watermark
 from contrast.utils.decorators import fail_quietly
-from contrast.utils.patch_utils import wrap_and_watermark
-from contrast_rewriter import PropagationRewriter, populate_operator_module
-
-
-INSTRUMENTED_FRAME_DEPTH = 1
-
-orig_compile = builtins.compile
-
-
-@fail_quietly("Error applying rule for exec/eval patch")
-def apply_rule(rule_applicator, orig_func, result, args, kwargs):
-    context = contrast.CS__CONTEXT_TRACKER.current()
-    if not (context and context.propagate_assess):
-        return
-
-    with scope.contrast_scope():
-        rule_applicator("BUILTIN", orig_func.__name__, result, args, kwargs)
 
+from contrast_vendor import structlog as logging
 
-@fail_quietly("Error running path traversal assess rule")
-def apply_pt_rule(module, method, result, args, kwargs):
-    trigger_rule = registry.get_triggers_by_rule("path-traversal")
+MODULE_NAME = "bottle"
 
-    trigger_nodes = trigger_rule.find_trigger_nodes(module, method)
+logger = logging.getLogger("contrast")
 
-    trigger_policy.apply(trigger_rule, trigger_nodes, result, args, kwargs)
 
+def build_prepare_patch(orig_func, patch_policy, bottle_module):
+    del patch_policy
 
-def rewrite(mode, code):
-    rewriter = PropagationRewriter()
-    return ast.fix_missing_locations(rewriter.visit(ast.parse(code, mode=mode)))
-
-
-@fail_quietly("Error when applying rewriter to eval/exec/compiled input")
-def apply_rewriter(mode, code):
-    if not isinstance(code, str):
-        return None
-
-    with scope.contrast_scope():
-        return orig_compile(
-            rewrite(mode, code),
-            filename="<internal>",
-            mode=mode,
-        )
-
-
-def build_exec_eval_patch(orig_func, _, rule_applicator, mode):
-    def exec_eval_patch(code, globs=None, locs=None):
+    def prepare_patch(wrapped, instance, args, kwargs):
         """
-        Run exec/eval call with proper context to adjust for current frame
+        Patch for bottle.SimpleTemplate.prepare.
 
-        Code ported from six module
-        See https://github.com/benjaminp/six/blob/master/six.py#L694
-
-        Reapplying the context from the 3rd frame (from top of stack) is necessary
-        because the globals and locals in that frame are used in the original call to
-        exec/eval. The exception to this is if the caller passes custom globals/locals
-        to the function.
-
-        If we fail provide this context we will see a number of errors due to things
-        not defined in the scope of this function upon calling the original function
-        definition.
+        This is needed because of the unfortunate way bottle calls on
+        `html_escape` as a kwarg in the prepare definition in SimpleTemplate.
+        See https://github.com/bottlepy/bottle/blob/master/bottle.py#L3952
+
+        Because of this behavior, the `html_escape` func is not our patched
+        `html_escape` defined in policy.
+        By patching prepare, we intercept its call and instead of allowing
+        it to use the default kwarg for `html_escape`, we pass our own
+        patched `html_escape` in order to prevent false positive XSS findings.
         """
-        result = None
-
-        if globs is None:
-            frame = getframe(INSTRUMENTED_FRAME_DEPTH)
-
-            globs = frame.f_globals
-            if locs is None:
-                locs = frame.f_locals
-            del frame
-        elif locs is None:
-            locs = globs
-
-        # Ensure our rewriter patches are in (global) scope for the code about to be executed
-        populate_operator_module(globs)
-
-        try:
-            code_to_run = apply_rewriter(mode, code) or code
-            result = orig_func(code_to_run, globs, locs)
-        except Exception:
-            result = None
-            raise
-        finally:
-            apply_rule(rule_applicator, orig_func, result, (code,), {})
+        del instance
 
+        # html_escape MUST already be patched by policy in order
+        # to pass in the patched func to prepare
+        kwargs.setdefault("escape_func", bottle_module.html_escape)
+        return wrapped(*args, **kwargs)
+
+    return wrap_and_watermark(orig_func, prepare_patch)
+
+
+def build_call_patch(orig_func, patch_policy):
+    """
+    Patch for bottle.Bottle.__call__
+
+    This is how we perform route discovery for Bottle. Many different patches could
+    probably work here, since we really just need a reference to the Bottle instance
+    after all routes have been registered.
+    """
+    del patch_policy
+
+    def call_patch(wrapped, instance, args, kwargs):
+        result = wrapped(*args, **kwargs)
+        do_bottle_route_discovery(instance)
         return result
 
-    # NOTE: do not wrap since it will potentially affect stack level
-    return exec_eval_patch
+    return wrap_and_watermark(orig_func, call_patch)
 
 
-# NOTE: maybe this should be moved to a utility module
-def find_arg(args, kwargs, idx, kw=None, default=None, pop=False):
-    if kw and kw in kwargs:
-        return kwargs.pop(kw) if pop else kwargs[kw]
+@fail_quietly("unable to perform Bottle route discovery")
+def do_bottle_route_discovery(bottle_instance):
+    with scope.contrast_scope():
+        from contrast.agent import agent_state
 
-    if len(args) <= idx:
-        return default
+        if not agent_state.is_first_request():
+            return
 
-    return args[idx]
+        discovered_routes = create_bottle_routes(bottle_instance)
+        agent_state.update_routes(discovered_routes)
+        logger.debug(
+            "Discovered the following Bottle routes: %s",
+            [f"{route.verb} {route.url}" for route in discovered_routes.values()],
+        )
 
 
-def build_compile_patch(orig_func, _, rule_applicator):
-    def compile_patch(wrapped, instance, args, kwargs):
-        del instance
+def build_match_patch(orig_func, patch_policy):
+    """
+    Patch for bottle.Router.match()
+
+    This sets up request context with all necessary info for current route observation
+    """
+    del patch_policy
 
-        if scope.in_contrast_scope():
-            return wrapped(*args, **kwargs)
+    def match_patch(wrapped, instance, args, kwargs):
+        del instance
 
-        result = None
-        orig_kwargs = copy.copy(kwargs)
+        result = wrapped(*args, **kwargs)
+        do_bottle_route_observation(result)
+        return result
 
-        try:
-            code = find_arg(args, kwargs, 0, kw="source", pop=True)
-            mode = find_arg(args, kwargs, 2, kw="mode", default="exec")
-
-            with scope.contrast_scope():
-                code_to_compile = rewrite(mode, code)
-                result = orig_compile(code_to_compile, *args[1:], **kwargs)
-        except Exception:
-            result = None
-            raise
-        finally:
-            apply_rule(rule_applicator, orig_func, result, args, orig_kwargs)
+    return wrap_and_watermark(orig_func, match_patch)
 
-        return result
 
-    return wrap_and_watermark(orig_func, compile_patch)
+@fail_quietly("unable to perform bottle route coverage in Bottle match patch")
+def do_bottle_route_observation(match_result):
+    with scope.contrast_scope():
+        if match_result is None:
+            return
 
+        context = contrast.CS__CONTEXT_TRACKER.current()
+        if context is None:
+            return
+
+        context.view_func = match_result[0].callback
+        context.view_func_str = build_route(
+            context.request.get_normalized_uri(),
+            context.view_func,
+        )
+        logger.debug("Observed Bottle route: %s", context.view_func_str)
 
-def patch_exec_and_eval(builtins_module):
-    build_and_apply_patch(
-        builtins_module,
-        "eval",
-        build_exec_eval_patch,
-        (apply_unsafe_code_exec_rule, "eval"),
-    )
 
-    build_and_apply_patch(
-        builtins_module,
-        "exec",
-        build_exec_eval_patch,
-        (apply_unsafe_code_exec_rule, "exec"),
-    )
+def patch_bottle(bottle_module):
+    # We ask policy to go ahead and do all bottle patches here (even though policy
+    # patches will happen later on) because we MUST have some bottle policy patches
+    # already applied for these non-policy patches to work.
+    # This would not be necessary if in _enable_patches policy_patches were applied
+    # first.
+    apply_module_patches(bottle_module)
 
     build_and_apply_patch(
-        builtins_module, "compile", build_compile_patch, (apply_unsafe_code_exec_rule,)
+        bottle_module.SimpleTemplate,
+        "prepare",
+        build_prepare_patch,
+        builder_args=(bottle_module,),
     )
+    build_and_apply_patch(bottle_module.Bottle, "__call__", build_call_patch)
+    build_and_apply_patch(bottle_module.Router, "match", build_match_patch)
 
 
 def register_patches():
-    register_post_import_hook(patch_exec_and_eval, builtins.__name__)
+    register_post_import_hook(patch_bottle, MODULE_NAME)
+
+
+def reverse_patches():
+    bottle_module = sys.modules.get(MODULE_NAME)
+    if not bottle_module:
+        return
+
+    patch_manager.reverse_patches_by_owner(bottle_module)
+    patch_manager.reverse_patches_by_owner(bottle_module.SimpleTemplate)
+    patch_manager.reverse_patches_by_owner(bottle_module.Bottle)
+    patch_manager.reverse_patches_by_owner(bottle_module.Router)
```

### Comparing `contrast-agent-7.6.0/src/contrast/patches/frameworks/django_patches.py` & `contrast-agent-7.7.0/src/contrast/patches/frameworks/django_patches.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         a class that inherits from str and that ends up propagating excessively.
 
         Because mark_safe is called many times when Django renders a template,
         excessive propagation is incredibly costly. So instead, we do the same work as
         the KEEP propagator would, but with a deadzoned call to the original function.
         """
         # if we're already in scope, don't bother doing any analysis
-        if scope.in_scope():
+        if scope.in_contrast_or_propagation_scope():
             return wrapped(*args, **kwargs)
 
         # if we're not yet in scope, call wrapped and analysis in scope
         with scope.contrast_scope():
             # We don't wrap wrapped call in try/catch because if it raises an error
             # we don't want to do any analysis.
             result = wrapped(*args, **kwargs)
```

### Comparing `contrast-agent-7.6.0/src/contrast/patches/frameworks/drf_patches.py` & `contrast-agent-7.7.0/src/contrast/patches/frameworks/drf_patches.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/frameworks/falcon_patches.py` & `contrast-agent-7.7.0/src/contrast/patches/frameworks/falcon_patches.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/frameworks/flask_and_quart_patches.py` & `contrast-agent-7.7.0/src/contrast/patches/frameworks/flask_and_quart_patches.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/frameworks/pyramid_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/frameworks/pyramid_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/frameworks/starlette_patches.py` & `contrast-agent-7.7.0/src/contrast/patches/frameworks/starlette_patches.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/genshi_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/genshi_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/import_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/import_patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,14 +229,17 @@
 
 
 def patch_import(module):
     build_and_apply_patch(module, "__import__", build_import_patch)
 
 
 def register_patches():
+    # Initialize the distribution context to avoid
+    # slow down when the first request is made.
+    DistributionContext()
     register_post_import_hook(patch_import, builtins.__name__)
     register_post_import_hook(patch_import, "importlib")
 
 
 def reverse_patches():
     patch_manager.reverse_patches_by_owner(builtins)
```

### Comparing `contrast-agent-7.6.0/src/contrast/patches/lxml_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/lxml_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/middleware/aiohttp.py` & `contrast-agent-7.7.0/src/contrast/patches/middleware/aiohttp.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/middleware/common.py` & `contrast-agent-7.7.0/src/contrast/patches/middleware/common.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/middleware/django.py` & `contrast-agent-7.7.0/src/contrast/patches/middleware/django.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/middleware/mod_wsgi.py` & `contrast-agent-7.7.0/src/contrast/patches/middleware/mod_wsgi.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/operator.py` & `contrast-agent-7.7.0/src/contrast/patches/operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     policy_node = get_propagation_node(patch_policy)
 
     def add(wrapped, instance, args, kwargs):
         del instance
 
         with scope.contrast_scope():
             result = wrapped(*args, **kwargs)
-        if not is_trackable(result) or scope.in_scope():
+        if not is_trackable(result) or scope.in_contrast_or_propagation_scope():
             return result
 
         analyze_policy(policy_node.name, result, args, kwargs)
 
         return result
 
     return wrap_and_watermark(original_func, add)
@@ -61,15 +61,15 @@
     del patch_policy
 
     def mod(wrapped, instance, args, kwargs):
         del instance
 
         with scope.contrast_scope():
             result = wrapped(*args, **kwargs)
-        if not is_trackable(result) or scope.in_scope():
+        if not is_trackable(result) or scope.in_contrast_or_propagation_scope():
             return result
 
         _propagate_cformat(result, *args)
 
         return result
 
     return wrap_and_watermark(original_func, mod)
```

### Comparing `contrast-agent-7.6.0/src/contrast/patches/pathlib_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/pathlib_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/re_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/re_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 def _trigger_redos(name, result, args, kwargs):
     context = contrast.CS__CONTEXT_TRACKER.current()
     if context is None:
         return
 
     rule = registry.get_triggers_by_rule("redos")
 
-    if not scope.in_trigger_scope() and not scope.in_scope():
+    if not scope.in_trigger_scope() and not scope.in_contrast_or_propagation_scope():
         if rule.disabled:
             # Given how often these patches are called within apps, it's well worth
             # returning early here even though this logic exists further down the stack.
             # However, we MUST call this here after the `in_scope` check because
             # `rule.disabled` calls on Settings code that recursively calls on
             # other patches.
             return
```

### Comparing `contrast-agent-7.6.0/src/contrast/patches/str_new.py` & `contrast-agent-7.7.0/src/contrast/patches/str_new.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/sys_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/sys_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/threading_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/threading_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/urllib_patch.py` & `contrast-agent-7.7.0/src/contrast/patches/urllib_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/patches/utils.py` & `contrast-agent-7.7.0/src/contrast/patches/utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/deadzones.py` & `contrast-agent-7.7.0/src/contrast/policy/deadzones.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/propagators/codecs.py` & `contrast-agent-7.7.0/src/contrast/policy/propagators/codecs.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/propagators/encodings.py` & `contrast-agent-7.7.0/src/contrast/policy/propagators/encodings.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/propagators/frameworks.py` & `contrast-agent-7.7.0/src/contrast/policy/propagators/frameworks.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/propagators/paths.py` & `contrast-agent-7.7.0/src/contrast/policy/propagators/paths.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/propagators/re.py` & `contrast-agent-7.7.0/src/contrast/policy/propagators/re.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/propagators/serialize.py` & `contrast-agent-7.7.0/src/contrast/policy/propagators/serialize.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/propagators/string.py` & `contrast-agent-7.7.0/src/contrast/policy/propagators/string.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/sources/asgi.py` & `contrast-agent-7.7.0/src/contrast/policy/sources/asgi.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/sources/cgi.py` & `contrast-agent-7.7.0/src/contrast/policy/sources/cgi.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/sources/django.py` & `contrast-agent-7.7.0/src/contrast/policy/sources/django.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/sources/falcon.py` & `contrast-agent-7.7.0/src/contrast/policy/sources/falcon.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,41 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 from contrast.agent.policy.registry import register_source_nodes
 from contrast.agent.policy.utils import CompositeNode
 
 
+_CYTHON_REQUEST_POLICY = [
+    {
+        "method_name": [
+            "uri",
+            "url",
+            "relative_uri",
+            "prefix",
+        ],
+        "node_type": "URI",
+        "tags": ["CROSS_SITE"],
+    },
+    {
+        "method_name": [
+            "forwarded_uri",
+            "forwarded_prefix",
+        ],
+        "node_type": "HEADER",
+        "tags": ["NO_NEWLINES"],
+    },
+]
+"""
+Cythonized Falcon cannot be rewritten, so we
+lose dataflow propagation through string concats.
+We need policy to cover this gap in the following
+properties on falcon.request.Request
+"""
+
+
 falcon_sources = [
     CompositeNode(
         {
             "module": "falcon.request",
             "class_name": "Request",
         },
         [
@@ -17,15 +45,16 @@
                 "tags": ["NO_NEWLINES", "CROSS_SITE"],
             },
             {
                 "method_name": "get_media",
                 "node_type": "BODY",
                 "tags": ["NO_NEWLINES", "CROSS_SITE"],
             },
-        ],
+        ]
+        + _CYTHON_REQUEST_POLICY,
     ),
     CompositeNode(
         {
             "module": "falcon.asgi.request",
             "class_name": "Request",
         },
         [
@@ -35,15 +64,16 @@
                 "tags": ["NO_NEWLINES", "CROSS_SITE"],
             },
             {
                 "method_name": "get_media",
                 "node_type": "BODY",
                 "tags": ["NO_NEWLINES", "CROSS_SITE"],
             },
-        ],
+        ]
+        + _CYTHON_REQUEST_POLICY,
     ),
     {
         "module": "falcon.asgi.stream",
         "class_name": "BoundedStream",
         "method_name": "read",
         "node_type": "BODY",
         "tags": ["NO_NEWLINES", "CROSS_SITE"],
```

### Comparing `contrast-agent-7.6.0/src/contrast/policy/sources/flask.py` & `contrast-agent-7.7.0/src/contrast/policy/sources/flask.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/sources/quart.py` & `contrast-agent-7.7.0/src/contrast/policy/sources/quart.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/sources/webob.py` & `contrast-agent-7.7.0/src/contrast/policy/sources/webob.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/__init__.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/cmd_injection.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/cmd_injection.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/crypto.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/crypto.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/httponly.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/httponly.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/nosql_injection.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/nosql_injection.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/path_traversal.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/path_traversal.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/prompt_injection.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/prompt_injection.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/redos.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/redos.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/reflected_xss.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/reflected_xss.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/secure_flag_missing.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/secure_flag_missing.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/session_rewriting.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/session_rewriting.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/session_timeout.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/session_timeout.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/sql_injection.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/sql_injection.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/ssrf.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/ssrf.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/trust_boundary_violation.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/trust_boundary_violation.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/unsafe_code_execution.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/unsafe_code_execution.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/untrusted_deserialization.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/untrusted_deserialization.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/unvalidated_redirect.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/unvalidated_redirect.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/xpath_injection.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/xpath_injection.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/policy/triggers/xxe.py` & `contrast-agent-7.7.0/src/contrast/policy/triggers/xxe.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/activity_masker.py` & `contrast-agent-7.7.0/src/contrast/reporting/activity_masker.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/reporting_client.py` & `contrast-agent-7.7.0/src/contrast/reporting/reporting_client.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/request_audit.py` & `contrast-agent-7.7.0/src/contrast/reporting/request_audit.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/__init__.py` & `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/_traces.py` & `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/_traces.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/application_activity.py` & `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/application_activity.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/application_inventory.py` & `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/application_inventory.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/application_startup.py` & `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/application_startup.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/application_update.py` & `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/application_update.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/base_ts_message.py` & `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/base_ts_message.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/effective_config.py` & `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/effective_config.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/heartbeat.py` & `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/heartbeat.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/library_usage.py` & `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/library_usage.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/observed_route.py` & `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/observed_route.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/preflight.py` & `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/preflight.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/server_activity.py` & `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/server_activity.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/reporting/teamserver_messages/server_startup.py` & `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/server_startup.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/scripts/fix_interpreter_permissions.py` & `contrast-agent-7.7.0/src/contrast/scripts/fix_interpreter_permissions.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/scripts/propagator_check.py` & `contrast-agent-7.7.0/src/contrast/scripts/propagator_check.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/scripts/runner.py` & `contrast-agent-7.7.0/src/contrast/scripts/runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,23 +37,33 @@
         usage=USAGE,
         epilog=EPILOG,
     )
     parser.add_argument(
         "--rewrite-for-pytest", action="store_true", help=argparse.SUPPRESS
     )
     # if you add public arguments here, update USAGE accordingly
-    parser.add_argument("cmd", nargs="+")
+    parser.add_argument(
+        "cmd",
+        nargs="+",
+        help="Command to run with the agent. cmd should be available in the operating system PATH.",
+    )
 
     parsed = parser.parse_args()
 
     config = AgentConfig()
 
     loader_path = os.path.join(os.path.dirname(__file__), "loader")
     os.environ[PYTHONPATH] = os.path.pathsep.join([loader_path] + sys.path)
     os.environ[USING_RUNNER_ENV_VAR] = "true"
 
     if parsed.rewrite_for_pytest or config.should_pytest_rewrite:
         os.environ[REWRITE_FOR_PYTEST] = "true"
     elif config.should_rewrite:
         os.environ[ENABLE_REWRITER] = "true"
 
-    os.execl(shutil.which(parsed.cmd[0]), *parsed.cmd)
+    cmd_path, *args = shutil.which(parsed.cmd[0]), *parsed.cmd
+    if cmd_path is None:
+        logger.error("Command not found in PATH", cmd=parsed.cmd[0])
+        logger.info(f"Run '{sys.argv[0]} --help' for usage information.")
+        sys.exit(1)
+        return
+    os.execl(cmd_path, *args)
```

### Comparing `contrast-agent-7.6.0/src/contrast/scripts/validate_config.py` & `contrast-agent-7.7.0/src/contrast/scripts/validate_config.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/assess/duck_utils.py` & `contrast-agent-7.7.0/src/contrast/utils/assess/duck_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/assess/formatting/base.py` & `contrast-agent-7.7.0/src/contrast/utils/assess/formatting/base.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/assess/formatting/tokenize_cformat.py` & `contrast-agent-7.7.0/src/contrast/utils/assess/formatting/tokenize_cformat.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/assess/formatting/tokenize_format.py` & `contrast-agent-7.7.0/src/contrast/utils/assess/formatting/tokenize_format.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/assess/stream_utils.py` & `contrast-agent-7.7.0/src/contrast/utils/assess/stream_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 from contrast_vendor.wrapt import ObjectProxy
 
 from contrast.agent import scope
-from contrast.agent.assess.policy import propagation_policy
 from contrast.agent.assess.policy.source_policy import apply_stream_source
 from contrast.utils.decorators import fail_quietly
 
 from contrast_vendor import structlog as logging
 
 logger = logging.getLogger("contrast")
 
@@ -122,44 +121,14 @@
     """
 
     def __init__(self, wrapped):
         super().__init__(wrapped)
         instrument_source_stream(self)
 
 
-def stream_patch_body(method_name, orig_func, self, *args, **kwargs):
-    # Since we need to make reference to the input multiple times, convert the
-    # first argument to a list and use that instead. This prevents any iterators
-    # from being exhausted before we can make use of them in propagation.
-    if method_name == "writelines" and len(args):
-        args_list = [list(args[0])] + list(args[1:])
-    else:
-        args_list = args
-
-    result = orig_func(*args_list, **kwargs)
-
-    if scope.in_scope():
-        return result
-
-    try:
-        with scope.propagation_scope():
-            propagation_policy.propagate_stream(
-                method_name,
-                result,
-                self,
-                result,
-                args_list,
-                kwargs,
-            )
-    except Exception as ex:
-        logger.debug("failed to propagate %s", method_name, exc_info=ex)
-    finally:
-        return result
-
-
 @fail_quietly("Error instrumenting source stream")
 def instrument_source_stream(stream):
     """
     Mark the provided stream as a source, and instrument methods that produce tracked
     content. This must be a stream that we have proxied. i.e., it has the
     `CS__METHOD_NAMES` attribute.
 
@@ -203,15 +172,15 @@
 
     @param orig_method: original instance method object
     @return method object that is an instrumented version of the original
     """
 
     def patched_method(*args, **kwargs):
         result = orig_method(*args, **kwargs)
-        if not scope.in_scope():
+        if not scope.in_contrast_or_propagation_scope():
             apply_stream_source(
                 orig_method.__name__, result, stream, result, args, kwargs
             )
         return result
 
     patched_method.__name__ = orig_method.__name__
     return patched_method
```

### Comparing `contrast-agent-7.6.0/src/contrast/utils/assess/tag_utils.py` & `contrast-agent-7.7.0/src/contrast/utils/assess/tag_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/assess/tracking_util.py` & `contrast-agent-7.7.0/src/contrast/utils/assess/tracking_util.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/base64_utils.py` & `contrast-agent-7.7.0/src/contrast/utils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/configuration_utils.py` & `contrast-agent-7.7.0/src/contrast/utils/configuration_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     os.path.join(os.getcwd(), 'settings')
     /etc/contrast/python/
     /etc/contrast/
     /etc/
 """
 
 # Valid options are defined in the spec:
-# https://bitbucket.org/contrastsecurity/assess-specifications/src/master/vulnerability/capture-stacktrace.md
+# https://github.com/Contrast-Security-Inc/assess-specifications/blob/master/vulnerability/capture-stacktrace.md
 STACKTRACE_OPTIONS = ["ALL", "SOME", "NONE"]
 
 
 @lru_cache(maxsize=1)
 def get_hostname():
     """
     Returns the hostname from the socket or "localhost"
```

### Comparing `contrast-agent-7.6.0/src/contrast/utils/context_tracker.py` & `contrast-agent-7.7.0/src/contrast/utils/context_tracker.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/decorators.py` & `contrast-agent-7.7.0/src/contrast/utils/decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import os
 import logging as stdlib_logging
 
 import contrast
 from contrast_vendor import structlog as logging
 from contrast.agent.validator import ValidationException
+from contrast_vendor.webob.request import DisconnectionError
 
 logger = logging.getLogger("contrast")
 
 DEBUG_LEVEL = stdlib_logging.DEBUG
 
 
 def _log_extra_safely(
@@ -50,15 +51,18 @@
     except Exception:
         # For complete safety, we're not going to try to log the logging error
         # because sometimes the logging error is actually an error (such as a recursive
         # error) within the logging module itself!
         pass
 
 
-def fail_loudly(log_message=None, log_level="exception", return_value=None):
+SILENCED_EXCEPTIONS = (DisconnectionError, ConnectionResetError)
+
+
+def _fail_safely(log_message, log_level, return_value):
     """
     Decorator that will run the decorated function/method and, if
     an exception is raised, return a safe value and log the error.
 
     Note that SecurityException will always be re-raised.
 
     :param log_message: message to log in case of failure
@@ -70,43 +74,50 @@
     def wrap(original_func):
         def run_safely(*args, **kwargs):
             try:
                 return original_func(*args, **kwargs)
             except contrast.SecurityException:
                 raise
             except Exception as ex:
+                if isinstance(ex, SILENCED_EXCEPTIONS):
+                    logger.debug("Silenced exception in fail_safely", exc_info=ex)
+                    return return_value
+
                 _log_extra_safely(
                     log_message, ex, original_func, args, kwargs, log_level
                 )
                 if os.environ.get("CONTRAST_TESTING"):
                     logger.warn(
-                        "Re-raising exception in fail_loudly (CONTRAST_TESTING is set)"
+                        "Re-raising exception in fail_safely (CONTRAST_TESTING is set)"
                     )
                     raise
 
             return return_value
 
         return run_safely
 
     return wrap
 
 
-def fail_quietly(log_message=None, return_value=None):
+def fail_loudly(log_message=None, log_level="exception", return_value=None):
+    return _fail_safely(log_message, log_level, return_value)
+
+
+def fail_quietly(log_message="fail_quietly caught an exception", return_value=None):
     """
     Similar to fail_loudly (see above)
 
     This decorator is intended to handle cases where an exception may occur but won't
     disrupt normal operation of the agent. This decorator should be used to protect
     against external exceptions we can't prevent but still want to handle.
 
     In these cases, we log an error message and the exception traceback, both at DEBUG
     level.
     """
-
-    return fail_loudly(log_message, "debug", return_value)
+    return _fail_safely(f"WARNING: {log_message}", "debug", return_value)
 
 
 class cached_property:
     """
     https://github.com/pydanny/cached-property
     """
```

### Comparing `contrast-agent-7.6.0/src/contrast/utils/deprecated_middleware.py` & `contrast-agent-7.7.0/src/contrast/utils/deprecated_middleware.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/environ.py` & `contrast-agent-7.7.0/src/contrast/utils/environ.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py` & `contrast-agent-7.7.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/ignored_modules.py` & `contrast-agent-7.7.0/src/contrast/utils/ignored_modules.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/library_reader/library_reader.py` & `contrast-agent-7.7.0/src/contrast/utils/library_reader/library_reader.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/library_reader/patched_state.py` & `contrast-agent-7.7.0/src/contrast/utils/library_reader/patched_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,33 +14,37 @@
 from contrast_vendor import importlib_metadata
 
 from contrast_vendor import structlog as logging
 
 logger = logging.getLogger("contrast")
 
 
+class DistributionNode:
+    def __init__(self, dist):
+        self.dist = dist
+        name = dist.lower()
+        self.dist_meta = importlib_metadata.distribution(dist)
+        self.dist_hash = get_hash(name, self.dist_meta.version)
+
+
 class DistributionContext(Singleton):
     """
     This class is used to maintain state between calls to python import functions.
     The main reason why we need to do all this is because Python doesn't provide
     us with a function that maps a loaded file name
     (e.g /Users/nliccione/lib/python3.8/site-packages/django/https.py)
     to the distribution it belongs to.
     """
 
     class TopLevelDirNode:
-        def __init__(self, top_level_dir, dist):
-            name = dist.lower()
-            dist_meta = importlib_metadata.distribution(dist)
-            version = dist_meta.version
-
+        def __init__(self, top_level_dir: str, dist: DistributionNode):
             self.namespace_tlds = set()
-            self.dist_hash = get_hash(name, version)
-            self.dist = dist
-            self.full_package_path = os.path.join(dist_meta._path.parent, top_level_dir)
+            self.dist_hash = dist.dist_hash
+            self.dist = dist.dist
+            self.full_package_path = str(dist.dist_meta.locate_file(top_level_dir))
 
     def init(self):
         # dictionary containing mapping of top level directory name -> ( TopLevelDirNode, )
         self.top_level_dir_map = {}
         self.installed_dists = get_installed_dist_top_level_imports()
 
         if self.installed_dists is not None:
@@ -143,19 +147,20 @@
         exists in self.top_level_dir_map. If it does, and the file path found in sys.module matches TopLevelDirNode.full_package_path, than
         we know the imported file belongs to the distribution cached in self.top_level_dir_map.
 
         This function also handles namespace distributions. Namespace distributions share a top level import name
         (e.g zope namespace where zope.deprecation is a distribution using that namespace). As a result, we need to have an additional
         data structure to maintain the list of top level directories or file names belonging to that namespace.
         """
+        dist_node = DistributionNode(dist)
         for tld in top_level_imports:
             # The namespace dist we support is building a namespace package
             # using the pkg_resources method of defining one
             # https://packaging.python.org/guides/packaging-namespace-packages/#pkg-resources-style-namespace-packages
-            new_node = DistributionContext.TopLevelDirNode(tld, dist)
+            new_node = DistributionContext.TopLevelDirNode(tld, dist_node)
 
             namespace_dists = self.top_level_dir_map.get(tld, None)
             if namespace_dists:
                 self._add_namespace_tlds_to_node(tld, new_node)
 
                 if len(namespace_dists) == 1:
                     # Handle case where we didn't know we have a namespace dist before.
```

### Comparing `contrast-agent-7.6.0/src/contrast/utils/library_reader/utils.py` & `contrast-agent-7.7.0/src/contrast/utils/library_reader/utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/loggers/logger.py` & `contrast-agent-7.7.0/src/contrast/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/loggers/structlog.py` & `contrast-agent-7.7.0/src/contrast/utils/loggers/structlog.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/module_parser.py` & `contrast-agent-7.7.0/src/contrast/utils/module_parser.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/namespace.py` & `contrast-agent-7.7.0/src/contrast/utils/namespace.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/object_utils.py` & `contrast-agent-7.7.0/src/contrast/utils/object_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/patch_utils.py` & `contrast-agent-7.7.0/src/contrast/utils/patch_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/pattern_builder.py` & `contrast-agent-7.7.0/src/contrast/utils/pattern_builder.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/profiler.py` & `contrast-agent-7.7.0/src/contrast/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/safe_import.py` & `contrast-agent-7.7.0/src/contrast/utils/safe_import.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/singleton.py` & `contrast-agent-7.7.0/src/contrast/utils/singleton.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,10 +33,16 @@
     def clear_instance(cls):
         """
         Delete the singleton's current instance.
 
         While singletons are objects intended to have one instance only, there
         may be time when deleting the existing instance is needed.
         """
-        instance = cls.__dict__.get("__instance__")
-        if instance is not None:
+        if cls.is_initialized():
             del cls.__instance__
+
+    @classmethod
+    def is_initialized(cls) -> bool:
+        """
+        Check if the singleton has been initialized.
+        """
+        return cls.__dict__.get("__instance__") is not None
```

### Comparing `contrast-agent-7.6.0/src/contrast/utils/stack_trace_utils.py` & `contrast-agent-7.7.0/src/contrast/utils/stack_trace_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/stdlib_modules.py` & `contrast-agent-7.7.0/src/contrast/utils/stdlib_modules.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/utils/string_utils.py` & `contrast-agent-7.7.0/src/contrast/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast/wsgi/middleware.py` & `contrast-agent-7.7.0/src/contrast/wsgi/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,29 +73,34 @@
             return self.wsgi_app(environ, start_response)
 
         self.request_path = environ.get("PATH_INFO", "")
 
         # the request_id context manager must come first!
         with request_state.request_id_context(), Profiler(
             self.request_path
-        ), log_request_start_and_end(self.request_path):
+        ), log_request_start_and_end(
+            environ.get("REQUEST_METHOD", ""), self.request_path
+        ):
             context = self.should_analyze_request(environ)
             if context:
                 with contrast.CS__CONTEXT_TRACKER.lifespan(context):
                     return self.call_with_agent(context, environ, start_response)
 
             return self.call_without_agent(environ, start_response)
 
+    @scope.with_contrast_scope
     def call_with_agent(self, context, environ, start_response):
         track_environ_sources("wsgi", context, environ)
 
         try:
             self.prefilter()
 
-            response = Request(environ).get_response(self.wsgi_app)
+            webob_request = Request(environ)
+            with scope.pop_contrast_scope():
+                response = webob_request.get_response(self.wsgi_app)
 
             context.extract_response_to_context(response)
 
             self.postfilter(context)
             self.check_for_blocked(context)
             self.swap_environ_path(environ)  # should not be moved to finally
```

### Comparing `contrast-agent-7.6.0/src/contrast_agent.egg-info/SOURCES.txt` & `contrast-agent-7.7.0/src/contrast_agent.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 src/contrast/agent/patch_controller.py
 src/contrast/agent/reaction_processor.py
 src/contrast/agent/request.py
 src/contrast/agent/request_context.py
 src/contrast/agent/request_state.py
 src/contrast/agent/runner.py
 src/contrast/agent/scope.py
-src/contrast/agent/scope.pyi
 src/contrast/agent/server_settings_poll.py
 src/contrast/agent/settings.py
 src/contrast/agent/sys_monitoring.py
 src/contrast/agent/telemetry.py
 src/contrast/agent/thread_watcher.py
 src/contrast/agent/validator.py
 src/contrast/agent/agent_lib/__init__.py
@@ -556,18 +555,19 @@
 src/contrast_vendor/importlib_metadata/__init__.py
 src/contrast_vendor/importlib_metadata/_adapters.py
 src/contrast_vendor/importlib_metadata/_collections.py
 src/contrast_vendor/importlib_metadata/_compat.py
 src/contrast_vendor/importlib_metadata/_functools.py
 src/contrast_vendor/importlib_metadata/_itertools.py
 src/contrast_vendor/importlib_metadata/_meta.py
-src/contrast_vendor/importlib_metadata/_py39compat.py
 src/contrast_vendor/importlib_metadata/_text.py
 src/contrast_vendor/importlib_metadata/diagnose.py
 src/contrast_vendor/importlib_metadata/py.typed
+src/contrast_vendor/importlib_metadata/compat/__init__.py
+src/contrast_vendor/importlib_metadata/compat/py39.py
 src/contrast_vendor/isort/LICENSE
 src/contrast_vendor/isort/__init__.py
 src/contrast_vendor/isort/stdlibs/__init__.py
 src/contrast_vendor/isort/stdlibs/all.py
 src/contrast_vendor/isort/stdlibs/py2.py
 src/contrast_vendor/isort/stdlibs/py27.py
 src/contrast_vendor/isort/stdlibs/py3.py
```

### Comparing `contrast-agent-7.6.0/src/contrast_rewriter/__init__.py` & `contrast-agent-7.7.0/src/contrast_rewriter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,17 +104,17 @@
 
         if (
             spec is None
             or spec.origin is None
             or not isinstance(spec.loader, importlib.machinery.SourceFileLoader)
         ):
             rewriter_module.logger.debug(
-                "Skipping non-source module - fullname=%s, path=%s",
-                fullname,
-                getattr(spec, "origin", "<unknown>"),
+                "WARNING: Skipping non-source module",
+                module_name=fullname,
+                path=getattr(spec, "origin", "<unknown>"),
             )
             return None
 
         new_spec = importlib.util.spec_from_file_location(
             fullname,
             spec.origin,
             loader=ContrastRewriteLoader(fullname, spec.origin),
@@ -158,34 +158,33 @@
             return
 
         try:
             original_source_code = self.get_source(self.name)
             tree = ast.parse(original_source_code)
         except Exception as ex:
             rewriter_module.logger.debug(
-                "WARNING: failed to rewrite %s", filename, exc_info=ex
+                "WARNING: failed to rewrite module", filename=filename, exc_info=ex
             )
 
             _load_module(original_source_code, module, filename)
 
             return
 
         if _CONTRAST_OPERATOR_NAME not in module.__dict__:
             try:
                 populate_operator_module(module.__dict__)
                 PropagationRewriter().visit(tree)
-                ast.fix_missing_locations(tree)
             except Exception as ex:
                 rewriter_module.logger.debug(
-                    "WARNING: failed to rewrite %s", filename, exc_info=ex
+                    "WARNING: failed to rewrite module", filename=filename, exc_info=ex
                 )
         else:
             rewriter_module.logger.debug(
-                "WARNING: module %s appears to have been already rewritten; will not rewrite again",
-                filename,
+                "WARNING: module appears to have been already rewritten; will not rewrite again",
+                filename=filename,
             )
 
         rewriter_module.registry.add(self.name)
 
         _load_module(tree, module, filename)
 
 
@@ -212,28 +211,27 @@
 
         if isinstance(binop.op, ast.Mod):
             binop_replacement = ast.Call(
                 func=self._make_attr(operator.mod),
                 args=[binop.left, binop.right],
                 keywords=[],
             )
-
             ast.copy_location(binop_replacement, binop)
-            return binop_replacement
+            return ast.fix_missing_locations(binop_replacement)
 
         if not isinstance(binop.op, ast.Add):
             return binop
 
         binop_replacement = ast.Call(
             func=self._make_attr(operator.add),
             args=[binop.left, binop.right],
             keywords=[],
         )
         ast.copy_location(binop_replacement, binop)
-        return binop_replacement
+        return ast.fix_missing_locations(binop_replacement)
 
     def visit_AugAssign(self, node: ast.AugAssign):
         """
         If we see an "Append", `+=` operation, rewrite it as a `+`.
         """
         node.value = self.visit(node.value)
 
@@ -253,26 +251,26 @@
             targets=[target],
             value=ast.Call(
                 func=self._make_attr(operator.iadd),
                 args=[self.visit(left), node.value],
                 keywords=[],
             ),
         )
-
         ast.copy_location(call_contrast_append_node, node)
-        # Recurse here in order to properly rewrite the `+` operation
-        return call_contrast_append_node
+        return ast.fix_missing_locations(call_contrast_append_node)
 
     def visit_JoinedStr(self, node: ast.JoinedStr):
         node.values = [self.visit(value) for value in node.values]
-        return ast.Call(
+        call_node = ast.Call(
             func=ast.Attribute(value=ast.Constant(""), attr="join", ctx=ast.Load()),
             args=[ast.List(elts=node.values, ctx=ast.Load())],
             keywords=[],
         )
+        ast.copy_location(call_node, node)
+        return ast.fix_missing_locations(call_node)
 
 
 def _non_contrast_module_filter(module_item) -> bool:
     return not _is_contrast_module_name(
         getattr(module_item[1], "__package__", "") or ""
     )
 
@@ -312,15 +310,14 @@
 def _hook_assertion_rewrites(rewrite_module):
     from contrast_vendor.wrapt import function_wrapper
 
     # This hook enables us to apply our rewriter before assertion rewrites are applied
     def rewrite_asserts(wrapped, _, args, kwargs):
         mod = args[0]
         PropagationRewriter().visit(mod)
-        ast.fix_missing_locations(mod)
         wrapped(*args, **kwargs)
 
     # This hook ensures that we add our contrast-specfic functions to the rewritten module
     def exec_module(wrapped, _, args, kwargs):
         module = args[0]
         populate_operator_module(module.__dict__)
         wrapped(*args, **kwargs)
```

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/__init__.py` & `contrast-agent-7.7.0/src/contrast_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/LICENSE` & `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/__init__.py` & `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import os
 import re
 import abc
-import csv
 import sys
 import json
 from contrast_vendor import zipp
 import email
 import types
 import inspect
 import pathlib
@@ -15,15 +14,16 @@
 import textwrap
 import warnings
 import functools
 import itertools
 import posixpath
 import collections
 
-from . import _adapters, _meta, _py39compat
+from . import _adapters, _meta
+from .compat import py39
 from ._collections import FreezableDefaultDict, Pair
 from ._compat import (
     NullFinder,
     install,
 )
 from ._functools import method_cache, pass_none
 from ._itertools import always_iterable, unique_everseen
@@ -276,15 +276,15 @@
         return '%s(%r)' % (self.__class__.__name__, tuple(self))
 
     def select(self, **params) -> EntryPoints:
         """
         Select entry points from self that match the
         given parameters (typically group and/or name).
         """
-        return EntryPoints(ep for ep in self if _py39compat.ep_matches(ep, **params))
+        return EntryPoints(ep for ep in self if py39.ep_matches(ep, **params))
 
     @property
     def names(self) -> Set[str]:
         """
         Return the set of all names of all entry points.
         """
         return {ep.name for ep in self}
@@ -518,14 +518,18 @@
             result.hash = FileHash(hash) if hash else None
             result.size = int(size_str) if size_str else None
             result.dist = self
             return result
 
         @pass_none
         def make_files(lines):
+            # Delay csv import, since Distribution.files is not as widely used
+            # as other parts of importlib.metadata
+            import csv
+
             return starmap(make_file, csv.reader(lines))
 
         @pass_none
         def skip_missing_files(package_paths):
             return list(filter(lambda path: path.locate().exists(), package_paths))
 
         return skip_missing_files(
@@ -869,36 +873,38 @@
 class MetadataPathFinder(NullFinder, DistributionFinder):
     """A degenerate finder for distribution packages on the file system.
 
     This finder supplies only a find_distributions() method for versions
     of Python that do not have a PathFinder find_distributions().
     """
 
+    @classmethod
     def find_distributions(
-        self, context=DistributionFinder.Context()
+        cls, context=DistributionFinder.Context()
     ) -> Iterable[PathDistribution]:
         """
         Find distributions.
 
         Return an iterable of all Distribution instances capable of
         loading the metadata for packages matching ``context.name``
         (or all names if ``None`` indicated) along the paths in the list
         of directories ``context.path``.
         """
-        found = self._search_paths(context.name, context.path)
+        found = cls._search_paths(context.name, context.path)
         return map(PathDistribution, found)
 
     @classmethod
     def _search_paths(cls, name, paths):
         """Find metadata directories in paths heuristically."""
         prepared = Prepared(name)
         return itertools.chain.from_iterable(
             path.search(prepared) for path in map(FastPath, paths)
         )
 
+    @classmethod
     def invalidate_caches(cls) -> None:
         FastPath.__new__.cache_clear()
 
 
 class PathDistribution(Distribution):
     def __init__(self, path: SimplePath) -> None:
         """Construct a distribution.
@@ -988,15 +994,15 @@
         "Version" metadata key.
     """
     return distribution(distribution_name).version
 
 
 _unique = functools.partial(
     unique_everseen,
-    key=_py39compat.normalized_name,
+    key=py39.normalized_name,
 )
 """
 Wrapper for ``distributions`` to return unique distributions by name.
 """
 
 
 def entry_points(**params) -> EntryPoints:
```

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_adapters.py` & `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_collections.py` & `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_compat.py` & `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_functools.py` & `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_itertools.py` & `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_meta.py` & `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_py39compat.py` & `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/compat/py39.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 Compatibility layer with Python 3.8/3.9
 """
 
 from typing import TYPE_CHECKING, Any, Optional
 
 if TYPE_CHECKING:  # pragma: no cover
     # Prevent circular imports on runtime.
-    from . import Distribution, EntryPoint
+    from .. import Distribution, EntryPoint
 else:
     Distribution = EntryPoint = Any
 
 
 def normalized_name(dist: Distribution) -> Optional[str]:
     """
     Honor name normalization for distributions that don't provide ``_normalized_name``.
     """
     try:
         return dist._normalized_name
     except AttributeError:
-        from . import Prepared  # -> delay to prevent circular imports.
+        from .. import Prepared  # -> delay to prevent circular imports.
 
         return Prepared.normalize(getattr(dist, "name", None) or dist.metadata['Name'])
 
 
 def ep_matches(ep: EntryPoint, **params) -> bool:
     """
     Workaround for ``EntryPoint`` objects without the ``matches`` method.
     """
     try:
         return ep.matches(**params)
     except AttributeError:
-        from . import EntryPoint  # -> delay to prevent circular imports.
+        from .. import EntryPoint  # -> delay to prevent circular imports.
 
         # Reconstruct the EntryPoint object to make sure it is compatible.
         return EntryPoint(ep.name, ep.value, ep.group).matches(**params)
```

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/importlib_metadata/_text.py` & `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/isort/LICENSE` & `contrast-agent-7.7.0/src/contrast_vendor/isort/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py27.py` & `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py27.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py310.py` & `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py310.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py311.py` & `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py311.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py312.py` & `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py312.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py36.py` & `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py36.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py37.py` & `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py37.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py38.py` & `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py38.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/isort/stdlibs/py39.py` & `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py39.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE` & `contrast-agent-7.7.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ported_cpython_code/import_functionality.py` & `contrast-agent-7.7.0/src/contrast_vendor/ported_cpython_code/import_functionality.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/LICENSE` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/__init__.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/comments.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/comments.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/compat.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/compat.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/composer.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/constructor.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/cyaml.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/dumper.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/emitter.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/error.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/error.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/events.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/events.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/loader.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/main.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/main.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/nodes.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/parser.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/reader.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/representer.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/resolver.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/scalarbool.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarbool.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/scalarint.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarint.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/scalarstring.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarstring.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/scanner.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/serializer.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/tag.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/tag.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/timestamp.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/timestamp.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/tokens.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/ruamel/yaml/util.py` & `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/util.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/LICENSE-APACHE` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/LICENSE-MIT` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/__init__.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/_base.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/_base.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/_config.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/_config.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/_frames.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/_frames.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/_generic.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/_generic.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/_greenlets.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/_greenlets.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/_log_levels.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/_log_levels.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/_native.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/_native.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/_output.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/_output.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/_utils.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/contextvars.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/contextvars.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/dev.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/dev.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/processors.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/stdlib.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/stdlib.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/testing.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/testing.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/threadlocal.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/threadlocal.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/tracebacks.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/tracebacks.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/twisted.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/twisted.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/types.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/types.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/structlog/typing.py` & `contrast-agent-7.7.0/src/contrast_vendor/structlog/typing.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/__init__.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/acceptparse.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/acceptparse.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/byterange.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/byterange.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/cachecontrol.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/cachecontrol.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/client.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/client.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/compat.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,31 +19,31 @@
     integer_types = (int, long)
     class_types = (type, types.ClassType)
     text_type = unicode
     long = long
 
 # TODO check if errors is ever used
 
-def text_(s, encoding='latin-1', errors='strict'):
+def text_(s, encoding='latin-1', errors='replace'):
     if isinstance(s, bytes):
         return s.decode(encoding, errors)
     return s
 
-def bytes_(s, encoding='latin-1', errors='strict'):
+def bytes_(s, encoding='latin-1', errors='replace'):
     if isinstance(s, text_type):
         return s.encode(encoding, errors)
     return s
 
 if PY3:
-    def native_(s, encoding='latin-1', errors='strict'):
+    def native_(s, encoding='latin-1', errors='replace'):
         if isinstance(s, text_type):
             return s
         return str(s, encoding, errors)
 else:
-    def native_(s, encoding='latin-1', errors='strict'):
+    def native_(s, encoding='latin-1', errors='replace'):
         if isinstance(s, text_type):
             return s.encode(encoding, errors)
         return str(s)
 
 try:
     from queue import Queue, Empty
 except ImportError:
```

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/cookies.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/cookies.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/datetime_utils.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/dec.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/dec.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/descriptors.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/descriptors.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/etag.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/etag.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/exc.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/exc.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/headers.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/headers.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/license.txt` & `contrast-agent-7.7.0/src/contrast_vendor/webob/license.txt`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/multidict.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/multidict.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/request.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         encoding = getattr(self, encattr)
 
         if PY2:
             return val.decode(encoding)
 
         if encoding in _LATIN_ENCODINGS: # shortcut
             return val
-        return bytes_(val, 'latin-1').decode(encoding)
+        return bytes_(val, 'latin-1').decode(encoding, errors='replace')
 
     def encset(self, key, val, encattr=None):
         if encattr:
             encoding = getattr(self, encattr)
         else:
             encoding = 'ascii'
         if PY2: # pragma: no cover
```

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/response.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/response.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/static.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/static.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/webob/util.py` & `contrast-agent-7.7.0/src/contrast_vendor/webob/util.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/wrapt/LICENSE` & `contrast-agent-7.7.0/src/contrast_vendor/wrapt/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/wrapt/__init__.py` & `contrast-agent-7.7.0/src/contrast_vendor/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/wrapt/arguments.py` & `contrast-agent-7.7.0/src/contrast_vendor/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/wrapt/decorators.py` & `contrast-agent-7.7.0/src/contrast_vendor/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/wrapt/importer.py` & `contrast-agent-7.7.0/src/contrast_vendor/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/wrapt/patches.py` & `contrast-agent-7.7.0/src/contrast_vendor/wrapt/patches.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/wrapt/weakrefs.py` & `contrast-agent-7.7.0/src/contrast_vendor/wrapt/weakrefs.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/wrapt/wrappers.py` & `contrast-agent-7.7.0/src/contrast_vendor/wrapt/wrappers.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/zipp/LICENSE` & `contrast-agent-7.7.0/src/contrast_vendor/zipp/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/zipp/__init__.py` & `contrast-agent-7.7.0/src/contrast_vendor/zipp/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.6.0/src/contrast_vendor/zipp/glob.py` & `contrast-agent-7.7.0/src/contrast_vendor/zipp/glob.py`

 * *Files identical despite different names*

