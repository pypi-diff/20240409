# Comparing `tmp/potato-annotation-1.2.2.2.tar.gz` & `tmp/potato-annotation-1.2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "potato-annotation-1.2.2.2.tar", last modified: Thu Mar 14 15:40:04 2024, max compression
+gzip compressed data, was "potato-annotation-1.2.2.3.tar", last modified: Tue Apr  9 17:09:08 2024, max compression
```

## Comparing `potato-annotation-1.2.2.2.tar` & `potato-annotation-1.2.2.3.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 pedropei   (504) staff       (20)        0 2024-03-14 15:40:04.191846 potato-annotation-1.2.2.2/
--rw-r--r--   0 pedropei   (504) staff       (20)     5748 2023-03-12 13:48:10.000000 potato-annotation-1.2.2.2/LICENSE
--rw-r--r--   0 pedropei   (504) staff       (20)      288 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.2/MANIFEST.in
--rw-r--r--   0 pedropei   (504) staff       (20)    13025 2024-03-14 15:40:04.191532 potato-annotation-1.2.2.2/PKG-INFO
--rw-r--r--   0 pedropei   (504) staff       (20)    12760 2024-03-10 21:28:07.000000 potato-annotation-1.2.2.2/README.md
-drwxr-xr-x   0 pedropei   (504) staff       (20)        0 2024-03-14 15:40:04.169950 potato-annotation-1.2.2.2/potato/
--rw-r--r--   0 pedropei   (504) staff       (20)       42 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.2/potato/__init__.py
--rw-r--r--   0 pedropei   (504) staff       (20)     1931 2023-02-09 19:03:46.000000 potato-annotation-1.2.2.2/potato/agreement.py
-drwxr-xr-x   0 pedropei   (504) staff       (20)        0 2024-03-14 15:40:04.171439 potato-annotation-1.2.2.2/potato/base_html/
--rw-r--r--   0 pedropei   (504) staff       (20)    25335 2023-10-03 20:32:17.000000 potato-annotation-1.2.2.2/potato/base_html/base_template.html
-drwxr-xr-x   0 pedropei   (504) staff       (20)        0 2024-03-14 15:40:04.173117 potato-annotation-1.2.2.2/potato/base_html/examples/
--rw-r--r--   0 pedropei   (504) staff       (20)      608 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.2/potato/base_html/examples/fixed_keybinding_layout.html
--rw-r--r--   0 pedropei   (504) staff       (20)      628 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.2/potato/base_html/examples/kwargs_example.html
--rw-r--r--   0 pedropei   (504) staff       (20)      447 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.2/potato/base_html/examples/plain_layout.html
--rw-r--r--   0 pedropei   (504) staff       (20)     7918 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.2/potato/base_html/header.html
--rw-r--r--   0 pedropei   (504) staff       (20)     2661 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.2/potato/base_html/home.html
--rw-r--r--   0 pedropei   (504) staff       (20)      147 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.2/potato/cli.py
--rw-r--r--   0 pedropei   (504) staff       (20)     6564 2023-09-22 13:02:49.000000 potato-annotation-1.2.2.2/potato/create_task_cli.py
--rw-r--r--   0 pedropei   (504) staff       (20)   117376 2024-03-14 15:39:48.000000 potato-annotation-1.2.2.2/potato/flask_server.py
--rw-r--r--   0 pedropei   (504) staff       (20)     3073 2022-12-19 17:15:12.000000 potato-annotation-1.2.2.2/potato/remove_users_from_queue.py
-drwxr-xr-x   0 pedropei   (504) staff       (20)        0 2024-03-14 15:40:04.174952 potato-annotation-1.2.2.2/potato/server_utils/
--rw-r--r--   0 pedropei   (504) staff       (20)        0 2023-02-20 00:09:39.000000 potato-annotation-1.2.2.2/potato/server_utils/__init__.py
--rw-r--r--   0 pedropei   (504) staff       (20)     1183 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.2/potato/server_utils/arg_utils.py
--rw-r--r--   0 pedropei   (504) staff       (20)     3050 2024-03-10 21:17:52.000000 potato-annotation-1.2.2.2/potato/server_utils/cli_utlis.py
--rw-r--r--   0 pedropei   (504) staff       (20)     3536 2023-08-30 12:40:02.000000 potato-annotation-1.2.2.2/potato/server_utils/config_module.py
--rw-r--r--   0 pedropei   (504) staff       (20)    22614 2023-09-27 23:04:08.000000 potato-annotation-1.2.2.2/potato/server_utils/front_end.py
--rw-r--r--   0 pedropei   (504) staff       (20)    11572 2024-03-10 20:01:44.000000 potato-annotation-1.2.2.2/potato/server_utils/prolific_apis.py
-drwxr-xr-x   0 pedropei   (504) staff       (20)        0 2024-03-14 15:40:04.179550 potato-annotation-1.2.2.2/potato/server_utils/schemas/
--rw-r--r--   0 pedropei   (504) staff       (20)      454 2023-09-26 14:35:15.000000 potato-annotation-1.2.2.2/potato/server_utils/schemas/__init__.py
--rw-r--r--   0 pedropei   (504) staff       (20)     4410 2023-03-29 13:13:23.000000 potato-annotation-1.2.2.2/potato/server_utils/schemas/likert.py
--rw-r--r--   0 pedropei   (504) staff       (20)     4161 2023-10-03 20:13:10.000000 potato-annotation-1.2.2.2/potato/server_utils/schemas/multirate.py
--rw-r--r--   0 pedropei   (504) staff       (20)     6363 2023-03-20 02:22:32.000000 potato-annotation-1.2.2.2/potato/server_utils/schemas/multiselect.py
--rw-r--r--   0 pedropei   (504) staff       (20)     3235 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/server_utils/schemas/number.py
--rw-r--r--   0 pedropei   (504) staff       (20)      254 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/server_utils/schemas/pure_display.py
--rw-r--r--   0 pedropei   (504) staff       (20)     6093 2023-03-20 02:22:38.000000 potato-annotation-1.2.2.2/potato/server_utils/schemas/radio.py
--rw-r--r--   0 pedropei   (504) staff       (20)     2927 2023-03-21 01:40:54.000000 potato-annotation-1.2.2.2/potato/server_utils/schemas/select.py
--rw-r--r--   0 pedropei   (504) staff       (20)     2537 2023-09-26 14:35:15.000000 potato-annotation-1.2.2.2/potato/server_utils/schemas/slider.py
--rw-r--r--   0 pedropei   (504) staff       (20)    10260 2023-03-24 12:55:26.000000 potato-annotation-1.2.2.2/potato/server_utils/schemas/span.py
--rw-r--r--   0 pedropei   (504) staff       (20)     5069 2023-10-07 22:14:03.000000 potato-annotation-1.2.2.2/potato/server_utils/schemas/textbox.py
--rw-r--r--   0 pedropei   (504) staff       (20)     4264 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/setup_multilingual_config.py
--rw-r--r--   0 pedropei   (504) staff       (20)     4195 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/setup_multitask_config.py
-drwxr-xr-x   0 pedropei   (504) staff       (20)        0 2024-03-14 15:40:04.182893 potato-annotation-1.2.2.2/potato/static/
--rw-r--r--   0 pedropei   (504) staff       (20)    51143 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/bootstrap.js
-drwxr-xr-x   0 pedropei   (504) staff       (20)        0 2024-03-14 15:40:04.183277 potato-annotation-1.2.2.2/potato/static/fonts/
--rw-r--r--   0 pedropei   (504) staff       (20)    77160 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 pedropei   (504) staff       (20)     1906 2023-02-14 16:23:59.000000 potato-annotation-1.2.2.2/potato/static/function.js
--rw-r--r--   0 pedropei   (504) staff       (20)     3798 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/img-01.webp
--rw-r--r--   0 pedropei   (504) staff       (20)    86659 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/jquery-3.js
--rw-r--r--   0 pedropei   (504) staff       (20)      875 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/main.js
--rw-r--r--   0 pedropei   (504) staff       (20)    34239 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/popper.js
--rw-r--r--   0 pedropei   (504) staff       (20)    66664 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/select2.js
--rw-r--r--   0 pedropei   (504) staff       (20)    18387 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/sha256.js
-drwxr-xr-x   0 pedropei   (504) staff       (20)        0 2024-03-14 15:40:04.186462 potato-annotation-1.2.2.2/potato/static/styles/
--rw-r--r--   0 pedropei   (504) staff       (20)    17502 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/styles/animate.css
--rw-r--r--   0 pedropei   (504) staff       (20)   124962 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/styles/bootstrap.css
--rw-r--r--   0 pedropei   (504) staff       (20)    31000 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/styles/font-awesome.css
--rw-r--r--   0 pedropei   (504) staff       (20)    19686 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/styles/hamburgers.css
--rw-r--r--   0 pedropei   (504) staff       (20)     6702 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/styles/main.css
--rw-r--r--   0 pedropei   (504) staff       (20)    15196 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/styles/select2.css
--rw-r--r--   0 pedropei   (504) staff       (20)      771 2023-02-16 02:45:18.000000 potato-annotation-1.2.2.2/potato/static/styles/style.css
--rw-r--r--   0 pedropei   (504) staff       (20)    70790 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/styles/util.css
-drwxr-xr-x   0 pedropei   (504) staff       (20)        0 2024-03-14 15:40:04.187496 potato-annotation-1.2.2.2/potato/static/survey_assets/
--rw-r--r--   0 pedropei   (504) staff       (20)    11223 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/survey_assets/country_dropdown_list.html
--rw-r--r--   0 pedropei   (504) staff       (20)     1834 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/survey_assets/ethnicity_dropdown_list.html
--rw-r--r--   0 pedropei   (504) staff       (20)     1376 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/survey_assets/religion_dropdown_list.html
--rw-r--r--   0 pedropei   (504) staff       (20)     5640 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/static/tilt.js
-drwxr-xr-x   0 pedropei   (504) staff       (20)        0 2024-03-14 15:40:04.189405 potato-annotation-1.2.2.2/potato/templates/
--rwxr-xr-x   0 pedropei   (504) staff       (20)      184 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/templates/congrats.html
--rwxr-xr-x   0 pedropei   (504) staff       (20)      150 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/templates/error.html
--rwxr-xr-x   0 pedropei   (504) staff       (20)    15973 2022-12-20 21:24:49.000000 potato-annotation-1.2.2.2/potato/templates/home.html
--rwxr-xr-x   0 pedropei   (504) staff       (20)    15934 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/templates/id_login_home.html
--rwxr-xr-x   0 pedropei   (504) staff       (20)     5395 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.2/potato/templates/signup.html
-drwxr-xr-x   0 pedropei   (504) staff       (20)        0 2024-03-14 15:40:04.191227 potato-annotation-1.2.2.2/potato_annotation.egg-info/
--rw-r--r--   0 pedropei   (504) staff       (20)    13025 2024-03-14 15:40:04.000000 potato-annotation-1.2.2.2/potato_annotation.egg-info/PKG-INFO
--rw-r--r--   0 pedropei   (504) staff       (20)     2218 2024-03-14 15:40:04.000000 potato-annotation-1.2.2.2/potato_annotation.egg-info/SOURCES.txt
--rw-r--r--   0 pedropei   (504) staff       (20)        1 2024-03-14 15:40:04.000000 potato-annotation-1.2.2.2/potato_annotation.egg-info/dependency_links.txt
--rw-r--r--   0 pedropei   (504) staff       (20)       45 2024-03-14 15:40:04.000000 potato-annotation-1.2.2.2/potato_annotation.egg-info/entry_points.txt
--rw-r--r--   0 pedropei   (504) staff       (20)      352 2024-03-14 15:40:04.000000 potato-annotation-1.2.2.2/potato_annotation.egg-info/requires.txt
--rw-r--r--   0 pedropei   (504) staff       (20)        7 2024-03-14 15:40:04.000000 potato-annotation-1.2.2.2/potato_annotation.egg-info/top_level.txt
--rw-r--r--   0 pedropei   (504) staff       (20)       38 2024-03-14 15:40:04.191911 potato-annotation-1.2.2.2/setup.cfg
--rw-r--r--   0 pedropei   (504) staff       (20)     1216 2024-03-14 15:39:48.000000 potato-annotation-1.2.2.2/setup.py
+drwxr-xr-x   0 pedropei   (501) staff       (20)        0 2024-04-09 17:09:08.771229 potato-annotation-1.2.2.3/
+-rw-r--r--   0 pedropei   (501) staff       (20)     5748 2023-03-12 13:48:10.000000 potato-annotation-1.2.2.3/LICENSE
+-rw-r--r--   0 pedropei   (501) staff       (20)      288 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.3/MANIFEST.in
+-rw-r--r--   0 pedropei   (501) staff       (20)    13111 2024-04-09 17:09:08.771079 potato-annotation-1.2.2.3/PKG-INFO
+-rw-r--r--   0 pedropei   (501) staff       (20)    12809 2024-03-14 15:42:04.000000 potato-annotation-1.2.2.3/README.md
+drwxr-xr-x   0 pedropei   (501) staff       (20)        0 2024-04-09 17:09:08.758478 potato-annotation-1.2.2.3/potato/
+-rw-r--r--   0 pedropei   (501) staff       (20)       42 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.3/potato/__init__.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     1931 2023-02-09 19:03:46.000000 potato-annotation-1.2.2.3/potato/agreement.py
+drwxr-xr-x   0 pedropei   (501) staff       (20)        0 2024-04-09 17:09:08.759335 potato-annotation-1.2.2.3/potato/base_html/
+-rw-r--r--   0 pedropei   (501) staff       (20)    25335 2023-10-03 20:32:17.000000 potato-annotation-1.2.2.3/potato/base_html/base_template.html
+drwxr-xr-x   0 pedropei   (501) staff       (20)        0 2024-04-09 17:09:08.759714 potato-annotation-1.2.2.3/potato/base_html/examples/
+-rw-r--r--   0 pedropei   (501) staff       (20)      608 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.3/potato/base_html/examples/fixed_keybinding_layout.html
+-rw-r--r--   0 pedropei   (501) staff       (20)      628 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.3/potato/base_html/examples/kwargs_example.html
+-rw-r--r--   0 pedropei   (501) staff       (20)      447 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.3/potato/base_html/examples/plain_layout.html
+-rw-r--r--   0 pedropei   (501) staff       (20)     7918 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.3/potato/base_html/header.html
+-rw-r--r--   0 pedropei   (501) staff       (20)     2661 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.3/potato/base_html/home.html
+-rw-r--r--   0 pedropei   (501) staff       (20)      147 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.3/potato/cli.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     6564 2023-09-22 13:02:49.000000 potato-annotation-1.2.2.3/potato/create_task_cli.py
+-rw-r--r--   0 pedropei   (501) staff       (20)   119568 2024-04-09 16:49:47.000000 potato-annotation-1.2.2.3/potato/flask_server.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     3073 2022-12-19 17:15:12.000000 potato-annotation-1.2.2.3/potato/remove_users_from_queue.py
+drwxr-xr-x   0 pedropei   (501) staff       (20)        0 2024-04-09 17:09:08.761347 potato-annotation-1.2.2.3/potato/server_utils/
+-rw-r--r--   0 pedropei   (501) staff       (20)        0 2023-02-20 00:09:39.000000 potato-annotation-1.2.2.3/potato/server_utils/__init__.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     1183 2023-03-21 01:11:11.000000 potato-annotation-1.2.2.3/potato/server_utils/arg_utils.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     3050 2024-03-10 21:17:52.000000 potato-annotation-1.2.2.3/potato/server_utils/cli_utlis.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     3536 2023-08-30 12:40:02.000000 potato-annotation-1.2.2.3/potato/server_utils/config_module.py
+-rw-r--r--   0 pedropei   (501) staff       (20)    22614 2023-09-27 23:04:08.000000 potato-annotation-1.2.2.3/potato/server_utils/front_end.py
+-rw-r--r--   0 pedropei   (501) staff       (20)      863 2024-03-21 14:29:02.000000 potato-annotation-1.2.2.3/potato/server_utils/prolific_api_test.py
+-rw-r--r--   0 pedropei   (501) staff       (20)    11572 2024-03-21 14:37:47.000000 potato-annotation-1.2.2.3/potato/server_utils/prolific_apis.py
+drwxr-xr-x   0 pedropei   (501) staff       (20)        0 2024-04-09 17:09:08.763595 potato-annotation-1.2.2.3/potato/server_utils/schemas/
+-rw-r--r--   0 pedropei   (501) staff       (20)      454 2023-09-26 14:35:15.000000 potato-annotation-1.2.2.3/potato/server_utils/schemas/__init__.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     4410 2023-03-29 13:13:23.000000 potato-annotation-1.2.2.3/potato/server_utils/schemas/likert.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     4161 2023-10-03 20:13:10.000000 potato-annotation-1.2.2.3/potato/server_utils/schemas/multirate.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     6363 2023-03-20 02:22:32.000000 potato-annotation-1.2.2.3/potato/server_utils/schemas/multiselect.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     3235 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/server_utils/schemas/number.py
+-rw-r--r--   0 pedropei   (501) staff       (20)      254 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/server_utils/schemas/pure_display.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     6093 2023-03-20 02:22:38.000000 potato-annotation-1.2.2.3/potato/server_utils/schemas/radio.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     2927 2023-03-21 01:40:54.000000 potato-annotation-1.2.2.3/potato/server_utils/schemas/select.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     2537 2023-09-26 14:35:15.000000 potato-annotation-1.2.2.3/potato/server_utils/schemas/slider.py
+-rw-r--r--   0 pedropei   (501) staff       (20)    10260 2023-03-24 12:55:26.000000 potato-annotation-1.2.2.3/potato/server_utils/schemas/span.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     5069 2023-10-07 22:14:03.000000 potato-annotation-1.2.2.3/potato/server_utils/schemas/textbox.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     4264 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/setup_multilingual_config.py
+-rw-r--r--   0 pedropei   (501) staff       (20)     4195 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/setup_multitask_config.py
+drwxr-xr-x   0 pedropei   (501) staff       (20)        0 2024-04-09 17:09:08.766250 potato-annotation-1.2.2.3/potato/static/
+-rw-r--r--   0 pedropei   (501) staff       (20)    51143 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/bootstrap.js
+drwxr-xr-x   0 pedropei   (501) staff       (20)        0 2024-04-09 17:09:08.766563 potato-annotation-1.2.2.3/potato/static/fonts/
+-rw-r--r--   0 pedropei   (501) staff       (20)    77160 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 pedropei   (501) staff       (20)     1906 2023-02-14 16:23:59.000000 potato-annotation-1.2.2.3/potato/static/function.js
+-rw-r--r--   0 pedropei   (501) staff       (20)     3798 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/img-01.webp
+-rw-r--r--   0 pedropei   (501) staff       (20)    86659 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/jquery-3.js
+-rw-r--r--   0 pedropei   (501) staff       (20)      875 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/main.js
+-rw-r--r--   0 pedropei   (501) staff       (20)    34239 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/popper.js
+-rw-r--r--   0 pedropei   (501) staff       (20)    66664 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/select2.js
+-rw-r--r--   0 pedropei   (501) staff       (20)    18387 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/sha256.js
+drwxr-xr-x   0 pedropei   (501) staff       (20)        0 2024-04-09 17:09:08.768327 potato-annotation-1.2.2.3/potato/static/styles/
+-rw-r--r--   0 pedropei   (501) staff       (20)    17502 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/styles/animate.css
+-rw-r--r--   0 pedropei   (501) staff       (20)   124962 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/styles/bootstrap.css
+-rw-r--r--   0 pedropei   (501) staff       (20)    31000 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/styles/font-awesome.css
+-rw-r--r--   0 pedropei   (501) staff       (20)    19686 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/styles/hamburgers.css
+-rw-r--r--   0 pedropei   (501) staff       (20)     6702 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/styles/main.css
+-rw-r--r--   0 pedropei   (501) staff       (20)    15196 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/styles/select2.css
+-rw-r--r--   0 pedropei   (501) staff       (20)      771 2023-02-16 02:45:18.000000 potato-annotation-1.2.2.3/potato/static/styles/style.css
+-rw-r--r--   0 pedropei   (501) staff       (20)    70790 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/styles/util.css
+drwxr-xr-x   0 pedropei   (501) staff       (20)        0 2024-04-09 17:09:08.768957 potato-annotation-1.2.2.3/potato/static/survey_assets/
+-rw-r--r--   0 pedropei   (501) staff       (20)    11223 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/survey_assets/country_dropdown_list.html
+-rw-r--r--   0 pedropei   (501) staff       (20)     1834 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/survey_assets/ethnicity_dropdown_list.html
+-rw-r--r--   0 pedropei   (501) staff       (20)     1376 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/survey_assets/religion_dropdown_list.html
+-rw-r--r--   0 pedropei   (501) staff       (20)     5640 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/static/tilt.js
+drwxr-xr-x   0 pedropei   (501) staff       (20)        0 2024-04-09 17:09:08.770169 potato-annotation-1.2.2.3/potato/templates/
+-rwxr-xr-x   0 pedropei   (501) staff       (20)      184 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/templates/congrats.html
+-rwxr-xr-x   0 pedropei   (501) staff       (20)      150 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/templates/error.html
+-rwxr-xr-x   0 pedropei   (501) staff       (20)    15973 2022-12-20 21:24:49.000000 potato-annotation-1.2.2.3/potato/templates/home.html
+-rwxr-xr-x   0 pedropei   (501) staff       (20)    15934 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/templates/id_login_home.html
+-rwxr-xr-x   0 pedropei   (501) staff       (20)     5395 2022-12-08 05:48:04.000000 potato-annotation-1.2.2.3/potato/templates/signup.html
+drwxr-xr-x   0 pedropei   (501) staff       (20)        0 2024-04-09 17:09:08.770956 potato-annotation-1.2.2.3/potato_annotation.egg-info/
+-rw-r--r--   0 pedropei   (501) staff       (20)    13111 2024-04-09 17:09:08.000000 potato-annotation-1.2.2.3/potato_annotation.egg-info/PKG-INFO
+-rw-r--r--   0 pedropei   (501) staff       (20)     2259 2024-04-09 17:09:08.000000 potato-annotation-1.2.2.3/potato_annotation.egg-info/SOURCES.txt
+-rw-r--r--   0 pedropei   (501) staff       (20)        1 2024-04-09 17:09:08.000000 potato-annotation-1.2.2.3/potato_annotation.egg-info/dependency_links.txt
+-rw-r--r--   0 pedropei   (501) staff       (20)       46 2024-04-09 17:09:08.000000 potato-annotation-1.2.2.3/potato_annotation.egg-info/entry_points.txt
+-rw-r--r--   0 pedropei   (501) staff       (20)      352 2024-04-09 17:09:08.000000 potato-annotation-1.2.2.3/potato_annotation.egg-info/requires.txt
+-rw-r--r--   0 pedropei   (501) staff       (20)        7 2024-04-09 17:09:08.000000 potato-annotation-1.2.2.3/potato_annotation.egg-info/top_level.txt
+-rw-r--r--   0 pedropei   (501) staff       (20)       38 2024-04-09 17:09:08.771262 potato-annotation-1.2.2.3/setup.cfg
+-rw-r--r--   0 pedropei   (501) staff       (20)     1216 2024-04-09 17:08:43.000000 potato-annotation-1.2.2.3/setup.py
```

### Comparing `potato-annotation-1.2.2.2/LICENSE` & `potato-annotation-1.2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/PKG-INFO` & `potato-annotation-1.2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: potato-annotation
-Version: 1.2.2.2
+Version: 1.2.2.3
 Summary: Potato text annotation tool
 Home-page: https://github.com/davidjurgens/potato
 Author: Jiaxin Pei
 Author-email: pedropei@umich.edu
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🥔Potato: the POrtable Text Annotation TOol
  
 [📖Documentation](https://potato-annotation.readthedocs.io/) | [🍎Feature hightlights](#Feature-hightlights)  |  [🛫️Quick Start](#Quick-Start) | [🌰Example projects (project hub)](#Example-projects-project-hub) | [🔥Design Team and Support](#Design-Team-and-Support) | [💰License](#License) | [🍞Cite us](#Cite-us)
 
@@ -25,14 +27,15 @@
 Please check out our [official documentation](https://potato-annotation.readthedocs.io/) for detailed instructions.
 
 >Jiaxin Pei, Aparna Ananthasubramaniam, Xingyao Wang, Naitian Zhou, Jackson Sargent, Apostolos Dedeloudis and David Jurgens. 🥔Potato: the POrtable Text Annotation TOol. In Proceedings of the 2022 Conference on Empirical Methods on Natural Language Processing (EMNLP'22 demo)
 
 
 
 ## Recent Updates
+- 1.2.2.2 small bugs fixed for label suggestions
 - 1.2.2.1 Supports displaying or prefilling label suggestions ([Documentation](https://potato-annotation.readthedocs.io/en/latest/productivity/#label-suggestions) | [Example project](https://github.com/davidjurgens/potato/tree/master/project-hub/label_suggestions))
 - 1.2.2.0 Supports automatic task management with prolific apis ([Documentation](https://potato-annotation.readthedocs.io/en/latest/crowdsourcing/#4-set-up-the-configuration-file-for-your-prolific-study) | [Example project](https://github.com/davidjurgens/potato/tree/master/project-hub/prolific_api_example))
 - 1.2.1.7 Supports randomizing the order of the displayed instances when it is defined with a dictionary ([link](https://potato-annotation.readthedocs.io/en/latest/data_format/#displaying-a-list-or-a-dictionary-of-instances))
 - 1.2.1.6 Supports different HTML templates for surveyflow and annotation pages ([link](https://potato-annotation.readthedocs.io/en/latest/schemas_and_templates/#different-layouts-for-surveyflow-and-annotation-pages))
 - 1.2.1.5 Supports disallowing copy-pasting into textboxes ([link](https://potato-annotation.readthedocs.io/en/latest/schemas_and_templates/#text-box))
 
 
@@ -167,7 +170,9 @@
 @inproceedings{pei2022potato,
   title={POTATO: The Portable Text Annotation Tool},
   author={Pei, Jiaxin and Ananthasubramaniam, Aparna and Wang, Xingyao and Zhou, Naitian and Dedeloudis, Apostolos and Sargent, Jackson and Jurgens, David},
   booktitle={Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing: System Demonstrations},
   year={2022}
 }
 ```
+
+
```

### Comparing `potato-annotation-1.2.2.2/README.md` & `potato-annotation-1.2.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 Please check out our [official documentation](https://potato-annotation.readthedocs.io/) for detailed instructions.
 
 >Jiaxin Pei, Aparna Ananthasubramaniam, Xingyao Wang, Naitian Zhou, Jackson Sargent, Apostolos Dedeloudis and David Jurgens. 🥔Potato: the POrtable Text Annotation TOol. In Proceedings of the 2022 Conference on Empirical Methods on Natural Language Processing (EMNLP'22 demo)
 
 
 
 ## Recent Updates
+- 1.2.2.2 small bugs fixed for label suggestions
 - 1.2.2.1 Supports displaying or prefilling label suggestions ([Documentation](https://potato-annotation.readthedocs.io/en/latest/productivity/#label-suggestions) | [Example project](https://github.com/davidjurgens/potato/tree/master/project-hub/label_suggestions))
 - 1.2.2.0 Supports automatic task management with prolific apis ([Documentation](https://potato-annotation.readthedocs.io/en/latest/crowdsourcing/#4-set-up-the-configuration-file-for-your-prolific-study) | [Example project](https://github.com/davidjurgens/potato/tree/master/project-hub/prolific_api_example))
 - 1.2.1.7 Supports randomizing the order of the displayed instances when it is defined with a dictionary ([link](https://potato-annotation.readthedocs.io/en/latest/data_format/#displaying-a-list-or-a-dictionary-of-instances))
 - 1.2.1.6 Supports different HTML templates for surveyflow and annotation pages ([link](https://potato-annotation.readthedocs.io/en/latest/schemas_and_templates/#different-layouts-for-surveyflow-and-annotation-pages))
 - 1.2.1.5 Supports disallowing copy-pasting into textboxes ([link](https://potato-annotation.readthedocs.io/en/latest/schemas_and_templates/#text-box))
```

### Comparing `potato-annotation-1.2.2.2/potato/agreement.py` & `potato-annotation-1.2.2.3/potato/agreement.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/base_html/base_template.html` & `potato-annotation-1.2.2.3/potato/base_html/base_template.html`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/base_html/examples/fixed_keybinding_layout.html` & `potato-annotation-1.2.2.3/potato/base_html/examples/fixed_keybinding_layout.html`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/base_html/examples/kwargs_example.html` & `potato-annotation-1.2.2.3/potato/base_html/examples/kwargs_example.html`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/base_html/header.html` & `potato-annotation-1.2.2.3/potato/base_html/header.html`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/base_html/home.html` & `potato-annotation-1.2.2.3/potato/base_html/home.html`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/create_task_cli.py` & `potato-annotation-1.2.2.3/potato/create_task_cli.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/flask_server.py` & `potato-annotation-1.2.2.3/potato/flask_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -2345,20 +2345,81 @@
 
                     # Find the right option and set it as selected if the current
                     # annotation schema is a select box
                     elif label == "select-one":
                         option = input_field.findChildren("option", {"value": value})[0]
                         option["selected"] = "selected"
 
+    # randomize the order of options for multirate schema
+    selected_schemas_for_option_randomization = []
+    for it in config['annotation_schemes']:
+        if it['annotation_type'] == 'multirate' and it.get('option_randomization'):
+            selected_schemas_for_option_randomization.append(it['description'])
+
+    if len(selected_schemas_for_option_randomization) > 0:
+        soup = randomize_options(soup, selected_schemas_for_option_randomization, map_user_id_to_digit(username))
 
     rendered_html = str(soup)
 
     return rendered_html
 
 
+def map_user_id_to_digit(user_id_str):
+    # Convert the user_id_str to an integer using a hash function
+    user_id_hash = hash(user_id_str)
+
+    # Map the hashed value to a single-digit integer using modulus
+    digit = abs(user_id_hash) % 9 + 1  # Add 1 to avoid 0
+
+    return digit
+
+
+def randomize_options(soup, legend_names, seed):
+    random.seed(seed)
+
+    # Find all fieldsets in the soup
+    fieldsets = soup.find_all('fieldset')
+    if not fieldsets:
+        print("No fieldsets found.")
+        return soup
+
+    # Initialize a variable to track whether the legend is found
+    legend_found = False
+
+    # Iterate through each fieldset
+    for fieldset in fieldsets:
+        # Find the legend within the current fieldset
+        legend = fieldset.find('legend')
+        if legend and legend.string in legend_names:
+            # Legend found, set the flag and break the loop
+            legend_found = True
+
+            # Find the table within the fieldset
+            table = fieldset.find('table')
+            if not table:
+                print("Table not found within the fieldset.")
+                continue
+
+            # Get the list of tr elements excluding the first one (title)
+            tr_elements = table.find_all('tr')[1:]
+
+            # Shuffle the tr elements based on the given random seed
+            random.shuffle(tr_elements)
+
+            # Insert the shuffled tr elements back into the tbody
+            for tr in tr_elements:
+                table.append(tr)
+
+    # Check if any legend was found
+    if not legend_found:
+        print(f"No matching legends found within any fieldset.")
+
+    return soup
+
+
 def get_color_for_schema_label(schema, label):
     global schema_label_to_color
 
     t = (schema, label)
     if t in schema_label_to_color:
         return schema_label_to_color[t]
     c = COLOR_PALETTE[len(schema_label_to_color)]
```

### Comparing `potato-annotation-1.2.2.2/potato/remove_users_from_queue.py` & `potato-annotation-1.2.2.3/potato/remove_users_from_queue.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/server_utils/arg_utils.py` & `potato-annotation-1.2.2.3/potato/server_utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/server_utils/cli_utlis.py` & `potato-annotation-1.2.2.3/potato/server_utils/cli_utlis.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/server_utils/config_module.py` & `potato-annotation-1.2.2.3/potato/server_utils/config_module.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/server_utils/front_end.py` & `potato-annotation-1.2.2.3/potato/server_utils/front_end.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/server_utils/prolific_apis.py` & `potato-annotation-1.2.2.3/potato/server_utils/prolific_apis.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     def add_new_user(self, user):
         status = self.get_submission_from_id(user['SESSION_ID'])['status']
         self.sessions[user['SESSION_ID']] = {'username':user['PROLIFIC_PID'], 'status':status}
         self.session_status_dict[status].append(user['SESSION_ID'])
 
 '''
 prolific = ProlificStudy(token = 'yRB91_ngkHclqd36bhXCGWwl5fqU4iVlXX-2i61cfNoh7Tpvh4tH8R6IAxEBsYrkMnyc4X8tEpmmJhHXiHiRkFZYIm_Jr-pCoXFqyrIHX30qUuT5RMcIc7rG',
-                         study_id='651ca114a0a3dc560dd00c2a', saving_dir='../')
+                         study_id='6498cf2053b6c5b98075f52c', saving_dir='../')
 prolific.list_all_studies()
 start_time = time.time()
 print(prolific.update_submission_status())
 end_time = time.time()
 execution_time = end_time - start_time
 print(execution_time)
```

### Comparing `potato-annotation-1.2.2.2/potato/server_utils/schemas/likert.py` & `potato-annotation-1.2.2.3/potato/server_utils/schemas/likert.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/server_utils/schemas/multirate.py` & `potato-annotation-1.2.2.3/potato/server_utils/schemas/multirate.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/server_utils/schemas/multiselect.py` & `potato-annotation-1.2.2.3/potato/server_utils/schemas/multiselect.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/server_utils/schemas/number.py` & `potato-annotation-1.2.2.3/potato/server_utils/schemas/number.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/server_utils/schemas/radio.py` & `potato-annotation-1.2.2.3/potato/server_utils/schemas/radio.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/server_utils/schemas/select.py` & `potato-annotation-1.2.2.3/potato/server_utils/schemas/select.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/server_utils/schemas/slider.py` & `potato-annotation-1.2.2.3/potato/server_utils/schemas/slider.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/server_utils/schemas/span.py` & `potato-annotation-1.2.2.3/potato/server_utils/schemas/span.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/server_utils/schemas/textbox.py` & `potato-annotation-1.2.2.3/potato/server_utils/schemas/textbox.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/setup_multilingual_config.py` & `potato-annotation-1.2.2.3/potato/setup_multilingual_config.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/setup_multitask_config.py` & `potato-annotation-1.2.2.3/potato/setup_multitask_config.py`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/bootstrap.js` & `potato-annotation-1.2.2.3/potato/static/bootstrap.js`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/fonts/fontawesome-webfont.woff2` & `potato-annotation-1.2.2.3/potato/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/function.js` & `potato-annotation-1.2.2.3/potato/static/function.js`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/img-01.webp` & `potato-annotation-1.2.2.3/potato/static/img-01.webp`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/jquery-3.js` & `potato-annotation-1.2.2.3/potato/static/jquery-3.js`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/main.js` & `potato-annotation-1.2.2.3/potato/static/main.js`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/popper.js` & `potato-annotation-1.2.2.3/potato/static/popper.js`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/select2.js` & `potato-annotation-1.2.2.3/potato/static/select2.js`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/sha256.js` & `potato-annotation-1.2.2.3/potato/static/sha256.js`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/styles/animate.css` & `potato-annotation-1.2.2.3/potato/static/styles/animate.css`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/styles/bootstrap.css` & `potato-annotation-1.2.2.3/potato/static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/styles/font-awesome.css` & `potato-annotation-1.2.2.3/potato/static/styles/font-awesome.css`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/styles/hamburgers.css` & `potato-annotation-1.2.2.3/potato/static/styles/hamburgers.css`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/styles/main.css` & `potato-annotation-1.2.2.3/potato/static/styles/main.css`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/styles/select2.css` & `potato-annotation-1.2.2.3/potato/static/styles/select2.css`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/styles/style.css` & `potato-annotation-1.2.2.3/potato/static/styles/style.css`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/styles/util.css` & `potato-annotation-1.2.2.3/potato/static/styles/util.css`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/survey_assets/country_dropdown_list.html` & `potato-annotation-1.2.2.3/potato/static/survey_assets/country_dropdown_list.html`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/survey_assets/ethnicity_dropdown_list.html` & `potato-annotation-1.2.2.3/potato/static/survey_assets/ethnicity_dropdown_list.html`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/survey_assets/religion_dropdown_list.html` & `potato-annotation-1.2.2.3/potato/static/survey_assets/religion_dropdown_list.html`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/static/tilt.js` & `potato-annotation-1.2.2.3/potato/static/tilt.js`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/templates/home.html` & `potato-annotation-1.2.2.3/potato/templates/home.html`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/templates/id_login_home.html` & `potato-annotation-1.2.2.3/potato/templates/id_login_home.html`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato/templates/signup.html` & `potato-annotation-1.2.2.3/potato/templates/signup.html`

 * *Files identical despite different names*

### Comparing `potato-annotation-1.2.2.2/potato_annotation.egg-info/PKG-INFO` & `potato-annotation-1.2.2.3/potato_annotation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: potato-annotation
-Version: 1.2.2.2
+Version: 1.2.2.3
 Summary: Potato text annotation tool
 Home-page: https://github.com/davidjurgens/potato
 Author: Jiaxin Pei
 Author-email: pedropei@umich.edu
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🥔Potato: the POrtable Text Annotation TOol
  
 [📖Documentation](https://potato-annotation.readthedocs.io/) | [🍎Feature hightlights](#Feature-hightlights)  |  [🛫️Quick Start](#Quick-Start) | [🌰Example projects (project hub)](#Example-projects-project-hub) | [🔥Design Team and Support](#Design-Team-and-Support) | [💰License](#License) | [🍞Cite us](#Cite-us)
 
@@ -25,14 +27,15 @@
 Please check out our [official documentation](https://potato-annotation.readthedocs.io/) for detailed instructions.
 
 >Jiaxin Pei, Aparna Ananthasubramaniam, Xingyao Wang, Naitian Zhou, Jackson Sargent, Apostolos Dedeloudis and David Jurgens. 🥔Potato: the POrtable Text Annotation TOol. In Proceedings of the 2022 Conference on Empirical Methods on Natural Language Processing (EMNLP'22 demo)
 
 
 
 ## Recent Updates
+- 1.2.2.2 small bugs fixed for label suggestions
 - 1.2.2.1 Supports displaying or prefilling label suggestions ([Documentation](https://potato-annotation.readthedocs.io/en/latest/productivity/#label-suggestions) | [Example project](https://github.com/davidjurgens/potato/tree/master/project-hub/label_suggestions))
 - 1.2.2.0 Supports automatic task management with prolific apis ([Documentation](https://potato-annotation.readthedocs.io/en/latest/crowdsourcing/#4-set-up-the-configuration-file-for-your-prolific-study) | [Example project](https://github.com/davidjurgens/potato/tree/master/project-hub/prolific_api_example))
 - 1.2.1.7 Supports randomizing the order of the displayed instances when it is defined with a dictionary ([link](https://potato-annotation.readthedocs.io/en/latest/data_format/#displaying-a-list-or-a-dictionary-of-instances))
 - 1.2.1.6 Supports different HTML templates for surveyflow and annotation pages ([link](https://potato-annotation.readthedocs.io/en/latest/schemas_and_templates/#different-layouts-for-surveyflow-and-annotation-pages))
 - 1.2.1.5 Supports disallowing copy-pasting into textboxes ([link](https://potato-annotation.readthedocs.io/en/latest/schemas_and_templates/#text-box))
 
 
@@ -167,7 +170,9 @@
 @inproceedings{pei2022potato,
   title={POTATO: The Portable Text Annotation Tool},
   author={Pei, Jiaxin and Ananthasubramaniam, Aparna and Wang, Xingyao and Zhou, Naitian and Dedeloudis, Apostolos and Sargent, Jackson and Jurgens, David},
   booktitle={Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing: System Demonstrations},
   year={2022}
 }
 ```
+
+
```

### Comparing `potato-annotation-1.2.2.2/potato_annotation.egg-info/SOURCES.txt` & `potato-annotation-1.2.2.3/potato_annotation.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 potato/base_html/examples/kwargs_example.html
 potato/base_html/examples/plain_layout.html
 potato/server_utils/__init__.py
 potato/server_utils/arg_utils.py
 potato/server_utils/cli_utlis.py
 potato/server_utils/config_module.py
 potato/server_utils/front_end.py
+potato/server_utils/prolific_api_test.py
 potato/server_utils/prolific_apis.py
 potato/server_utils/schemas/__init__.py
 potato/server_utils/schemas/likert.py
 potato/server_utils/schemas/multirate.py
 potato/server_utils/schemas/multiselect.py
 potato/server_utils/schemas/number.py
 potato/server_utils/schemas/pure_display.py
```

### Comparing `potato-annotation-1.2.2.2/setup.py` & `potato-annotation-1.2.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(
     name='potato-annotation',
-    version='1.2.2.2',
+    version='1.2.2.3',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'potato = potato.cli:potato',
         ],
     },
     url="https://github.com/davidjurgens/potato",
```

