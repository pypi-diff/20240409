# Comparing `tmp/bodhi_server-8.0.2.tar.gz` & `tmp/bodhi_server-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodhi_server-8.0.2.tar", max compression
+gzip compressed data, was "bodhi_server-8.1.0.tar", max compression
```

## Comparing `bodhi_server-8.0.2.tar` & `bodhi_server-8.1.0.tar`

### file list

```diff
@@ -1,337 +1,337 @@
--rw-r--r--   0        0        0    18018 2023-05-13 08:55:56.420718 bodhi_server-8.0.2/COPYING
--rw-r--r--   0        0        0     1655 2023-05-13 08:55:56.420718 bodhi_server-8.0.2/README.rst
--rw-r--r--   0        0        0     1258 2023-07-30 09:10:09.778541 bodhi_server-8.0.2/alembic.ini
--rw-r--r--   0        0        0      580 2023-05-13 08:55:56.420718 bodhi_server-8.0.2/apache/bodhi.conf
--rw-r--r--   0        0        0      260 2023-05-13 08:55:56.420718 bodhi_server-8.0.2/apache/bodhi.wsgi
--rw-r--r--   0        0        0    12197 2024-01-11 15:54:23.986056 bodhi_server-8.0.2/bodhi/server/__init__.py
--rw-r--r--   0        0        0     1552 2023-05-13 08:55:56.420718 bodhi_server-8.0.2/bodhi/server/auth/__init__.py
--rw-r--r--   0        0        0      220 2023-05-13 08:55:56.420718 bodhi_server-8.0.2/bodhi/server/auth/constants.py
--rw-r--r--   0        0        0     5960 2023-05-13 08:55:56.420718 bodhi_server-8.0.2/bodhi/server/auth/fedora.py
--rw-r--r--   0        0        0     2604 2023-05-13 08:55:56.421718 bodhi_server-8.0.2/bodhi/server/auth/oauth.py
--rw-r--r--   0        0        0     2794 2023-05-13 08:55:56.421718 bodhi_server-8.0.2/bodhi/server/auth/oauth_015.py
--rw-r--r--   0        0        0     3597 2023-05-13 08:55:56.421718 bodhi_server-8.0.2/bodhi/server/auth/oauth_1.py
--rw-r--r--   0        0        0     5965 2023-05-13 08:55:56.421718 bodhi_server-8.0.2/bodhi/server/auth/utils.py
--rw-r--r--   0        0        0     3960 2023-05-13 08:55:56.421718 bodhi_server-8.0.2/bodhi/server/auth/views.py
--rw-r--r--   0        0        0    12401 2023-05-13 08:55:56.421718 bodhi_server-8.0.2/bodhi/server/bugs.py
--rw-r--r--   0        0        0    30472 2023-12-05 13:18:07.849647 bodhi_server-8.0.2/bodhi/server/buildsys.py
--rw-r--r--   0        0        0    25822 2023-12-05 13:18:07.849647 bodhi_server-8.0.2/bodhi/server/config.py
--rw-r--r--   0        0        0     3616 2023-05-13 08:55:56.423718 bodhi_server-8.0.2/bodhi/server/consumers/__init__.py
--rw-r--r--   0        0        0     8807 2023-05-13 08:55:56.424718 bodhi_server-8.0.2/bodhi/server/consumers/automatic_updates.py
--rw-r--r--   0        0        0     4009 2023-05-13 08:55:56.424718 bodhi_server-8.0.2/bodhi/server/consumers/ci.py
--rw-r--r--   0        0        0     2863 2023-07-30 15:01:32.019770 bodhi_server-8.0.2/bodhi/server/consumers/resultsdb.py
--rw-r--r--   0        0        0     5651 2023-05-14 16:00:16.124253 bodhi_server-8.0.2/bodhi/server/consumers/signed.py
--rw-r--r--   0        0        0     2728 2023-05-13 08:55:56.424718 bodhi_server-8.0.2/bodhi/server/consumers/util.py
--rw-r--r--   0        0        0     2569 2023-07-30 15:01:32.019770 bodhi_server-8.0.2/bodhi/server/consumers/waiverdb.py
--rw-r--r--   0        0        0     1040 2023-05-13 08:55:56.425718 bodhi_server-8.0.2/bodhi/server/email/templates/fedora_epel_errata_template.tpl
--rw-r--r--   0        0        0     1070 2023-05-13 08:55:56.425718 bodhi_server-8.0.2/bodhi/server/email/templates/fedora_epel_legacy_errata_template.tpl
--rw-r--r--   0        0        0     1051 2023-05-13 08:55:56.425718 bodhi_server-8.0.2/bodhi/server/email/templates/fedora_errata_template.tpl
--rw-r--r--   0        0        0     1059 2023-05-13 08:55:56.425718 bodhi_server-8.0.2/bodhi/server/email/templates/fedora_modular_errata_template.tpl
--rw-r--r--   0        0        0      261 2023-05-13 08:55:56.425718 bodhi_server-8.0.2/bodhi/server/email/templates/maillist_template.tpl
--rw-r--r--   0        0        0     1249 2023-05-13 08:55:56.425718 bodhi_server-8.0.2/bodhi/server/exceptions.py
--rw-r--r--   0        0        0     7154 2023-05-13 08:55:56.425718 bodhi_server-8.0.2/bodhi/server/ffmarkdown.py
--rw-r--r--   0        0        0        0 2023-05-13 08:55:56.425718 bodhi_server-8.0.2/bodhi/server/locale/.placeholder
--rw-r--r--   0        0        0     3641 2023-05-13 08:55:56.425718 bodhi_server-8.0.2/bodhi/server/logging.py
--rw-r--r--   0        0        0    14685 2023-12-05 13:18:07.849647 bodhi_server-8.0.2/bodhi/server/mail.py
--rw-r--r--   0        0        0    12411 2023-12-05 13:18:07.849647 bodhi_server-8.0.2/bodhi/server/metadata.py
--rw-r--r--   0        0        0      706 2023-05-13 08:55:56.425718 bodhi_server-8.0.2/bodhi/server/migrations/README.rst
--rw-r--r--   0        0        0      845 2023-05-13 08:55:56.425718 bodhi_server-8.0.2/bodhi/server/migrations/__init__.py
--rw-r--r--   0        0        0     3018 2023-10-03 14:39:17.931214 bodhi_server-8.0.2/bodhi/server/migrations/env.py
--rw-r--r--   0        0        0     1181 2023-05-13 08:55:56.425718 bodhi_server-8.0.2/bodhi/server/migrations/script.py.mako
--rw-r--r--   0        0        0     1568 2023-12-05 13:18:07.850647 bodhi_server-8.0.2/bodhi/server/migrations/versions/16864f8ff395_remove_requirements_column_from_build_.py
--rw-r--r--   0        0        0     2918 2023-05-13 08:55:56.425718 bodhi_server-8.0.2/bodhi/server/migrations/versions/190ba571c7d2_remove_the_batching_request_state.py
--rw-r--r--   0        0        0     1333 2023-05-13 08:55:56.425718 bodhi_server-8.0.2/bodhi/server/migrations/versions/19e28e9851a2_index_comment_update_id.py
--rw-r--r--   0        0        0     1380 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/1c97477e38ee_convert_br_override_notes_to_unicodetext.py
--rw-r--r--   0        0        0     1443 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/2fc96aa44a74_drop_the_user_show_popup_column.py
--rw-r--r--   0        0        0     3846 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/325954bac9f7_link_testcases_to_builds.py
--rw-r--r--   0        0        0     2732 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/3a2e248d1757_add_the_unspecified_enum_to_updatetype.py
--rw-r--r--   0        0        0     1530 2023-12-05 13:18:07.850647 bodhi_server-8.0.2/bodhi/server/migrations/versions/3b34650a0cf6_update_type_of_users_email_with_new_.py
--rw-r--r--   0        0        0     3041 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/499ac8bbe09a_remove_unused_update_sidetag_statuses.py
--rw-r--r--   0        0        0     1822 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/559acf7e2c16_make_comments_update_not_nullable.py
--rw-r--r--   0        0        0     2279 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/5703ddfe855d_add_package_manager_and_testing_.py
--rw-r--r--   0        0        0     2187 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/58b7919b942c_remove_the_updates_title_column.py
--rw-r--r--   0        0        0     2586 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/5c86a3f9dc03_drop_support_for_cve_tracking.py
--rw-r--r--   0        0        0     2708 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/6b3eb9ae2b87_remove_unused_updatestatus_processing.py
--rw-r--r--   0        0        0     1741 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/7ba286412ad4_drop_the_relationship_between_packages_.py
--rw-r--r--   0        0        0     2812 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/8c4d6aad9b78_add_the_greenwave_failed_enum_to_.py
--rw-r--r--   0        0        0     1503 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/8e9dc57e082d_obsolete_updates_for_archived_release.py
--rw-r--r--   0        0        0     1368 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/9991cf10ec50_mark_the_bugs_private_field_as_nullable.py
--rw-r--r--   0        0        0     1501 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/9c0a34961768_remove_the_greenwave_unsatisfied_.py
--rw-r--r--   0        0        0      843 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/__init__.py
--rw-r--r--   0        0        0     1321 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/a3580bdf5129_remove_the_ci_url_field_from_builds.py
--rw-r--r--   0        0        0     2991 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/a418acf470f8_drop_the_stacks_table.py
--rw-r--r--   0        0        0     1346 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/aae0d29d49b7_remove_the_private_field_on_the_bug_.py
--rw-r--r--   0        0        0     1808 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/b1fd856efcf6_add_autopush_boolean_and_stable_days_to_update.py
--rw-r--r--   0        0        0     2341 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/bdf0e37ab793_disallow_null_values_in_stable_karma_.py
--rw-r--r--   0        0        0     2593 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/c60d95eef4f1_add_frozen_release_state.py
--rw-r--r--   0        0        0     2316 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/c98beb4940b5_remove_the_comments_anonymous_column.py
--rw-r--r--   0        0        0     1296 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/d399493275b6_add_the_eol_column.py
--rw-r--r--   0        0        0     1329 2023-05-13 08:55:56.426718 bodhi_server-8.0.2/bodhi/server/migrations/versions/d3f8bd499ecd_add_from_tag_column_to_updates.py
--rw-r--r--   0        0        0     1405 2023-12-05 13:18:07.850647 bodhi_server-8.0.2/bodhi/server/migrations/versions/d986618207bc_add_composed_by_bodhi_flag_to_releases_.py
--rw-r--r--   0        0        0     1670 2023-05-13 08:55:56.427718 bodhi_server-8.0.2/bodhi/server/migrations/versions/e3988e00b338_drop_date_pushed.py
--rw-r--r--   0        0        0     1421 2023-05-13 08:55:56.427718 bodhi_server-8.0.2/bodhi/server/migrations/versions/e5b3ddb35df3_remove_the_greenwave_summary_string_.py
--rw-r--r--   0        0        0     1403 2023-05-13 08:55:56.427718 bodhi_server-8.0.2/bodhi/server/migrations/versions/e8a059156d38_add_the_create_automatic_updates_bool_.py
--rw-r--r--   0        0        0     1312 2023-05-13 08:55:56.427718 bodhi_server-8.0.2/bodhi/server/migrations/versions/eec610d7ab3a_index_the_builds_update_id_column.py
--rw-r--r--   0        0        0     1345 2023-05-13 08:55:56.427718 bodhi_server-8.0.2/bodhi/server/migrations/versions/f393d006559b_add_critpath_groups_to_update.py
--rw-r--r--   0        0        0     1469 2023-05-13 08:55:56.427718 bodhi_server-8.0.2/bodhi/server/migrations/versions/f50dc199039c_make_comments_user_id_not_nullable.py
--rw-r--r--   0        0        0     1308 2023-12-05 13:18:07.850647 bodhi_server-8.0.2/bodhi/server/migrations/versions/f660455231d4_add_released_on_to_release.py
--rw-r--r--   0        0        0     1353 2023-05-13 08:55:56.427718 bodhi_server-8.0.2/bodhi/server/migrations/versions/f8a44498c806_remove_legacy_old_updateid.py
--rw-r--r--   0        0        0     1347 2023-05-13 08:55:56.427718 bodhi_server-8.0.2/bodhi/server/migrations/versions/ff834fa4f23e_increase_the_update_alias_size.py
--rw-r--r--   0        0        0   196804 2023-12-09 14:25:00.563911 bodhi_server-8.0.2/bodhi/server/models.py
--rw-r--r--   0        0        0     3016 2023-05-13 08:55:56.428718 bodhi_server-8.0.2/bodhi/server/notifications.py
--rw-r--r--   0        0        0    11988 2023-07-30 15:01:32.084769 bodhi_server-8.0.2/bodhi/server/push.py
--rw-r--r--   0        0        0     7143 2023-05-13 08:55:56.428718 bodhi_server-8.0.2/bodhi/server/renderers.py
--rw-r--r--   0        0        0    22577 2023-12-05 13:18:07.851647 bodhi_server-8.0.2/bodhi/server/schemas.py
--rw-r--r--   0        0        0      849 2023-05-13 08:55:56.429718 bodhi_server-8.0.2/bodhi/server/scripts/__init__.py
--rw-r--r--   0        0        0     1397 2023-05-13 08:55:56.429718 bodhi_server-8.0.2/bodhi/server/scripts/bshell.py
--rw-r--r--   0        0        0     3871 2023-05-13 08:55:56.429718 bodhi_server-8.0.2/bodhi/server/scripts/compat.py
--rw-r--r--   0        0        0     1847 2023-05-21 12:57:14.742024 bodhi_server-8.0.2/bodhi/server/scripts/initializedb.py
--rw-r--r--   0        0        0     4206 2023-12-05 13:18:07.851647 bodhi_server-8.0.2/bodhi/server/scripts/sar.py
--rw-r--r--   0        0        0     3839 2023-12-09 14:25:00.566911 bodhi_server-8.0.2/bodhi/server/scripts/untag_branched.py
--rw-r--r--   0        0        0     9576 2024-01-09 15:35:23.203917 bodhi_server-8.0.2/bodhi/server/security.py
--rw-r--r--   0        0        0      815 2023-05-13 08:55:56.429718 bodhi_server-8.0.2/bodhi/server/services/__init__.py
--rw-r--r--   0        0        0     5246 2023-10-03 14:39:17.933214 bodhi_server-8.0.2/bodhi/server/services/builds.py
--rw-r--r--   0        0        0     8705 2023-10-03 14:39:17.933214 bodhi_server-8.0.2/bodhi/server/services/comments.py
--rw-r--r--   0        0        0     3936 2023-05-13 08:55:56.430718 bodhi_server-8.0.2/bodhi/server/services/composes.py
--rw-r--r--   0        0        0     2058 2023-05-13 08:55:56.430718 bodhi_server-8.0.2/bodhi/server/services/csrf.py
--rw-r--r--   0        0        0     3793 2023-05-13 08:55:56.430718 bodhi_server-8.0.2/bodhi/server/services/errors.py
--rw-r--r--   0        0        0     1969 2023-05-13 08:55:56.430718 bodhi_server-8.0.2/bodhi/server/services/markdown.py
--rw-r--r--   0        0        0     1916 2023-05-13 08:55:56.430718 bodhi_server-8.0.2/bodhi/server/services/metrics_tween.py
--rw-r--r--   0        0        0    13051 2023-10-03 14:39:17.933214 bodhi_server-8.0.2/bodhi/server/services/overrides.py
--rw-r--r--   0        0        0     3786 2023-10-03 14:39:17.933214 bodhi_server-8.0.2/bodhi/server/services/packages.py
--rw-r--r--   0        0        0    16838 2023-12-05 13:18:07.851647 bodhi_server-8.0.2/bodhi/server/services/releases.py
--rw-r--r--   0        0        0     3481 2023-05-13 08:55:56.430718 bodhi_server-8.0.2/bodhi/server/services/schemas.py
--rw-r--r--   0        0        0    29245 2023-12-05 13:18:07.851647 bodhi_server-8.0.2/bodhi/server/services/updates.py
--rw-r--r--   0        0        0     6676 2023-10-03 14:39:17.934214 bodhi_server-8.0.2/bodhi/server/services/user.py
--rw-r--r--   0        0        0      832 2023-05-13 08:55:56.431718 bodhi_server-8.0.2/bodhi/server/static/__init__.py
--rw-r--r--   0        0        0    10425 2023-05-13 08:55:56.431718 bodhi_server-8.0.2/bodhi/server/static/bodhi-logo.svg
--rw-r--r--   0        0        0     6423 2023-05-13 08:55:56.431718 bodhi_server-8.0.2/bodhi/server/static/css/site.css
--rw-r--r--   0        0        0   124988 2023-05-13 08:55:56.432718 bodhi_server-8.0.2/bodhi/server/static/fonts/font-awesome/FontAwesome.otf
--rw-r--r--   0        0        0    76518 2023-05-13 08:55:56.432718 bodhi_server-8.0.2/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.eot
--rw-r--r--   0        0        0   391622 2023-05-13 08:55:56.433718 bodhi_server-8.0.2/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.svg
--rw-r--r--   0        0        0   152796 2023-05-13 08:55:56.434718 bodhi_server-8.0.2/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    90412 2023-05-13 08:55:56.434718 bodhi_server-8.0.2/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff
--rw-r--r--   0        0        0    71896 2023-05-13 08:55:56.434718 bodhi_server-8.0.2/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff2
--rw-r--r--   0        0        0    35152 2023-05-13 08:55:56.431718 bodhi_server-8.0.2/bodhi/server/static/fonts/font-awesome.css
--rwxr-xr-x   0        0        0   139140 2023-05-13 08:55:56.434718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/hack-bold-webfont.eot
--rwxr-xr-x   0        0        0   146800 2023-05-13 08:55:56.434718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/hack-bolditalic-webfont.eot
--rwxr-xr-x   0        0        0   143488 2023-05-13 08:55:56.434718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/hack-italic-webfont.eot
--rwxr-xr-x   0        0        0   137266 2023-05-13 08:55:56.435718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/hack-regular-webfont.eot
--rwxr-xr-x   0        0        0    28782 2023-05-13 08:55:56.435718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/latin/hack-bold-latin-webfont.eot
--rwxr-xr-x   0        0        0    31454 2023-05-13 08:55:56.435718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/latin/hack-bolditalic-latin-webfont.eot
--rwxr-xr-x   0        0        0    30512 2023-05-13 08:55:56.435718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/latin/hack-italic-latin-webfont.eot
--rwxr-xr-x   0        0        0    28527 2023-05-13 08:55:56.435718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/latin/hack-regular-latin-webfont.eot
--rwxr-xr-x   0        0        0   389828 2023-05-13 08:55:56.436718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/hack-bold-webfont.ttf
--rwxr-xr-x   0        0        0   398888 2023-05-13 08:55:56.438718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/hack-bolditalic-webfont.ttf
--rwxr-xr-x   0        0        0   393880 2023-05-13 08:55:56.439718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/hack-italic-webfont.ttf
--rwxr-xr-x   0        0        0   387660 2023-05-13 08:55:56.440718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/hack-regular-webfont.ttf
--rwxr-xr-x   0        0        0    73056 2023-05-13 08:55:56.440718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bold-latin-webfont.ttf
--rwxr-xr-x   0        0        0    77808 2023-05-13 08:55:56.441718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bolditalic-latin-webfont.ttf
--rwxr-xr-x   0        0        0    76444 2023-05-13 08:55:56.441718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/latin/hack-italic-latin-webfont.ttf
--rwxr-xr-x   0        0        0    73256 2023-05-13 08:55:56.442718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/latin/hack-regular-latin-webfont.ttf
--rwxr-xr-x   0        0        0   171820 2023-05-13 08:55:56.442718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/hack-bold-webfont.woff
--rwxr-xr-x   0        0        0   180204 2023-05-13 08:55:56.442718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/hack-bolditalic-webfont.woff
--rwxr-xr-x   0        0        0   176864 2023-05-13 08:55:56.443718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/hack-italic-webfont.woff
--rwxr-xr-x   0        0        0   168376 2023-05-13 08:55:56.443718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/hack-regular-webfont.woff
--rwxr-xr-x   0        0        0    31964 2023-05-13 08:55:56.443718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/latin/hack-bold-latin-webfont.woff
--rwxr-xr-x   0        0        0    34720 2023-05-13 08:55:56.443718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/latin/hack-bolditalic-latin-webfont.woff
--rwxr-xr-x   0        0        0    33556 2023-05-13 08:55:56.443718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/latin/hack-italic-latin-webfont.woff
--rwxr-xr-x   0        0        0    31584 2023-05-13 08:55:56.443718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/latin/hack-regular-latin-webfont.woff
--rwxr-xr-x   0        0        0   124552 2023-05-13 08:55:56.443718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/hack-bold-webfont.woff2
--rwxr-xr-x   0        0        0   131588 2023-05-13 08:55:56.444718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/hack-bolditalic-webfont.woff2
--rwxr-xr-x   0        0        0   128624 2023-05-13 08:55:56.444718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/hack-italic-webfont.woff2
--rwxr-xr-x   0        0        0   122888 2023-05-13 08:55:56.444718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/hack-regular-webfont.woff2
--rwxr-xr-x   0        0        0    25884 2023-05-13 08:55:56.444718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/latin/hack-bold-latin-webfont.woff2
--rwxr-xr-x   0        0        0    28232 2023-05-13 08:55:56.444718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/latin/hack-bolditalic-latin-webfont.woff2
--rwxr-xr-x   0        0        0    27576 2023-05-13 08:55:56.444718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/latin/hack-italic-latin-webfont.woff2
--rwxr-xr-x   0        0        0    25696 2023-05-13 08:55:56.444718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/latin/hack-regular-latin-webfont.woff2
--rw-r--r--   0        0        0     1947 2023-05-13 08:55:56.434718 bodhi_server-8.0.2/bodhi/server/static/fonts/hack.css
--rw-r--r--   0        0        0    31896 2023-05-13 08:55:56.444718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.eot
--rw-r--r--   0        0        0   254253 2023-05-13 08:55:56.445718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.svg
--rw-r--r--   0        0        0    68444 2023-05-13 08:55:56.445718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.ttf
--rw-r--r--   0        0        0    33704 2023-05-13 08:55:56.445718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff
--rw-r--r--   0        0        0    23816 2023-05-13 08:55:56.445718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff2
--rw-r--r--   0        0        0    30763 2023-05-13 08:55:56.445718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.eot
--rw-r--r--   0        0        0   258568 2023-05-13 08:55:56.446718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.svg
--rw-r--r--   0        0        0    64668 2023-05-13 08:55:56.446718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.ttf
--rw-r--r--   0        0        0    32300 2023-05-13 08:55:56.446718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff
--rw-r--r--   0        0        0    22220 2023-05-13 08:55:56.446718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff2
--rw-r--r--   0        0        0    32088 2023-05-13 08:55:56.446718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.eot
--rw-r--r--   0        0        0   254724 2023-05-13 08:55:56.446718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.svg
--rw-r--r--   0        0        0    68776 2023-05-13 08:55:56.447718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.ttf
--rw-r--r--   0        0        0    33876 2023-05-13 08:55:56.447718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff
--rw-r--r--   0        0        0    23652 2023-05-13 08:55:56.447718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff2
--rw-r--r--   0        0        0    30546 2023-05-13 08:55:56.447718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.eot
--rw-r--r--   0        0        0   257617 2023-05-13 08:55:56.447718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.svg
--rw-r--r--   0        0        0    65236 2023-05-13 08:55:56.447718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.ttf
--rw-r--r--   0        0        0    32180 2023-05-13 08:55:56.448718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff
--rw-r--r--   0        0        0    22176 2023-05-13 08:55:56.448718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff2
--rw-r--r--   0        0        0    30880 2023-05-13 08:55:56.448718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.eot
--rw-r--r--   0        0        0   258434 2023-05-13 08:55:56.448718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.svg
--rw-r--r--   0        0        0    65072 2023-05-13 08:55:56.448718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.ttf
--rw-r--r--   0        0        0    32212 2023-05-13 08:55:56.448718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff
--rw-r--r--   0        0        0    22196 2023-05-13 08:55:56.448718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff2
--rw-r--r--   0        0        0    31491 2023-05-13 08:55:56.448718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.eot
--rw-r--r--   0        0        0   255338 2023-05-13 08:55:56.448718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.svg
--rw-r--r--   0        0        0    66740 2023-05-13 08:55:56.448718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.ttf
--rw-r--r--   0        0        0    33060 2023-05-13 08:55:56.448718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff
--rw-r--r--   0        0        0    23048 2023-05-13 08:55:56.449718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff2
--rw-r--r--   0        0        0     4956 2023-05-13 08:55:56.444718 bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans.css
--rw-r--r--   0        0        0     4255 2023-05-13 08:55:56.449718 bodhi_server-8.0.2/bodhi/server/static/ico/favicon.ico
--rw-r--r--   0        0        0    13117 2023-05-13 08:55:56.449718 bodhi_server-8.0.2/bodhi/server/static/img/bodhi-logo.png
--rw-r--r--   0        0        0    17444 2023-05-13 08:55:56.449718 bodhi_server-8.0.2/bodhi/server/static/img/bodhi-logo.svg
--rw-r--r--   0        0        0    30769 2023-05-13 08:55:56.449718 bodhi_server-8.0.2/bodhi/server/static/img/logo-large.png
--rw-r--r--   0        0        0     4388 2023-05-13 08:55:56.449718 bodhi_server-8.0.2/bodhi/server/static/img/logo.png
--rw-r--r--   0        0        0     1775 2023-05-13 08:55:56.449718 bodhi_server-8.0.2/bodhi/server/static/js/comment_form.js
--rw-r--r--   0        0        0     4723 2023-05-13 08:55:56.449718 bodhi_server-8.0.2/bodhi/server/static/js/forms.js
--rw-r--r--   0        0        0     3238 2023-05-13 08:55:56.449718 bodhi_server-8.0.2/bodhi/server/static/js/override_form.js
--rw-r--r--   0        0        0     3485 2023-05-13 08:55:56.449718 bodhi_server-8.0.2/bodhi/server/static/js/search.js
--rw-r--r--   0        0        0     1475 2023-05-13 08:55:56.449718 bodhi_server-8.0.2/bodhi/server/static/js/site.js
--rw-r--r--   0        0        0    14110 2023-12-05 13:18:07.851647 bodhi_server-8.0.2/bodhi/server/static/js/update_form.js
--rw-r--r--   0        0        0   197005 2023-05-13 08:55:56.450718 bodhi_server-8.0.2/bodhi/server/static/vendor/chartjs/chart.min.js
--rw-r--r--   0        0        0   199088 2023-05-13 08:55:56.451718 bodhi_server-8.0.2/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css
--rw-r--r--   0        0        0    75244 2023-05-13 08:55:56.451718 bodhi_server-8.0.2/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css.map
--rw-r--r--   0        0        0    79790 2023-05-13 08:55:56.451718 bodhi_server-8.0.2/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js
--rw-r--r--   0        0        0   330849 2023-05-13 08:55:56.453718 bodhi_server-8.0.2/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js.map
--rw-r--r--   0        0        0    89501 2023-05-13 08:55:56.454718 bodhi_server-8.0.2/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.js
--rw-r--r--   0        0        0   137972 2023-05-13 08:55:56.455718 bodhi_server-8.0.2/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.map
--rw-r--r--   0        0        0    12438 2023-05-13 08:55:56.453718 bodhi_server-8.0.2/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.css
--rw-r--r--   0        0        0    48148 2023-05-13 08:55:56.453718 bodhi_server-8.0.2/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.js
--rw-r--r--   0        0        0     5855 2023-05-13 08:55:56.455718 bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/css/messenger-spinner.css
--rw-r--r--   0        0        0    12969 2023-05-13 08:55:56.455718 bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/css/messenger-theme-air.css
--rw-r--r--   0        0        0     3908 2023-05-13 08:55:56.455718 bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/css/messenger-theme-block.css
--rw-r--r--   0        0        0    13273 2023-05-13 08:55:56.455718 bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/css/messenger-theme-flat.css
--rw-r--r--   0        0        0    16828 2023-05-13 08:55:56.455718 bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/css/messenger-theme-future.css
--rw-r--r--   0        0        0     4399 2023-05-13 08:55:56.455718 bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/css/messenger-theme-ice.css
--rw-r--r--   0        0        0     3086 2023-05-13 08:55:56.455718 bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/css/messenger.css
--rw-r--r--   0        0        0     1281 2023-05-13 08:55:56.455718 bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/js/messenger-theme-flat.js
--rw-r--r--   0        0        0     1301 2023-05-13 08:55:56.455718 bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/js/messenger-theme-future.js
--rw-r--r--   0        0        0    40813 2023-05-13 08:55:56.455718 bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/js/messenger.js
--rw-r--r--   0        0        0    19068 2023-05-13 08:55:56.455718 bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/js/messenger.min.js
--rw-r--r--   0        0        0    32364 2023-05-13 08:55:56.455718 bodhi_server-8.0.2/bodhi/server/static/vendor/moment/moment.min.js
--rw-r--r--   0        0        0    66344 2023-07-30 15:01:32.170768 bodhi_server-8.0.2/bodhi/server/static/vendor/selectize/selectize-0.14.0.min.js
--rw-r--r--   0        0        0   126299 2023-05-13 08:55:56.456718 bodhi_server-8.0.2/bodhi/server/static/vendor/selectize/selectize-0.15.2.js
--rw-r--r--   0        0        0    55382 2023-05-13 08:55:56.457718 bodhi_server-8.0.2/bodhi/server/static/vendor/selectize/selectize-0.15.2.min.js
--rw-r--r--   0        0        0     9368 2023-07-30 15:01:32.170768 bodhi_server-8.0.2/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.14.0.css
--rw-r--r--   0        0        0    14594 2023-05-13 08:55:56.457718 bodhi_server-8.0.2/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.2.css
--rw-r--r--   0        0        0   104302 2023-05-13 08:55:56.457718 bodhi_server-8.0.2/bodhi/server/static/vendor/typeahead/typeahead.bundle.js
--rw-r--r--   0        0        0     6095 2023-05-13 08:55:56.458718 bodhi_server-8.0.2/bodhi/server/tasks/__init__.py
--rw-r--r--   0        0        0     7848 2023-05-13 08:55:56.458718 bodhi_server-8.0.2/bodhi/server/tasks/approve_testing.py
--rw-r--r--   0        0        0     2220 2023-12-05 13:18:07.851647 bodhi_server-8.0.2/bodhi/server/tasks/check_policies.py
--rw-r--r--   0        0        0     5083 2023-12-09 14:25:00.567911 bodhi_server-8.0.2/bodhi/server/tasks/check_signed_builds.py
--rw-r--r--   0        0        0     2397 2023-05-13 08:55:56.458718 bodhi_server-8.0.2/bodhi/server/tasks/clean_old_composes.py
--rw-r--r--   0        0        0    62502 2023-12-09 14:25:00.567911 bodhi_server-8.0.2/bodhi/server/tasks/composer.py
--rw-r--r--   0        0        0     2035 2023-12-09 14:25:00.571911 bodhi_server-8.0.2/bodhi/server/tasks/expire_overrides.py
--rw-r--r--   0        0        0     1785 2023-05-13 08:55:56.459718 bodhi_server-8.0.2/bodhi/server/tasks/fetch_test_cases.py
--rw-r--r--   0        0        0     2833 2023-05-13 08:55:56.459718 bodhi_server-8.0.2/bodhi/server/tasks/handle_side_and_related_tags.py
--rw-r--r--   0        0        0     1469 2023-05-13 08:55:56.459718 bodhi_server-8.0.2/bodhi/server/tasks/tag_update_builds.py
--rw-r--r--   0        0        0     3927 2023-12-05 13:18:07.852647 bodhi_server-8.0.2/bodhi/server/tasks/work_on_bugs.py
--rw-r--r--   0        0        0      105 2023-05-13 08:55:56.459718 bodhi_server-8.0.2/bodhi/server/templates/comment.html
--rw-r--r--   0        0        0     1331 2023-05-13 08:55:56.459718 bodhi_server-8.0.2/bodhi/server/templates/comments.html
--rw-r--r--   0        0        0     3575 2023-05-13 08:55:56.459718 bodhi_server-8.0.2/bodhi/server/templates/compose.html
--rw-r--r--   0        0        0     1270 2023-05-13 08:55:56.459718 bodhi_server-8.0.2/bodhi/server/templates/composes.html
--rw-r--r--   0        0        0      352 2023-05-13 08:55:56.459718 bodhi_server-8.0.2/bodhi/server/templates/errors.html
--rw-r--r--   0        0        0    15764 2023-07-30 15:01:31.985770 bodhi_server-8.0.2/bodhi/server/templates/fragments.html
--rw-r--r--   0        0        0     5537 2023-10-03 14:39:17.935214 bodhi_server-8.0.2/bodhi/server/templates/home.html
--rw-r--r--   0        0        0    10659 2023-10-03 14:39:17.935214 bodhi_server-8.0.2/bodhi/server/templates/master.html
--rw-r--r--   0        0        0    20248 2023-12-05 13:18:07.852647 bodhi_server-8.0.2/bodhi/server/templates/new_update.html
--rw-r--r--   0        0        0     9376 2023-10-03 14:39:17.935214 bodhi_server-8.0.2/bodhi/server/templates/override.html
--rw-r--r--   0        0        0     9735 2023-10-03 14:39:17.935214 bodhi_server-8.0.2/bodhi/server/templates/overrides.html
--rw-r--r--   0        0        0      882 2023-05-13 08:55:56.460718 bodhi_server-8.0.2/bodhi/server/templates/pager.html
--rw-r--r--   0        0        0    12735 2023-12-05 13:18:07.852647 bodhi_server-8.0.2/bodhi/server/templates/release.html
--rw-r--r--   0        0        0     2938 2023-07-30 15:01:32.160768 bodhi_server-8.0.2/bodhi/server/templates/releases.html
--rw-r--r--   0        0        0    60300 2024-01-11 16:19:57.756575 bodhi_server-8.0.2/bodhi/server/templates/update.html
--rw-r--r--   0        0        0    15968 2023-10-03 14:39:17.936214 bodhi_server-8.0.2/bodhi/server/templates/updates.html
--rw-r--r--   0        0        0     4808 2023-10-03 14:39:17.936214 bodhi_server-8.0.2/bodhi/server/templates/user.html
--rw-r--r--   0        0        0    50005 2023-12-09 14:25:00.571911 bodhi_server-8.0.2/bodhi/server/util.py
--rw-r--r--   0        0        0    52077 2023-12-09 14:25:00.571911 bodhi_server-8.0.2/bodhi/server/validators.py
--rw-r--r--   0        0        0      812 2023-05-13 08:55:56.462718 bodhi_server-8.0.2/bodhi/server/views/__init__.py
--rw-r--r--   0        0        0    23529 2023-12-09 14:25:00.572911 bodhi_server-8.0.2/bodhi/server/views/generic.py
--rw-r--r--   0        0        0     3545 2023-05-13 08:55:56.462718 bodhi_server-8.0.2/bodhi/server/webapp.py
--rw-r--r--   0        0        0     1592 2023-05-13 08:55:56.463718 bodhi_server-8.0.2/celeryconfig.py
--rw-r--r--   0        0        0      776 2023-05-13 08:55:56.463718 bodhi_server-8.0.2/docs/Makefile
--rw-r--r--   0        0        0     1631 2023-12-09 14:25:00.573911 bodhi_server-8.0.2/docs/conf.py
--rw-r--r--   0        0        0        0 2023-05-13 08:55:56.463718 bodhi_server-8.0.2/docs/index.rst
--rw-r--r--   0        0        0     1244 2023-05-13 08:55:56.463718 bodhi_server-8.0.2/docs/man_pages/bodhi-push.rst
--rw-r--r--   0        0        0      797 2023-05-13 08:55:56.463718 bodhi_server-8.0.2/docs/man_pages/bodhi-sar.rst
--rw-r--r--   0        0        0      523 2023-05-13 08:55:56.463718 bodhi_server-8.0.2/docs/man_pages/bodhi-shell.rst
--rw-r--r--   0        0        0      718 2023-05-13 08:55:56.463718 bodhi_server-8.0.2/docs/man_pages/bodhi-untag-branched.rst
--rw-r--r--   0        0        0      623 2023-05-13 08:55:56.463718 bodhi_server-8.0.2/docs/man_pages/initialize_bodhi_db.rst
--rw-r--r--   0        0        0    23994 2023-12-05 16:02:35.252783 bodhi_server-8.0.2/production.ini
--rw-r--r--   0        0        0     4986 2024-01-11 16:21:46.360973 bodhi_server-8.0.2/pyproject.toml
--rw-r--r--   0        0        0      418 2023-05-13 08:55:56.464717 bodhi_server-8.0.2/setup.cfg
--rw-r--r--   0        0        0      816 2023-05-13 08:55:56.464717 bodhi_server-8.0.2/tests/__init__.py
--rw-r--r--   0        0        0       39 2023-05-13 08:55:56.464717 bodhi_server-8.0.2/tests/auth/__init__.py
--rw-r--r--   0        0        0     4790 2023-05-13 08:55:56.464717 bodhi_server-8.0.2/tests/auth/test_fedora.py
--rw-r--r--   0        0        0    16947 2023-05-13 08:55:56.464717 bodhi_server-8.0.2/tests/auth/test_oauth.py
--rw-r--r--   0        0        0     5487 2023-05-13 08:55:56.464717 bodhi_server-8.0.2/tests/auth/test_utils.py
--rw-r--r--   0        0        0     5442 2023-05-13 08:55:56.464717 bodhi_server-8.0.2/tests/auth/test_views.py
--rw-r--r--   0        0        0     2293 2023-05-13 08:55:56.465717 bodhi_server-8.0.2/tests/auth/utils.py
--rw-r--r--   0        0        0    19449 2024-01-11 16:19:52.044659 bodhi_server-8.0.2/tests/base.py
--rw-r--r--   0        0        0     2214 2023-05-13 08:55:56.465717 bodhi_server-8.0.2/tests/conftest.py
--rw-r--r--   0        0        0      821 2023-05-13 08:55:56.465717 bodhi_server-8.0.2/tests/consumers/__init__.py
--rwxr-xr-x   0        0        0      335 2023-05-13 08:55:56.465717 bodhi_server-8.0.2/tests/consumers/pungi.basepath/fake-pungi.sh
--rw-r--r--   0        0        0       76 2023-05-13 08:55:56.465717 bodhi_server-8.0.2/tests/consumers/pungi.basepath/pungi.module.conf
--rw-r--r--   0        0        0       76 2023-05-13 08:55:56.465717 bodhi_server-8.0.2/tests/consumers/pungi.basepath/pungi.rpm.conf
--rw-r--r--   0        0        0      210 2023-05-13 08:55:56.465717 bodhi_server-8.0.2/tests/consumers/pungi.basepath/variants.module.xml.j2
--rw-r--r--   0        0        0       76 2023-05-13 08:55:56.465717 bodhi_server-8.0.2/tests/consumers/pungi.basepath/variants.rpm.xml.j2
--rw-r--r--   0        0        0    20084 2023-12-05 13:18:07.855647 bodhi_server-8.0.2/tests/consumers/test_automatic_updates.py
--rw-r--r--   0        0        0    11457 2023-05-13 08:55:56.465717 bodhi_server-8.0.2/tests/consumers/test_ci.py
--rw-r--r--   0        0        0     4779 2023-05-13 08:55:56.465717 bodhi_server-8.0.2/tests/consumers/test_consumers.py
--rw-r--r--   0        0        0    14326 2023-07-30 15:01:32.019770 bodhi_server-8.0.2/tests/consumers/test_resultsdb.py
--rw-r--r--   0        0        0    13114 2023-12-05 13:18:07.855647 bodhi_server-8.0.2/tests/consumers/test_signed.py
--rw-r--r--   0        0        0    10129 2023-07-30 15:01:32.019770 bodhi_server-8.0.2/tests/consumers/test_waiverdb.py
--rw-r--r--   0        0        0     1104 2023-12-08 13:18:21.186817 bodhi_server-8.0.2/tests/createrepo_c.ini
--rw-r--r--   0        0        0      913 2023-05-13 08:55:56.466718 bodhi_server-8.0.2/tests/functional/__init__.py
--rw-r--r--   0        0        0     2571 2023-05-13 08:55:56.466718 bodhi_server-8.0.2/tests/functional/test_packages.py
--rw-r--r--   0        0        0     8272 2023-05-13 08:55:56.466718 bodhi_server-8.0.2/tests/functional/test_users.py
--rw-r--r--   0        0        0      819 2023-05-13 08:55:56.466718 bodhi_server-8.0.2/tests/scripts/__init__.py
--rw-r--r--   0        0        0     2072 2023-05-13 08:55:56.466718 bodhi_server-8.0.2/tests/scripts/test_bshell.py
--rw-r--r--   0        0        0     5128 2023-05-13 08:55:56.466718 bodhi_server-8.0.2/tests/scripts/test_compat.py
--rw-r--r--   0        0        0     3597 2023-05-13 08:55:56.466718 bodhi_server-8.0.2/tests/scripts/test_initializedb.py
--rw-r--r--   0        0        0     5314 2023-12-09 14:25:00.573911 bodhi_server-8.0.2/tests/scripts/test_sar.py
--rw-r--r--   0        0        0    15411 2023-12-09 14:25:00.574911 bodhi_server-8.0.2/tests/scripts/test_untag_branched.py
--rw-r--r--   0        0        0      820 2023-05-13 08:55:56.467718 bodhi_server-8.0.2/tests/services/__init__.py
--rw-r--r--   0        0        0     4067 2023-05-13 08:55:56.467718 bodhi_server-8.0.2/tests/services/test_builds.py
--rw-r--r--   0        0        0    26822 2023-12-09 14:25:00.574911 bodhi_server-8.0.2/tests/services/test_comments.py
--rw-r--r--   0        0        0     6469 2023-05-13 08:55:56.467718 bodhi_server-8.0.2/tests/services/test_composes.py
--rw-r--r--   0        0        0     1512 2023-05-13 08:55:56.467718 bodhi_server-8.0.2/tests/services/test_csrf.py
--rw-r--r--   0        0        0     1827 2023-05-13 08:55:56.467718 bodhi_server-8.0.2/tests/services/test_errors.py
--rw-r--r--   0        0        0    31133 2023-12-09 14:25:00.578911 bodhi_server-8.0.2/tests/services/test_overrides.py
--rw-r--r--   0        0        0    30772 2023-12-05 13:18:07.855647 bodhi_server-8.0.2/tests/services/test_releases.py
--rw-r--r--   0        0        0     3801 2023-05-13 08:55:56.468717 bodhi_server-8.0.2/tests/services/test_schemas.py
--rw-r--r--   0        0        0   303697 2023-12-09 14:25:00.580911 bodhi_server-8.0.2/tests/services/test_updates.py
--rw-r--r--   0        0        0      817 2023-05-13 08:55:56.469717 bodhi_server-8.0.2/tests/tasks/__init__.py
--rw-r--r--   0        0        0     1531 2023-05-13 08:55:56.469717 bodhi_server-8.0.2/tests/tasks/base.py
--rw-r--r--   0        0        0    42724 2023-12-09 14:25:00.580911 bodhi_server-8.0.2/tests/tasks/test_approve_testing.py
--rw-r--r--   0        0        0    29342 2023-12-09 14:25:00.581911 bodhi_server-8.0.2/tests/tasks/test_check_policies.py
--rw-r--r--   0        0        0     9679 2023-12-09 14:25:00.581911 bodhi_server-8.0.2/tests/tasks/test_check_signed_builds.py
--rw-r--r--   0        0        0     5949 2023-05-13 08:55:56.469717 bodhi_server-8.0.2/tests/tasks/test_clean_old_composes.py
--rw-r--r--   0        0        0   168925 2023-12-09 14:25:00.582911 bodhi_server-8.0.2/tests/tasks/test_composer.py
--rw-r--r--   0        0        0     3792 2023-05-13 08:55:56.470718 bodhi_server-8.0.2/tests/tasks/test_expire_overrides.py
--rw-r--r--   0        0        0     3677 2023-05-13 08:55:56.470718 bodhi_server-8.0.2/tests/tasks/test_fetch_test_cases.py
--rw-r--r--   0        0        0     2799 2023-05-13 08:55:56.470718 bodhi_server-8.0.2/tests/tasks/test_handle_side_and_related_tags.py
--rw-r--r--   0        0        0     2321 2023-05-13 08:55:56.470718 bodhi_server-8.0.2/tests/tasks/test_tag_update_builds.py
--rw-r--r--   0        0        0     5085 2023-05-13 08:55:56.470718 bodhi_server-8.0.2/tests/tasks/test_work_on_bugs.py
--rw-r--r--   0        0        0     8783 2024-01-09 15:35:23.204917 bodhi_server-8.0.2/tests/test___init__.py
--rw-r--r--   0        0        0     2185 2023-05-13 08:55:56.470718 bodhi_server-8.0.2/tests/test_alembic.py
--rw-r--r--   0        0        0    28061 2023-05-13 08:55:56.470718 bodhi_server-8.0.2/tests/test_bugs.py
--rw-r--r--   0        0        0    17610 2023-12-05 13:18:07.856647 bodhi_server-8.0.2/tests/test_buildsys.py
--rw-r--r--   0        0        0    16273 2023-12-05 13:18:07.857647 bodhi_server-8.0.2/tests/test_config.py
--rw-r--r--   0        0        0     4319 2023-05-13 08:55:56.471717 bodhi_server-8.0.2/tests/test_logging.py
--rw-r--r--   0        0        0    16102 2023-12-05 13:18:07.857647 bodhi_server-8.0.2/tests/test_mail.py
--rw-r--r--   0        0        0    26451 2023-12-09 14:25:00.583911 bodhi_server-8.0.2/tests/test_metadata.py
--rw-r--r--   0        0        0   215576 2023-12-09 14:25:00.585911 bodhi_server-8.0.2/tests/test_models.py
--rw-r--r--   0        0        0     3897 2023-05-13 08:55:56.472717 bodhi_server-8.0.2/tests/test_notifications.py
--rw-r--r--   0        0        0    72415 2023-12-09 14:25:00.585911 bodhi_server-8.0.2/tests/test_push.py
--rw-r--r--   0        0        0     2238 2023-05-13 08:55:56.472717 bodhi_server-8.0.2/tests/test_renderers.py
--rw-r--r--   0        0        0     1642 2023-05-13 08:55:56.472717 bodhi_server-8.0.2/tests/test_schemas.py
--rw-r--r--   0        0        0     7785 2023-10-03 14:39:17.941214 bodhi_server-8.0.2/tests/test_security.py
--rw-r--r--   0        0        0    64181 2023-12-09 14:25:00.585911 bodhi_server-8.0.2/tests/test_util.py
--rw-r--r--   0        0        0    47092 2023-12-09 14:25:00.585911 bodhi_server-8.0.2/tests/test_validators.py
--rw-r--r--   0        0        0     2614 2023-05-13 08:55:56.473717 bodhi_server-8.0.2/tests/test_webapp.py
--rw-r--r--   0        0        0     4237 2023-12-10 12:46:06.078132 bodhi_server-8.0.2/tests/testing.ini
--rw-r--r--   0        0        0      992 2023-12-09 14:25:00.586911 bodhi_server-8.0.2/tests/utils.py
--rw-r--r--   0        0        0      817 2023-05-13 08:55:56.473717 bodhi_server-8.0.2/tests/views/__init__.py
--rw-r--r--   0        0        0    26550 2023-12-05 13:18:07.859647 bodhi_server-8.0.2/tests/views/test_generic.py
--rw-r--r--   0        0        0     5788 1970-01-01 00:00:00.000000 bodhi_server-8.0.2/setup.py
--rw-r--r--   0        0        0     4206 1970-01-01 00:00:00.000000 bodhi_server-8.0.2/PKG-INFO
+-rw-r--r--   0        0        0    18018 2024-02-09 16:37:01.453329 bodhi_server-8.1.0/COPYING
+-rw-r--r--   0        0        0     1655 2024-02-09 16:37:01.453329 bodhi_server-8.1.0/README.rst
+-rw-r--r--   0        0        0     1258 2024-02-09 16:37:01.453329 bodhi_server-8.1.0/alembic.ini
+-rw-r--r--   0        0        0      580 2024-02-09 16:37:01.453329 bodhi_server-8.1.0/apache/bodhi.conf
+-rw-r--r--   0        0        0      260 2024-02-09 16:37:01.453329 bodhi_server-8.1.0/apache/bodhi.wsgi
+-rw-r--r--   0        0        0    12379 2024-04-09 11:49:25.515646 bodhi_server-8.1.0/bodhi/server/__init__.py
+-rw-r--r--   0        0        0     1552 2024-03-11 08:36:24.654849 bodhi_server-8.1.0/bodhi/server/auth/__init__.py
+-rw-r--r--   0        0        0      220 2024-02-09 16:37:01.454329 bodhi_server-8.1.0/bodhi/server/auth/constants.py
+-rw-r--r--   0        0        0     5960 2024-02-09 16:37:01.454329 bodhi_server-8.1.0/bodhi/server/auth/fedora.py
+-rw-r--r--   0        0        0     2604 2024-02-09 16:37:01.455329 bodhi_server-8.1.0/bodhi/server/auth/oauth.py
+-rw-r--r--   0        0        0     2794 2024-02-09 16:37:01.455329 bodhi_server-8.1.0/bodhi/server/auth/oauth_015.py
+-rw-r--r--   0        0        0     3597 2024-02-09 16:37:01.455329 bodhi_server-8.1.0/bodhi/server/auth/oauth_1.py
+-rw-r--r--   0        0        0     5965 2024-03-11 08:36:24.655849 bodhi_server-8.1.0/bodhi/server/auth/utils.py
+-rw-r--r--   0        0        0     3960 2024-03-11 08:36:24.655849 bodhi_server-8.1.0/bodhi/server/auth/views.py
+-rw-r--r--   0        0        0    12401 2024-02-09 16:37:01.455329 bodhi_server-8.1.0/bodhi/server/bugs.py
+-rw-r--r--   0        0        0    31018 2024-03-26 07:10:28.073273 bodhi_server-8.1.0/bodhi/server/buildsys.py
+-rw-r--r--   0        0        0    26043 2024-03-26 07:10:28.073273 bodhi_server-8.1.0/bodhi/server/config.py
+-rw-r--r--   0        0        0     3616 2024-02-09 16:37:01.459329 bodhi_server-8.1.0/bodhi/server/consumers/__init__.py
+-rw-r--r--   0        0        0     8807 2024-02-09 16:37:01.459329 bodhi_server-8.1.0/bodhi/server/consumers/automatic_updates.py
+-rw-r--r--   0        0        0     4009 2024-02-09 16:37:01.459329 bodhi_server-8.1.0/bodhi/server/consumers/ci.py
+-rw-r--r--   0        0        0     2863 2024-02-09 16:37:01.459329 bodhi_server-8.1.0/bodhi/server/consumers/resultsdb.py
+-rw-r--r--   0        0        0     5651 2024-02-09 16:37:01.459329 bodhi_server-8.1.0/bodhi/server/consumers/signed.py
+-rw-r--r--   0        0        0     2728 2024-02-09 16:37:01.459329 bodhi_server-8.1.0/bodhi/server/consumers/util.py
+-rw-r--r--   0        0        0     2569 2024-02-09 16:37:01.459329 bodhi_server-8.1.0/bodhi/server/consumers/waiverdb.py
+-rw-r--r--   0        0        0     1040 2024-02-09 16:37:01.459329 bodhi_server-8.1.0/bodhi/server/email/templates/fedora_epel_errata_template.tpl
+-rw-r--r--   0        0        0     1070 2024-02-09 16:37:01.459329 bodhi_server-8.1.0/bodhi/server/email/templates/fedora_epel_legacy_errata_template.tpl
+-rw-r--r--   0        0        0     1051 2024-02-09 16:37:01.459329 bodhi_server-8.1.0/bodhi/server/email/templates/fedora_errata_template.tpl
+-rw-r--r--   0        0        0     1059 2024-02-09 16:37:01.459329 bodhi_server-8.1.0/bodhi/server/email/templates/fedora_modular_errata_template.tpl
+-rw-r--r--   0        0        0      261 2024-02-09 16:37:01.459329 bodhi_server-8.1.0/bodhi/server/email/templates/maillist_template.tpl
+-rw-r--r--   0        0        0     1249 2024-02-09 16:37:01.459329 bodhi_server-8.1.0/bodhi/server/exceptions.py
+-rw-r--r--   0        0        0     7524 2024-02-09 16:37:01.460328 bodhi_server-8.1.0/bodhi/server/ffmarkdown.py
+-rw-r--r--   0        0        0        0 2024-02-09 16:37:01.460328 bodhi_server-8.1.0/bodhi/server/locale/.placeholder
+-rw-r--r--   0        0        0     3641 2024-02-09 16:37:01.460328 bodhi_server-8.1.0/bodhi/server/logging.py
+-rw-r--r--   0        0        0    14685 2024-02-09 16:37:01.460328 bodhi_server-8.1.0/bodhi/server/mail.py
+-rw-r--r--   0        0        0    12411 2024-02-09 16:37:01.460328 bodhi_server-8.1.0/bodhi/server/metadata.py
+-rw-r--r--   0        0        0      706 2024-02-09 16:37:01.460328 bodhi_server-8.1.0/bodhi/server/migrations/README.rst
+-rw-r--r--   0        0        0      845 2024-02-09 16:37:01.460328 bodhi_server-8.1.0/bodhi/server/migrations/__init__.py
+-rw-r--r--   0        0        0     3018 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/env.py
+-rw-r--r--   0        0        0     1181 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/script.py.mako
+-rw-r--r--   0        0        0     1568 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/16864f8ff395_remove_requirements_column_from_build_.py
+-rw-r--r--   0        0        0     2918 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/190ba571c7d2_remove_the_batching_request_state.py
+-rw-r--r--   0        0        0     1333 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/19e28e9851a2_index_comment_update_id.py
+-rw-r--r--   0        0        0     1380 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/1c97477e38ee_convert_br_override_notes_to_unicodetext.py
+-rw-r--r--   0        0        0     1443 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/2fc96aa44a74_drop_the_user_show_popup_column.py
+-rw-r--r--   0        0        0     3846 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/325954bac9f7_link_testcases_to_builds.py
+-rw-r--r--   0        0        0     2732 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/3a2e248d1757_add_the_unspecified_enum_to_updatetype.py
+-rw-r--r--   0        0        0     1530 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/3b34650a0cf6_update_type_of_users_email_with_new_.py
+-rw-r--r--   0        0        0     3041 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/499ac8bbe09a_remove_unused_update_sidetag_statuses.py
+-rw-r--r--   0        0        0     1822 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/559acf7e2c16_make_comments_update_not_nullable.py
+-rw-r--r--   0        0        0     2279 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/5703ddfe855d_add_package_manager_and_testing_.py
+-rw-r--r--   0        0        0     2187 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/58b7919b942c_remove_the_updates_title_column.py
+-rw-r--r--   0        0        0     2586 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/5c86a3f9dc03_drop_support_for_cve_tracking.py
+-rw-r--r--   0        0        0     2708 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/6b3eb9ae2b87_remove_unused_updatestatus_processing.py
+-rw-r--r--   0        0        0     1741 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/7ba286412ad4_drop_the_relationship_between_packages_.py
+-rw-r--r--   0        0        0     2812 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/8c4d6aad9b78_add_the_greenwave_failed_enum_to_.py
+-rw-r--r--   0        0        0     1503 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/8e9dc57e082d_obsolete_updates_for_archived_release.py
+-rw-r--r--   0        0        0     1368 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/9991cf10ec50_mark_the_bugs_private_field_as_nullable.py
+-rw-r--r--   0        0        0     1501 2024-02-09 16:37:01.461329 bodhi_server-8.1.0/bodhi/server/migrations/versions/9c0a34961768_remove_the_greenwave_unsatisfied_.py
+-rw-r--r--   0        0        0      843 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/__init__.py
+-rw-r--r--   0        0        0     1321 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/a3580bdf5129_remove_the_ci_url_field_from_builds.py
+-rw-r--r--   0        0        0     2991 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/a418acf470f8_drop_the_stacks_table.py
+-rw-r--r--   0        0        0     1346 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/aae0d29d49b7_remove_the_private_field_on_the_bug_.py
+-rw-r--r--   0        0        0     1808 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/b1fd856efcf6_add_autopush_boolean_and_stable_days_to_update.py
+-rw-r--r--   0        0        0     2341 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/bdf0e37ab793_disallow_null_values_in_stable_karma_.py
+-rw-r--r--   0        0        0     2593 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/c60d95eef4f1_add_frozen_release_state.py
+-rw-r--r--   0        0        0     2316 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/c98beb4940b5_remove_the_comments_anonymous_column.py
+-rw-r--r--   0        0        0     1296 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/d399493275b6_add_the_eol_column.py
+-rw-r--r--   0        0        0     1329 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/d3f8bd499ecd_add_from_tag_column_to_updates.py
+-rw-r--r--   0        0        0     1405 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/d986618207bc_add_composed_by_bodhi_flag_to_releases_.py
+-rw-r--r--   0        0        0     1670 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/e3988e00b338_drop_date_pushed.py
+-rw-r--r--   0        0        0     1421 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/e5b3ddb35df3_remove_the_greenwave_summary_string_.py
+-rw-r--r--   0        0        0     1403 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/e8a059156d38_add_the_create_automatic_updates_bool_.py
+-rw-r--r--   0        0        0     1312 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/eec610d7ab3a_index_the_builds_update_id_column.py
+-rw-r--r--   0        0        0     1345 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/f393d006559b_add_critpath_groups_to_update.py
+-rw-r--r--   0        0        0     1469 2024-02-09 16:37:01.462329 bodhi_server-8.1.0/bodhi/server/migrations/versions/f50dc199039c_make_comments_user_id_not_nullable.py
+-rw-r--r--   0        0        0     1308 2024-02-09 16:37:01.463328 bodhi_server-8.1.0/bodhi/server/migrations/versions/f660455231d4_add_released_on_to_release.py
+-rw-r--r--   0        0        0     1353 2024-02-09 16:37:01.463328 bodhi_server-8.1.0/bodhi/server/migrations/versions/f8a44498c806_remove_legacy_old_updateid.py
+-rw-r--r--   0        0        0     1347 2024-02-09 16:37:01.463328 bodhi_server-8.1.0/bodhi/server/migrations/versions/ff834fa4f23e_increase_the_update_alias_size.py
+-rw-r--r--   0        0        0   196767 2024-03-26 07:10:28.074272 bodhi_server-8.1.0/bodhi/server/models.py
+-rw-r--r--   0        0        0     3016 2024-02-09 16:37:01.464328 bodhi_server-8.1.0/bodhi/server/notifications.py
+-rw-r--r--   0        0        0    11988 2024-02-09 16:37:01.464328 bodhi_server-8.1.0/bodhi/server/push.py
+-rw-r--r--   0        0        0     7143 2024-02-09 16:37:01.464328 bodhi_server-8.1.0/bodhi/server/renderers.py
+-rw-r--r--   0        0        0    22577 2024-02-09 16:37:01.464328 bodhi_server-8.1.0/bodhi/server/schemas.py
+-rw-r--r--   0        0        0      849 2024-02-09 16:37:01.464328 bodhi_server-8.1.0/bodhi/server/scripts/__init__.py
+-rw-r--r--   0        0        0     1397 2024-02-09 16:37:01.464328 bodhi_server-8.1.0/bodhi/server/scripts/bshell.py
+-rw-r--r--   0        0        0     3871 2024-02-09 16:37:01.464328 bodhi_server-8.1.0/bodhi/server/scripts/compat.py
+-rw-r--r--   0        0        0     1847 2024-02-09 16:37:01.464328 bodhi_server-8.1.0/bodhi/server/scripts/initializedb.py
+-rw-r--r--   0        0        0     4206 2024-02-09 16:37:01.464328 bodhi_server-8.1.0/bodhi/server/scripts/sar.py
+-rw-r--r--   0        0        0     3839 2024-02-09 16:37:01.464328 bodhi_server-8.1.0/bodhi/server/scripts/untag_branched.py
+-rw-r--r--   0        0        0     9576 2024-02-09 16:37:01.465329 bodhi_server-8.1.0/bodhi/server/security.py
+-rw-r--r--   0        0        0      815 2024-02-09 16:37:01.465329 bodhi_server-8.1.0/bodhi/server/services/__init__.py
+-rw-r--r--   0        0        0     5246 2024-02-09 16:37:01.465329 bodhi_server-8.1.0/bodhi/server/services/builds.py
+-rw-r--r--   0        0        0     8705 2024-02-09 16:37:01.466328 bodhi_server-8.1.0/bodhi/server/services/comments.py
+-rw-r--r--   0        0        0     3936 2024-02-09 16:37:01.466328 bodhi_server-8.1.0/bodhi/server/services/composes.py
+-rw-r--r--   0        0        0     2058 2024-02-09 16:37:01.466328 bodhi_server-8.1.0/bodhi/server/services/csrf.py
+-rw-r--r--   0        0        0     3793 2024-02-09 16:37:01.466328 bodhi_server-8.1.0/bodhi/server/services/errors.py
+-rw-r--r--   0        0        0     1969 2024-02-09 16:37:01.466328 bodhi_server-8.1.0/bodhi/server/services/markdown.py
+-rw-r--r--   0        0        0     1916 2024-02-09 16:37:01.466328 bodhi_server-8.1.0/bodhi/server/services/metrics_tween.py
+-rw-r--r--   0        0        0    13051 2024-02-09 16:37:01.466328 bodhi_server-8.1.0/bodhi/server/services/overrides.py
+-rw-r--r--   0        0        0     3786 2024-02-09 16:37:01.466328 bodhi_server-8.1.0/bodhi/server/services/packages.py
+-rw-r--r--   0        0        0    17316 2024-02-09 16:37:01.466328 bodhi_server-8.1.0/bodhi/server/services/releases.py
+-rw-r--r--   0        0        0     3503 2024-03-26 07:10:28.074272 bodhi_server-8.1.0/bodhi/server/services/schemas.py
+-rw-r--r--   0        0        0    29245 2024-02-09 16:37:01.467328 bodhi_server-8.1.0/bodhi/server/services/updates.py
+-rw-r--r--   0        0        0     6676 2024-02-09 16:37:01.467328 bodhi_server-8.1.0/bodhi/server/services/user.py
+-rw-r--r--   0        0        0      832 2024-02-09 16:37:01.467328 bodhi_server-8.1.0/bodhi/server/static/__init__.py
+-rw-r--r--   0        0        0    10425 2024-02-09 16:37:01.467328 bodhi_server-8.1.0/bodhi/server/static/bodhi-logo.svg
+-rw-r--r--   0        0        0     6423 2024-02-09 16:37:01.467328 bodhi_server-8.1.0/bodhi/server/static/css/site.css
+-rw-r--r--   0        0        0   124988 2024-02-09 16:37:01.468328 bodhi_server-8.1.0/bodhi/server/static/fonts/font-awesome/FontAwesome.otf
+-rw-r--r--   0        0        0    76518 2024-02-09 16:37:01.468328 bodhi_server-8.1.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   391622 2024-02-09 16:37:01.469328 bodhi_server-8.1.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   152796 2024-02-09 16:37:01.470328 bodhi_server-8.1.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    90412 2024-02-09 16:37:01.470328 bodhi_server-8.1.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    71896 2024-02-09 16:37:01.470328 bodhi_server-8.1.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0    35152 2024-02-09 16:37:01.467328 bodhi_server-8.1.0/bodhi/server/static/fonts/font-awesome.css
+-rwxr-xr-x   0        0        0   139140 2024-02-09 16:37:01.470328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/hack-bold-webfont.eot
+-rwxr-xr-x   0        0        0   146800 2024-02-09 16:37:01.470328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/hack-bolditalic-webfont.eot
+-rwxr-xr-x   0        0        0   143488 2024-02-09 16:37:01.471328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/hack-italic-webfont.eot
+-rwxr-xr-x   0        0        0   137266 2024-02-09 16:37:01.471328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/hack-regular-webfont.eot
+-rwxr-xr-x   0        0        0    28782 2024-02-09 16:37:01.471328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/latin/hack-bold-latin-webfont.eot
+-rwxr-xr-x   0        0        0    31454 2024-02-09 16:37:01.471328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/latin/hack-bolditalic-latin-webfont.eot
+-rwxr-xr-x   0        0        0    30512 2024-02-09 16:37:01.471328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/latin/hack-italic-latin-webfont.eot
+-rwxr-xr-x   0        0        0    28527 2024-02-09 16:37:01.471328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/latin/hack-regular-latin-webfont.eot
+-rwxr-xr-x   0        0        0   389828 2024-02-09 16:37:01.473328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/hack-bold-webfont.ttf
+-rwxr-xr-x   0        0        0   398888 2024-02-09 16:37:01.474328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/hack-bolditalic-webfont.ttf
+-rwxr-xr-x   0        0        0   393880 2024-02-09 16:37:01.475328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/hack-italic-webfont.ttf
+-rwxr-xr-x   0        0        0   387660 2024-02-09 16:37:01.477328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/hack-regular-webfont.ttf
+-rwxr-xr-x   0        0        0    73056 2024-02-09 16:37:01.477328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bold-latin-webfont.ttf
+-rwxr-xr-x   0        0        0    77808 2024-02-09 16:37:01.477328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bolditalic-latin-webfont.ttf
+-rwxr-xr-x   0        0        0    76444 2024-02-09 16:37:01.477328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-italic-latin-webfont.ttf
+-rwxr-xr-x   0        0        0    73256 2024-02-09 16:37:01.479328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-regular-latin-webfont.ttf
+-rwxr-xr-x   0        0        0   171820 2024-02-09 16:37:01.479328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/hack-bold-webfont.woff
+-rwxr-xr-x   0        0        0   180204 2024-02-09 16:37:01.479328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/hack-bolditalic-webfont.woff
+-rwxr-xr-x   0        0        0   176864 2024-02-09 16:37:01.479328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/hack-italic-webfont.woff
+-rwxr-xr-x   0        0        0   168376 2024-02-09 16:37:01.480328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/hack-regular-webfont.woff
+-rwxr-xr-x   0        0        0    31964 2024-02-09 16:37:01.480328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/latin/hack-bold-latin-webfont.woff
+-rwxr-xr-x   0        0        0    34720 2024-02-09 16:37:01.480328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/latin/hack-bolditalic-latin-webfont.woff
+-rwxr-xr-x   0        0        0    33556 2024-02-09 16:37:01.480328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/latin/hack-italic-latin-webfont.woff
+-rwxr-xr-x   0        0        0    31584 2024-02-09 16:37:01.480328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/latin/hack-regular-latin-webfont.woff
+-rwxr-xr-x   0        0        0   124552 2024-02-09 16:37:01.480328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/hack-bold-webfont.woff2
+-rwxr-xr-x   0        0        0   131588 2024-02-09 16:37:01.481328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/hack-bolditalic-webfont.woff2
+-rwxr-xr-x   0        0        0   128624 2024-02-09 16:37:01.481328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/hack-italic-webfont.woff2
+-rwxr-xr-x   0        0        0   122888 2024-02-09 16:37:01.481328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/hack-regular-webfont.woff2
+-rwxr-xr-x   0        0        0    25884 2024-02-09 16:37:01.481328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/latin/hack-bold-latin-webfont.woff2
+-rwxr-xr-x   0        0        0    28232 2024-02-09 16:37:01.481328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/latin/hack-bolditalic-latin-webfont.woff2
+-rwxr-xr-x   0        0        0    27576 2024-02-09 16:37:01.481328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/latin/hack-italic-latin-webfont.woff2
+-rwxr-xr-x   0        0        0    25696 2024-02-09 16:37:01.481328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/latin/hack-regular-latin-webfont.woff2
+-rw-r--r--   0        0        0     1947 2024-02-09 16:37:01.470328 bodhi_server-8.1.0/bodhi/server/static/fonts/hack.css
+-rw-r--r--   0        0        0    31896 2024-02-09 16:37:01.481328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.eot
+-rw-r--r--   0        0        0   254253 2024-02-09 16:37:01.482328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.svg
+-rw-r--r--   0        0        0    68444 2024-02-09 16:37:01.482328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.ttf
+-rw-r--r--   0        0        0    33704 2024-02-09 16:37:01.482328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff
+-rw-r--r--   0        0        0    23816 2024-02-09 16:37:01.483328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff2
+-rw-r--r--   0        0        0    30763 2024-02-09 16:37:01.483328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.eot
+-rw-r--r--   0        0        0   258568 2024-02-09 16:37:01.483328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.svg
+-rw-r--r--   0        0        0    64668 2024-02-09 16:37:01.483328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.ttf
+-rw-r--r--   0        0        0    32300 2024-02-09 16:37:01.483328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff
+-rw-r--r--   0        0        0    22220 2024-02-09 16:37:01.483328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff2
+-rw-r--r--   0        0        0    32088 2024-02-09 16:37:01.484328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.eot
+-rw-r--r--   0        0        0   254724 2024-02-09 16:37:01.484328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.svg
+-rw-r--r--   0        0        0    68776 2024-02-09 16:37:01.484328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.ttf
+-rw-r--r--   0        0        0    33876 2024-02-09 16:37:01.484328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff
+-rw-r--r--   0        0        0    23652 2024-02-09 16:37:01.484328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff2
+-rw-r--r--   0        0        0    30546 2024-02-09 16:37:01.484328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.eot
+-rw-r--r--   0        0        0   257617 2024-02-09 16:37:01.485328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.svg
+-rw-r--r--   0        0        0    65236 2024-02-09 16:37:01.485328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.ttf
+-rw-r--r--   0        0        0    32180 2024-02-09 16:37:01.485328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff
+-rw-r--r--   0        0        0    22176 2024-02-09 16:37:01.485328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff2
+-rw-r--r--   0        0        0    30880 2024-02-09 16:37:01.485328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.eot
+-rw-r--r--   0        0        0   258434 2024-02-09 16:37:01.486328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.svg
+-rw-r--r--   0        0        0    65072 2024-02-09 16:37:01.486328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.ttf
+-rw-r--r--   0        0        0    32212 2024-02-09 16:37:01.486328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff
+-rw-r--r--   0        0        0    22196 2024-02-09 16:37:01.486328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff2
+-rw-r--r--   0        0        0    31491 2024-02-09 16:37:01.486328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.eot
+-rw-r--r--   0        0        0   255338 2024-02-09 16:37:01.486328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.svg
+-rw-r--r--   0        0        0    66740 2024-02-09 16:37:01.486328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.ttf
+-rw-r--r--   0        0        0    33060 2024-02-09 16:37:01.486328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff
+-rw-r--r--   0        0        0    23048 2024-02-09 16:37:01.486328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff2
+-rw-r--r--   0        0        0     4956 2024-02-09 16:37:01.481328 bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans.css
+-rw-r--r--   0        0        0     4255 2024-02-09 16:37:01.486328 bodhi_server-8.1.0/bodhi/server/static/ico/favicon.ico
+-rw-r--r--   0        0        0    13117 2024-02-09 16:37:01.487328 bodhi_server-8.1.0/bodhi/server/static/img/bodhi-logo.png
+-rw-r--r--   0        0        0    17444 2024-02-09 16:37:01.487328 bodhi_server-8.1.0/bodhi/server/static/img/bodhi-logo.svg
+-rw-r--r--   0        0        0    30769 2024-02-09 16:37:01.487328 bodhi_server-8.1.0/bodhi/server/static/img/logo-large.png
+-rw-r--r--   0        0        0     4388 2024-02-09 16:37:01.487328 bodhi_server-8.1.0/bodhi/server/static/img/logo.png
+-rw-r--r--   0        0        0     1775 2024-02-09 16:37:01.487328 bodhi_server-8.1.0/bodhi/server/static/js/comment_form.js
+-rw-r--r--   0        0        0     4723 2024-02-09 16:37:01.487328 bodhi_server-8.1.0/bodhi/server/static/js/forms.js
+-rw-r--r--   0        0        0     3238 2024-02-09 16:37:01.487328 bodhi_server-8.1.0/bodhi/server/static/js/override_form.js
+-rw-r--r--   0        0        0     3485 2024-02-09 16:37:01.487328 bodhi_server-8.1.0/bodhi/server/static/js/search.js
+-rw-r--r--   0        0        0     1475 2024-02-09 16:37:01.487328 bodhi_server-8.1.0/bodhi/server/static/js/site.js
+-rw-r--r--   0        0        0    14110 2024-02-09 16:37:01.487328 bodhi_server-8.1.0/bodhi/server/static/js/update_form.js
+-rw-r--r--   0        0        0   197005 2024-02-09 16:37:01.488328 bodhi_server-8.1.0/bodhi/server/static/vendor/chartjs/chart.min.js
+-rw-r--r--   0        0        0   199088 2024-02-09 16:37:01.488328 bodhi_server-8.1.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css
+-rw-r--r--   0        0        0    75244 2024-02-09 16:37:01.488328 bodhi_server-8.1.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css.map
+-rw-r--r--   0        0        0    79790 2024-02-09 16:37:01.488328 bodhi_server-8.1.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js
+-rw-r--r--   0        0        0   330849 2024-02-09 16:37:01.489328 bodhi_server-8.1.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js.map
+-rw-r--r--   0        0        0    89501 2024-02-09 16:37:01.491328 bodhi_server-8.1.0/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0   137972 2024-02-09 16:37:01.491328 bodhi_server-8.1.0/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.map
+-rw-r--r--   0        0        0    12438 2024-02-09 16:37:01.489328 bodhi_server-8.1.0/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.css
+-rw-r--r--   0        0        0    48148 2024-02-09 16:37:01.490328 bodhi_server-8.1.0/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.js
+-rw-r--r--   0        0        0     5855 2024-02-09 16:37:01.492328 bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/css/messenger-spinner.css
+-rw-r--r--   0        0        0    12969 2024-02-09 16:37:01.492328 bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/css/messenger-theme-air.css
+-rw-r--r--   0        0        0     3908 2024-02-09 16:37:01.492328 bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/css/messenger-theme-block.css
+-rw-r--r--   0        0        0    13273 2024-02-09 16:37:01.492328 bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/css/messenger-theme-flat.css
+-rw-r--r--   0        0        0    16828 2024-02-09 16:37:01.492328 bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/css/messenger-theme-future.css
+-rw-r--r--   0        0        0     4399 2024-02-09 16:37:01.492328 bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/css/messenger-theme-ice.css
+-rw-r--r--   0        0        0     3086 2024-02-09 16:37:01.492328 bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/css/messenger.css
+-rw-r--r--   0        0        0     1281 2024-02-09 16:37:01.492328 bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/js/messenger-theme-flat.js
+-rw-r--r--   0        0        0     1301 2024-02-09 16:37:01.492328 bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/js/messenger-theme-future.js
+-rw-r--r--   0        0        0    40813 2024-02-09 16:37:01.492328 bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/js/messenger.js
+-rw-r--r--   0        0        0    19068 2024-02-09 16:37:01.492328 bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/js/messenger.min.js
+-rw-r--r--   0        0        0    32364 2024-02-09 16:37:01.492328 bodhi_server-8.1.0/bodhi/server/static/vendor/moment/moment.min.js
+-rw-r--r--   0        0        0    66344 2024-02-09 16:37:01.493328 bodhi_server-8.1.0/bodhi/server/static/vendor/selectize/selectize-0.14.0.min.js
+-rw-r--r--   0        0        0   126299 2024-02-09 16:37:01.493328 bodhi_server-8.1.0/bodhi/server/static/vendor/selectize/selectize-0.15.2.js
+-rw-r--r--   0        0        0    55382 2024-02-09 16:37:01.493328 bodhi_server-8.1.0/bodhi/server/static/vendor/selectize/selectize-0.15.2.min.js
+-rw-r--r--   0        0        0     9368 2024-02-09 16:37:01.493328 bodhi_server-8.1.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.14.0.css
+-rw-r--r--   0        0        0    14594 2024-02-09 16:37:01.493328 bodhi_server-8.1.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.2.css
+-rw-r--r--   0        0        0   104302 2024-02-09 16:37:01.493328 bodhi_server-8.1.0/bodhi/server/static/vendor/typeahead/typeahead.bundle.js
+-rw-r--r--   0        0        0     6095 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/tasks/__init__.py
+-rw-r--r--   0        0        0     7848 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/tasks/approve_testing.py
+-rw-r--r--   0        0        0     2220 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/tasks/check_policies.py
+-rw-r--r--   0        0        0     5083 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/tasks/check_signed_builds.py
+-rw-r--r--   0        0        0     2397 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/tasks/clean_old_composes.py
+-rw-r--r--   0        0        0    62684 2024-03-26 07:10:28.075272 bodhi_server-8.1.0/bodhi/server/tasks/composer.py
+-rw-r--r--   0        0        0     2035 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/tasks/expire_overrides.py
+-rw-r--r--   0        0        0     1785 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/tasks/fetch_test_cases.py
+-rw-r--r--   0        0        0     2833 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/tasks/handle_side_and_related_tags.py
+-rw-r--r--   0        0        0     1469 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/tasks/tag_update_builds.py
+-rw-r--r--   0        0        0     3927 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/tasks/work_on_bugs.py
+-rw-r--r--   0        0        0      105 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/templates/comment.html
+-rw-r--r--   0        0        0     1331 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/templates/comments.html
+-rw-r--r--   0        0        0     3575 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/templates/compose.html
+-rw-r--r--   0        0        0     1270 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/templates/composes.html
+-rw-r--r--   0        0        0      352 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/templates/errors.html
+-rw-r--r--   0        0        0    15764 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/templates/fragments.html
+-rw-r--r--   0        0        0     5537 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/templates/home.html
+-rw-r--r--   0        0        0    10659 2024-03-11 08:36:24.657849 bodhi_server-8.1.0/bodhi/server/templates/master.html
+-rw-r--r--   0        0        0    20248 2024-02-09 16:37:01.494328 bodhi_server-8.1.0/bodhi/server/templates/new_update.html
+-rw-r--r--   0        0        0     9376 2024-02-09 16:37:01.495328 bodhi_server-8.1.0/bodhi/server/templates/override.html
+-rw-r--r--   0        0        0     9735 2024-02-09 16:37:01.495328 bodhi_server-8.1.0/bodhi/server/templates/overrides.html
+-rw-r--r--   0        0        0      882 2024-02-09 16:37:01.495328 bodhi_server-8.1.0/bodhi/server/templates/pager.html
+-rw-r--r--   0        0        0    12735 2024-02-09 16:37:01.495328 bodhi_server-8.1.0/bodhi/server/templates/release.html
+-rw-r--r--   0        0        0     2938 2024-02-09 16:37:01.495328 bodhi_server-8.1.0/bodhi/server/templates/releases.html
+-rw-r--r--   0        0        0    60300 2024-02-09 16:37:01.495328 bodhi_server-8.1.0/bodhi/server/templates/update.html
+-rw-r--r--   0        0        0    15968 2024-02-09 16:37:01.495328 bodhi_server-8.1.0/bodhi/server/templates/updates.html
+-rw-r--r--   0        0        0     4808 2024-02-09 16:37:01.495328 bodhi_server-8.1.0/bodhi/server/templates/user.html
+-rw-r--r--   0        0        0    50978 2024-03-26 07:10:28.075272 bodhi_server-8.1.0/bodhi/server/util.py
+-rw-r--r--   0        0        0    52883 2024-03-26 07:10:28.076272 bodhi_server-8.1.0/bodhi/server/validators.py
+-rw-r--r--   0        0        0      812 2024-02-09 16:37:01.496328 bodhi_server-8.1.0/bodhi/server/views/__init__.py
+-rw-r--r--   0        0        0    23529 2024-02-09 16:37:01.497328 bodhi_server-8.1.0/bodhi/server/views/generic.py
+-rw-r--r--   0        0        0     3545 2024-02-09 16:37:01.497328 bodhi_server-8.1.0/bodhi/server/webapp.py
+-rw-r--r--   0        0        0     1592 2024-02-09 16:37:01.497328 bodhi_server-8.1.0/celeryconfig.py
+-rw-r--r--   0        0        0      776 2024-02-09 16:37:01.497328 bodhi_server-8.1.0/docs/Makefile
+-rw-r--r--   0        0        0     1631 2024-02-09 16:37:01.497328 bodhi_server-8.1.0/docs/conf.py
+-rw-r--r--   0        0        0        0 2024-02-09 16:37:01.497328 bodhi_server-8.1.0/docs/index.rst
+-rw-r--r--   0        0        0     1244 2024-02-09 16:37:01.497328 bodhi_server-8.1.0/docs/man_pages/bodhi-push.rst
+-rw-r--r--   0        0        0      797 2024-02-09 16:37:01.497328 bodhi_server-8.1.0/docs/man_pages/bodhi-sar.rst
+-rw-r--r--   0        0        0      523 2024-02-09 16:37:01.497328 bodhi_server-8.1.0/docs/man_pages/bodhi-shell.rst
+-rw-r--r--   0        0        0      718 2024-02-09 16:37:01.497328 bodhi_server-8.1.0/docs/man_pages/bodhi-untag-branched.rst
+-rw-r--r--   0        0        0      623 2024-02-09 16:37:01.497328 bodhi_server-8.1.0/docs/man_pages/initialize_bodhi_db.rst
+-rw-r--r--   0        0        0    24132 2024-03-26 07:10:28.077273 bodhi_server-8.1.0/production.ini
+-rw-r--r--   0        0        0     4986 2024-04-09 11:59:27.266243 bodhi_server-8.1.0/pyproject.toml
+-rw-r--r--   0        0        0      418 2024-02-09 16:37:01.499328 bodhi_server-8.1.0/setup.cfg
+-rw-r--r--   0        0        0      816 2024-02-09 16:37:01.499328 bodhi_server-8.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       39 2024-02-09 16:37:01.499328 bodhi_server-8.1.0/tests/auth/__init__.py
+-rw-r--r--   0        0        0     4790 2024-02-09 16:37:01.499328 bodhi_server-8.1.0/tests/auth/test_fedora.py
+-rw-r--r--   0        0        0    16947 2024-02-09 16:37:01.499328 bodhi_server-8.1.0/tests/auth/test_oauth.py
+-rw-r--r--   0        0        0     5487 2024-02-09 16:37:01.499328 bodhi_server-8.1.0/tests/auth/test_utils.py
+-rw-r--r--   0        0        0     5442 2024-02-09 16:37:01.499328 bodhi_server-8.1.0/tests/auth/test_views.py
+-rw-r--r--   0        0        0     2293 2024-03-11 08:36:24.657849 bodhi_server-8.1.0/tests/auth/utils.py
+-rw-r--r--   0        0        0    19449 2024-02-09 16:37:01.499328 bodhi_server-8.1.0/tests/base.py
+-rw-r--r--   0        0        0     2214 2024-02-09 16:37:01.499328 bodhi_server-8.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      821 2024-02-09 16:37:01.499328 bodhi_server-8.1.0/tests/consumers/__init__.py
+-rwxr-xr-x   0        0        0      335 2024-02-09 16:37:01.499328 bodhi_server-8.1.0/tests/consumers/pungi.basepath/fake-pungi.sh
+-rw-r--r--   0        0        0       76 2024-02-09 16:37:01.499328 bodhi_server-8.1.0/tests/consumers/pungi.basepath/pungi.module.conf
+-rw-r--r--   0        0        0       76 2024-02-09 16:37:01.499328 bodhi_server-8.1.0/tests/consumers/pungi.basepath/pungi.rpm.conf
+-rw-r--r--   0        0        0      210 2024-02-09 16:37:01.499328 bodhi_server-8.1.0/tests/consumers/pungi.basepath/variants.module.xml.j2
+-rw-r--r--   0        0        0       76 2024-02-09 16:37:01.499328 bodhi_server-8.1.0/tests/consumers/pungi.basepath/variants.rpm.xml.j2
+-rw-r--r--   0        0        0    20084 2024-02-09 16:37:01.500328 bodhi_server-8.1.0/tests/consumers/test_automatic_updates.py
+-rw-r--r--   0        0        0    11457 2024-02-09 16:37:01.500328 bodhi_server-8.1.0/tests/consumers/test_ci.py
+-rw-r--r--   0        0        0     4779 2024-02-09 16:37:01.500328 bodhi_server-8.1.0/tests/consumers/test_consumers.py
+-rw-r--r--   0        0        0    14326 2024-02-09 16:37:01.500328 bodhi_server-8.1.0/tests/consumers/test_resultsdb.py
+-rw-r--r--   0        0        0    13114 2024-02-09 16:37:01.500328 bodhi_server-8.1.0/tests/consumers/test_signed.py
+-rw-r--r--   0        0        0    10129 2024-02-09 16:37:01.500328 bodhi_server-8.1.0/tests/consumers/test_waiverdb.py
+-rw-r--r--   0        0        0     1104 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/createrepo_c.ini
+-rw-r--r--   0        0        0      913 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/functional/__init__.py
+-rw-r--r--   0        0        0     2571 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/functional/test_packages.py
+-rw-r--r--   0        0        0     8272 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/functional/test_users.py
+-rw-r--r--   0        0        0      819 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/scripts/__init__.py
+-rw-r--r--   0        0        0     2072 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/scripts/test_bshell.py
+-rw-r--r--   0        0        0     5128 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/scripts/test_compat.py
+-rw-r--r--   0        0        0     3597 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/scripts/test_initializedb.py
+-rw-r--r--   0        0        0     5314 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/scripts/test_sar.py
+-rw-r--r--   0        0        0    15411 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/scripts/test_untag_branched.py
+-rw-r--r--   0        0        0      820 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/services/__init__.py
+-rw-r--r--   0        0        0     4067 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/services/test_builds.py
+-rw-r--r--   0        0        0    26822 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/services/test_comments.py
+-rw-r--r--   0        0        0     6469 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/services/test_composes.py
+-rw-r--r--   0        0        0     1512 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/services/test_csrf.py
+-rw-r--r--   0        0        0     1827 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/services/test_errors.py
+-rw-r--r--   0        0        0    31133 2024-02-09 16:37:01.501328 bodhi_server-8.1.0/tests/services/test_overrides.py
+-rw-r--r--   0        0        0    30866 2024-02-09 16:37:01.502328 bodhi_server-8.1.0/tests/services/test_releases.py
+-rw-r--r--   0        0        0     3801 2024-02-09 16:37:01.502328 bodhi_server-8.1.0/tests/services/test_schemas.py
+-rw-r--r--   0        0        0   303697 2024-02-09 16:37:01.503328 bodhi_server-8.1.0/tests/services/test_updates.py
+-rw-r--r--   0        0        0      817 2024-02-09 16:37:01.503328 bodhi_server-8.1.0/tests/tasks/__init__.py
+-rw-r--r--   0        0        0     1531 2024-02-09 16:37:01.503328 bodhi_server-8.1.0/tests/tasks/base.py
+-rw-r--r--   0        0        0    42724 2024-02-09 16:37:01.503328 bodhi_server-8.1.0/tests/tasks/test_approve_testing.py
+-rw-r--r--   0        0        0    29342 2024-02-09 16:37:01.503328 bodhi_server-8.1.0/tests/tasks/test_check_policies.py
+-rw-r--r--   0        0        0     9679 2024-02-09 16:37:01.503328 bodhi_server-8.1.0/tests/tasks/test_check_signed_builds.py
+-rw-r--r--   0        0        0     5949 2024-02-09 16:37:01.503328 bodhi_server-8.1.0/tests/tasks/test_clean_old_composes.py
+-rw-r--r--   0        0        0   168925 2024-02-09 16:37:01.504328 bodhi_server-8.1.0/tests/tasks/test_composer.py
+-rw-r--r--   0        0        0     3792 2024-02-09 16:37:01.504328 bodhi_server-8.1.0/tests/tasks/test_expire_overrides.py
+-rw-r--r--   0        0        0     3677 2024-02-09 16:37:01.504328 bodhi_server-8.1.0/tests/tasks/test_fetch_test_cases.py
+-rw-r--r--   0        0        0     2799 2024-02-09 16:37:01.504328 bodhi_server-8.1.0/tests/tasks/test_handle_side_and_related_tags.py
+-rw-r--r--   0        0        0     2321 2024-02-09 16:37:01.504328 bodhi_server-8.1.0/tests/tasks/test_tag_update_builds.py
+-rw-r--r--   0        0        0     5085 2024-02-09 16:37:01.504328 bodhi_server-8.1.0/tests/tasks/test_work_on_bugs.py
+-rw-r--r--   0        0        0     8504 2024-04-09 11:49:25.516646 bodhi_server-8.1.0/tests/test___init__.py
+-rw-r--r--   0        0        0     2185 2024-02-09 16:37:01.504328 bodhi_server-8.1.0/tests/test_alembic.py
+-rw-r--r--   0        0        0    28061 2024-02-09 16:37:01.504328 bodhi_server-8.1.0/tests/test_bugs.py
+-rw-r--r--   0        0        0    17610 2024-02-09 16:37:01.505328 bodhi_server-8.1.0/tests/test_buildsys.py
+-rw-r--r--   0        0        0    16273 2024-02-09 16:37:01.505328 bodhi_server-8.1.0/tests/test_config.py
+-rw-r--r--   0        0        0     4319 2024-02-09 16:37:01.505328 bodhi_server-8.1.0/tests/test_logging.py
+-rw-r--r--   0        0        0    16102 2024-02-09 16:37:01.506328 bodhi_server-8.1.0/tests/test_mail.py
+-rw-r--r--   0        0        0    26451 2024-02-09 16:37:01.506328 bodhi_server-8.1.0/tests/test_metadata.py
+-rw-r--r--   0        0        0   215576 2024-02-09 16:37:01.507328 bodhi_server-8.1.0/tests/test_models.py
+-rw-r--r--   0        0        0     3897 2024-02-09 16:37:01.507328 bodhi_server-8.1.0/tests/test_notifications.py
+-rw-r--r--   0        0        0    72415 2024-02-09 16:37:01.507328 bodhi_server-8.1.0/tests/test_push.py
+-rw-r--r--   0        0        0     2238 2024-02-09 16:37:01.507328 bodhi_server-8.1.0/tests/test_renderers.py
+-rw-r--r--   0        0        0     1642 2024-02-09 16:37:01.507328 bodhi_server-8.1.0/tests/test_schemas.py
+-rw-r--r--   0        0        0     7785 2024-02-09 16:37:01.507328 bodhi_server-8.1.0/tests/test_security.py
+-rw-r--r--   0        0        0    65890 2024-03-26 07:10:28.078272 bodhi_server-8.1.0/tests/test_util.py
+-rw-r--r--   0        0        0    48619 2024-03-26 07:10:28.078272 bodhi_server-8.1.0/tests/test_validators.py
+-rw-r--r--   0        0        0     2614 2024-02-09 16:37:01.508328 bodhi_server-8.1.0/tests/test_webapp.py
+-rw-r--r--   0        0        0     4237 2024-02-09 16:37:01.508328 bodhi_server-8.1.0/tests/testing.ini
+-rw-r--r--   0        0        0      992 2024-02-09 16:37:01.508328 bodhi_server-8.1.0/tests/utils.py
+-rw-r--r--   0        0        0      817 2024-02-09 16:37:01.508328 bodhi_server-8.1.0/tests/views/__init__.py
+-rw-r--r--   0        0        0    26610 2024-03-26 07:10:28.079272 bodhi_server-8.1.0/tests/views/test_generic.py
+-rw-r--r--   0        0        0     5788 1970-01-01 00:00:00.000000 bodhi_server-8.1.0/setup.py
+-rw-r--r--   0        0        0     4206 1970-01-01 00:00:00.000000 bodhi_server-8.1.0/PKG-INFO
```

### Comparing `bodhi_server-8.0.2/COPYING` & `bodhi_server-8.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/README.rst` & `bodhi_server-8.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/alembic.ini` & `bodhi_server-8.1.0/alembic.ini`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/apache/bodhi.conf` & `bodhi_server-8.1.0/apache/bodhi.conf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/__init__.py` & `bodhi_server-8.1.0/bodhi/server/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from munch import munchify
 from pyramid.config import Configurator
 from pyramid.renderers import JSONP
 from pyramid.session import JSONSerializer, SignedCookieSessionFactory
 from pyramid.tweens import EXCVIEW
 from sqlalchemy import engine_from_config, event
 from sqlalchemy.orm import scoped_session, sessionmaker
-import pkg_resources
 
 from bodhi.server import bugs, buildsys
 from bodhi.server.config import config as bodhi_config
 from bodhi.server.security import BodhiSecurityPolicy
 
 
 METADATA = importlib.metadata.metadata('bodhi-server')
@@ -161,15 +160,25 @@
 
     Returns:
         sqlalchemy.engine: The database engine created from the configuration.
     """
     # The SQLAlchemy database engine. This is constructed using the value of
     # ``DB_URL`` in :data:`config``. Note: A copy is provided since ``engine_from_config``
     # uses ``pop``.
-    engine = engine_from_config(config.copy(), 'sqlalchemy.')
+    if config['sqlalchemy.url'].startswith('postgresql'):  # pragma: no cover
+        engine = engine_from_config(
+            config.copy(),
+            'sqlalchemy.',
+            connect_args={
+                'options': f'-c statement_timeout={config["sqlalchemy_extra.statement_timeout"]}'
+            }
+        )
+    else:
+        engine = engine_from_config(config.copy(), 'sqlalchemy.')
+
     # When using SQLite we need to make sure foreign keys are enabled:
     # http://docs.sqlalchemy.org/en/latest/dialects/sqlite.html#foreign-key-support
     if config['sqlalchemy.url'].startswith('sqlite:'):
         event.listen(
             engine,
             'connect',
             lambda db_con, con_record: db_con.execute('PRAGMA foreign_keys=ON')
@@ -234,15 +243,15 @@
     config.add_request_method(get_cacheregion, 'cache', reify=True)
     config.add_request_method(get_buildinfo, 'buildinfo', reify=True)
     config.add_request_method(get_from_tag_inherited, 'from_tag_inherited', reify=True)
     config.add_request_method(get_releases, 'releases', reify=True)
 
     # Templating
     config.add_mako_renderer('.html', settings_prefix='mako.')
-    config.add_static_view(f'static/v{pkg_resources.get_distribution("bodhi-server").version}',
+    config.add_static_view(f'static/v{__version__}',
                            'bodhi.server:static')
 
     from bodhi.server.renderers import rss
     config.add_renderer('rss', rss)
     config.add_renderer('jsonp', JSONP(param_name='callback'))
 
     # i18n
@@ -331,13 +340,10 @@
         models.Release.all_releases()
         models.Release.get_tags()
 
         # Let's warm up the home page cache by calling _generate_home_page_stats(). We can ignore
         # the return value.
         generic._generate_home_page_stats()
 
-    # Let's close out the db session we used to warm the caches.
-    Session.remove()
-
     log.info('Bodhi ready and at your service!')
     app = config.make_wsgi_app()
     return app
```

### Comparing `bodhi_server-8.0.2/bodhi/server/auth/__init__.py` & `bodhi_server-8.1.0/bodhi/server/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/auth/fedora.py` & `bodhi_server-8.1.0/bodhi/server/auth/fedora.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/auth/oauth.py` & `bodhi_server-8.1.0/bodhi/server/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/auth/oauth_015.py` & `bodhi_server-8.1.0/bodhi/server/auth/oauth_015.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/auth/oauth_1.py` & `bodhi_server-8.1.0/bodhi/server/auth/oauth_1.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/auth/utils.py` & `bodhi_server-8.1.0/bodhi/server/auth/utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/auth/views.py` & `bodhi_server-8.1.0/bodhi/server/auth/views.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/bugs.py` & `bodhi_server-8.1.0/bodhi/server/bugs.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/buildsys.py` & `bodhi_server-8.1.0/bodhi/server/buildsys.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
                    'creation_event_id': 151517,
                    'creation_time': '2007-08-24 19:38:29.422344',
                    'extra': None,
                    'epoch': None,
                    'owner_id': 388,
                    'owner_name': 'lmacken',
                    'package_id': 8,
+                   'source': 'git+https://src.fedoraproject.org/rpms/foo.git#abc',
                    'state': 1,
                    'tag_id': 19,
                    'task_id': 127621}
 
     def __init__(self):
         """Initialize the DevBuildsys."""
         self._multicall = False
@@ -206,29 +207,31 @@
             return {'name': 'gnome-backgrounds',
                     'nvr': 'gnome-backgrounds-3.0-1.fc17',
                     'package_name': 'gnome-backgrounds',
                     'release': '1.fc17',
                     'tag_name': 'f17-build-side-7777',
                     'version': '3.0',
                     'id': 16061,
-                    'task_id': 15051}
+                    'task_id': 15051,
+                    'source': 'git+https://src.fedoraproject.org/rpms/gnome-backgrounds.git#abc'}
 
         theid = 16058
         if other and not testing:
             theid = 16059
         elif other and testing:
             theid = 16060
 
         data = self._build_data.copy()
         data['id'] = theid
         if 'noowner' in build:
             del data['owner_name']
 
         name, version, release = build.rsplit("-", 2)
         release_tokens = release.split(".")
+        data['source'] = f'git+https://src.fedoraproject.org/rpms/{name}.git#abc'
 
         for token in release_tokens:
             # Starting to hardcode some dev buildsys bits for docker.
             # See https://github.com/fedora-infra/bodhi/pull/1543
             if token.endswith("container") or token.endswith("flatpak"):
                 fedora_release = "f" + (token
                                         .replace("fc", "")
@@ -243,17 +246,19 @@
                     'hash': hashlib.sha256(f"{version}-{release}".encode("UTF-8")).hexdigest(),
                     'version': version,
                     'release': release
                 }
 
                 if token.endswith("flatpak"):
                     format_data['repository'] = name
+                    data['source'] = f'git+https://src.fedoraproject.org/flatpaks/{name}.git#abc'
                 else:
                     tag = "f%s-updates-testing" % token.replace("fc", "").replace("container", "")
                     format_data['repository'] = "{}/{}".format(fedora_release, name)
+                    data['source'] = f'https://src.fedoraproject.org/container/{name}.git#abc'
 
                 data['extra'] = {
                     'typeinfo': {
                         'image': {
                             'index': {
                                 'pull': ['{registry}/{repository}@sha256:{hash}'
                                          .format(**format_data),
@@ -271,14 +276,15 @@
 
             # Hardcoding for modules in the dev buildsys
             if token.startswith("2017"):
                 tag = "f27M-updates-testing"
                 data['extra'] = {
                     'typeinfo': {'module': {'more': 'mbs stuff goes here'}}
                 }
+                data['source'] = f'https://src.fedoraproject.org/modules/{name}.git?#abc'
                 break
 
             if token.startswith("fc"):
                 if testing:
                     tag = "f%s-updates-testing" % token.replace("fc", "")
                     break
                 else:
```

### Comparing `bodhi_server-8.0.2/bodhi/server/config.py` & `bodhi_server-8.1.0/bodhi/server/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -558,14 +558,17 @@
         },
         'smtp_server': {
             'value': None,
             'validator': _validate_none_or(str)},
         'sqlalchemy.url': {
             'value': 'postgresql://localhost/bodhi',
             'validator': str},
+        'sqlalchemy_extra.statement_timeout': {
+            'value': 30000,
+            'validator': int},
         'stable_bug_msg': {
             'value': ('{update_alias} ({update_beauty_title}) has been pushed to '
                       'the {repo} repository.\n'
                       'If problem still persists, please make note of it in this bug report.'),
             'validator': str},
         'stats_blacklist': {
             'value': ['bodhi', 'anonymous'],
@@ -600,14 +603,17 @@
             'validator': int},
         'test_gating.required': {
             'value': False,
             'validator': _validate_bool},
         'test_gating.url': {
             'value': '',
             'validator': str},
+        'trusted_build_sources': {
+            'value': [],
+            'validator': _generate_list_validator()},
         'update_notes_maxlength': {
             'value': 10000,
             'validator': int},
         'updateinfo_rights': {
             'value': 'Copyright (C) {} Red Hat, Inc. and others.'.format(datetime.now().year),
             'validator': str},
         'wait_for_repo_sig': {
```

### Comparing `bodhi_server-8.0.2/bodhi/server/consumers/__init__.py` & `bodhi_server-8.1.0/bodhi/server/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/consumers/automatic_updates.py` & `bodhi_server-8.1.0/bodhi/server/consumers/automatic_updates.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/consumers/ci.py` & `bodhi_server-8.1.0/bodhi/server/consumers/ci.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/consumers/resultsdb.py` & `bodhi_server-8.1.0/bodhi/server/consumers/resultsdb.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/consumers/signed.py` & `bodhi_server-8.1.0/bodhi/server/consumers/signed.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/consumers/util.py` & `bodhi_server-8.1.0/bodhi/server/consumers/util.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/consumers/waiverdb.py` & `bodhi_server-8.1.0/bodhi/server/consumers/waiverdb.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/email/templates/fedora_epel_errata_template.tpl` & `bodhi_server-8.1.0/bodhi/server/email/templates/fedora_epel_errata_template.tpl`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/email/templates/fedora_epel_legacy_errata_template.tpl` & `bodhi_server-8.1.0/bodhi/server/email/templates/fedora_epel_legacy_errata_template.tpl`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/email/templates/fedora_errata_template.tpl` & `bodhi_server-8.1.0/bodhi/server/email/templates/fedora_errata_template.tpl`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/email/templates/fedora_modular_errata_template.tpl` & `bodhi_server-8.1.0/bodhi/server/email/templates/fedora_modular_errata_template.tpl`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/exceptions.py` & `bodhi_server-8.1.0/bodhi/server/exceptions.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/ffmarkdown.py` & `bodhi_server-8.1.0/bodhi/server/ffmarkdown.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,17 +37,14 @@
 
 if typing.TYPE_CHECKING:  # pragma: no cover
     import re  # noqa: 401
     import xml  # noqa: 401
 
 
 BUGZILLA_RE = r'([a-zA-Z]+)(#[0-9]{5,})'
-UPDATE_RE = (r'(?:(?<!\S)|('
-             + escape(config['base_address'])
-             + r'updates/))([A-Z\-]+-\d{4}-[^\W_]{10})(?:(?=[\.,;:])|(?!\S))')
 
 
 def user_url(name: str) -> str:
     """
     Return a URL to the given username.
 
     Args:
@@ -200,11 +197,19 @@
     def extendMarkdown(self, md: markdown.Markdown) -> None:
         """
         Extend markdown to add our patterns and postprocessor.
 
         Args:
             md: An instance of the Markdown class.
         """
+        # it is intentional that update_re is defined here, not in
+        # global scope at the top of this file. When testing, defining
+        # it early results in config['base_address'] being read before
+        # the test setup method has changed the config to use the
+        # values from testing.ini and the value may not be as expected
+        update_re = (r'(?:(?<!\S)|('
+                     + escape(config['base_address'])
+                     + r'updates/))([A-Z\-]+-\d{4}-[^\W_]{10})(?:(?=[\.,;:])|(?!\S))')
         md.inlinePatterns.register(MentionProcessor(MENTION_RE, md), 'mention', 175)
         md.inlinePatterns.register(BugzillaProcessor(BUGZILLA_RE, md), 'bugzilla', 175)
-        md.inlinePatterns.register(UpdateProcessor(UPDATE_RE, md), 'update', 175)
+        md.inlinePatterns.register(UpdateProcessor(update_re, md), 'update', 175)
         md.postprocessors.register(SurroundPostprocessor(md), 'surround', 175)
```

### Comparing `bodhi_server-8.0.2/bodhi/server/logging.py` & `bodhi_server-8.1.0/bodhi/server/logging.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/mail.py` & `bodhi_server-8.1.0/bodhi/server/mail.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/metadata.py` & `bodhi_server-8.1.0/bodhi/server/metadata.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/README.rst` & `bodhi_server-8.1.0/bodhi/server/migrations/README.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/__init__.py` & `bodhi_server-8.1.0/bodhi/server/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/env.py` & `bodhi_server-8.1.0/bodhi/server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/script.py.mako` & `bodhi_server-8.1.0/bodhi/server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/16864f8ff395_remove_requirements_column_from_build_.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/16864f8ff395_remove_requirements_column_from_build_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/190ba571c7d2_remove_the_batching_request_state.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/190ba571c7d2_remove_the_batching_request_state.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/19e28e9851a2_index_comment_update_id.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/19e28e9851a2_index_comment_update_id.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/1c97477e38ee_convert_br_override_notes_to_unicodetext.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/1c97477e38ee_convert_br_override_notes_to_unicodetext.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/2fc96aa44a74_drop_the_user_show_popup_column.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/2fc96aa44a74_drop_the_user_show_popup_column.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/325954bac9f7_link_testcases_to_builds.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/325954bac9f7_link_testcases_to_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/3a2e248d1757_add_the_unspecified_enum_to_updatetype.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/3a2e248d1757_add_the_unspecified_enum_to_updatetype.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/3b34650a0cf6_update_type_of_users_email_with_new_.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/3b34650a0cf6_update_type_of_users_email_with_new_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/499ac8bbe09a_remove_unused_update_sidetag_statuses.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/499ac8bbe09a_remove_unused_update_sidetag_statuses.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/559acf7e2c16_make_comments_update_not_nullable.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/559acf7e2c16_make_comments_update_not_nullable.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/5703ddfe855d_add_package_manager_and_testing_.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/5703ddfe855d_add_package_manager_and_testing_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/58b7919b942c_remove_the_updates_title_column.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/58b7919b942c_remove_the_updates_title_column.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/5c86a3f9dc03_drop_support_for_cve_tracking.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/5c86a3f9dc03_drop_support_for_cve_tracking.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/6b3eb9ae2b87_remove_unused_updatestatus_processing.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/6b3eb9ae2b87_remove_unused_updatestatus_processing.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/7ba286412ad4_drop_the_relationship_between_packages_.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/7ba286412ad4_drop_the_relationship_between_packages_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/8c4d6aad9b78_add_the_greenwave_failed_enum_to_.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/8c4d6aad9b78_add_the_greenwave_failed_enum_to_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/8e9dc57e082d_obsolete_updates_for_archived_release.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/8e9dc57e082d_obsolete_updates_for_archived_release.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/9991cf10ec50_mark_the_bugs_private_field_as_nullable.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/9991cf10ec50_mark_the_bugs_private_field_as_nullable.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/9c0a34961768_remove_the_greenwave_unsatisfied_.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/9c0a34961768_remove_the_greenwave_unsatisfied_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/__init__.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/a3580bdf5129_remove_the_ci_url_field_from_builds.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/a3580bdf5129_remove_the_ci_url_field_from_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/a418acf470f8_drop_the_stacks_table.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/a418acf470f8_drop_the_stacks_table.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/aae0d29d49b7_remove_the_private_field_on_the_bug_.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/aae0d29d49b7_remove_the_private_field_on_the_bug_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/b1fd856efcf6_add_autopush_boolean_and_stable_days_to_update.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/b1fd856efcf6_add_autopush_boolean_and_stable_days_to_update.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/bdf0e37ab793_disallow_null_values_in_stable_karma_.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/bdf0e37ab793_disallow_null_values_in_stable_karma_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/c60d95eef4f1_add_frozen_release_state.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/c60d95eef4f1_add_frozen_release_state.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/c98beb4940b5_remove_the_comments_anonymous_column.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/c98beb4940b5_remove_the_comments_anonymous_column.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/d399493275b6_add_the_eol_column.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/d399493275b6_add_the_eol_column.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/d3f8bd499ecd_add_from_tag_column_to_updates.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/d3f8bd499ecd_add_from_tag_column_to_updates.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/d986618207bc_add_composed_by_bodhi_flag_to_releases_.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/d986618207bc_add_composed_by_bodhi_flag_to_releases_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/e3988e00b338_drop_date_pushed.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/e3988e00b338_drop_date_pushed.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/e5b3ddb35df3_remove_the_greenwave_summary_string_.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/e5b3ddb35df3_remove_the_greenwave_summary_string_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/e8a059156d38_add_the_create_automatic_updates_bool_.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/e8a059156d38_add_the_create_automatic_updates_bool_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/eec610d7ab3a_index_the_builds_update_id_column.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/eec610d7ab3a_index_the_builds_update_id_column.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/f393d006559b_add_critpath_groups_to_update.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/f393d006559b_add_critpath_groups_to_update.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/f50dc199039c_make_comments_user_id_not_nullable.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/f50dc199039c_make_comments_user_id_not_nullable.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/f660455231d4_add_released_on_to_release.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/f660455231d4_add_released_on_to_release.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/f8a44498c806_remove_legacy_old_updateid.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/f8a44498c806_remove_legacy_old_updateid.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/migrations/versions/ff834fa4f23e_increase_the_update_alias_size.py` & `bodhi_server-8.1.0/bodhi/server/migrations/versions/ff834fa4f23e_increase_the_update_alias_size.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/models.py` & `bodhi_server-8.1.0/bodhi/server/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Bodhi's database models."""
 
 from collections import defaultdict
 from datetime import date, datetime, timedelta
 from functools import lru_cache
 from textwrap import wrap
+from urllib.parse import urljoin
 import hashlib
 import json
-import os
 import re
 import time
 import typing
 import uuid
 
 from mediawiki import MediaWiki
 from packaging.version import parse as parse_version
@@ -3417,27 +3417,25 @@
     def get_url(self):
         """
         Return the relative URL to this update.
 
         Returns:
             str: A URL.
         """
-        path = ['updates']
-        path.append(self.alias)
-        return os.path.join(*path)
+        return f'updates/{self.alias}'
 
     def abs_url(self, request=None):
         """
         Return the absolute URL to this update.
 
         Args:
             request (pyramid.request.Request or None): The current web request. Unused.
         """
         base = config['base_address']
-        return os.path.join(base, self.get_url())
+        return urljoin(base, self.get_url())
 
     url = abs_url
 
     def __str__(self):
         """
         Return a string representation of this update.
```

### Comparing `bodhi_server-8.0.2/bodhi/server/notifications.py` & `bodhi_server-8.1.0/bodhi/server/notifications.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/push.py` & `bodhi_server-8.1.0/bodhi/server/push.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/renderers.py` & `bodhi_server-8.1.0/bodhi/server/renderers.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/schemas.py` & `bodhi_server-8.1.0/bodhi/server/schemas.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/scripts/__init__.py` & `bodhi_server-8.1.0/bodhi/server/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/scripts/bshell.py` & `bodhi_server-8.1.0/bodhi/server/scripts/bshell.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/scripts/compat.py` & `bodhi_server-8.1.0/bodhi/server/scripts/compat.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/scripts/initializedb.py` & `bodhi_server-8.1.0/bodhi/server/scripts/initializedb.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/scripts/sar.py` & `bodhi_server-8.1.0/bodhi/server/scripts/sar.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/scripts/untag_branched.py` & `bodhi_server-8.1.0/bodhi/server/scripts/untag_branched.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/security.py` & `bodhi_server-8.1.0/bodhi/server/security.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/services/__init__.py` & `bodhi_server-8.1.0/bodhi/server/services/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/services/builds.py` & `bodhi_server-8.1.0/bodhi/server/services/builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/services/comments.py` & `bodhi_server-8.1.0/bodhi/server/services/comments.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/services/composes.py` & `bodhi_server-8.1.0/bodhi/server/services/composes.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/services/csrf.py` & `bodhi_server-8.1.0/bodhi/server/services/csrf.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/services/errors.py` & `bodhi_server-8.1.0/bodhi/server/services/errors.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/services/markdown.py` & `bodhi_server-8.1.0/bodhi/server/services/markdown.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/services/metrics_tween.py` & `bodhi_server-8.1.0/bodhi/server/services/metrics_tween.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/services/overrides.py` & `bodhi_server-8.1.0/bodhi/server/services/overrides.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/services/packages.py` & `bodhi_server-8.1.0/bodhi/server/services/packages.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/services/releases.py` & `bodhi_server-8.1.0/bodhi/server/services/releases.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,17 @@
                   cors_origins=bodhi.server.security.cors_origins_ro)
 releases = Service(name='releases', path='/releases/',
                    description='Fedora Releases',
                    factory=security.AdminACLFactory,
                    # Note, this 'rw' is not a typo. The @releases service has
                    # a ``post`` section at the bottom.
                    cors_origins=bodhi.server.security.cors_origins_rw)
+list_releases = Service(name='list_releases', path='/list_releases/',
+                        description='Fedora Releases',
+                        cors_origins=bodhi.server.security.cors_origins_ro)
 
 
 @release.get(accept="text/html", renderer="release.html",
              error_handler=bodhi.server.services.errors.html_handler)
 def get_release_html(request):
     """
     Render a release given by id as HTML.
@@ -277,14 +280,18 @@
         for release in (releases['current'] + releases['pending'] + releases['frozen']):
             release_updates_counts[release["name"]] = get_update_counts(release["name"])
 
     return {"release_updates_counts": release_updates_counts,
             "active": active}
 
 
+@list_releases.get(accept=('application/json', 'text/json'),
+                   schema=bodhi.server.schemas.ListReleaseSchema(), renderer='json',
+                   error_handler=bodhi.server.services.errors.json_handler,
+                   validators=releases_get_validators)
 @releases.get(accept=('application/json', 'text/json'),
               schema=bodhi.server.schemas.ListReleaseSchema(), renderer='json',
               error_handler=bodhi.server.services.errors.json_handler,
               validators=releases_get_validators)
 def query_releases_json(request):
     """
     Search releases by given criteria, returning the results as JSON.
```

### Comparing `bodhi_server-8.0.2/bodhi/server/services/schemas.py` & `bodhi_server-8.1.0/bodhi/server/services/schemas.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Defines service endpoints for our message schemas."""
 
+from importlib import metadata
 import typing
 
 from cornice.resource import resource, view
 from pyramid import httpexceptions
 from pyramid.authorization import Allow, Everyone
-import pkg_resources
 
 from bodhi.server import security
 from bodhi.server.services import errors
 
 
 if typing.TYPE_CHECKING:  # pragma: no cover
     import pyramid.request.Request  # noqa: 401
@@ -74,29 +74,29 @@
         List schemas.
 
         This method responds to the ``/message-schemas/v1/`` endpoint.
 
         Returns:
             A list of message topics that Bodhi supports.
         """
-        return [m.load().topic for m in pkg_resources.iter_entry_points('fedora.messages')
-                if m.module_name.startswith('bodhi.')]
+        return [m.load().topic for m in metadata.entry_points(group='fedora.messages')
+                if m.value.startswith('bodhi.')]
 
     @view(accept=('application/json', 'text/json'), renderer='json',
           cors_origins=security.cors_origins_ro, error_handler=errors.json_handler,
           permission=READ_ACL)
     def get(self) -> dict:
         """
         Retrieve and render a single message schema.
 
         This API responses to the ``/message_schemas/v1/<topic>`` endpoint.
 
         Returns:
             The requested message schema.
         """
         try:
-            return pkg_resources.load_entry_point(
-                'bodhi-messages', 'fedora.messages',
-                f"{self.request.matchdict['topic']}.v1").body_schema
-        except ImportError:
+            (ep,) = metadata.entry_points(group='fedora.messages',
+                                          name=f"{self.request.matchdict['topic']}.v1")
+            return ep.load().body_schema
+        except ValueError:
             # The user has requested a topic that does not exist
             raise httpexceptions.HTTPNotFound()
```

### Comparing `bodhi_server-8.0.2/bodhi/server/services/updates.py` & `bodhi_server-8.1.0/bodhi/server/services/updates.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/services/user.py` & `bodhi_server-8.1.0/bodhi/server/services/user.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/__init__.py` & `bodhi_server-8.1.0/bodhi/server/static/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/bodhi-logo.svg` & `bodhi_server-8.1.0/bodhi/server/static/bodhi-logo.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/css/site.css` & `bodhi_server-8.1.0/bodhi/server/static/css/site.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/font-awesome/FontAwesome.otf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/font-awesome/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.eot` & `bodhi_server-8.1.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.svg` & `bodhi_server-8.1.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.ttf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff` & `bodhi_server-8.1.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff2` & `bodhi_server-8.1.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/font-awesome.css` & `bodhi_server-8.1.0/bodhi/server/static/fonts/font-awesome.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/hack-bold-webfont.eot` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/hack-bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/hack-bolditalic-webfont.eot` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/hack-bolditalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/hack-italic-webfont.eot` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/hack-italic-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/hack-regular-webfont.eot` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/hack-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/latin/hack-bold-latin-webfont.eot` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/latin/hack-bold-latin-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/latin/hack-bolditalic-latin-webfont.eot` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/latin/hack-bolditalic-latin-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/latin/hack-italic-latin-webfont.eot` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/latin/hack-italic-latin-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/eot/latin/hack-regular-latin-webfont.eot` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/eot/latin/hack-regular-latin-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/hack-bold-webfont.ttf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/hack-bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/hack-bolditalic-webfont.ttf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/hack-bolditalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/hack-italic-webfont.ttf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/hack-italic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/hack-regular-webfont.ttf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/hack-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bold-latin-webfont.ttf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bold-latin-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bolditalic-latin-webfont.ttf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bolditalic-latin-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/latin/hack-italic-latin-webfont.ttf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-italic-latin-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/web-ttf/latin/hack-regular-latin-webfont.ttf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-regular-latin-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/hack-bold-webfont.woff` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/hack-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/hack-bolditalic-webfont.woff` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/hack-bolditalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/hack-italic-webfont.woff` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/hack-italic-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/hack-regular-webfont.woff` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/hack-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/latin/hack-bold-latin-webfont.woff` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/latin/hack-bold-latin-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/latin/hack-bolditalic-latin-webfont.woff` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/latin/hack-bolditalic-latin-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/latin/hack-italic-latin-webfont.woff` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/latin/hack-italic-latin-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff/latin/hack-regular-latin-webfont.woff` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff/latin/hack-regular-latin-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/hack-bold-webfont.woff2` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/hack-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/hack-bolditalic-webfont.woff2` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/hack-bolditalic-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/hack-italic-webfont.woff2` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/hack-italic-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/hack-regular-webfont.woff2` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/hack-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/latin/hack-bold-latin-webfont.woff2` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/latin/hack-bold-latin-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/latin/hack-bolditalic-latin-webfont.woff2` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/latin/hack-bolditalic-latin-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/latin/hack-italic-latin-webfont.woff2` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/latin/hack-italic-latin-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack/woff2/latin/hack-regular-latin-webfont.woff2` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack/woff2/latin/hack-regular-latin-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/hack.css` & `bodhi_server-8.1.0/bodhi/server/static/fonts/hack.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.eot` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.svg` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.ttf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff2` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.eot` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.svg` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.ttf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff2` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.eot` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.svg` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.ttf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff2` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.eot` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.svg` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.ttf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff2` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.eot` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.svg` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.ttf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff2` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.eot` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.svg` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.ttf` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff2` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/fonts/open-sans.css` & `bodhi_server-8.1.0/bodhi/server/static/fonts/open-sans.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/ico/favicon.ico` & `bodhi_server-8.1.0/bodhi/server/static/ico/favicon.ico`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/img/bodhi-logo.png` & `bodhi_server-8.1.0/bodhi/server/static/img/bodhi-logo.png`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/img/bodhi-logo.svg` & `bodhi_server-8.1.0/bodhi/server/static/img/bodhi-logo.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/img/logo-large.png` & `bodhi_server-8.1.0/bodhi/server/static/img/logo-large.png`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/img/logo.png` & `bodhi_server-8.1.0/bodhi/server/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/js/comment_form.js` & `bodhi_server-8.1.0/bodhi/server/static/js/comment_form.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/js/forms.js` & `bodhi_server-8.1.0/bodhi/server/static/js/forms.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/js/override_form.js` & `bodhi_server-8.1.0/bodhi/server/static/js/override_form.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/js/search.js` & `bodhi_server-8.1.0/bodhi/server/static/js/search.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/js/site.js` & `bodhi_server-8.1.0/bodhi/server/static/js/site.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/js/update_form.js` & `bodhi_server-8.1.0/bodhi/server/static/js/update_form.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/chartjs/chart.min.js` & `bodhi_server-8.1.0/bodhi/server/static/vendor/chartjs/chart.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css` & `bodhi_server-8.1.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css.map` & `bodhi_server-8.1.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js` & `bodhi_server-8.1.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js.map` & `bodhi_server-8.1.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.js` & `bodhi_server-8.1.0/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.map` & `bodhi_server-8.1.0/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.css` & `bodhi_server-8.1.0/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.js` & `bodhi_server-8.1.0/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/css/messenger-spinner.css` & `bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/css/messenger-spinner.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/css/messenger-theme-air.css` & `bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/css/messenger-theme-air.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/css/messenger-theme-block.css` & `bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/css/messenger-theme-block.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/css/messenger-theme-flat.css` & `bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/css/messenger-theme-flat.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/css/messenger-theme-future.css` & `bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/css/messenger-theme-future.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/css/messenger-theme-ice.css` & `bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/css/messenger-theme-ice.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/css/messenger.css` & `bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/css/messenger.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/js/messenger-theme-flat.js` & `bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/js/messenger-theme-flat.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/js/messenger-theme-future.js` & `bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/js/messenger-theme-future.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/js/messenger.js` & `bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/js/messenger.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/messenger/js/messenger.min.js` & `bodhi_server-8.1.0/bodhi/server/static/vendor/messenger/js/messenger.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/moment/moment.min.js` & `bodhi_server-8.1.0/bodhi/server/static/vendor/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/selectize/selectize-0.14.0.min.js` & `bodhi_server-8.1.0/bodhi/server/static/vendor/selectize/selectize-0.14.0.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/selectize/selectize-0.15.2.js` & `bodhi_server-8.1.0/bodhi/server/static/vendor/selectize/selectize-0.15.2.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/selectize/selectize-0.15.2.min.js` & `bodhi_server-8.1.0/bodhi/server/static/vendor/selectize/selectize-0.15.2.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.14.0.css` & `bodhi_server-8.1.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.14.0.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.2.css` & `bodhi_server-8.1.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.2.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/static/vendor/typeahead/typeahead.bundle.js` & `bodhi_server-8.1.0/bodhi/server/static/vendor/typeahead/typeahead.bundle.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/tasks/__init__.py` & `bodhi_server-8.1.0/bodhi/server/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/tasks/approve_testing.py` & `bodhi_server-8.1.0/bodhi/server/tasks/approve_testing.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/tasks/check_policies.py` & `bodhi_server-8.1.0/bodhi/server/tasks/check_policies.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/tasks/check_signed_builds.py` & `bodhi_server-8.1.0/bodhi/server/tasks/check_signed_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/tasks/clean_old_composes.py` & `bodhi_server-8.1.0/bodhi/server/tasks/clean_old_composes.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/tasks/composer.py` & `bodhi_server-8.1.0/bodhi/server/tasks/composer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1160,20 +1160,22 @@
 
         for arch in arches:
             # sanity check our repodata
             try:
                 if arch == 'source':
                     repodata = os.path.join(self.path, 'compose',
                                             'Everything', arch, 'tree', 'repodata')
-                    sanity_check_repodata(repodata, repo_type='source')
+                    sanity_check_repodata(repodata, repo_type='source', drpms=False)
                 else:
                     repodata = os.path.join(self.path, 'compose',
                                             'Everything', arch, 'os', 'repodata')
                     repo_type = 'module' if self.ctype == ContentType.module else 'yum'
-                    sanity_check_repodata(repodata, repo_type=repo_type)
+                    drpms = get_createrepo_config(self.compose.release).get('drpms_enabled')
+                    # for module repos drpms is not considered
+                    sanity_check_repodata(repodata, repo_type=repo_type, drpms=drpms)
             except Exception:
                 log.exception("Repodata sanity check failed, compose thrown out")
                 self._toss_out_repo()
                 raise
 
             # make sure that pungi didn't symlink our packages
             try:
```

### Comparing `bodhi_server-8.0.2/bodhi/server/tasks/expire_overrides.py` & `bodhi_server-8.1.0/bodhi/server/tasks/expire_overrides.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/tasks/fetch_test_cases.py` & `bodhi_server-8.1.0/bodhi/server/tasks/fetch_test_cases.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/tasks/handle_side_and_related_tags.py` & `bodhi_server-8.1.0/bodhi/server/tasks/handle_side_and_related_tags.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/tasks/tag_update_builds.py` & `bodhi_server-8.1.0/bodhi/server/tasks/tag_update_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/tasks/work_on_bugs.py` & `bodhi_server-8.1.0/bodhi/server/tasks/work_on_bugs.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/templates/comments.html` & `bodhi_server-8.1.0/bodhi/server/templates/comments.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/templates/compose.html` & `bodhi_server-8.1.0/bodhi/server/templates/compose.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/templates/composes.html` & `bodhi_server-8.1.0/bodhi/server/templates/composes.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/templates/fragments.html` & `bodhi_server-8.1.0/bodhi/server/templates/fragments.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/templates/home.html` & `bodhi_server-8.1.0/bodhi/server/templates/home.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/templates/master.html` & `bodhi_server-8.1.0/bodhi/server/templates/master.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/templates/new_update.html` & `bodhi_server-8.1.0/bodhi/server/templates/new_update.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/templates/override.html` & `bodhi_server-8.1.0/bodhi/server/templates/override.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/templates/overrides.html` & `bodhi_server-8.1.0/bodhi/server/templates/overrides.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/templates/pager.html` & `bodhi_server-8.1.0/bodhi/server/templates/pager.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/templates/release.html` & `bodhi_server-8.1.0/bodhi/server/templates/release.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/templates/releases.html` & `bodhi_server-8.1.0/bodhi/server/templates/releases.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/templates/update.html` & `bodhi_server-8.1.0/bodhi/server/templates/update.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/templates/updates.html` & `bodhi_server-8.1.0/bodhi/server/templates/updates.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/templates/user.html` & `bodhi_server-8.1.0/bodhi/server/templates/user.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/util.py` & `bodhi_server-8.1.0/bodhi/server/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,20 +47,19 @@
 import bleach
 import colander
 import libcomps
 import libravatar
 import librepo
 import markdown
 import packaging
-import pkg_resources
 import requests
 import rpm
 import zstandard
 
-from bodhi.server import ffmarkdown, log, buildsys, Session
+from bodhi.server import __version__, ffmarkdown, log, buildsys, Session
 from bodhi.server.config import config
 from bodhi.server.exceptions import RepodataException
 
 
 _ = TranslationStringFactory('bodhi')
 
 http_session = requests.Session()
@@ -266,22 +265,23 @@
     # not take our request into account.
     if components is not None:
         critpath_components = [c for c in critpath_components if c in components]
 
     return critpath_components
 
 
-def sanity_check_repodata(myurl, repo_type):
+def sanity_check_repodata(myurl, repo_type, drpms=True):
     """
     Sanity check the repodata for a given repository.
 
     Args:
         myurl (str): A path to a repodata directory.
         repo_type (str): This should be set to 'yum' for Yum repositories, 'module' for module
             repositories, or 'source' for source repositories.
+        drpms (bool): A boolean to express if DRPMs generation is enabled.
     Raises:
         RepodataException: If the repodata is not valid or does not exist.
         ValueError: If repo_type is not an acceptable value.
     """
     if repo_type not in ('module', 'source', 'yum'):
         raise ValueError('repo_type must be one of module, source, or yum.')
 
@@ -308,15 +308,16 @@
             rc, msg, general_msg = e.args
             raise RepodataException(msg)
 
         repo_info = r.getinfo(librepo.LRR_YUM_REPO)
         reqparts = ['filelists', 'primary', 'repomd', 'updateinfo']
         # Source and module repos don't have DRPMs.
         if repo_type == 'yum':
-            reqparts.append('prestodelta')
+            if drpms:
+                reqparts.append('prestodelta')
             reqparts.append('group')
         elif repo_type == 'module':
             reqparts.append('modules')
         missing = []
         for part in reqparts:
             if part not in repo_info:
                 missing.append(part)
@@ -506,15 +507,15 @@
     Return the Bodhi server's version.
 
     Args:
         context (mako.runtime.Context or None): Unused. Defaults to None.
     Returns:
         str: The Bodhi server's version.
     """
-    return pkg_resources.get_distribution('bodhi-server').version
+    return __version__
 
 
 def hostname(context=None):
     """
     Return the Bodhi server's hostname.
 
     Args:
@@ -546,16 +547,15 @@
         "b", "i", "strong", "em", "tt",
         "p", "br",
         "span", "div", "blockquote", "code", "hr", "pre",
         "ul", "ol", "li", "dd", "dt",
         "img",
         "a",
     ]
-    bleach_v = pkg_resources.get_distribution('bleach').version
-    if packaging.version.parse(bleach_v) >= packaging.version.parse("6.0.0"):
+    if packaging.version.parse(bleach.__version__) >= packaging.version.parse("6.0.0"):
         markdown_tags = set(markdown_tags)
 
     extensions = ['markdown.extensions.fenced_code', ]
     if bodhi is True:
         extensions.append(ffmarkdown.BodhiExtension())
     markdown_text = markdown.markdown(text, extensions=extensions)
 
@@ -1362,37 +1362,49 @@
             configfile = None
             log.error(f'Error reading {configpath}.')
     if not configfile:
         log.warning('No createrepo_c config file found.')
         return munchify({'uinfo_comp': 'XZ',
                          'repodata_comp': '',
                          'general_comp': False,
-                         'zchunk': True})
+                         'zchunk': True,
+                         'drpms_enabled': True,
+                         'sqlite_enabled': True,
+                         'compatibility': False})
     if f'release.{rel.name}' in configfile.sections():
         log.info(f'Using custom createrepo_c config for {rel.name}.')
         return munchify(
             {'uinfo_comp': configfile[f'release.{rel.name}'].get('updateinfo-compress-type'),
              'repodata_comp':
                  configfile[f'release.{rel.name}'].get('repodata-compress-type', None),
              'general_comp': configfile[f'release.{rel.name}'].getboolean('general-compress'),
-             'zchunk': configfile[f'release.{rel.name}'].getboolean('zchunk')
+             'zchunk': configfile[f'release.{rel.name}'].getboolean('zchunk'),
+             'drpms_enabled': configfile[f'release.{rel.name}'].getboolean('drpms_enabled'),
+             'sqlite_enabled': configfile[f'release.{rel.name}'].getboolean('sqlite_enabled'),
+             'compatibility': configfile[f'release.{rel.name}'].getboolean('compatibility')
              }
         )
     elif f'prefix.{rel.id_prefix}' in configfile.sections():
         log.info(f'Using custom createrepo_c config for {rel.id_prefix}.')
         return munchify(
             {'uinfo_comp': configfile[f'prefix.{rel.id_prefix}'].get('updateinfo-compress-type'),
              'repodata_comp':
                  configfile[f'prefix.{rel.id_prefix}'].get('repodata-compress-type', None),
              'general_comp': configfile[f'prefix.{rel.id_prefix}'].getboolean('general-compress'),
-             'zchunk': configfile[f'prefix.{rel.id_prefix}'].getboolean('zchunk')
+             'zchunk': configfile[f'prefix.{rel.id_prefix}'].getboolean('zchunk'),
+             'drpms_enabled': configfile[f'prefix.{rel.id_prefix}'].getboolean('drpms_enabled'),
+             'sqlite_enabled': configfile[f'prefix.{rel.id_prefix}'].getboolean('sqlite_enabled'),
+             'compatibility': configfile[f'prefix.{rel.id_prefix}'].getboolean('compatibility')
              }
         )
     else:
         log.info('Using createrepo_c defaults config.')
         return munchify(
             {'uinfo_comp': configfile['DEFAULT'].get('updateinfo-compress-type'),
              'repodata_comp': configfile['DEFAULT'].get('repodata-compress-type', None),
              'general_comp': configfile['DEFAULT'].getboolean('general-compress'),
-             'zchunk': configfile['DEFAULT'].getboolean('zchunk')
+             'zchunk': configfile['DEFAULT'].getboolean('zchunk'),
+             'drpms_enabled': configfile['DEFAULT'].getboolean('drpms_enabled'),
+             'sqlite_enabled': configfile['DEFAULT'].getboolean('sqlite_enabled'),
+             'compatibility': configfile['DEFAULT'].getboolean('compatibility')
              }
         )
```

### Comparing `bodhi_server-8.0.2/bodhi/server/validators.py` & `bodhi_server-8.1.0/bodhi/server/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,27 +195,36 @@
     """
     Ensure that the given builds reference valid Build objects.
 
     Args:
         request (pyramid.request.Request): The current request.
         kwargs (dict): The kwargs of the related service definition. Unused.
     """
+    trusted_sources = config.get('trusted_build_sources', [])
+
     for build in request.validated.get('builds') or []:  # cope with builds being None
         try:
             cache_nvrs(request, build)
             if request.validated.get('from_tag'):
                 n, v, r = request.buildinfo[build]['nvr']
                 release = request.db.query(Release).filter(or_(Release.name == r,
                                                                Release.name == r.upper(),
                                                                Release.version == r)).first()
                 if release and release.composed_by_bodhi:
                     request.errors.add(
                         'body', 'builds',
                         f"Can't create update from tag for release"
                         f" '{release.name}' composed by Bodhi.")
+
+            if trusted_sources:
+                build_source = request.buildinfo[build]['info']['source']
+                if not any(build_source.startswith(source) for source in trusted_sources):
+                    request.validated['builds'] = []
+                    request.errors.add('body', 'builds',
+                                       f'{build} was not built from an allowed source')
         except ValueError:
             request.validated['builds'] = []
             request.errors.add('body', 'builds', 'Build does not exist: %s' % build)
             return
         except koji.GenericError:
             log.exception("Error retrieving koji build for %s" % build)
             request.validated['builds'] = []
@@ -605,14 +614,22 @@
                     # Just log it.
                     log.warning(f'Unable to retrieve committers list from Pagure '
                                 f'for {package.name}.')
         elif acl_system == 'dummy':
             committers = ['ralph', 'bowlofeggs', 'guest']
             if config['acl_dummy_committer']:
                 committers.append(config['acl_dummy_committer'])
+            # let's also assume the update's owner can edit it
+            update = request.validated.get('update')
+            if not update:
+                alias = request.validated.get('edited')
+                if alias:
+                    update = Update.get(alias)
+            if update:
+                committers.append(update.user.name)
             if user.name in committers:
                 has_access = True
             people = committers
         else:
             log.warning('No acl_system configured')
             people = None
```

### Comparing `bodhi_server-8.0.2/bodhi/server/views/__init__.py` & `bodhi_server-8.1.0/bodhi/server/views/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/views/generic.py` & `bodhi_server-8.1.0/bodhi/server/views/generic.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/bodhi/server/webapp.py` & `bodhi_server-8.1.0/bodhi/server/webapp.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/celeryconfig.py` & `bodhi_server-8.1.0/celeryconfig.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/docs/Makefile` & `bodhi_server-8.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/docs/conf.py` & `bodhi_server-8.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/docs/man_pages/bodhi-push.rst` & `bodhi_server-8.1.0/docs/man_pages/bodhi-push.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/docs/man_pages/bodhi-sar.rst` & `bodhi_server-8.1.0/docs/man_pages/bodhi-sar.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/docs/man_pages/bodhi-shell.rst` & `bodhi_server-8.1.0/docs/man_pages/bodhi-shell.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/docs/man_pages/bodhi-untag-branched.rst` & `bodhi_server-8.1.0/docs/man_pages/bodhi-untag-branched.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/docs/man_pages/initialize_bodhi_db.rst` & `bodhi_server-8.1.0/docs/man_pages/initialize_bodhi_db.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/production.ini` & `bodhi_server-8.1.0/production.ini`

 * *Files 2% similar despite different names*

```diff
@@ -274,14 +274,16 @@
 ##
 
 # What buildsystem do we want to use?  For development, we'll use a fake
 # buildsystem that always does what we tell it to do.  For production, we'll
 # want to use 'koji'.
 # buildsystem = dev
 
+# trusted_build_sources = git+https://src.fedoraproject.org/,https://src.fedoraproject.org/
+
 # The base URL to Koji, used to construct HTML links to Koji builds in the web UI
 # koji_web_url = https://koji.fedoraproject.org/koji/
 
 # Koji's XML-RPC hub
 # koji_hub = https://koji.stg.fedoraproject.org/kojihub
 
 
@@ -524,14 +526,15 @@
 
 ##
 ## Database
 ##
 # This must be a PostgreSQL database. You can encode a username and password in the URL. For
 # example, postgresql://username:password@hostname/database_name
 # sqlalchemy.url = postgresql://localhost/bodhi
+# sqlalchemy_extra.statement_timeout = 30000
 
 ##
 ## Templates
 ##
 # Where Bodhi's templates are stored. You likely don't want or need to adjust this setting.
 # mako.directories = bodhi.server:templates
```

#### html2text {}

```diff
@@ -157,17 +157,18 @@
 dogpile.cache.dbm # dogpile.cache.expiration_time = 100 #
 dogpile.cache.arguments.filename = /var/cache/bodhi-dogpile-cache.dbm # If True
 (the default), warm up caches when the Bodhi process starts up. Otherwise, they
 will get warmed # on first use. # warm_cache_on_start = True # Exclude sending
 emails to these users # exclude_mail = bodhi ## ## Buildsystem settings ## #
 What buildsystem do we want to use? For development, we'll use a fake #
 buildsystem that always does what we tell it to do. For production, we'll #
-want to use 'koji'. # buildsystem = dev # The base URL to Koji, used to
-construct HTML links to Koji builds in the web UI # koji_web_url = https://
-koji.fedoraproject.org/koji/ # Koji's XML-RPC hub # koji_hub = https://
+want to use 'koji'. # buildsystem = dev # trusted_build_sources = git+https://
+src.fedoraproject.org/,https://src.fedoraproject.org/ # The base URL to Koji,
+used to construct HTML links to Koji builds in the web UI # koji_web_url =
+https://koji.fedoraproject.org/koji/ # Koji's XML-RPC hub # koji_hub = https://
 koji.stg.fedoraproject.org/kojihub # URL of where users should go to set up
 their notifications # fmn_url = https://apps.fedoraproject.org/notifications/ #
 Koji krb5 # krb_principal = # krb_keytab = # krb_ccache= ## ## ACL system ##
 Choices are 'pagure', which will query the pagure_url below, or 'dummy', which
 will ## always return guest credentials (used for local development). ## #
 acl_system = dummy # Add your username here to enable ACL rights in the
 development environment. Only has an effect if # you are using the dummy
@@ -282,35 +283,35 @@
 cors_connect_src = https://*.fedoraproject.org/ wss://hub.fedoraproject.org:
 9939/ ## ## Pyramid settings ## pyramid.reload_templates = false
 pyramid.debug_authorization = false pyramid.debug_notfound = false
 pyramid.debug_routematch = false pyramid.default_locale_name = en
 debugtoolbar.hosts = 127.0.0.1 ::1 ## ## Database ## # This must be a
 PostgreSQL database. You can encode a username and password in the URL. For #
 example, postgresql://username:password@hostname/database_name # sqlalchemy.url
-= postgresql://localhost/bodhi ## ## Templates ## # Where Bodhi's templates are
-stored. You likely don't want or need to adjust this setting. #
-mako.directories = bodhi.server:templates ## ## Authentication & Sessions ## #
-CHANGE THESE IN PRODUCTION! # authtkt.secret = CHANGEME # session.secret =
-CHANGEME # authtkt.secure = True # How long should an authorization ticket be
-valid for, in seconds? Defaults to one day. # authtkt.timeout = 86400 #
-pyramid_beaker session.type = file session.data_dir = %(here)s/data/sessions/
-data session.lock_dir = %(here)s/data/sessions/lock session.key = mykey
-session.cookie_on_exception = true # Tell the browser to only send the cookie
-over TLS session.secure = true # Create a cookie that is only valid for one day
-session.timeout = 86400 cache.regions = default_term, second, short_term,
-long_term cache.type = memory cache.second.expire = 1 cache.short_term.expire =
-60 cache.default_term.expire = 300 cache.long_term.expire = 3600 # Celery
-configuration file celery_config = /etc/bodhi/celeryconfig.py [server:main] use
-= egg:waitress#main host = 0.0.0.0 port = 6543 [pshell] m = bodhi.server.models
-#db = bodhi.server.util.pshell_db t = transaction # Begin logging configuration
-[loggers] keys = root, bodhi, sqlalchemy, celery, celery_worker_job [handlers]
-keys = console [formatters] keys = generic [logger_root] level = INFO handlers
-= console [logger_bodhi] level = DEBUG handlers = qualname = bodhi
-[logger_sqlalchemy] level = INFO handlers = qualname = sqlalchemy.engine #
-"level = INFO" logs SQL queries. # "level = DEBUG" logs SQL queries and
-results. # "level = WARN" logs neither. (Recommended for production systems.)
-[logger_celery] level = INFO handlers = qualname = celery
-[logger_celery_worker_job] level = ERROR handlers = qualname =
-celery.worker.job propagate = 1 [handler_console] class = StreamHandler args =
-(sys.stderr,) level = NOTSET formatter = generic [formatter_generic] format = %
-(asctime)s %(levelname)-5.5s [%(name)s][%(threadName)s] %(message)s # End
+= postgresql://localhost/bodhi # sqlalchemy_extra.statement_timeout = 30000 ##
+## Templates ## # Where Bodhi's templates are stored. You likely don't want or
+need to adjust this setting. # mako.directories = bodhi.server:templates ## ##
+Authentication & Sessions ## # CHANGE THESE IN PRODUCTION! # authtkt.secret =
+CHANGEME # session.secret = CHANGEME # authtkt.secure = True # How long should
+an authorization ticket be valid for, in seconds? Defaults to one day. #
+authtkt.timeout = 86400 # pyramid_beaker session.type = file session.data_dir =
+%(here)s/data/sessions/data session.lock_dir = %(here)s/data/sessions/lock
+session.key = mykey session.cookie_on_exception = true # Tell the browser to
+only send the cookie over TLS session.secure = true # Create a cookie that is
+only valid for one day session.timeout = 86400 cache.regions = default_term,
+second, short_term, long_term cache.type = memory cache.second.expire = 1
+cache.short_term.expire = 60 cache.default_term.expire = 300
+cache.long_term.expire = 3600 # Celery configuration file celery_config = /etc/
+bodhi/celeryconfig.py [server:main] use = egg:waitress#main host = 0.0.0.0 port
+= 6543 [pshell] m = bodhi.server.models #db = bodhi.server.util.pshell_db t =
+transaction # Begin logging configuration [loggers] keys = root, bodhi,
+sqlalchemy, celery, celery_worker_job [handlers] keys = console [formatters]
+keys = generic [logger_root] level = INFO handlers = console [logger_bodhi]
+level = DEBUG handlers = qualname = bodhi [logger_sqlalchemy] level = INFO
+handlers = qualname = sqlalchemy.engine # "level = INFO" logs SQL queries. #
+"level = DEBUG" logs SQL queries and results. # "level = WARN" logs neither.
+(Recommended for production systems.) [logger_celery] level = INFO handlers =
+qualname = celery [logger_celery_worker_job] level = ERROR handlers = qualname
+= celery.worker.job propagate = 1 [handler_console] class = StreamHandler args
+= (sys.stderr,) level = NOTSET formatter = generic [formatter_generic] format =
+%(asctime)s %(levelname)-5.5s [%(name)s][%(threadName)s] %(message)s # End
 logging configuration
```

### Comparing `bodhi_server-8.0.2/pyproject.toml` & `bodhi_server-8.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bodhi-server"
-version = "8.0.2"
+version = "8.1.0"
 description = "Bodhi server"
 readme = "README.rst"
 authors = ["Fedora Infrastructure Team"]
 maintainers = ["Fedora Infrastructure Team <infrastructure@lists.fedoraproject.org>"]
 repository = "https://github.com/fedora-infra/bodhi"
 homepage = "https://bodhi.fedoraproject.rog"
 keywords = ["web", "fedora", "pyramid"]
```

### Comparing `bodhi_server-8.0.2/tests/__init__.py` & `bodhi_server-8.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/auth/test_fedora.py` & `bodhi_server-8.1.0/tests/auth/test_fedora.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/auth/test_oauth.py` & `bodhi_server-8.1.0/tests/auth/test_oauth.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/auth/test_utils.py` & `bodhi_server-8.1.0/tests/auth/test_utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/auth/test_views.py` & `bodhi_server-8.1.0/tests/auth/test_views.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/auth/utils.py` & `bodhi_server-8.1.0/tests/auth/utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/base.py` & `bodhi_server-8.1.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/conftest.py` & `bodhi_server-8.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/consumers/__init__.py` & `bodhi_server-8.1.0/tests/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/consumers/test_automatic_updates.py` & `bodhi_server-8.1.0/tests/consumers/test_automatic_updates.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/consumers/test_ci.py` & `bodhi_server-8.1.0/tests/consumers/test_ci.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/consumers/test_consumers.py` & `bodhi_server-8.1.0/tests/consumers/test_consumers.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/consumers/test_resultsdb.py` & `bodhi_server-8.1.0/tests/consumers/test_resultsdb.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/consumers/test_signed.py` & `bodhi_server-8.1.0/tests/consumers/test_signed.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/consumers/test_waiverdb.py` & `bodhi_server-8.1.0/tests/consumers/test_waiverdb.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/createrepo_c.ini` & `bodhi_server-8.1.0/tests/createrepo_c.ini`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/functional/__init__.py` & `bodhi_server-8.1.0/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/functional/test_packages.py` & `bodhi_server-8.1.0/tests/functional/test_packages.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/functional/test_users.py` & `bodhi_server-8.1.0/tests/functional/test_users.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/scripts/__init__.py` & `bodhi_server-8.1.0/tests/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/scripts/test_bshell.py` & `bodhi_server-8.1.0/tests/scripts/test_bshell.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/scripts/test_compat.py` & `bodhi_server-8.1.0/tests/scripts/test_compat.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/scripts/test_initializedb.py` & `bodhi_server-8.1.0/tests/scripts/test_initializedb.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/scripts/test_sar.py` & `bodhi_server-8.1.0/tests/scripts/test_sar.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/scripts/test_untag_branched.py` & `bodhi_server-8.1.0/tests/scripts/test_untag_branched.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/services/__init__.py` & `bodhi_server-8.1.0/tests/services/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/services/test_builds.py` & `bodhi_server-8.1.0/tests/services/test_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/services/test_comments.py` & `bodhi_server-8.1.0/tests/services/test_comments.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/services/test_composes.py` & `bodhi_server-8.1.0/tests/services/test_composes.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/services/test_csrf.py` & `bodhi_server-8.1.0/tests/services/test_csrf.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/services/test_errors.py` & `bodhi_server-8.1.0/tests/services/test_errors.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/services/test_overrides.py` & `bodhi_server-8.1.0/tests/services/test_overrides.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/services/test_releases.py` & `bodhi_server-8.1.0/tests/services/test_releases.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,14 +106,17 @@
         res = self.app.get('/releases/')
         body = res.json_body
         assert len(body['releases']) == 2
 
         assert body['releases'][0]['name'] == 'F17'
         assert body['releases'][1]['name'] == 'F22'
 
+        res_list = self.app.get('/list_releases/')
+        assert res_list.json_body == body
+
     def test_list_releases_with_pagination(self):
         res = self.app.get('/releases/')
         body = res.json_body
         assert len(body['releases']) == 2
 
         res = self.app.get('/releases/', {'rows_per_page': 1})
         body = res.json_body
```

### Comparing `bodhi_server-8.0.2/tests/services/test_schemas.py` & `bodhi_server-8.1.0/tests/services/test_schemas.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/services/test_updates.py` & `bodhi_server-8.1.0/tests/services/test_updates.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/tasks/__init__.py` & `bodhi_server-8.1.0/tests/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/tasks/base.py` & `bodhi_server-8.1.0/tests/tasks/base.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/tasks/test_approve_testing.py` & `bodhi_server-8.1.0/tests/tasks/test_approve_testing.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/tasks/test_check_policies.py` & `bodhi_server-8.1.0/tests/tasks/test_check_policies.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/tasks/test_check_signed_builds.py` & `bodhi_server-8.1.0/tests/tasks/test_check_signed_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/tasks/test_clean_old_composes.py` & `bodhi_server-8.1.0/tests/tasks/test_clean_old_composes.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/tasks/test_composer.py` & `bodhi_server-8.1.0/tests/tasks/test_composer.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/tasks/test_expire_overrides.py` & `bodhi_server-8.1.0/tests/tasks/test_expire_overrides.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/tasks/test_fetch_test_cases.py` & `bodhi_server-8.1.0/tests/tasks/test_fetch_test_cases.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/tasks/test_handle_side_and_related_tags.py` & `bodhi_server-8.1.0/tests/tasks/test_handle_side_and_related_tags.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/tasks/test_tag_update_builds.py` & `bodhi_server-8.1.0/tests/tasks/test_tag_update_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/tasks/test_work_on_bugs.py` & `bodhi_server-8.1.0/tests/tasks/test_work_on_bugs.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/test___init__.py` & `bodhi_server-8.1.0/tests/test___init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,21 +139,14 @@
         assert policy.helper.hashalg == 'sha512'
         assert policy.helper.max_age == 86400
         assert policy.helper.secure is True
         assert policy.helper.secret == 'hunter2'
         assert policy.helper.timeout == 86400
         set_security_policy.assert_called_once_with(policy)
 
-    def test_calls_session_remove(self):
-        """Let's assert that main() calls Session.remove()."""
-        with mock.patch('bodhi.server.Session.remove') as remove:
-            server.main({}, session=self.db, **self.app_settings)
-
-        remove.assert_called_once_with()
-
     @mock.patch('bodhi.server.bugs.set_bugtracker')
     def test_calls_set_bugtracker(self, set_bugtracker):
         """
         Ensure that main() calls set_bugtracker().
         """
         server.main({}, testing='guest', session=self.db, **self.app_settings)
```

### Comparing `bodhi_server-8.0.2/tests/test_alembic.py` & `bodhi_server-8.1.0/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/test_bugs.py` & `bodhi_server-8.1.0/tests/test_bugs.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/test_buildsys.py` & `bodhi_server-8.1.0/tests/test_buildsys.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/test_config.py` & `bodhi_server-8.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/test_logging.py` & `bodhi_server-8.1.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/test_mail.py` & `bodhi_server-8.1.0/tests/test_mail.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/test_metadata.py` & `bodhi_server-8.1.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/test_models.py` & `bodhi_server-8.1.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/test_notifications.py` & `bodhi_server-8.1.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/test_push.py` & `bodhi_server-8.1.0/tests/test_push.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/test_renderers.py` & `bodhi_server-8.1.0/tests/test_renderers.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/test_schemas.py` & `bodhi_server-8.1.0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/test_security.py` & `bodhi_server-8.1.0/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/test_util.py` & `bodhi_server-8.1.0/tests/test_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 import subprocess
 import tempfile
 
 from webob.multidict import MultiDict
 import bleach
 import createrepo_c
 import packaging
-import pkg_resources
 import pytest
 
 from bodhi.server import models, util
 from bodhi.server.config import config
 from bodhi.server.exceptions import RepodataException
 from bodhi.server.models import ReleaseState, TestGatingStatus, Update
 
@@ -138,16 +137,15 @@
         bug.bug_id = 1473091
         bug.title = '<disk> <driver name="..."> should be optional'
 
         link = util.bug_link(None, bug)
         # bleach v3 fixed a bug that closed out tags when sanitizing. so we check for
         # either possible results here.
         # https://github.com/mozilla/bleach/issues/392
-        bleach_v = pkg_resources.parse_version(bleach.__version__)
-        if bleach_v >= pkg_resources.parse_version('3.0.0'):
+        if packaging.version.parse(bleach.__version__) >= packaging.version.parse('3.0.0'):
             assert link == \
                 ("<a target='_blank' href='https://bugzilla.redhat.com/show_bug.cgi?id=1473091' "
                  "class='notblue'>BZ#1473091</a> &lt;disk&gt; &lt;driver name=\"...\"&gt; should "
                  "be optional")
         else:
             assert link == \
                 ("<a target='_blank' href='https://bugzilla.redhat.com/show_bug.cgi?id=1473091' "
@@ -406,69 +404,69 @@
         super().teardown_method(method)
 
     def test_correct_yum_repo_with_xz_compress(self):
         """No Exception should be raised if the repo is normal.
 
         This is using default XZ compression.
         """
-        base.mkmetadatadir(self.tempdir)
+        base.mkmetadatadir(self.tempdir, compress_type='xz')
 
         # No exception should be raised here.
-        util.sanity_check_repodata(self.tempdir, repo_type='yum')
+        util.sanity_check_repodata(self.tempdir, repo_type='yum', drpms=True)
 
     def test_correct_yum_repo_with_gz_compress(self):
         """No Exception should be raised if the repo is normal.
 
         This is using GZ compression.
         """
         base.mkmetadatadir(self.tempdir, compress_type='gz')
 
         # No exception should be raised here.
-        util.sanity_check_repodata(self.tempdir, repo_type='yum')
+        util.sanity_check_repodata(self.tempdir, repo_type='yum', drpms=True)
 
     def test_correct_yum_repo_with_bz2_compress(self):
         """No Exception should be raised if the repo is normal.
 
         This is using BZ2 compression.
         """
         base.mkmetadatadir(self.tempdir, compress_type='bz2')
 
         # No exception should be raised here.
-        util.sanity_check_repodata(self.tempdir, repo_type='yum')
+        util.sanity_check_repodata(self.tempdir, repo_type='yum', drpms=True)
 
     @pytest.mark.skipif(
-        pkg_resources.parse_version(createrepo_c.VERSION) < pkg_resources.parse_version('1.0.0'),
+        packaging.version.parse(createrepo_c.VERSION) < packaging.version.parse('1.0.0'),
         reason='ZSTD compression requires createrepo_c 1.0.0 or higher'
     )
     def test_correct_yum_repo_with_zstd_compress(self):
         """No Exception should be raised if the repo is normal.
 
         This is using ZSTD compression.
         """
         base.mkmetadatadir(self.tempdir, compress_type='zstd')
 
         # No exception should be raised here.
-        util.sanity_check_repodata(self.tempdir, repo_type='yum')
+        util.sanity_check_repodata(self.tempdir, repo_type='yum', drpms=True)
 
     def test_invalid_repo_type(self):
         """A ValueError should be raised with invalid repo type."""
         with pytest.raises(ValueError) as excinfo:
-            util.sanity_check_repodata("so", "wrong")
+            util.sanity_check_repodata("so", "wrong", drpms=True)
         assert str(excinfo.value) == 'repo_type must be one of module, source, or yum.'
 
     @mock.patch('bodhi.server.util.librepo')
     def test_librepo_exception(self, librepo):
         """Verify that LibrepoExceptions are re-wrapped."""
         class MockException(Exception):
             pass
         librepo.LibrepoException = MockException
         librepo.Handle.return_value.perform.side_effect = MockException(-1, 'msg', 'general_msg')
 
         with pytest.raises(RepodataException) as excinfo:
-            util.sanity_check_repodata('/tmp/', 'yum')
+            util.sanity_check_repodata('/tmp/', 'yum', drpms=True)
         assert str(excinfo.value) == 'msg'
 
     def _mkmetadatadir_w_modules(self):
         base.mkmetadatadir(self.tempdir)
         # We need to add a modules tag to repomd.
         repomd_path = os.path.join(self.tempdir, 'repodata', 'repomd.xml')
         repomd_tree = ElementTree.parse(repomd_path)
@@ -486,58 +484,58 @@
         repomd_tree.write(repomd_path, encoding='UTF-8', xml_declaration=True)
 
     @mock.patch('subprocess.check_output', return_value='Some output')
     def test_correct_module_repo(self, *args):
         """No Exception should be raised if the repo is a normal module repo."""
         self._mkmetadatadir_w_modules()
         # No exception should be raised here.
-        util.sanity_check_repodata(self.tempdir, repo_type='module')
+        util.sanity_check_repodata(self.tempdir, repo_type='module', drpms=True)
 
     @mock.patch('subprocess.check_output', return_value='')
     def test_module_repo_no_dnf_output(self, *args):
         """No Exception should be raised if the repo is a normal module repo."""
         self._mkmetadatadir_w_modules()
 
         with pytest.raises(util.RepodataException) as exc:
-            util.sanity_check_repodata(self.tempdir, repo_type='module')
+            util.sanity_check_repodata(self.tempdir, repo_type='module', drpms=True)
         assert str(exc.value) == \
             ("DNF did not return expected output when running test!"
              " Test: ['module', 'list'], expected: .*, output: ")
 
     def test_updateinfo_empty_tags(self):
         """RepodataException should be raised if <id/> is found in updateinfo."""
         updateinfo = os.path.join(self.tempdir, 'updateinfo.xml')
         with open(updateinfo, 'w') as uinfo:
             uinfo.write('<id/>')
         base.mkmetadatadir(self.tempdir, updateinfo=updateinfo)
 
         with pytest.raises(util.RepodataException) as exc:
-            util.sanity_check_repodata(self.tempdir, repo_type='yum')
+            util.sanity_check_repodata(self.tempdir, repo_type='yum', drpms=True)
         assert str(exc.value) == 'updateinfo.xml.gz contains empty ID tags'
 
     def test_comps_invalid_notxml(self):
         """RepodataException should be raised if comps is invalid."""
         comps = os.path.join(self.tempdir, 'comps.xml')
         with open(comps, 'w') as uinfo:
             uinfo.write('this is not even xml')
         base.mkmetadatadir(self.tempdir, comps=comps)
 
         with pytest.raises(util.RepodataException) as exc:
-            util.sanity_check_repodata(self.tempdir, repo_type='yum')
+            util.sanity_check_repodata(self.tempdir, repo_type='yum', drpms=True)
         assert str(exc.value) == 'Comps file unable to be parsed'
 
     def test_comps_invalid_nonsense(self):
         """RepodataException should be raised if comps is invalid."""
         comps = os.path.join(self.tempdir, 'comps.xml')
         with open(comps, 'w') as uinfo:
             uinfo.write('<whatever />')
         base.mkmetadatadir(self.tempdir, comps=comps)
 
         with pytest.raises(util.RepodataException) as exc:
-            util.sanity_check_repodata(self.tempdir, repo_type='yum')
+            util.sanity_check_repodata(self.tempdir, repo_type='yum', drpms=True)
         assert str(exc.value) == 'Comps file empty'
 
     def test_repomd_missing_updateinfo(self):
         """If the updateinfo data tag is missing in repomd.xml, an Exception should be raised."""
         base.mkmetadatadir(self.tempdir)
         repomd_path = os.path.join(self.tempdir, 'repodata', 'repomd.xml')
         repomd = ElementTree.parse(repomd_path)
@@ -546,32 +544,63 @@
         # Find the <data type="updateinfo"> tag and delete it
         for data in root.findall('{http://linux.duke.edu/metadata/repo}data'):
             if data.attrib['type'] == 'updateinfo':
                 root.remove(data)
         repomd.write(repomd_path, encoding='UTF-8', xml_declaration=True)
 
         with pytest.raises(util.RepodataException) as exc:
-            util.sanity_check_repodata(self.tempdir, repo_type='yum')
+            util.sanity_check_repodata(self.tempdir, repo_type='yum', drpms=True)
         assert str(exc.value) == 'Required parts not in repomd.xml: updateinfo'
 
+    def test_repomd_missing_prestodelta(self):
+        """If the prestodelta data tag is missing in repomd.xml, an Exception should be raised."""
+        base.mkmetadatadir(self.tempdir)
+        repomd_path = os.path.join(self.tempdir, 'repodata', 'repomd.xml')
+        repomd = ElementTree.parse(repomd_path)
+        ElementTree.register_namespace('', 'http://linux.duke.edu/metadata/repo')
+        root = repomd.getroot()
+        for data in root.findall('{http://linux.duke.edu/metadata/repo}data'):
+            if data.attrib['type'] == 'prestodelta':
+                root.remove(data)
+        repomd.write(repomd_path, encoding='UTF-8', xml_declaration=True)
+
+        with pytest.raises(util.RepodataException) as exc:
+            util.sanity_check_repodata(self.tempdir, repo_type='yum', drpms=True)
+        assert str(exc.value) == 'Required parts not in repomd.xml: prestodelta'
+
+    def test_repomd_drpms_disabled(self):
+        """If the prestodelta data tag is missing in a repo without DRPMs is fine."""
+        base.mkmetadatadir(self.tempdir)
+        repomd_path = os.path.join(self.tempdir, 'repodata', 'repomd.xml')
+        repomd = ElementTree.parse(repomd_path)
+        ElementTree.register_namespace('', 'http://linux.duke.edu/metadata/repo')
+        root = repomd.getroot()
+        for data in root.findall('{http://linux.duke.edu/metadata/repo}data'):
+            if data.attrib['type'] == 'prestodelta':
+                root.remove(data)
+        repomd.write(repomd_path, encoding='UTF-8', xml_declaration=True)
+
+        # No exception should be raised.
+        util.sanity_check_repodata(self.tempdir, repo_type='yum', drpms=False)
+
     def test_source_true(self):
         """It should not fail source repos for missing prestodelta or comps."""
         base.mkmetadatadir(self.tempdir)
         repomd_path = os.path.join(self.tempdir, 'repodata', 'repomd.xml')
         repomd = ElementTree.parse(repomd_path)
         ElementTree.register_namespace('', 'http://linux.duke.edu/metadata/repo')
         root = repomd.getroot()
         for data in root.findall('{http://linux.duke.edu/metadata/repo}data'):
             # Source repos don't have drpms or comps.
             if data.attrib['type'] in ('group', 'prestodelta'):
                 root.remove(data)
         repomd.write(repomd_path, encoding='UTF-8', xml_declaration=True)
 
         # No exception should be raised.
-        util.sanity_check_repodata(self.tempdir, repo_type='source')
+        util.sanity_check_repodata(self.tempdir, repo_type='source', drpms=True)
 
 
 class TestTestcaseLink(base.BasePyTestCase):
     """Test the testcase_link() function."""
 
     base_url = 'http://example.com/'
     displayed_name = 'test case name'
@@ -1016,16 +1045,15 @@
             '<div class="markdown"><h1>this is a header</h1>\n<p>this is some <strong>text'
             '</strong></p></div>')
         expected_tags = [
             "h1", "h2", "h3", "h4", "h5", "h6", "b", "i", "strong", "em", "tt", "p", "br", "span",
             "div", "blockquote", "code", "hr", "pre", "ul", "ol", "li", "dd", "dt", "img", "a"]
         expected_attributes = {
             "img": ["src", "alt", "title"], "a": ["href", "alt", "title"], "div": ["class"]}
-        bleach_v = pkg_resources.get_distribution('bleach').version
-        if packaging.version.parse(bleach_v) >= packaging.version.parse("6.0.0"):
+        if packaging.version.parse(bleach.__version__) >= packaging.version.parse("6.0.0"):
             expected_tags = set(expected_tags)
         # The bleach 2 API should get these attrs passed.
         clean.assert_called_once_with(expected_text, tags=expected_tags,
                                       attributes=expected_attributes)
 
     def test_markup_without_bodhi_extensions(self):
         """Ensure Bodhi extensions are not used with bodhi=False"""
```

### Comparing `bodhi_server-8.0.2/tests/test_validators.py` & `bodhi_server-8.1.0/tests/test_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -971,25 +971,60 @@
     @mock.patch('bodhi.server.validators.cache_nvrs')
     def test_build_from_release_composed_by_bodhi(self, mock_cache_nvrs):
         """Assert that release composed by Bodhi will not be validated when from_tag is provided."""
         self.request.validated = {'from_tag': 'f17-build-side-7777',
                                   'builds': ['foo-1-1.f17']}
         self.request.buildinfo = {'foo-1-1.f17': {
             'nvr': ('foo', '1-1', 'f17'),
+            'info': {'source': 'git+https://src.fedoraproject.org/rpms/foo.git#aabbccdd'}
         }}
         self.release.composed_by_bodhi = True
         validators.validate_build_nvrs(self.request)
 
         assert self.request.errors == [
             {'location': 'body', 'name': 'builds',
              'description':
                  f"Can't create update from tag for release"
                  f" '{self.release.name}' composed by Bodhi."}
         ]
 
+    @mock.patch.dict(
+        'bodhi.server.validators.config',
+        {'trusted_build_sources': ['git+https://src.fedoraproject.org/']})
+    @mock.patch('bodhi.server.validators.cache_nvrs')
+    def test_build_from_distgit(self, mock_cache_nvrs):
+        """Assert that a build from distgit is allowed."""
+        self.request.validated = {'builds': ['foo-1-1.f17']}
+        self.request.buildinfo = {'foo-1-1.f17': {
+            'nvr': ('foo', '1-1', 'f17'),
+            'info': {'source': 'git+https://src.fedoraproject.org/rpms/foo.git#aabbccdd'}
+        }}
+        validators.validate_build_nvrs(self.request)
+
+        assert self.request.errors == []
+
+    @mock.patch.dict(
+        'bodhi.server.validators.config',
+        {'trusted_build_sources': ['git+https://src.fedoraproject.org/']})
+    @mock.patch('bodhi.server.validators.cache_nvrs')
+    def test_build_from_srpm(self, mock_cache_nvrs):
+        """Assert that a build from srpm is not allowed."""
+        self.request.validated = {'builds': ['foo-1-1.f17']}
+        self.request.buildinfo = {'foo-1-1.f17': {
+            'nvr': ('foo', '1-1', 'f17'),
+            'info': {'source': 'foo-1-1.f17.src.rpm'}
+        }}
+        validators.validate_build_nvrs(self.request)
+
+        assert self.request.errors == [
+            {'location': 'body', 'name': 'builds',
+             'description':
+                 "foo-1-1.f17 was not built from an allowed source"}
+        ]
+
 
 class TestValidateBuildTags(BasePyTestCase):
     """Test the validate_build_tags() function."""
 
     def setup_method(self, method):
         """Sets up the environment for each test method call."""
         super().setup_method(method)
```

### Comparing `bodhi_server-8.0.2/tests/test_webapp.py` & `bodhi_server-8.1.0/tests/test_webapp.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/testing.ini` & `bodhi_server-8.1.0/tests/testing.ini`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/utils.py` & `bodhi_server-8.1.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/views/__init__.py` & `bodhi_server-8.1.0/tests/views/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-8.0.2/tests/views/test_generic.py` & `bodhi_server-8.1.0/tests/views/test_generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 from unittest import mock
 import copy
 
+from bleach import __version__ as bleachver
 from pyramid.testing import DummyRequest
 import packaging
-import pkg_resources
 import pytest
 import webtest
 
 from bodhi.server import __version__, main, util
 from bodhi.server.config import config
 from bodhi.server.models import Release, ReleaseState, Update, UpdateStatus
 
@@ -223,16 +223,18 @@
             ('<div class="markdown"><p>See '
              '<a href="http://localhost/updates/FEDORA-2019-1a2b3c4d5e">'
              'FEDORA-2019-1a2b3c4d5e</a>.</p></div>')
 
     def test_markdown_with_update_link(self):
         """Update link should be converted to alias."""
         res = self.app.get('/markdown', {
-            'text': 'See https://bodhi-dev.example.com/updates/FEDORA-2019-1a2b3c4d5e.',
+            'text': f'See {config["base_address"]}updates/FEDORA-2019-1a2b3c4d5e.',
         }, status=200)
+        # the server name changing to 'localhost' is just an effect
+        # of using webtest, don't panic
         assert res.json_body['html'] == \
             ('<div class="markdown"><p>See '
              '<a href="http://localhost/updates/FEDORA-2019-1a2b3c4d5e">'
              'FEDORA-2019-1a2b3c4d5e</a>.</p></div>')
 
     def test_markdown_with_fake_update_link(self):
         """Update link of another domain isn't converted to alias."""
@@ -268,23 +270,22 @@
 
     def test_markdown_with_email_in_lt_gt(self):
         res = self.app.get('/markdown', {
             'text': 'email me at <dude@mcpants.org>',
         }, status=200)
         # markdown tries to obfuscate email addresses, bleach versions prior to
         # 6.0.0 restored the email in plain text
-        bleach_v = pkg_resources.get_distribution('bleach').version
-        if packaging.version.parse(bleach_v) >= packaging.version.parse("6.1.0"):
+        if packaging.version.parse(bleachver) >= packaging.version.parse("6.1.0"):
             assert res.json_body['html'] == \
                 ('<div class="markdown">'
                  '<p>email me at <a href="&#109;&#97;&#105;&#108;&#116;&#111;&#58;&#100;&#117;'
                  '&#100;&#101;&#64;&#109;&#99;&#112;&#97;&#110;&#116;&#115;&#46;&#111;&#114;'
                  '&#103;">&#100;&#117;&#100;&#101;&#64;&#109;&#99;&#112;&#97;&#110;&#116;&#115;'
                  '&#46;&#111;&#114;&#103;</a></p></div>')
-        elif packaging.version.parse(bleach_v) < packaging.version.parse("6.0.0"):
+        elif packaging.version.parse(bleachver) < packaging.version.parse("6.0.0"):
             assert res.json_body['html'] == \
                 ('<div class="markdown">'
                  '<p>email me at <a href="mailto:dude@mcpants.org">dude@mcpants.org</a></p>'
                  '</div>')
         else:
             assert res.json_body['html'] == \
                 ('<div class="markdown">'
```

### Comparing `bodhi_server-8.0.2/setup.py` & `bodhi_server-8.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                      'bodhi.server.scripts.untag_branched:main',
                      'initialize_bodhi_db = '
                      'bodhi.server.scripts.initializedb:main'],
  'paste.app_factory': ['main = bodhi.server:main']}
 
 setup_kwargs = {
     'name': 'bodhi-server',
-    'version': '8.0.2',
+    'version': '8.1.0',
     'description': 'Bodhi server',
     'long_description': "=====\nBodhi\n=====\n\nWelcome to Bodhi, Fedora's update gating system.\n\nBodhi is designed to democratize the package update testing and release process for RPM based Linux\ndistributions. It provides an interface for developers to propose updates to a distribution, and an\ninterface for testers to leave feedback about updates through a +1/-1 karma system.\n\nBodhi’s main features are:\n\n\n- Provides an interface for developers and release engineers to manage pushing out package updates\n  for multiple distribution versions.\n- Generates pre-release test repositories for end users and testers to install proposed updates.\n- Gives testers an interface to leave feedback about package updates, leading to higher quality\n  package updates.\n- Announces the arrival of new packages entering the collection.\n- Publishes end-user release notes known as errata.\n- Generates yum repositories.\n- Queries ResultsDB for automated test results and displays them on updates.\n\n\n\nDocumentation\n=============\n\nYou can read Bodhi's\n`release notes <https://fedora-infra.github.io/bodhi/user/release_notes.html>`_\nand documentation `online <https://fedora-infra.github.io/bodhi>`_.\n\nIf you are interested in contributing to Bodhi, you can read the\n`developer documentation`_.\n\n.. _developer documentation: https://fedora-infra.github.io/bodhi/docs/developer/index.html\n\n\nIRC\n===\n\nCome join us on `Libera <https://www.libera.chat/>`_! We've got two channels:\n\n* #bodhi - We use this channel to discuss upstream bodhi development\n* #fedora-apps - We use this channel to discuss Fedora's Bodhi deployment (it is more generally\n  about all of Fedora's infrastructure applications.)\n",
     'author': 'Fedora Infrastructure Team',
     'author_email': 'None',
     'maintainer': 'Fedora Infrastructure Team',
     'maintainer_email': 'infrastructure@lists.fedoraproject.org',
     'url': 'https://bodhi.fedoraproject.rog',
```

### Comparing `bodhi_server-8.0.2/PKG-INFO` & `bodhi_server-8.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodhi-server
-Version: 8.0.2
+Version: 8.1.0
 Summary: Bodhi server
 Home-page: https://bodhi.fedoraproject.rog
 License: GPL-2.0-or-later
 Keywords: web,fedora,pyramid
 Author: Fedora Infrastructure Team
 Maintainer: Fedora Infrastructure Team
 Maintainer-email: infrastructure@lists.fedoraproject.org
```

