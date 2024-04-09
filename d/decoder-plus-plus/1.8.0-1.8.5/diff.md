# Comparing `tmp/decoder-plus-plus-1.8.0.tar.gz` & `tmp/decoder-plus-plus-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoder-plus-plus-1.8.0.tar", last modified: Sun Apr  7 22:34:08 2024, max compression
+gzip compressed data, was "decoder-plus-plus-1.8.5.tar", last modified: Tue Apr  9 13:35:13 2024, max compression
```

## Comparing `decoder-plus-plus-1.8.0.tar` & `decoder-plus-plus-1.8.5.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.743225 decoder-plus-plus-1.8.0/
--rw-rw-r--   0 tom       (1000) tom       (1000)    35147 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       43 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)     7935 2024-04-07 22:34:08.743225 decoder-plus-plus-1.8.0/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     7367 2024-04-07 09:27:21.000000 decoder-plus-plus-1.8.0/README.md
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.631226 decoder-plus-plus-1.8.0/data/
--rwxrwxr-x   0 tom       (1000) tom       (1000)      116 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/data/dpp.desktop
--rw-rw-r--   0 tom       (1000) tom       (1000)    19277 2024-04-06 19:21:46.000000 decoder-plus-plus-1.8.0/data/dpp.png
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.631226 decoder-plus-plus-1.8.0/decoder_plus_plus.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)     7935 2024-04-07 22:34:08.000000 decoder-plus-plus-1.8.0/decoder_plus_plus.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     9125 2024-04-07 22:34:08.000000 decoder-plus-plus-1.8.0/decoder_plus_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-04-07 22:34:08.000000 decoder-plus-plus-1.8.0/decoder_plus_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       40 2024-04-07 22:34:08.000000 decoder-plus-plus-1.8.0/decoder_plus_plus.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)      391 2024-04-07 22:34:08.000000 decoder-plus-plus-1.8.0/decoder_plus_plus.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       10 2024-04-07 22:34:08.000000 decoder-plus-plus-1.8.0/decoder_plus_plus.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.635226 decoder-plus-plus-1.8.0/dpp/
--rw-rw-r--   0 tom       (1000) tom       (1000)      850 2024-04-07 22:31:04.000000 decoder-plus-plus-1.8.0/dpp/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      239 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/dpp/__main__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.639226 decoder-plus-plus-1.8.0/dpp/core/
--rw-rw-r--   0 tom       (1000) tom       (1000)      915 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/dpp/core/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2353 2022-09-12 19:05:02.000000 decoder-plus-plus-1.8.0/dpp/core/argparse.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2871 2022-09-12 21:57:24.000000 decoder-plus-plus-1.8.0/dpp/core/assertions.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3279 2022-08-17 05:09:19.000000 decoder-plus-plus-1.8.0/dpp/core/config.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10068 2024-04-05 20:12:39.000000 decoder-plus-plus-1.8.0/dpp/core/context.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/core/decoder_plus_plus.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      906 2022-09-18 10:36:35.000000 decoder-plus-plus-1.8.0/dpp/core/exceptions.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2860 2024-04-07 11:17:10.000000 decoder-plus-plus-1.8.0/dpp/core/icons.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3650 2023-02-28 12:27:33.000000 decoder-plus-plus-1.8.0/dpp/core/listener.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4546 2023-01-29 15:42:26.000000 decoder-plus-plus-1.8.0/dpp/core/logger.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1329 2022-09-14 00:12:52.000000 decoder-plus-plus-1.8.0/dpp/core/math.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.643226 decoder-plus-plus-1.8.0/dpp/core/plugin/
--rw-rw-r--   0 tom       (1000) tom       (1000)    14067 2024-04-06 16:14:35.000000 decoder-plus-plus-1.8.0/dpp/core/plugin/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2324 2024-04-06 15:25:06.000000 decoder-plus-plus-1.8.0/dpp/core/plugin/builder.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.643226 decoder-plus-plus-1.8.0/dpp/core/plugin/config/
--rw-rw-r--   0 tom       (1000) tom       (1000)     8387 2024-04-06 08:18:07.000000 decoder-plus-plus-1.8.0/dpp/core/plugin/config/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.643226 decoder-plus-plus-1.8.0/dpp/core/plugin/config/options/
--rw-rw-r--   0 tom       (1000) tom       (1000)     3478 2024-04-06 16:14:35.000000 decoder-plus-plus-1.8.0/dpp/core/plugin/config/options/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.647226 decoder-plus-plus-1.8.0/dpp/core/plugin/config/ui/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1572 2022-09-12 21:57:24.000000 decoder-plus-plus-1.8.0/dpp/core/plugin/config/ui/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      858 2022-09-06 21:38:42.000000 decoder-plus-plus-1.8.0/dpp/core/plugin/config/ui/layouts.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2111 2024-04-06 15:51:05.000000 decoder-plus-plus-1.8.0/dpp/core/plugin/config/ui/widgets.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3048 2022-09-13 07:31:54.000000 decoder-plus-plus-1.8.0/dpp/core/plugin/loader.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4301 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/core/plugin/manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3878 2022-08-21 00:18:15.000000 decoder-plus-plus-1.8.0/dpp/core/shortcuts.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.663226 decoder-plus-plus-1.8.0/dpp/images/
--rw-rw-r--   0 tom       (1000) tom       (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/dpp/images/dpp.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/dpp/images/dpp_128.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/dpp/images/dpp_classic.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/dpp/images/dpp_classic_128.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    90434 2022-09-06 22:45:08.000000 decoder-plus-plus-1.8.0/dpp/images/dpp_modern.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    30058 2022-09-06 22:47:19.000000 decoder-plus-plus-1.8.0/dpp/images/dpp_modern_128.png
--rw-rw-r--   0 tom       (1000) tom       (1000)  1494359 2022-09-06 22:43:36.000000 decoder-plus-plus-1.8.0/dpp/images/dpp_modern_big.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    56153 2024-04-06 19:21:10.000000 decoder-plus-plus-1.8.0/dpp/images/dpp_stylized.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    19277 2024-04-06 19:21:46.000000 decoder-plus-plus-1.8.0/dpp/images/dpp_stylized_128.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    25196 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/dpp/images/dpp_xmas.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    52648 2024-04-06 19:39:41.000000 decoder-plus-plus-1.8.0/dpp/images/dpp_xmas_stylized.png
--rw-rw-r--   0 tom       (1000) tom       (1000)      258 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/dpp/images/hidden.png
--rw-rw-r--   0 tom       (1000) tom       (1000)      349 2022-09-13 21:04:47.000000 decoder-plus-plus-1.8.0/dpp/images/indicator_green.png
--rw-rw-r--   0 tom       (1000) tom       (1000)      417 2022-09-13 21:05:13.000000 decoder-plus-plus-1.8.0/dpp/images/indicator_grey.png
--rw-rw-r--   0 tom       (1000) tom       (1000)      319 2022-09-13 21:05:36.000000 decoder-plus-plus-1.8.0/dpp/images/indicator_red.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    11652 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/dpp/images/keyboard.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    27999 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/dpp/images/keyboard.svg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.707225 decoder-plus-plus-1.8.0/dpp/plugins/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/adler32_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1393 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/apache_md5_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/base16_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/base16_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1824 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/base32_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1529 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/base32_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1755 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/base45_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1482 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/base45_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2097 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/base64_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1470 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/base64_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2678 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/base64_url_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1693 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/base64_url_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1241 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.0/dpp/plugins/bin_int_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1249 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.0/dpp/plugins/bin_int_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1519 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.0/dpp/plugins/bin_str_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1695 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.0/dpp/plugins/bin_str_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5641 2024-04-05 16:00:23.000000 decoder-plus-plus-1.8.0/dpp/plugins/caesar_cipher_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1065 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/clone_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1320 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/crc32_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1159 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/css_minify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5888 2024-04-06 15:56:04.000000 decoder-plus-plus-1.8.0/dpp/plugins/custom_code.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1475 2022-09-17 09:13:06.000000 decoder-plus-plus-1.8.0/dpp/plugins/dec_str_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1441 2022-09-17 09:13:12.000000 decoder-plus-plus-1.8.0/dpp/plugins/dec_str_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1068 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/escape_string_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1211 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/extract_urls_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5143 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/filter_lines_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1386 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/free_bsd_nt_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1653 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/gzip_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1408 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/gzip_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2110 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.0/dpp/plugins/hex_char_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1582 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.0/dpp/plugins/hex_char_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1448 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.0/dpp/plugins/hex_int_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1217 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.0/dpp/plugins/hex_int_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2331 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.0/dpp/plugins/hex_shell_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1980 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.0/dpp/plugins/hex_shell_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1709 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.0/dpp/plugins/hex_str_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1561 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.0/dpp/plugins/hex_str_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1221 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/html_beautify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1783 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/html_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1377 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/html_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1138 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/html_minify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2539 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/http64_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1841 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/http64_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2265 2024-04-07 11:11:41.000000 decoder-plus-plus-1.8.0/dpp/plugins/identify_decoder_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1371 2024-04-07 11:16:17.000000 decoder-plus-plus-1.8.0/dpp/plugins/identify_file_type_filemagic_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2024-04-07 11:16:17.000000 decoder-plus-plus-1.8.0/dpp/plugins/identify_file_type_magika_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1389 2024-04-07 11:03:59.000000 decoder-plus-plus-1.8.0/dpp/plugins/identify_hash_format_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2254 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/jq_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1336 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/js_beautify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1131 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/js_minify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1171 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/js_to_xml_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    15185 2024-04-07 08:30:22.000000 decoder-plus-plus-1.8.0/dpp/plugins/jsonify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2621 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/jsonpath_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2568 2024-04-07 18:47:41.000000 decoder-plus-plus-1.8.0/dpp/plugins/jwt_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2345 2024-04-07 18:56:21.000000 decoder-plus-plus-1.8.0/dpp/plugins/jwt_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1432 2022-09-15 16:34:02.000000 decoder-plus-plus-1.8.0/dpp/plugins/keccak224_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1440 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/keccak256_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1472 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/keccak384_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1519 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/keccak512_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1446 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/little_big_endian_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/lm_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2024-04-07 19:19:24.000000 decoder-plus-plus-1.8.0/dpp/plugins/md2_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2024-04-07 19:19:24.000000 decoder-plus-plus-1.8.0/dpp/plugins/md4_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1352 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/md5_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/nt_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1223 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.0/dpp/plugins/oct_int_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1228 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.0/dpp/plugins/oct_int_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1775 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.0/dpp/plugins/oct_str_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1576 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.0/dpp/plugins/oct_str_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1368 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/phpass_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6590 2024-04-05 18:32:58.000000 decoder-plus-plus-1.8.0/dpp/plugins/reformat_text_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1115 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/remove_newlines_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1121 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/remove_whitespaces_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1693 2024-04-07 07:30:09.000000 decoder-plus-plus-1.8.0/dpp/plugins/ripemd160_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/rot13_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/rot13_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4506 2024-04-05 18:32:58.000000 decoder-plus-plus-1.8.0/dpp/plugins/search_and_replace_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1363 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/sha1_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1401 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/sha224_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1409 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/sha256_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1441 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/sha384_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1382 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/sha3_224_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1383 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/sha3_256_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1415 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/sha3_384_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1462 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/plugins/sha3_512_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.0/dpp/plugins/sha512_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4998 2024-04-05 18:32:58.000000 decoder-plus-plus-1.8.0/dpp/plugins/split_and_rejoin_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1400 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.0/dpp/plugins/sun_md5_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1107 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.0/dpp/plugins/unescape_string_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1993 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.0/dpp/plugins/url_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1487 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.0/dpp/plugins/url_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1974 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.0/dpp/plugins/url_plus_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1525 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.0/dpp/plugins/url_plus_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2291 2023-01-15 14:37:27.000000 decoder-plus-plus-1.8.0/dpp/plugins/xpath_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1821 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.0/dpp/plugins/zlib_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1394 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.0/dpp/plugins/zlib_encoder.py
--rwxrwxr-x   0 tom       (1000) tom       (1000)    16769 2022-09-21 05:00:04.000000 decoder-plus-plus-1.8.0/dpp/runner.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.707225 decoder-plus-plus-1.8.0/dpp/ui/
--rw-rw-r--   0 tom       (1000) tom       (1000)      967 2022-09-06 05:50:59.000000 decoder-plus-plus-1.8.0/dpp/ui/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.711225 decoder-plus-plus-1.8.0/dpp/ui/builder/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/dpp/ui/builder/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1962 2022-08-15 20:49:18.000000 decoder-plus-plus-1.8.0/dpp/ui/builder/action_builder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1682 2024-04-05 15:27:20.000000 decoder-plus-plus-1.8.0/dpp/ui/builder/plugin_config_widget_builder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10393 2024-04-07 07:53:50.000000 decoder-plus-plus-1.8.0/dpp/ui/builder/widget_builder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6388 2023-01-29 15:44:47.000000 decoder-plus-plus-1.8.0/dpp/ui/decoder_plus_plus_gui.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.711225 decoder-plus-plus-1.8.0/dpp/ui/dialog/
--rw-rw-r--   0 tom       (1000) tom       (1000)      706 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/dpp/ui/dialog/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5833 2024-04-06 19:42:04.000000 decoder-plus-plus-1.8.0/dpp/ui/dialog/config_dialog.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5273 2022-09-10 21:34:51.000000 decoder-plus-plus-1.8.0/dpp/ui/dialog/keyboard_shortcut_dialog.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5810 2024-04-07 18:45:09.000000 decoder-plus-plus-1.8.0/dpp/ui/dialog/plugin_config_dialog.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.711225 decoder-plus-plus-1.8.0/dpp/ui/dock/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.0/dpp/ui/dock/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10582 2023-02-28 12:28:51.000000 decoder-plus-plus-1.8.0/dpp/ui/dock/hex_dock.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    12701 2022-09-12 19:05:02.000000 decoder-plus-plus-1.8.0/dpp/ui/dock/log_dock.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2564 2022-09-07 22:11:21.000000 decoder-plus-plus-1.8.0/dpp/ui/instance_handler.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.711225 decoder-plus-plus-1.8.0/dpp/ui/view/
--rw-rw-r--   0 tom       (1000) tom       (1000)      706 2022-08-18 00:21:03.000000 decoder-plus-plus-1.8.0/dpp/ui/view/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.715225 decoder-plus-plus-1.8.0/dpp/ui/view/classic/
--rw-rw-r--   0 tom       (1000) tom       (1000)      839 2022-08-20 19:51:05.000000 decoder-plus-plus-1.8.0/dpp/ui/view/classic/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10186 2024-04-06 16:14:35.000000 decoder-plus-plus-1.8.0/dpp/ui/view/classic/classic_main_window_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    16776 2024-04-07 22:32:06.000000 decoder-plus-plus-1.8.0/dpp/ui/view/classic/codec_frame.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    13154 2024-04-07 22:17:55.000000 decoder-plus-plus-1.8.0/dpp/ui/view/classic/codec_frame_header.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    20558 2024-04-07 22:18:29.000000 decoder-plus-plus-1.8.0/dpp/ui/view/classic/codec_frames.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2401 2022-09-20 04:28:03.000000 decoder-plus-plus-1.8.0/dpp/ui/view/classic/codec_tab.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     9167 2023-01-30 13:35:51.000000 decoder-plus-plus-1.8.0/dpp/ui/view/classic/combo_box_frame.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10716 2022-09-21 05:00:04.000000 decoder-plus-plus-1.8.0/dpp/ui/view/main_window_widget.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.715225 decoder-plus-plus-1.8.0/dpp/ui/view/modern/
--rw-rw-r--   0 tom       (1000) tom       (1000)      705 2022-08-20 19:51:05.000000 decoder-plus-plus-1.8.0/dpp/ui/view/modern/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2460 2022-09-17 10:02:26.000000 decoder-plus-plus-1.8.0/dpp/ui/view/modern/modern_main_window_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      705 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/ui/view/modern/node_data.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5229 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/ui/view/modern/node_data_models.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      409 2022-08-30 00:07:08.000000 decoder-plus-plus-1.8.0/dpp/ui/view/modern/node_data_models_builder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2001 2022-09-17 10:02:44.000000 decoder-plus-plus-1.8.0/dpp/ui/view/modern/node_editor.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1782 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/ui/view/modern/node_editor_tab.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.727225 decoder-plus-plus-1.8.0/dpp/ui/widget/
--rw-rw-r--   0 tom       (1000) tom       (1000)      805 2022-08-16 19:35:20.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1367 2022-08-15 23:02:30.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/clickable_label.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3507 2024-04-06 16:14:35.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/code_editor_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3404 2024-04-07 09:41:34.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/codec_preview_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    11051 2024-04-06 07:30:01.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/collapsible_frame.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2161 2022-09-10 22:00:08.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/combo_box.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4686 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/dock_tabs_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     7690 2022-08-20 19:51:05.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/dock_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1887 2022-08-15 20:48:14.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/dyna_frame.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      755 2022-08-15 20:44:52.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/elided_label.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2453 2024-04-06 20:17:41.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/hover_label.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1793 2024-04-06 07:22:30.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/icon_label.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3270 2024-04-07 11:20:24.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/identify_format_button.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3269 2022-09-12 19:34:03.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/list_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1151 2022-08-21 00:18:15.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/menu_bar.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2136 2024-04-06 09:24:31.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/message_box_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6687 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/message_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6110 2024-04-06 15:44:53.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/option_widgets.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    17112 2024-04-07 22:03:57.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/plain_view.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2621 2022-09-08 00:44:43.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/plugin_frame.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     9593 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/plugin_tab.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4396 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/search_field.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1246 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/separater_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5000 2022-08-15 23:02:30.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/shortcut_table.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2846 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/slider_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4055 2022-09-20 10:34:13.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/smart_decode_button.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1442 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/spacers.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2425 2023-01-30 12:23:56.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/status_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3757 2022-08-20 19:51:05.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/tab_bar.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8075 2022-09-15 01:50:24.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/tabs_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3210 2024-04-05 11:52:36.000000 decoder-plus-plus-1.8.0/dpp/ui/widget/text_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-04-07 22:34:08.743225 decoder-plus-plus-1.8.0/setup.cfg
--rw-rw-r--   0 tom       (1000) tom       (1000)     2681 2024-04-07 18:40:37.000000 decoder-plus-plus-1.8.0/setup.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.727225 decoder-plus-plus-1.8.0/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1805 2023-01-15 14:31:34.000000 decoder-plus-plus-1.8.0/tests/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.743225 decoder-plus-plus-1.8.0/tests/plugins/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2022-11-01 13:33:59.000000 decoder-plus-plus-1.8.0/tests/plugins/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1113 2022-11-01 14:08:45.000000 decoder-plus-plus-1.8.0/tests/plugins/adler32_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1191 2022-11-01 18:50:27.000000 decoder-plus-plus-1.8.0/tests/plugins/apache_md5_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1295 2022-11-01 18:05:54.000000 decoder-plus-plus-1.8.0/tests/plugins/base16_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1680 2023-01-15 13:01:54.000000 decoder-plus-plus-1.8.0/tests/plugins/base32_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1287 2023-01-15 13:32:25.000000 decoder-plus-plus-1.8.0/tests/plugins/base45_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1288 2023-01-15 12:36:51.000000 decoder-plus-plus-1.8.0/tests/plugins/base64_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2023-01-15 12:47:27.000000 decoder-plus-plus-1.8.0/tests/plugins/base64_url_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1229 2023-01-15 13:29:43.000000 decoder-plus-plus-1.8.0/tests/plugins/bin_int_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1040 2022-11-01 18:51:09.000000 decoder-plus-plus-1.8.0/tests/plugins/bin_str_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      992 2023-01-15 12:47:59.000000 decoder-plus-plus-1.8.0/tests/plugins/caesar_cipher_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1222 2022-11-01 18:35:38.000000 decoder-plus-plus-1.8.0/tests/plugins/clone_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2023-01-15 12:37:31.000000 decoder-plus-plus-1.8.0/tests/plugins/crc32_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1183 2022-11-01 18:39:55.000000 decoder-plus-plus-1.8.0/tests/plugins/css_minify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1401 2022-11-01 18:35:21.000000 decoder-plus-plus-1.8.0/tests/plugins/dec_str_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1245 2022-11-01 18:59:45.000000 decoder-plus-plus-1.8.0/tests/plugins/escape_string_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1123 2022-11-01 18:47:57.000000 decoder-plus-plus-1.8.0/tests/plugins/extract_urls_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1165 2022-11-01 18:40:22.000000 decoder-plus-plus-1.8.0/tests/plugins/filter_lines_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1189 2023-01-15 13:03:50.000000 decoder-plus-plus-1.8.0/tests/plugins/free_bsd_nt_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1253 2023-01-15 12:29:09.000000 decoder-plus-plus-1.8.0/tests/plugins/gzip_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1067 2022-11-01 18:47:18.000000 decoder-plus-plus-1.8.0/tests/plugins/hex_char_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1193 2023-01-15 13:10:42.000000 decoder-plus-plus-1.8.0/tests/plugins/hex_int_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1614 2022-11-01 18:43:06.000000 decoder-plus-plus-1.8.0/tests/plugins/hex_shell_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1313 2023-01-15 13:16:46.000000 decoder-plus-plus-1.8.0/tests/plugins/hex_str_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1173 2022-11-01 18:43:28.000000 decoder-plus-plus-1.8.0/tests/plugins/html_beautify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1168 2022-11-01 18:48:47.000000 decoder-plus-plus-1.8.0/tests/plugins/html_minify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1172 2023-01-15 12:22:31.000000 decoder-plus-plus-1.8.0/tests/plugins/html_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1219 2022-11-01 18:32:01.000000 decoder-plus-plus-1.8.0/tests/plugins/http64_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1016 2024-04-07 12:31:43.000000 decoder-plus-plus-1.8.0/tests/plugins/identify_file_type_filemagic_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1019 2024-04-07 12:32:46.000000 decoder-plus-plus-1.8.0/tests/plugins/identify_file_type_magika_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2022-11-01 18:39:55.000000 decoder-plus-plus-1.8.0/tests/plugins/identify_hash_format_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1145 2023-01-15 13:26:35.000000 decoder-plus-plus-1.8.0/tests/plugins/jq_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      988 2023-01-15 12:41:00.000000 decoder-plus-plus-1.8.0/tests/plugins/js_beautify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1164 2022-11-01 18:49:20.000000 decoder-plus-plus-1.8.0/tests/plugins/js_minify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      977 2023-01-15 13:06:33.000000 decoder-plus-plus-1.8.0/tests/plugins/js_to_xml_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      981 2023-01-15 13:02:34.000000 decoder-plus-plus-1.8.0/tests/plugins/jsonify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1163 2022-11-01 18:49:36.000000 decoder-plus-plus-1.8.0/tests/plugins/jsonpath_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      976 2023-01-15 12:39:55.000000 decoder-plus-plus-1.8.0/tests/plugins/jwt_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1163 2023-01-15 13:02:49.000000 decoder-plus-plus-1.8.0/tests/plugins/keccak224_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1171 2022-11-01 18:56:46.000000 decoder-plus-plus-1.8.0/tests/plugins/keccak256_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1203 2022-11-01 18:45:25.000000 decoder-plus-plus-1.8.0/tests/plugins/keccak384_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1235 2022-11-01 18:48:57.000000 decoder-plus-plus-1.8.0/tests/plugins/keccak512_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1245 2022-11-01 18:31:13.000000 decoder-plus-plus-1.8.0/tests/plugins/little_big_endian_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1124 2022-11-01 18:56:24.000000 decoder-plus-plus-1.8.0/tests/plugins/lm_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:24:14.000000 decoder-plus-plus-1.8.0/tests/plugins/md2_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:56:15.000000 decoder-plus-plus-1.8.0/tests/plugins/md4_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:45:18.000000 decoder-plus-plus-1.8.0/tests/plugins/md5_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1124 2022-11-01 18:46:24.000000 decoder-plus-plus-1.8.0/tests/plugins/nt_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1193 2023-01-15 13:13:49.000000 decoder-plus-plus-1.8.0/tests/plugins/oct_int_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1405 2022-11-01 18:20:57.000000 decoder-plus-plus-1.8.0/tests/plugins/oct_str_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1181 2023-01-15 12:51:06.000000 decoder-plus-plus-1.8.0/tests/plugins/phpass_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1167 2022-11-01 18:57:07.000000 decoder-plus-plus-1.8.0/tests/plugins/reformat_text_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1187 2023-01-15 13:04:21.000000 decoder-plus-plus-1.8.0/tests/plugins/remove_newlines_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1064 2022-11-01 18:56:04.000000 decoder-plus-plus-1.8.0/tests/plugins/remove_whitespaces_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1146 2022-11-01 18:56:36.000000 decoder-plus-plus-1.8.0/tests/plugins/ripemd160_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1225 2022-11-01 18:26:44.000000 decoder-plus-plus-1.8.0/tests/plugins/rot13_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1503 2023-01-15 13:05:35.000000 decoder-plus-plus-1.8.0/tests/plugins/search_and_replace_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2022-11-01 18:27:54.000000 decoder-plus-plus-1.8.0/tests/plugins/sha1_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1192 2022-11-01 18:29:14.000000 decoder-plus-plus-1.8.0/tests/plugins/sha224_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1200 2022-11-01 18:29:35.000000 decoder-plus-plus-1.8.0/tests/plugins/sha256_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1231 2022-11-01 18:29:59.000000 decoder-plus-plus-1.8.0/tests/plugins/sha384_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1160 2023-01-15 12:37:21.000000 decoder-plus-plus-1.8.0/tests/plugins/sha3_224_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1168 2022-11-01 18:53:45.000000 decoder-plus-plus-1.8.0/tests/plugins/sha3_256_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1200 2022-11-01 18:28:35.000000 decoder-plus-plus-1.8.0/tests/plugins/sha3_384_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1268 2022-11-01 18:28:57.000000 decoder-plus-plus-1.8.0/tests/plugins/sha3_512_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1263 2022-11-01 18:30:17.000000 decoder-plus-plus-1.8.0/tests/plugins/sha512_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1170 2022-11-01 18:57:46.000000 decoder-plus-plus-1.8.0/tests/plugins/split_and_rejoin_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      983 2023-01-15 12:39:55.000000 decoder-plus-plus-1.8.0/tests/plugins/sun_md5_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1247 2022-11-01 18:32:56.000000 decoder-plus-plus-1.8.0/tests/plugins/unescape_string_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1282 2022-11-01 18:45:08.000000 decoder-plus-plus-1.8.0/tests/plugins/url_plus_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2022-11-01 18:53:35.000000 decoder-plus-plus-1.8.0/tests/plugins/url_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2023-01-15 14:38:44.000000 decoder-plus-plus-1.8.0/tests/plugins/xpath_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1223 2023-01-15 13:12:30.000000 decoder-plus-plus-1.8.0/tests/plugins/zlib_test.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 22:34:08.743225 decoder-plus-plus-1.8.0/tests/ui/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-01-15 14:39:42.000000 decoder-plus-plus-1.8.0/tests/ui/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10085 2024-04-07 18:07:00.000000 decoder-plus-plus-1.8.0/tests/ui/classic_mode_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      512 2023-01-15 15:28:09.000000 decoder-plus-plus-1.8.0/tests/utils.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.845847 decoder-plus-plus-1.8.5/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    35147 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       43 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8353 2024-04-09 13:35:13.845847 decoder-plus-plus-1.8.5/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7765 2024-04-09 10:22:06.000000 decoder-plus-plus-1.8.5/README.md
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.737846 decoder-plus-plus-1.8.5/data/
+-rwxrwxr-x   0 tom       (1000) tom       (1000)      116 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/data/dpp.desktop
+-rw-rw-r--   0 tom       (1000) tom       (1000)    19277 2024-04-06 19:21:46.000000 decoder-plus-plus-1.8.5/data/dpp.png
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.737846 decoder-plus-plus-1.8.5/decoder_plus_plus.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8353 2024-04-09 13:35:13.000000 decoder-plus-plus-1.8.5/decoder_plus_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9125 2024-04-09 13:35:13.000000 decoder-plus-plus-1.8.5/decoder_plus_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-04-09 13:35:13.000000 decoder-plus-plus-1.8.5/decoder_plus_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       41 2024-04-09 13:35:13.000000 decoder-plus-plus-1.8.5/decoder_plus_plus.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)      412 2024-04-09 13:35:13.000000 decoder-plus-plus-1.8.5/decoder_plus_plus.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       10 2024-04-09 13:35:13.000000 decoder-plus-plus-1.8.5/decoder_plus_plus.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.741846 decoder-plus-plus-1.8.5/dpp/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      850 2024-04-09 13:26:51.000000 decoder-plus-plus-1.8.5/dpp/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      239 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/dpp/__main__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.745846 decoder-plus-plus-1.8.5/dpp/core/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      915 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/dpp/core/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2353 2022-09-12 19:05:02.000000 decoder-plus-plus-1.8.5/dpp/core/argparse.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2871 2022-09-12 21:57:24.000000 decoder-plus-plus-1.8.5/dpp/core/assertions.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3279 2022-08-17 05:09:19.000000 decoder-plus-plus-1.8.5/dpp/core/config.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10068 2024-04-09 13:11:44.000000 decoder-plus-plus-1.8.5/dpp/core/context.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/core/decoder_plus_plus.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      906 2022-09-18 10:36:35.000000 decoder-plus-plus-1.8.5/dpp/core/exceptions.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2860 2024-04-07 11:17:10.000000 decoder-plus-plus-1.8.5/dpp/core/icons.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4394 2024-04-09 13:19:10.000000 decoder-plus-plus-1.8.5/dpp/core/listener.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4546 2023-01-29 15:42:26.000000 decoder-plus-plus-1.8.5/dpp/core/logger.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1329 2022-09-14 00:12:52.000000 decoder-plus-plus-1.8.5/dpp/core/math.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.745846 decoder-plus-plus-1.8.5/dpp/core/plugin/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    14067 2024-04-09 13:12:10.000000 decoder-plus-plus-1.8.5/dpp/core/plugin/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2324 2024-04-06 15:25:06.000000 decoder-plus-plus-1.8.5/dpp/core/plugin/builder.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.745846 decoder-plus-plus-1.8.5/dpp/core/plugin/config/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8387 2024-04-06 08:18:07.000000 decoder-plus-plus-1.8.5/dpp/core/plugin/config/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.745846 decoder-plus-plus-1.8.5/dpp/core/plugin/config/options/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3478 2024-04-06 16:14:35.000000 decoder-plus-plus-1.8.5/dpp/core/plugin/config/options/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.745846 decoder-plus-plus-1.8.5/dpp/core/plugin/config/ui/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1572 2022-09-12 21:57:24.000000 decoder-plus-plus-1.8.5/dpp/core/plugin/config/ui/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      858 2022-09-06 21:38:42.000000 decoder-plus-plus-1.8.5/dpp/core/plugin/config/ui/layouts.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2111 2024-04-06 15:51:05.000000 decoder-plus-plus-1.8.5/dpp/core/plugin/config/ui/widgets.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3048 2022-09-13 07:31:54.000000 decoder-plus-plus-1.8.5/dpp/core/plugin/loader.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4301 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/core/plugin/manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3878 2022-08-21 00:18:15.000000 decoder-plus-plus-1.8.5/dpp/core/shortcuts.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.761846 decoder-plus-plus-1.8.5/dpp/images/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/dpp/images/dpp.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/dpp/images/dpp_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/dpp/images/dpp_classic.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/dpp/images/dpp_classic_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    90434 2022-09-06 22:45:08.000000 decoder-plus-plus-1.8.5/dpp/images/dpp_modern.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    30058 2022-09-06 22:47:19.000000 decoder-plus-plus-1.8.5/dpp/images/dpp_modern_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1494359 2022-09-06 22:43:36.000000 decoder-plus-plus-1.8.5/dpp/images/dpp_modern_big.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    56153 2024-04-06 19:21:10.000000 decoder-plus-plus-1.8.5/dpp/images/dpp_stylized.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    19277 2024-04-06 19:21:46.000000 decoder-plus-plus-1.8.5/dpp/images/dpp_stylized_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    25196 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/dpp/images/dpp_xmas.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    52648 2024-04-06 19:39:41.000000 decoder-plus-plus-1.8.5/dpp/images/dpp_xmas_stylized.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      258 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/dpp/images/hidden.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      349 2022-09-13 21:04:47.000000 decoder-plus-plus-1.8.5/dpp/images/indicator_green.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      417 2022-09-13 21:05:13.000000 decoder-plus-plus-1.8.5/dpp/images/indicator_grey.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      319 2022-09-13 21:05:36.000000 decoder-plus-plus-1.8.5/dpp/images/indicator_red.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    11652 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/dpp/images/keyboard.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    27999 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/dpp/images/keyboard.svg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.793846 decoder-plus-plus-1.8.5/dpp/plugins/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/adler32_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1393 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/apache_md5_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/base16_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/base16_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1824 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/base32_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1529 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/base32_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1755 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/base45_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1482 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/base45_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2097 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/base64_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1470 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/base64_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2678 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/base64_url_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1693 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/base64_url_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1241 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.5/dpp/plugins/bin_int_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1249 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.5/dpp/plugins/bin_int_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1519 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.5/dpp/plugins/bin_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1695 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.5/dpp/plugins/bin_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5641 2024-04-05 16:00:23.000000 decoder-plus-plus-1.8.5/dpp/plugins/caesar_cipher_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1065 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/clone_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1320 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/crc32_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1159 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/css_minify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5888 2024-04-06 15:56:04.000000 decoder-plus-plus-1.8.5/dpp/plugins/custom_code.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1475 2022-09-17 09:13:06.000000 decoder-plus-plus-1.8.5/dpp/plugins/dec_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1441 2022-09-17 09:13:12.000000 decoder-plus-plus-1.8.5/dpp/plugins/dec_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1068 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/escape_string_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1211 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/extract_urls_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5143 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/filter_lines_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1386 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/free_bsd_nt_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1653 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/gzip_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1408 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/gzip_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2110 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.5/dpp/plugins/hex_char_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1582 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.5/dpp/plugins/hex_char_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1448 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.5/dpp/plugins/hex_int_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1217 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.5/dpp/plugins/hex_int_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2331 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.5/dpp/plugins/hex_shell_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1980 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.5/dpp/plugins/hex_shell_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1709 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.5/dpp/plugins/hex_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1561 2022-11-01 18:01:29.000000 decoder-plus-plus-1.8.5/dpp/plugins/hex_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1221 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/html_beautify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1783 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/html_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1377 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/html_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1138 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/html_minify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2539 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/http64_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1841 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/http64_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2265 2024-04-07 11:11:41.000000 decoder-plus-plus-1.8.5/dpp/plugins/identify_decoder_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1371 2024-04-07 11:16:17.000000 decoder-plus-plus-1.8.5/dpp/plugins/identify_file_type_filemagic_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2024-04-07 11:16:17.000000 decoder-plus-plus-1.8.5/dpp/plugins/identify_file_type_magika_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1389 2024-04-07 11:03:59.000000 decoder-plus-plus-1.8.5/dpp/plugins/identify_hash_format_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2254 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/jq_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1336 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/js_beautify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1131 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/js_minify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1171 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/js_to_xml_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    15185 2024-04-07 08:30:22.000000 decoder-plus-plus-1.8.5/dpp/plugins/jsonify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2621 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/jsonpath_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2645 2024-04-09 12:18:02.000000 decoder-plus-plus-1.8.5/dpp/plugins/jwt_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2345 2024-04-07 18:56:21.000000 decoder-plus-plus-1.8.5/dpp/plugins/jwt_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1432 2022-09-15 16:34:02.000000 decoder-plus-plus-1.8.5/dpp/plugins/keccak224_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1440 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/keccak256_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1472 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/keccak384_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1519 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/keccak512_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1446 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/little_big_endian_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/lm_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2024-04-07 19:19:24.000000 decoder-plus-plus-1.8.5/dpp/plugins/md2_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2024-04-07 19:19:24.000000 decoder-plus-plus-1.8.5/dpp/plugins/md4_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1352 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/md5_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/nt_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1223 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.5/dpp/plugins/oct_int_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1228 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.5/dpp/plugins/oct_int_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1775 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.5/dpp/plugins/oct_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1576 2022-09-17 09:11:33.000000 decoder-plus-plus-1.8.5/dpp/plugins/oct_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1368 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/phpass_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6590 2024-04-05 18:32:58.000000 decoder-plus-plus-1.8.5/dpp/plugins/reformat_text_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1115 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/remove_newlines_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1121 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/remove_whitespaces_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1693 2024-04-07 07:30:09.000000 decoder-plus-plus-1.8.5/dpp/plugins/ripemd160_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/rot13_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/rot13_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4506 2024-04-05 18:32:58.000000 decoder-plus-plus-1.8.5/dpp/plugins/search_and_replace_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1363 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/sha1_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1401 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/sha224_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1409 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/sha256_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1441 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/sha384_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1382 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/sha3_224_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1383 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/sha3_256_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1415 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/sha3_384_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1462 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/plugins/sha3_512_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.5/dpp/plugins/sha512_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4998 2024-04-05 18:32:58.000000 decoder-plus-plus-1.8.5/dpp/plugins/split_and_rejoin_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1400 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.5/dpp/plugins/sun_md5_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1107 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.5/dpp/plugins/unescape_string_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1993 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.5/dpp/plugins/url_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1487 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.5/dpp/plugins/url_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1974 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.5/dpp/plugins/url_plus_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1525 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.5/dpp/plugins/url_plus_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2291 2023-01-15 14:37:27.000000 decoder-plus-plus-1.8.5/dpp/plugins/xpath_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1821 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.5/dpp/plugins/zlib_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1394 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.5/dpp/plugins/zlib_encoder.py
+-rwxrwxr-x   0 tom       (1000) tom       (1000)    16769 2022-09-21 05:00:04.000000 decoder-plus-plus-1.8.5/dpp/runner.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.797846 decoder-plus-plus-1.8.5/dpp/ui/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      967 2022-09-06 05:50:59.000000 decoder-plus-plus-1.8.5/dpp/ui/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.797846 decoder-plus-plus-1.8.5/dpp/ui/builder/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/dpp/ui/builder/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1962 2022-08-15 20:49:18.000000 decoder-plus-plus-1.8.5/dpp/ui/builder/action_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1682 2024-04-05 15:27:20.000000 decoder-plus-plus-1.8.5/dpp/ui/builder/plugin_config_widget_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10393 2024-04-07 07:53:50.000000 decoder-plus-plus-1.8.5/dpp/ui/builder/widget_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6388 2023-01-29 15:44:47.000000 decoder-plus-plus-1.8.5/dpp/ui/decoder_plus_plus_gui.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.797846 decoder-plus-plus-1.8.5/dpp/ui/dialog/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      706 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/dpp/ui/dialog/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5833 2024-04-06 19:42:04.000000 decoder-plus-plus-1.8.5/dpp/ui/dialog/config_dialog.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5273 2022-09-10 21:34:51.000000 decoder-plus-plus-1.8.5/dpp/ui/dialog/keyboard_shortcut_dialog.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5810 2024-04-07 18:45:09.000000 decoder-plus-plus-1.8.5/dpp/ui/dialog/plugin_config_dialog.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.801846 decoder-plus-plus-1.8.5/dpp/ui/dock/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.8.5/dpp/ui/dock/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10582 2023-02-28 12:28:51.000000 decoder-plus-plus-1.8.5/dpp/ui/dock/hex_dock.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    12701 2022-09-12 19:05:02.000000 decoder-plus-plus-1.8.5/dpp/ui/dock/log_dock.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2564 2022-09-07 22:11:21.000000 decoder-plus-plus-1.8.5/dpp/ui/instance_handler.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.801846 decoder-plus-plus-1.8.5/dpp/ui/view/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      706 2022-08-18 00:21:03.000000 decoder-plus-plus-1.8.5/dpp/ui/view/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.801846 decoder-plus-plus-1.8.5/dpp/ui/view/classic/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      839 2022-08-20 19:51:05.000000 decoder-plus-plus-1.8.5/dpp/ui/view/classic/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10186 2024-04-06 16:14:35.000000 decoder-plus-plus-1.8.5/dpp/ui/view/classic/classic_main_window_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18053 2024-04-07 23:13:56.000000 decoder-plus-plus-1.8.5/dpp/ui/view/classic/codec_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    13154 2024-04-08 09:28:50.000000 decoder-plus-plus-1.8.5/dpp/ui/view/classic/codec_frame_header.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20298 2024-04-08 09:28:58.000000 decoder-plus-plus-1.8.5/dpp/ui/view/classic/codec_frames.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2401 2022-09-20 04:28:03.000000 decoder-plus-plus-1.8.5/dpp/ui/view/classic/codec_tab.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9167 2023-01-30 13:35:51.000000 decoder-plus-plus-1.8.5/dpp/ui/view/classic/combo_box_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10716 2022-09-21 05:00:04.000000 decoder-plus-plus-1.8.5/dpp/ui/view/main_window_widget.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.805846 decoder-plus-plus-1.8.5/dpp/ui/view/modern/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      705 2022-08-20 19:51:05.000000 decoder-plus-plus-1.8.5/dpp/ui/view/modern/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2460 2022-09-17 10:02:26.000000 decoder-plus-plus-1.8.5/dpp/ui/view/modern/modern_main_window_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      705 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/ui/view/modern/node_data.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5229 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/ui/view/modern/node_data_models.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      409 2022-08-30 00:07:08.000000 decoder-plus-plus-1.8.5/dpp/ui/view/modern/node_data_models_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2001 2022-09-17 10:02:44.000000 decoder-plus-plus-1.8.5/dpp/ui/view/modern/node_editor.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1782 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/ui/view/modern/node_editor_tab.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.821847 decoder-plus-plus-1.8.5/dpp/ui/widget/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      805 2022-08-16 19:35:20.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1367 2022-08-15 23:02:30.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/clickable_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3507 2024-04-06 16:14:35.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/code_editor_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3404 2024-04-07 09:41:34.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/codec_preview_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    11051 2024-04-06 07:30:01.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/collapsible_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2161 2022-09-10 22:00:08.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/combo_box.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4686 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/dock_tabs_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7690 2022-08-20 19:51:05.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/dock_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1887 2022-08-15 20:48:14.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/dyna_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      755 2022-08-15 20:44:52.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/elided_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2453 2024-04-06 20:17:41.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/hover_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1793 2024-04-06 07:22:30.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/icon_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3270 2024-04-07 11:20:24.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/identify_format_button.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3269 2022-09-12 19:34:03.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/list_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1151 2022-08-21 00:18:15.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/menu_bar.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2136 2024-04-06 09:24:31.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/message_box_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6687 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/message_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6110 2024-04-06 15:44:53.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/option_widgets.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    17880 2024-04-07 23:00:07.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/plain_view.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2621 2022-09-08 00:44:43.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/plugin_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9593 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/plugin_tab.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4396 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/search_field.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1246 2022-09-12 17:32:16.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/separater_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5000 2022-08-15 23:02:30.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/shortcut_table.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2846 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/slider_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4055 2022-09-20 10:34:13.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/smart_decode_button.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1442 2022-09-12 18:36:42.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/spacers.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2425 2023-01-30 12:23:56.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/status_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3757 2022-08-20 19:51:05.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/tab_bar.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8075 2022-09-15 01:50:24.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/tabs_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3210 2024-04-05 11:52:36.000000 decoder-plus-plus-1.8.5/dpp/ui/widget/text_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-04-09 13:35:13.845847 decoder-plus-plus-1.8.5/setup.cfg
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2681 2024-04-07 18:40:37.000000 decoder-plus-plus-1.8.5/setup.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.821847 decoder-plus-plus-1.8.5/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1805 2023-01-15 14:31:34.000000 decoder-plus-plus-1.8.5/tests/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.841847 decoder-plus-plus-1.8.5/tests/plugins/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2022-11-01 13:33:59.000000 decoder-plus-plus-1.8.5/tests/plugins/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1113 2022-11-01 14:08:45.000000 decoder-plus-plus-1.8.5/tests/plugins/adler32_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1191 2022-11-01 18:50:27.000000 decoder-plus-plus-1.8.5/tests/plugins/apache_md5_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1295 2022-11-01 18:05:54.000000 decoder-plus-plus-1.8.5/tests/plugins/base16_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1680 2023-01-15 13:01:54.000000 decoder-plus-plus-1.8.5/tests/plugins/base32_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1287 2023-01-15 13:32:25.000000 decoder-plus-plus-1.8.5/tests/plugins/base45_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1288 2023-01-15 12:36:51.000000 decoder-plus-plus-1.8.5/tests/plugins/base64_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2023-01-15 12:47:27.000000 decoder-plus-plus-1.8.5/tests/plugins/base64_url_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1229 2023-01-15 13:29:43.000000 decoder-plus-plus-1.8.5/tests/plugins/bin_int_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1040 2022-11-01 18:51:09.000000 decoder-plus-plus-1.8.5/tests/plugins/bin_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      992 2023-01-15 12:47:59.000000 decoder-plus-plus-1.8.5/tests/plugins/caesar_cipher_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1222 2022-11-01 18:35:38.000000 decoder-plus-plus-1.8.5/tests/plugins/clone_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2023-01-15 12:37:31.000000 decoder-plus-plus-1.8.5/tests/plugins/crc32_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1183 2022-11-01 18:39:55.000000 decoder-plus-plus-1.8.5/tests/plugins/css_minify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1401 2022-11-01 18:35:21.000000 decoder-plus-plus-1.8.5/tests/plugins/dec_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1245 2022-11-01 18:59:45.000000 decoder-plus-plus-1.8.5/tests/plugins/escape_string_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1123 2022-11-01 18:47:57.000000 decoder-plus-plus-1.8.5/tests/plugins/extract_urls_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1165 2022-11-01 18:40:22.000000 decoder-plus-plus-1.8.5/tests/plugins/filter_lines_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1189 2023-01-15 13:03:50.000000 decoder-plus-plus-1.8.5/tests/plugins/free_bsd_nt_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1253 2023-01-15 12:29:09.000000 decoder-plus-plus-1.8.5/tests/plugins/gzip_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1067 2022-11-01 18:47:18.000000 decoder-plus-plus-1.8.5/tests/plugins/hex_char_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1193 2023-01-15 13:10:42.000000 decoder-plus-plus-1.8.5/tests/plugins/hex_int_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1614 2022-11-01 18:43:06.000000 decoder-plus-plus-1.8.5/tests/plugins/hex_shell_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1313 2023-01-15 13:16:46.000000 decoder-plus-plus-1.8.5/tests/plugins/hex_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1173 2022-11-01 18:43:28.000000 decoder-plus-plus-1.8.5/tests/plugins/html_beautify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1168 2022-11-01 18:48:47.000000 decoder-plus-plus-1.8.5/tests/plugins/html_minify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1172 2023-01-15 12:22:31.000000 decoder-plus-plus-1.8.5/tests/plugins/html_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1219 2022-11-01 18:32:01.000000 decoder-plus-plus-1.8.5/tests/plugins/http64_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1016 2024-04-07 12:31:43.000000 decoder-plus-plus-1.8.5/tests/plugins/identify_file_type_filemagic_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1019 2024-04-07 12:32:46.000000 decoder-plus-plus-1.8.5/tests/plugins/identify_file_type_magika_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2022-11-01 18:39:55.000000 decoder-plus-plus-1.8.5/tests/plugins/identify_hash_format_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1145 2023-01-15 13:26:35.000000 decoder-plus-plus-1.8.5/tests/plugins/jq_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      988 2023-01-15 12:41:00.000000 decoder-plus-plus-1.8.5/tests/plugins/js_beautify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1164 2022-11-01 18:49:20.000000 decoder-plus-plus-1.8.5/tests/plugins/js_minify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      977 2023-01-15 13:06:33.000000 decoder-plus-plus-1.8.5/tests/plugins/js_to_xml_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      981 2023-01-15 13:02:34.000000 decoder-plus-plus-1.8.5/tests/plugins/jsonify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1163 2022-11-01 18:49:36.000000 decoder-plus-plus-1.8.5/tests/plugins/jsonpath_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      976 2023-01-15 12:39:55.000000 decoder-plus-plus-1.8.5/tests/plugins/jwt_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1163 2023-01-15 13:02:49.000000 decoder-plus-plus-1.8.5/tests/plugins/keccak224_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1171 2022-11-01 18:56:46.000000 decoder-plus-plus-1.8.5/tests/plugins/keccak256_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1203 2022-11-01 18:45:25.000000 decoder-plus-plus-1.8.5/tests/plugins/keccak384_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1235 2022-11-01 18:48:57.000000 decoder-plus-plus-1.8.5/tests/plugins/keccak512_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1245 2022-11-01 18:31:13.000000 decoder-plus-plus-1.8.5/tests/plugins/little_big_endian_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1124 2022-11-01 18:56:24.000000 decoder-plus-plus-1.8.5/tests/plugins/lm_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:24:14.000000 decoder-plus-plus-1.8.5/tests/plugins/md2_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:56:15.000000 decoder-plus-plus-1.8.5/tests/plugins/md4_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:45:18.000000 decoder-plus-plus-1.8.5/tests/plugins/md5_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1124 2022-11-01 18:46:24.000000 decoder-plus-plus-1.8.5/tests/plugins/nt_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1193 2023-01-15 13:13:49.000000 decoder-plus-plus-1.8.5/tests/plugins/oct_int_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1405 2022-11-01 18:20:57.000000 decoder-plus-plus-1.8.5/tests/plugins/oct_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1181 2023-01-15 12:51:06.000000 decoder-plus-plus-1.8.5/tests/plugins/phpass_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1167 2022-11-01 18:57:07.000000 decoder-plus-plus-1.8.5/tests/plugins/reformat_text_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1187 2023-01-15 13:04:21.000000 decoder-plus-plus-1.8.5/tests/plugins/remove_newlines_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1064 2022-11-01 18:56:04.000000 decoder-plus-plus-1.8.5/tests/plugins/remove_whitespaces_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1146 2022-11-01 18:56:36.000000 decoder-plus-plus-1.8.5/tests/plugins/ripemd160_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1225 2022-11-01 18:26:44.000000 decoder-plus-plus-1.8.5/tests/plugins/rot13_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1503 2023-01-15 13:05:35.000000 decoder-plus-plus-1.8.5/tests/plugins/search_and_replace_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2022-11-01 18:27:54.000000 decoder-plus-plus-1.8.5/tests/plugins/sha1_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1192 2022-11-01 18:29:14.000000 decoder-plus-plus-1.8.5/tests/plugins/sha224_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1200 2022-11-01 18:29:35.000000 decoder-plus-plus-1.8.5/tests/plugins/sha256_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1231 2022-11-01 18:29:59.000000 decoder-plus-plus-1.8.5/tests/plugins/sha384_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1160 2023-01-15 12:37:21.000000 decoder-plus-plus-1.8.5/tests/plugins/sha3_224_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1168 2022-11-01 18:53:45.000000 decoder-plus-plus-1.8.5/tests/plugins/sha3_256_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1200 2022-11-01 18:28:35.000000 decoder-plus-plus-1.8.5/tests/plugins/sha3_384_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1268 2022-11-01 18:28:57.000000 decoder-plus-plus-1.8.5/tests/plugins/sha3_512_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1263 2022-11-01 18:30:17.000000 decoder-plus-plus-1.8.5/tests/plugins/sha512_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1170 2022-11-01 18:57:46.000000 decoder-plus-plus-1.8.5/tests/plugins/split_and_rejoin_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      983 2023-01-15 12:39:55.000000 decoder-plus-plus-1.8.5/tests/plugins/sun_md5_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1247 2022-11-01 18:32:56.000000 decoder-plus-plus-1.8.5/tests/plugins/unescape_string_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1282 2022-11-01 18:45:08.000000 decoder-plus-plus-1.8.5/tests/plugins/url_plus_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2022-11-01 18:53:35.000000 decoder-plus-plus-1.8.5/tests/plugins/url_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2023-01-15 14:38:44.000000 decoder-plus-plus-1.8.5/tests/plugins/xpath_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1223 2023-01-15 13:12:30.000000 decoder-plus-plus-1.8.5/tests/plugins/zlib_test.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-09 13:35:13.845847 decoder-plus-plus-1.8.5/tests/ui/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-01-15 14:39:42.000000 decoder-plus-plus-1.8.5/tests/ui/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10557 2024-04-07 23:08:00.000000 decoder-plus-plus-1.8.5/tests/ui/classic_mode_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      512 2023-01-15 15:28:09.000000 decoder-plus-plus-1.8.5/tests/utils.py
```

### Comparing `decoder-plus-plus-1.8.0/LICENSE` & `decoder-plus-plus-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/PKG-INFO` & `decoder-plus-plus-1.8.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: decoder-plus-plus
-Version: 1.8.0
+Version: 1.8.5
 Summary: An extensible application for penetration testers and software developers to decode/encode data into various formats.
 Home-page: https://github.com/bytebutcher/decoder-plus-plus
 Author: bytebutcher
 Author-email: thomas.engel.web@gmail.com
 License: GPL-3.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: extras
 Provides-Extra: qt5
 Provides-Extra: qt6
-Provides-Extra: extras
 Provides-Extra: test
 License-File: LICENSE
 
 ![Decoder++ Logo](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp.png)
 
 <a href="https://pypi.python.org/pypi/decoder-plus-plus"><img src="https://img.shields.io/pypi/v/decoder-plus-plus.svg"></a>
 <a href="https://pypi.python.org/pypi/decoder-plus-plus"><img src="https://img.shields.io/pypi/dm/decoder-plus-plus"></a>
@@ -60,14 +61,20 @@
 While the ```main-window-mode``` supports tabbing, the ```dialog-mode``` has the ability to return the transformed 
 content to ```stdout``` ready for further processing. 
 As a result ```Decoder++``` can enhance other tools/scripts 
 by providing a graphical user interface for flexible transformation of any input.
 
 ![Decoder++ Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-preview-dialog.png)
 
+While ```Decoder++``` processes the entire input text by default, it allows for selective data transformation as well. 
+To transform only a specific portion of your text, simply highlight the necessary text segment in the input field 
+and then apply the desired codec.
+
+![Decoder++ Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-selective-input.png)
+
 ### Command Line
 
 In addition to the graphical user interface Decoder++ also provides a command line interface:
 ```bash
 $ dpp -e base64 -h sha1 "Hello, world!"
 e52d74c6d046c390345ae4343406b99587f2af0d
 ```
@@ -214,7 +221,9 @@
 ## Inspired By
 * PortSwigger's Burp Decoder
 
 ## Powered By
 
 * QtPy / PyQt5 / PyQt6
 * QtAwesome
+
+
```

#### html2text {}

```diff
@@ -1,57 +1,63 @@
-Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.8.0 Summary: An
+Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.8.5 Summary: An
 extensible application for penetration testers and software developers to
 decode/encode data into various formats. Home-page: https://github.com/
 bytebutcher/decoder-plus-plus Author: bytebutcher Author-email:
-thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming Language ::
-Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
-Type: text/markdown Provides-Extra: qt5 Provides-Extra: qt6 Provides-Extra:
-extras Provides-Extra: test License-File: LICENSE ![Decoder++ Logo](https://
-raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp.png)
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_p_y_p_i_/_d_m_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_e_c_o_d_e_r_-_p_l_u_s_-
-_p_l_u_s_._s_v_g_]# Decoder++ Decoder++ is an extensible application designed for
-penetration testers, software developers, and anyone in between looking to
-effortlessly decode and encode data across various formats. It includes a wide
-range of preinstalled scripts and codecs, smart decoding and format
-identification, and supports both graphical user interface (GUI) and command-
-line interface (CLI) operations. ## Quick Start Get up and running with
-Decoder++ in just a few steps: ```bash # Install using pip (latest:qt6) pip3
-install decoder-plus-plus[qt6] # Or, for a qt5 backport: pip3 install decoder-
-plus-plus[qt5] # To leverage all features and plugins: pip3 install decoder-
-plus-plus[extras] ``` For a detailed installation guide, including platform-
-specific instructions, see the [Installation Guide](docs/INSTALL.md). ##
-Overview This section provides an overview about the individual ways of
-interacting with ```Decoder++```. For additional usage information check out
-the ```Advanced Usage``` section. ### Graphical User Interface The graphical
-user interface provides two distinct interaction modes: a ```main-window-
-mode``` and a ```dialog-mode```. ![Decoder++ Screenshot](https://
-raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
-preview-001.png) While the ```main-window-mode``` supports tabbing, the
-```dialog-mode``` has the ability to return the transformed content to
-```stdout``` ready for further processing. As a result ```Decoder++``` can
-enhance other tools/scripts by providing a graphical user interface for
-flexible transformation of any input. ![Decoder++ Screenshot](https://
-raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
-preview-dialog.png) ### Command Line In addition to the graphical user
-interface Decoder++ also provides a command line interface: ```bash $ dpp -
-e base64 -h sha1 "Hello, world!" e52d74c6d046c390345ae4343406b99587f2af0d ```
-### Codecs and Scripts ```Decoder++``` allows you to choose from a variety of
-codecs and scripts: * **Encode/Decode:** - Base16, Base32, Base45, Base64,
-Base64 (URL-safe) - Binary, Gzip, Hex, Html, JWT, HTTP64 - Octal, Url, Url+,
-Zlib * **Hashing:** - Adler-32, Apache-Md5, CRC32, FreeBSD-NT - Keccak224,
-Keccak256, Keccak384, Keccak512 - LM, Md2, Md4, Md5, NT, PHPass - RipeMd160,
-Sha1, Sha3 224, Sha3 256, Sha3 384, Sha3 512 - Sha224, Sha256, Sha348, Sha512,
-Sun Md5 * **Scripts:** - Caesar, CSS-Minify, Custom Code, Extract URLs, Filter-
-Lines - Identify File Format, Identify Hash Format, JS-Beautifier, JS-to-XML,
-JQ - JSONify, JSONPath, HTML-Beautifier - Little/Big-Endian Transform, Reformat
-Text, Remove Newlines, Remove Whitespaces - Search and Replace, Split and
-Rejoin, Unescape/Escape String, XPath In cases where you require a bit more
-flexibility ```Decoder++``` allows you to process your data with custom scripts
-by using the ```Custom Code``` script: ![Decoder++ Screenshot](https://
+thomas.engel.web@gmail.com License: GPL-3.0 Platform: UNKNOWN Classifier:
+Programming Language :: Python :: 3 Classifier: Operating System :: OS
+Independent Description-Content-Type: text/markdown Provides-Extra: extras
+Provides-Extra: qt5 Provides-Extra: qt6 Provides-Extra: test License-File:
+LICENSE ![Decoder++ Logo](https://raw.githubusercontent.com/bytebutcher/
+decoder-plus-plus/master/images/dpp.png) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
+_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_]_[_h_t_t_p_s_:
+_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_._s_v_g_]# Decoder++ Decoder++ is
+an extensible application designed for penetration testers, software
+developers, and anyone in between looking to effortlessly decode and encode
+data across various formats. It includes a wide range of preinstalled scripts
+and codecs, smart decoding and format identification, and supports both
+graphical user interface (GUI) and command-line interface (CLI) operations. ##
+Quick Start Get up and running with Decoder++ in just a few steps: ```bash #
+Install using pip (latest:qt6) pip3 install decoder-plus-plus[qt6] # Or, for a
+qt5 backport: pip3 install decoder-plus-plus[qt5] # To leverage all features
+and plugins: pip3 install decoder-plus-plus[extras] ``` For a detailed
+installation guide, including platform-specific instructions, see the
+[Installation Guide](docs/INSTALL.md). ## Overview This section provides an
+overview about the individual ways of interacting with ```Decoder++```. For
+additional usage information check out the ```Advanced Usage``` section. ###
+Graphical User Interface The graphical user interface provides two distinct
+interaction modes: a ```main-window-mode``` and a ```dialog-mode```. !
+[Decoder++ Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-
+plus-plus/master/images/dpp-preview-001.png) While the ```main-window-mode```
+supports tabbing, the ```dialog-mode``` has the ability to return the
+transformed content to ```stdout``` ready for further processing. As a result
+```Decoder++``` can enhance other tools/scripts by providing a graphical user
+interface for flexible transformation of any input. ![Decoder++ Screenshot]
+(https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/
+dpp-preview-dialog.png) While ```Decoder++``` processes the entire input text
+by default, it allows for selective data transformation as well. To transform
+only a specific portion of your text, simply highlight the necessary text
+segment in the input field and then apply the desired codec. ![Decoder++
+Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/
+master/images/dpp-selective-input.png) ### Command Line In addition to the
+graphical user interface Decoder++ also provides a command line interface:
+```bash $ dpp -e base64 -h sha1 "Hello, world!"
+e52d74c6d046c390345ae4343406b99587f2af0d ``` ### Codecs and Scripts
+```Decoder++``` allows you to choose from a variety of codecs and scripts: *
+**Encode/Decode:** - Base16, Base32, Base45, Base64, Base64 (URL-safe) -
+Binary, Gzip, Hex, Html, JWT, HTTP64 - Octal, Url, Url+, Zlib * **Hashing:** -
+Adler-32, Apache-Md5, CRC32, FreeBSD-NT - Keccak224, Keccak256, Keccak384,
+Keccak512 - LM, Md2, Md4, Md5, NT, PHPass - RipeMd160, Sha1, Sha3 224, Sha3
+256, Sha3 384, Sha3 512 - Sha224, Sha256, Sha348, Sha512, Sun Md5 * **Scripts:
+** - Caesar, CSS-Minify, Custom Code, Extract URLs, Filter-Lines - Identify
+File Format, Identify Hash Format, JS-Beautifier, JS-to-XML, JQ - JSONify,
+JSONPath, HTML-Beautifier - Little/Big-Endian Transform, Reformat Text, Remove
+Newlines, Remove Whitespaces - Search and Replace, Split and Rejoin, Unescape/
+Escape String, XPath In cases where you require a bit more flexibility
+```Decoder++``` allows you to process your data with custom scripts by using
+the ```Custom Code``` script: ![Decoder++ Screenshot](https://
 raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
 custom-code-script.png) ## Advanced Usage This section provides additional
 information about how the command line interface can be used. ### Command Line
 Interface The commandline interface gives easy access to all available codecs.
 To list them the ```-l``` argument can be used. To narrow down the search the
 ```-l``` argument accepts additional parameters which work as filter: ```bash $
 dpp -l base enc Codec Type ----- ---- base16 encoder base32 encoder base64
```

### Comparing `decoder-plus-plus-1.8.0/README.md` & `decoder-plus-plus-1.8.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,20 @@
 While the ```main-window-mode``` supports tabbing, the ```dialog-mode``` has the ability to return the transformed 
 content to ```stdout``` ready for further processing. 
 As a result ```Decoder++``` can enhance other tools/scripts 
 by providing a graphical user interface for flexible transformation of any input.
 
 ![Decoder++ Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-preview-dialog.png)
 
+While ```Decoder++``` processes the entire input text by default, it allows for selective data transformation as well. 
+To transform only a specific portion of your text, simply highlight the necessary text segment in the input field 
+and then apply the desired codec.
+
+![Decoder++ Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-selective-input.png)
+
 ### Command Line
 
 In addition to the graphical user interface Decoder++ also provides a command line interface:
 ```bash
 $ dpp -e base64 -h sha1 "Hello, world!"
 e52d74c6d046c390345ae4343406b99587f2af0d
 ```
```

#### html2text {}

```diff
@@ -20,30 +20,36 @@
 [Decoder++ Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-
 plus-plus/master/images/dpp-preview-001.png) While the ```main-window-mode```
 supports tabbing, the ```dialog-mode``` has the ability to return the
 transformed content to ```stdout``` ready for further processing. As a result
 ```Decoder++``` can enhance other tools/scripts by providing a graphical user
 interface for flexible transformation of any input. ![Decoder++ Screenshot]
 (https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/
-dpp-preview-dialog.png) ### Command Line In addition to the graphical user
-interface Decoder++ also provides a command line interface: ```bash $ dpp -
-e base64 -h sha1 "Hello, world!" e52d74c6d046c390345ae4343406b99587f2af0d ```
-### Codecs and Scripts ```Decoder++``` allows you to choose from a variety of
-codecs and scripts: * **Encode/Decode:** - Base16, Base32, Base45, Base64,
-Base64 (URL-safe) - Binary, Gzip, Hex, Html, JWT, HTTP64 - Octal, Url, Url+,
-Zlib * **Hashing:** - Adler-32, Apache-Md5, CRC32, FreeBSD-NT - Keccak224,
-Keccak256, Keccak384, Keccak512 - LM, Md2, Md4, Md5, NT, PHPass - RipeMd160,
-Sha1, Sha3 224, Sha3 256, Sha3 384, Sha3 512 - Sha224, Sha256, Sha348, Sha512,
-Sun Md5 * **Scripts:** - Caesar, CSS-Minify, Custom Code, Extract URLs, Filter-
-Lines - Identify File Format, Identify Hash Format, JS-Beautifier, JS-to-XML,
-JQ - JSONify, JSONPath, HTML-Beautifier - Little/Big-Endian Transform, Reformat
-Text, Remove Newlines, Remove Whitespaces - Search and Replace, Split and
-Rejoin, Unescape/Escape String, XPath In cases where you require a bit more
-flexibility ```Decoder++``` allows you to process your data with custom scripts
-by using the ```Custom Code``` script: ![Decoder++ Screenshot](https://
+dpp-preview-dialog.png) While ```Decoder++``` processes the entire input text
+by default, it allows for selective data transformation as well. To transform
+only a specific portion of your text, simply highlight the necessary text
+segment in the input field and then apply the desired codec. ![Decoder++
+Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/
+master/images/dpp-selective-input.png) ### Command Line In addition to the
+graphical user interface Decoder++ also provides a command line interface:
+```bash $ dpp -e base64 -h sha1 "Hello, world!"
+e52d74c6d046c390345ae4343406b99587f2af0d ``` ### Codecs and Scripts
+```Decoder++``` allows you to choose from a variety of codecs and scripts: *
+**Encode/Decode:** - Base16, Base32, Base45, Base64, Base64 (URL-safe) -
+Binary, Gzip, Hex, Html, JWT, HTTP64 - Octal, Url, Url+, Zlib * **Hashing:** -
+Adler-32, Apache-Md5, CRC32, FreeBSD-NT - Keccak224, Keccak256, Keccak384,
+Keccak512 - LM, Md2, Md4, Md5, NT, PHPass - RipeMd160, Sha1, Sha3 224, Sha3
+256, Sha3 384, Sha3 512 - Sha224, Sha256, Sha348, Sha512, Sun Md5 * **Scripts:
+** - Caesar, CSS-Minify, Custom Code, Extract URLs, Filter-Lines - Identify
+File Format, Identify Hash Format, JS-Beautifier, JS-to-XML, JQ - JSONify,
+JSONPath, HTML-Beautifier - Little/Big-Endian Transform, Reformat Text, Remove
+Newlines, Remove Whitespaces - Search and Replace, Split and Rejoin, Unescape/
+Escape String, XPath In cases where you require a bit more flexibility
+```Decoder++``` allows you to process your data with custom scripts by using
+the ```Custom Code``` script: ![Decoder++ Screenshot](https://
 raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
 custom-code-script.png) ## Advanced Usage This section provides additional
 information about how the command line interface can be used. ### Command Line
 Interface The commandline interface gives easy access to all available codecs.
 To list them the ```-l``` argument can be used. To narrow down the search the
 ```-l``` argument accepts additional parameters which work as filter: ```bash $
 dpp -l base enc Codec Type ----- ---- base16 encoder base32 encoder base64
```

### Comparing `decoder-plus-plus-1.8.0/data/dpp.png` & `decoder-plus-plus-1.8.5/data/dpp.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/decoder_plus_plus.egg-info/PKG-INFO` & `decoder-plus-plus-1.8.5/decoder_plus_plus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: decoder-plus-plus
-Version: 1.8.0
+Version: 1.8.5
 Summary: An extensible application for penetration testers and software developers to decode/encode data into various formats.
 Home-page: https://github.com/bytebutcher/decoder-plus-plus
 Author: bytebutcher
 Author-email: thomas.engel.web@gmail.com
 License: GPL-3.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: extras
 Provides-Extra: qt5
 Provides-Extra: qt6
-Provides-Extra: extras
 Provides-Extra: test
 License-File: LICENSE
 
 ![Decoder++ Logo](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp.png)
 
 <a href="https://pypi.python.org/pypi/decoder-plus-plus"><img src="https://img.shields.io/pypi/v/decoder-plus-plus.svg"></a>
 <a href="https://pypi.python.org/pypi/decoder-plus-plus"><img src="https://img.shields.io/pypi/dm/decoder-plus-plus"></a>
@@ -60,14 +61,20 @@
 While the ```main-window-mode``` supports tabbing, the ```dialog-mode``` has the ability to return the transformed 
 content to ```stdout``` ready for further processing. 
 As a result ```Decoder++``` can enhance other tools/scripts 
 by providing a graphical user interface for flexible transformation of any input.
 
 ![Decoder++ Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-preview-dialog.png)
 
+While ```Decoder++``` processes the entire input text by default, it allows for selective data transformation as well. 
+To transform only a specific portion of your text, simply highlight the necessary text segment in the input field 
+and then apply the desired codec.
+
+![Decoder++ Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-selective-input.png)
+
 ### Command Line
 
 In addition to the graphical user interface Decoder++ also provides a command line interface:
 ```bash
 $ dpp -e base64 -h sha1 "Hello, world!"
 e52d74c6d046c390345ae4343406b99587f2af0d
 ```
@@ -214,7 +221,9 @@
 ## Inspired By
 * PortSwigger's Burp Decoder
 
 ## Powered By
 
 * QtPy / PyQt5 / PyQt6
 * QtAwesome
+
+
```

#### html2text {}

```diff
@@ -1,57 +1,63 @@
-Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.8.0 Summary: An
+Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.8.5 Summary: An
 extensible application for penetration testers and software developers to
 decode/encode data into various formats. Home-page: https://github.com/
 bytebutcher/decoder-plus-plus Author: bytebutcher Author-email:
-thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming Language ::
-Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
-Type: text/markdown Provides-Extra: qt5 Provides-Extra: qt6 Provides-Extra:
-extras Provides-Extra: test License-File: LICENSE ![Decoder++ Logo](https://
-raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp.png)
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_p_y_p_i_/_d_m_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_e_c_o_d_e_r_-_p_l_u_s_-
-_p_l_u_s_._s_v_g_]# Decoder++ Decoder++ is an extensible application designed for
-penetration testers, software developers, and anyone in between looking to
-effortlessly decode and encode data across various formats. It includes a wide
-range of preinstalled scripts and codecs, smart decoding and format
-identification, and supports both graphical user interface (GUI) and command-
-line interface (CLI) operations. ## Quick Start Get up and running with
-Decoder++ in just a few steps: ```bash # Install using pip (latest:qt6) pip3
-install decoder-plus-plus[qt6] # Or, for a qt5 backport: pip3 install decoder-
-plus-plus[qt5] # To leverage all features and plugins: pip3 install decoder-
-plus-plus[extras] ``` For a detailed installation guide, including platform-
-specific instructions, see the [Installation Guide](docs/INSTALL.md). ##
-Overview This section provides an overview about the individual ways of
-interacting with ```Decoder++```. For additional usage information check out
-the ```Advanced Usage``` section. ### Graphical User Interface The graphical
-user interface provides two distinct interaction modes: a ```main-window-
-mode``` and a ```dialog-mode```. ![Decoder++ Screenshot](https://
-raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
-preview-001.png) While the ```main-window-mode``` supports tabbing, the
-```dialog-mode``` has the ability to return the transformed content to
-```stdout``` ready for further processing. As a result ```Decoder++``` can
-enhance other tools/scripts by providing a graphical user interface for
-flexible transformation of any input. ![Decoder++ Screenshot](https://
-raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
-preview-dialog.png) ### Command Line In addition to the graphical user
-interface Decoder++ also provides a command line interface: ```bash $ dpp -
-e base64 -h sha1 "Hello, world!" e52d74c6d046c390345ae4343406b99587f2af0d ```
-### Codecs and Scripts ```Decoder++``` allows you to choose from a variety of
-codecs and scripts: * **Encode/Decode:** - Base16, Base32, Base45, Base64,
-Base64 (URL-safe) - Binary, Gzip, Hex, Html, JWT, HTTP64 - Octal, Url, Url+,
-Zlib * **Hashing:** - Adler-32, Apache-Md5, CRC32, FreeBSD-NT - Keccak224,
-Keccak256, Keccak384, Keccak512 - LM, Md2, Md4, Md5, NT, PHPass - RipeMd160,
-Sha1, Sha3 224, Sha3 256, Sha3 384, Sha3 512 - Sha224, Sha256, Sha348, Sha512,
-Sun Md5 * **Scripts:** - Caesar, CSS-Minify, Custom Code, Extract URLs, Filter-
-Lines - Identify File Format, Identify Hash Format, JS-Beautifier, JS-to-XML,
-JQ - JSONify, JSONPath, HTML-Beautifier - Little/Big-Endian Transform, Reformat
-Text, Remove Newlines, Remove Whitespaces - Search and Replace, Split and
-Rejoin, Unescape/Escape String, XPath In cases where you require a bit more
-flexibility ```Decoder++``` allows you to process your data with custom scripts
-by using the ```Custom Code``` script: ![Decoder++ Screenshot](https://
+thomas.engel.web@gmail.com License: GPL-3.0 Platform: UNKNOWN Classifier:
+Programming Language :: Python :: 3 Classifier: Operating System :: OS
+Independent Description-Content-Type: text/markdown Provides-Extra: extras
+Provides-Extra: qt5 Provides-Extra: qt6 Provides-Extra: test License-File:
+LICENSE ![Decoder++ Logo](https://raw.githubusercontent.com/bytebutcher/
+decoder-plus-plus/master/images/dpp.png) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
+_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_]_[_h_t_t_p_s_:
+_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_._s_v_g_]# Decoder++ Decoder++ is
+an extensible application designed for penetration testers, software
+developers, and anyone in between looking to effortlessly decode and encode
+data across various formats. It includes a wide range of preinstalled scripts
+and codecs, smart decoding and format identification, and supports both
+graphical user interface (GUI) and command-line interface (CLI) operations. ##
+Quick Start Get up and running with Decoder++ in just a few steps: ```bash #
+Install using pip (latest:qt6) pip3 install decoder-plus-plus[qt6] # Or, for a
+qt5 backport: pip3 install decoder-plus-plus[qt5] # To leverage all features
+and plugins: pip3 install decoder-plus-plus[extras] ``` For a detailed
+installation guide, including platform-specific instructions, see the
+[Installation Guide](docs/INSTALL.md). ## Overview This section provides an
+overview about the individual ways of interacting with ```Decoder++```. For
+additional usage information check out the ```Advanced Usage``` section. ###
+Graphical User Interface The graphical user interface provides two distinct
+interaction modes: a ```main-window-mode``` and a ```dialog-mode```. !
+[Decoder++ Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-
+plus-plus/master/images/dpp-preview-001.png) While the ```main-window-mode```
+supports tabbing, the ```dialog-mode``` has the ability to return the
+transformed content to ```stdout``` ready for further processing. As a result
+```Decoder++``` can enhance other tools/scripts by providing a graphical user
+interface for flexible transformation of any input. ![Decoder++ Screenshot]
+(https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/
+dpp-preview-dialog.png) While ```Decoder++``` processes the entire input text
+by default, it allows for selective data transformation as well. To transform
+only a specific portion of your text, simply highlight the necessary text
+segment in the input field and then apply the desired codec. ![Decoder++
+Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/
+master/images/dpp-selective-input.png) ### Command Line In addition to the
+graphical user interface Decoder++ also provides a command line interface:
+```bash $ dpp -e base64 -h sha1 "Hello, world!"
+e52d74c6d046c390345ae4343406b99587f2af0d ``` ### Codecs and Scripts
+```Decoder++``` allows you to choose from a variety of codecs and scripts: *
+**Encode/Decode:** - Base16, Base32, Base45, Base64, Base64 (URL-safe) -
+Binary, Gzip, Hex, Html, JWT, HTTP64 - Octal, Url, Url+, Zlib * **Hashing:** -
+Adler-32, Apache-Md5, CRC32, FreeBSD-NT - Keccak224, Keccak256, Keccak384,
+Keccak512 - LM, Md2, Md4, Md5, NT, PHPass - RipeMd160, Sha1, Sha3 224, Sha3
+256, Sha3 384, Sha3 512 - Sha224, Sha256, Sha348, Sha512, Sun Md5 * **Scripts:
+** - Caesar, CSS-Minify, Custom Code, Extract URLs, Filter-Lines - Identify
+File Format, Identify Hash Format, JS-Beautifier, JS-to-XML, JQ - JSONify,
+JSONPath, HTML-Beautifier - Little/Big-Endian Transform, Reformat Text, Remove
+Newlines, Remove Whitespaces - Search and Replace, Split and Rejoin, Unescape/
+Escape String, XPath In cases where you require a bit more flexibility
+```Decoder++``` allows you to process your data with custom scripts by using
+the ```Custom Code``` script: ![Decoder++ Screenshot](https://
 raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
 custom-code-script.png) ## Advanced Usage This section provides additional
 information about how the command line interface can be used. ### Command Line
 Interface The commandline interface gives easy access to all available codecs.
 To list them the ```-l``` argument can be used. To narrow down the search the
 ```-l``` argument accepts additional parameters which work as filter: ```bash $
 dpp -l base enc Codec Type ----- ---- base16 encoder base32 encoder base64
```

### Comparing `decoder-plus-plus-1.8.0/decoder_plus_plus.egg-info/SOURCES.txt` & `decoder-plus-plus-1.8.5/decoder_plus_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/__init__.py` & `decoder-plus-plus-1.8.5/dpp/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __name__ = 'decoder-plus-plus'
-__version__ = '1.8.0'
+__version__ = '1.8.5'
 __author__ = 'bytebutcher'
 
 import os
 app_path = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `decoder-plus-plus-1.8.0/dpp/core/__init__.py` & `decoder-plus-plus-1.8.5/dpp/core/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/argparse.py` & `decoder-plus-plus-1.8.5/dpp/core/argparse.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/assertions.py` & `decoder-plus-plus-1.8.5/dpp/core/assertions.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/config.py` & `decoder-plus-plus-1.8.5/dpp/core/config.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/context.py` & `decoder-plus-plus-1.8.5/dpp/core/context.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/decoder_plus_plus.py` & `decoder-plus-plus-1.8.5/dpp/core/decoder_plus_plus.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/exceptions.py` & `decoder-plus-plus-1.8.5/dpp/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/icons.py` & `decoder-plus-plus-1.8.5/dpp/core/icons.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/listener.py` & `decoder-plus-plus-1.8.5/dpp/core/listener.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-from typing import Callable
+from typing import Callable, Dict, List
 
 
 class Signal:
     """ A custom implementation of the Qt Signal without the class required to inherit from QObject.
 
     Usage:
 
     class FooBar:
 
-        onChange = Singal('str')
+        onChange = Signal('str')
 
         def __init__(self):
             self._foo = 'bar'
 
         @property
         def foo(self):
             return self._foo
@@ -42,23 +42,41 @@
     bar = FooBar()
     bar.onChange.connect(lambda foo: print(foo))
 
     """
 
     def __init__(self, *args):
         self._args = args
-        self._callbacks = []
+        self._callbacks: Dict[int, List[Callable]] = {}
 
-    def connect(self, callback: Callable):
-        self._callbacks.append(callback)
+    def __get__(self, instance, owner):
+        if instance is None:
+            return self
+        return self.SignalInstanceProxy(self, instance)
+
+    class SignalInstanceProxy:
+        def __init__(self, signal, instance):
+            self._signal = signal
+            self._instance = instance
+
+        def connect(self, callback: Callable):
+            """Connect a callback to the signal for this instance."""
+            instance_id = id(self._instance)
+            if instance_id not in self._signal._callbacks:
+                self._signal._callbacks[instance_id] = []
+            self._signal._callbacks[instance_id].append(callback)
+
+        def emit(self, *args):
+            """Emit the signal for this instance, calling all connected callbacks."""
+            instance_id = id(self._instance)
+            if instance_id in self._signal._callbacks:
+                callbacks = self._signal._callbacks[instance_id]
+                for callback in callbacks:
+                    callback(*args)
 
-    def emit(self, *args):
-        assert len(args) == len(self._args), f'Invalid number of arguments! Expected {len(self._args)}, got {len(args)}!'
-        for callback in self._callbacks:
-            callback(*args)
 
 
 class Listener:
     """ A set of global signals to emit or connect to. """
 
     # Signals that a new tab should be created with the specified input text
     newTabRequested = Signal(str, str)  # title, input_text
```

### Comparing `decoder-plus-plus-1.8.0/dpp/core/logger.py` & `decoder-plus-plus-1.8.5/dpp/core/logger.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/math.py` & `decoder-plus-plus-1.8.5/dpp/core/math.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/plugin/__init__.py` & `decoder-plus-plus-1.8.5/dpp/core/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/plugin/builder.py` & `decoder-plus-plus-1.8.5/dpp/core/plugin/builder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/plugin/config/__init__.py` & `decoder-plus-plus-1.8.5/dpp/core/plugin/config/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/plugin/config/options/__init__.py` & `decoder-plus-plus-1.8.5/dpp/core/plugin/config/options/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/plugin/config/ui/__init__.py` & `decoder-plus-plus-1.8.5/dpp/core/plugin/config/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/plugin/config/ui/layouts.py` & `decoder-plus-plus-1.8.5/dpp/core/plugin/config/ui/layouts.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/plugin/config/ui/widgets.py` & `decoder-plus-plus-1.8.5/dpp/core/plugin/config/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/plugin/loader.py` & `decoder-plus-plus-1.8.5/dpp/core/plugin/loader.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/plugin/manager.py` & `decoder-plus-plus-1.8.5/dpp/core/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/core/shortcuts.py` & `decoder-plus-plus-1.8.5/dpp/core/shortcuts.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/images/dpp.png` & `decoder-plus-plus-1.8.5/dpp/images/dpp.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/images/dpp_128.png` & `decoder-plus-plus-1.8.5/dpp/images/dpp_128.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/images/dpp_classic.png` & `decoder-plus-plus-1.8.5/dpp/images/dpp_classic.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/images/dpp_classic_128.png` & `decoder-plus-plus-1.8.5/dpp/images/dpp_classic_128.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/images/dpp_modern.png` & `decoder-plus-plus-1.8.5/dpp/images/dpp_modern.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/images/dpp_modern_128.png` & `decoder-plus-plus-1.8.5/dpp/images/dpp_modern_128.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/images/dpp_modern_big.png` & `decoder-plus-plus-1.8.5/dpp/images/dpp_modern_big.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/images/dpp_stylized.png` & `decoder-plus-plus-1.8.5/dpp/images/dpp_stylized.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/images/dpp_stylized_128.png` & `decoder-plus-plus-1.8.5/dpp/images/dpp_stylized_128.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/images/dpp_xmas.png` & `decoder-plus-plus-1.8.5/dpp/images/dpp_xmas.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/images/dpp_xmas_stylized.png` & `decoder-plus-plus-1.8.5/dpp/images/dpp_xmas_stylized.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/images/keyboard.png` & `decoder-plus-plus-1.8.5/dpp/images/keyboard.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/images/keyboard.svg` & `decoder-plus-plus-1.8.5/dpp/images/keyboard.svg`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/adler32_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/adler32_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/apache_md5_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/apache_md5_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/base16_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/base16_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/base16_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/base16_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/base32_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/base32_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/base32_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/base32_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/base45_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/base45_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/base45_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/base45_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/base64_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/base64_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/base64_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/base64_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/base64_url_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/base64_url_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/base64_url_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/base64_url_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/bin_int_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/bin_int_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/bin_int_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/bin_int_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/bin_str_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/bin_str_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/bin_str_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/bin_str_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/caesar_cipher_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/caesar_cipher_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/clone_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/clone_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/crc32_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/crc32_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/css_minify_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/css_minify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/custom_code.py` & `decoder-plus-plus-1.8.5/dpp/plugins/custom_code.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/dec_str_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/dec_str_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/dec_str_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/dec_str_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/escape_string_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/escape_string_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/extract_urls_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/extract_urls_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/filter_lines_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/filter_lines_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/free_bsd_nt_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/free_bsd_nt_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/gzip_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/gzip_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/gzip_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/gzip_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/hex_char_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/hex_char_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/hex_char_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/hex_char_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/hex_int_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/hex_int_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/hex_int_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/hex_int_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/hex_shell_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/hex_shell_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/hex_shell_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/hex_shell_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/hex_str_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/hex_str_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/hex_str_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/hex_str_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/html_beautify_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/html_beautify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/html_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/html_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/html_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/html_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/html_minify_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/html_minify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/http64_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/http64_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/http64_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/http64_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/identify_decoder_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/identify_decoder_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/identify_file_type_filemagic_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/identify_file_type_filemagic_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/identify_file_type_magika_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/identify_file_type_magika_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/identify_hash_format_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/identify_hash_format_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/jq_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/jq_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/js_beautify_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/js_beautify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/js_minify_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/js_minify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/js_to_xml_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/js_to_xml_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/jsonify_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/jsonify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/jsonpath_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/jsonpath_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/jwt_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/jwt_decoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from dpp.core.plugin import DecoderPlugin
 from dpp.core.plugin.config import Label
-from dpp.core.plugin.config.options import String
+from dpp.core.plugin.config.options import String, ComboBox
 
 
 class Plugin(DecoderPlugin):
     """
     Decodes JSON Web Tokens.
 
     Example:
@@ -46,17 +46,20 @@
         super().__init__('JWT', "Thomas Engel", ["jwt"], context)
         self.config.add(String(
             label=Plugin.Option.Key,
             value="",
             description="the key suitable for the allowed algorithm",
             is_required=False
         ))
-        self.config.add(String(
+        self.config.add(ComboBox(
             label=Plugin.Option.Algorithm,
-            value="",
+            value="HS256",
+            values=[
+                "HS256"
+            ],
             description="allowed algorithm",
             is_required=False
         ))
 
     def run(self, input_text: str) -> str:
         import jwt
         parameters = {}
```

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/jwt_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/jwt_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/keccak224_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/keccak224_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/keccak256_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/keccak256_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/keccak384_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/keccak384_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/keccak512_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/keccak512_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/little_big_endian_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/little_big_endian_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/lm_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/lm_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/md2_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/md2_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/md4_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/md4_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/md5_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/md5_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/nt_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/nt_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/oct_int_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/oct_int_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/oct_int_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/oct_int_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/oct_str_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/oct_str_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/oct_str_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/oct_str_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/phpass_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/phpass_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/reformat_text_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/reformat_text_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/remove_newlines_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/remove_newlines_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/remove_whitespaces_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/remove_whitespaces_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/ripemd160_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/ripemd160_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/rot13_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/rot13_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/rot13_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/rot13_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/search_and_replace_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/search_and_replace_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/sha1_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/sha1_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/sha224_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/sha224_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/sha256_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/sha256_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/sha384_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/sha384_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/sha3_224_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/sha3_224_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/sha3_256_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/sha3_256_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/sha3_384_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/sha3_384_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/sha3_512_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/sha3_512_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/sha512_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/sha512_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/split_and_rejoin_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/split_and_rejoin_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/sun_md5_hasher.py` & `decoder-plus-plus-1.8.5/dpp/plugins/sun_md5_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/unescape_string_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/unescape_string_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/url_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/url_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/url_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/url_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/url_plus_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/url_plus_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/url_plus_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/url_plus_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/xpath_script.py` & `decoder-plus-plus-1.8.5/dpp/plugins/xpath_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/zlib_decoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/zlib_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/plugins/zlib_encoder.py` & `decoder-plus-plus-1.8.5/dpp/plugins/zlib_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/runner.py` & `decoder-plus-plus-1.8.5/dpp/runner.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/__init__.py` & `decoder-plus-plus-1.8.5/dpp/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/builder/action_builder.py` & `decoder-plus-plus-1.8.5/dpp/ui/builder/action_builder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/builder/plugin_config_widget_builder.py` & `decoder-plus-plus-1.8.5/dpp/ui/builder/plugin_config_widget_builder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/builder/widget_builder.py` & `decoder-plus-plus-1.8.5/dpp/ui/builder/widget_builder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/decoder_plus_plus_gui.py` & `decoder-plus-plus-1.8.5/dpp/ui/decoder_plus_plus_gui.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/dialog/__init__.py` & `decoder-plus-plus-1.8.5/dpp/ui/dialog/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/dialog/config_dialog.py` & `decoder-plus-plus-1.8.5/dpp/ui/dialog/config_dialog.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/dialog/keyboard_shortcut_dialog.py` & `decoder-plus-plus-1.8.5/dpp/ui/dialog/keyboard_shortcut_dialog.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/dialog/plugin_config_dialog.py` & `decoder-plus-plus-1.8.5/dpp/ui/dialog/plugin_config_dialog.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/dock/hex_dock.py` & `decoder-plus-plus-1.8.5/dpp/ui/dock/hex_dock.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/dock/log_dock.py` & `decoder-plus-plus-1.8.5/dpp/ui/dock/log_dock.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/instance_handler.py` & `decoder-plus-plus-1.8.5/dpp/ui/instance_handler.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/view/__init__.py` & `decoder-plus-plus-1.8.5/dpp/ui/view/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/view/classic/__init__.py` & `decoder-plus-plus-1.8.5/dpp/ui/view/classic/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/view/classic/classic_main_window_widget.py` & `decoder-plus-plus-1.8.5/dpp/ui/view/classic/classic_main_window_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/view/classic/codec_frame.py` & `decoder-plus-plus-1.8.5/dpp/ui/view/classic/codec_frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -208,17 +208,43 @@
     def setStatus(self, type, message):
         self._header_frame.setStatus(type, message)
         self._status_widget.setStatus(type, message)
 
     # ------------------------------------------------------------------------------------------------------------------
 
     def hasTextSelected(self) -> bool:
+        """ Returns whether there is a current text selection. """
         return self._plain_view_widget.hasTextSelected()
 
+    def selectText(self, start: int, end: int):
+        """
+        Selects text within the QPlainTextEdit widget, given the start and end positions.
+
+        Args:
+            start (int): The position to start the selection.
+            end (int): The position to end the selection.
+
+        Raises:
+            ValueError: If 'start' or 'end' positions are out of the text range.
+        """
+        self._plain_view_widget.selectText(start, end)
+
     def getSelectedText(self) -> Tuple[str, str, str]:
+        """
+        Retrieves the text selected by the user in the QPlainTextEdit widget.
+        If no text is selected, it raises an Exception.
+
+        Returns:
+            Tuple[str, str, str]: A tuple containing three strings:
+                                   - The text before the selection,
+                                   - The selected text,
+                                   - The text after the selection.
+        Raises:
+            Exception: If no text is selected.
+        """
         return self._plain_view_widget.getSelectedText()
 
     # ------------------------------------------------------------------------------------------------------------------
 
     @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def selectComboBoxEntryByPlugin(self, plugin, block_signals=False):
         self._combo_box_frame.selectItem(plugin.type, plugin.name, block_signals=block_signals)
@@ -232,15 +258,21 @@
         self._plain_view_widget.setPlainText(text)
         self.header().refresh()
 
     def getInputText(self) -> str:
         return self._plain_view_widget.toPlainText()
 
     def getOutputText(self) -> str:
-        return self.getPlugin().run(self.getInputText())
+        if self.hasTextSelected():
+            start_text, input_text, end_text = self.getSelectedText()
+            output = start_text + self.getPlugin().run(input_text) + end_text
+        else:
+            input_text = self.getInputText()
+            output = self.getPlugin().run(input_text)
+        return output
 
     def getComboBoxes(self):
         return self._combo_box_frame
 
     @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def cutSelectedInputText(self):
         self._plain_view_widget.cutSelectedInputText()
```

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/view/classic/codec_frame_header.py` & `decoder-plus-plus-1.8.5/dpp/ui/view/classic/codec_frame_header.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/view/classic/codec_frames.py` & `decoder-plus-plus-1.8.5/dpp/ui/view/classic/codec_frames.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,20 +59,15 @@
         @param frame: the frame to run.
         @return: the new CodecFrame or None if plugin configuration failed.
         """
         output = ""
         error = None
         plugin = frame.getPlugin()
         try:
-            if frame.hasTextSelected():
-                start_text, input_text, end_text = frame.getSelectedText()
-                output = start_text + plugin.run(input_text) + end_text
-            else:
-                input_text = frame.getInputText()
-                output = plugin.run(input_text)
+            output = frame.getOutputText()
             status = StatusWidget.SUCCESS
         except BaseException as err:
             status = StatusWidget.ERROR
             error = str(err)
             self._context.logger.error(f'{plugin.name} {plugin.type}: {error}')
             self._context.logger.debug(str(err), exc_info=True)
         return output, status, error
```

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/view/classic/codec_tab.py` & `decoder-plus-plus-1.8.5/dpp/ui/view/classic/codec_tab.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/view/classic/combo_box_frame.py` & `decoder-plus-plus-1.8.5/dpp/ui/view/classic/combo_box_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/view/main_window_widget.py` & `decoder-plus-plus-1.8.5/dpp/ui/view/main_window_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/view/modern/__init__.py` & `decoder-plus-plus-1.8.5/dpp/ui/view/modern/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/view/modern/modern_main_window_widget.py` & `decoder-plus-plus-1.8.5/dpp/ui/view/modern/modern_main_window_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/view/modern/node_data.py` & `decoder-plus-plus-1.8.5/dpp/ui/view/modern/node_data.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/view/modern/node_data_models.py` & `decoder-plus-plus-1.8.5/dpp/ui/view/modern/node_data_models.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/view/modern/node_editor.py` & `decoder-plus-plus-1.8.5/dpp/ui/view/modern/node_editor.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/view/modern/node_editor_tab.py` & `decoder-plus-plus-1.8.5/dpp/ui/view/modern/node_editor_tab.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/__init__.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/clickable_label.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/clickable_label.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/code_editor_widget.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/code_editor_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/codec_preview_widget.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/codec_preview_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/collapsible_frame.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/collapsible_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/combo_box.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/combo_box.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/dock_tabs_widget.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/dock_tabs_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/dock_widget.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/dock_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/dyna_frame.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/dyna_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/elided_label.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/elided_label.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/hover_label.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/hover_label.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/icon_label.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/icon_label.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/identify_format_button.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/identify_format_button.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/list_widget.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/list_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/menu_bar.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/menu_bar.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/message_box_widget.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/message_box_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/message_widget.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/message_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/option_widgets.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/option_widgets.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/plain_view.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/plain_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -344,15 +344,15 @@
         for stor_sel_start, stor_sel_end, stor_sel_color in tmp_selections:
             available_colors.remove(stor_sel_color)
 
         tmp_selections.append((cur_sel_start, cur_sel_end, self.color_codes[0]))
         self._apply_selections_highlighting(tmp_selections)
 
     def hasTextSelected(self) -> bool:
-        """ Returns whether there are current and stored text selections. """
+        """ Returns whether there is a current text selection. """
         cursor = self._plain_text.textCursor()
         selected_text = cursor.selectedText()
         return selected_text or self._selections
 
     def getSelectedText(self) -> Tuple[str, str, str]:
         """
         Retrieves the text selected by the user in the QPlainTextEdit widget.
@@ -373,14 +373,34 @@
 
         start = text[:cursor.selectionStart()]
         selection = text[cursor.selectionStart():cursor.selectionEnd()]
         end = text[cursor.selectionEnd():]
 
         return start, selection, end
 
+    def selectText(self, start: int, end: int):
+        """
+        Selects text within the QPlainTextEdit widget, given the start and end positions.
+
+        Args:
+            start (int): The position to start the selection.
+            end (int): The position to end the selection.
+
+        Raises:
+            ValueError: If 'start' or 'end' positions are out of the text range.
+        """
+        text_length = len(self._plain_text.toPlainText())
+        if start < 0 or end > text_length or start > end:
+            raise ValueError('Invalid start or end position for text selection.')
+
+        cursor = self._plain_text.textCursor()
+        cursor.setPosition(start)
+        cursor.setPosition(end, QTextCursor.KeepAnchor)
+        self._plain_text.setTextCursor(cursor)
+
     # ------------------------------------------------------------------------------------------------------------------
 
     def toggleSearchField(self):
         """ Toggles the search field. """
         if self._search_field.hasFocus() and self._search_field.isVisible():
             self._do_close_search_field()
         else:
```

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/plugin_frame.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/plugin_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/plugin_tab.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/plugin_tab.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/search_field.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/search_field.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/separater_widget.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/separater_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/shortcut_table.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/shortcut_table.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/slider_widget.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/slider_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/smart_decode_button.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/smart_decode_button.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/spacers.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/spacers.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/status_widget.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/status_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/tab_bar.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/tab_bar.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/tabs_widget.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/tabs_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/dpp/ui/widget/text_widget.py` & `decoder-plus-plus-1.8.5/dpp/ui/widget/text_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/setup.py` & `decoder-plus-plus-1.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/__init__.py` & `decoder-plus-plus-1.8.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/adler32_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/adler32_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/apache_md5_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/apache_md5_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/base16_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/base16_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/base32_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/base32_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/base45_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/base45_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/base64_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/base64_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/base64_url_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/base64_url_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/bin_int_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/bin_int_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/bin_str_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/bin_str_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/caesar_cipher_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/caesar_cipher_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/clone_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/clone_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/crc32_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/crc32_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/css_minify_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/css_minify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/dec_str_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/dec_str_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/escape_string_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/escape_string_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/extract_urls_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/extract_urls_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/filter_lines_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/filter_lines_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/free_bsd_nt_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/free_bsd_nt_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/gzip_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/gzip_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/hex_char_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/hex_char_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/hex_int_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/hex_int_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/hex_shell_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/hex_shell_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/hex_str_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/hex_str_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/html_beautify_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/html_beautify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/html_minify_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/html_minify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/html_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/html_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/http64_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/http64_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/identify_file_type_filemagic_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/identify_file_type_filemagic_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/identify_file_type_magika_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/identify_file_type_magika_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/identify_hash_format_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/identify_hash_format_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/jq_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/jq_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/js_beautify_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/js_beautify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/js_minify_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/js_minify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/js_to_xml_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/js_to_xml_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/jsonify_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/jsonify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/jsonpath_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/jsonpath_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/jwt_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/jwt_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/keccak224_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/keccak224_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/keccak256_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/keccak256_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/keccak384_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/keccak384_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/keccak512_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/keccak512_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/little_big_endian_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/little_big_endian_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/lm_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/lm_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/md2_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/md2_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/md4_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/md4_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/md5_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/md5_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/nt_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/nt_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/oct_int_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/oct_int_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/oct_str_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/oct_str_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/phpass_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/phpass_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/reformat_text_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/reformat_text_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/remove_newlines_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/remove_newlines_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/remove_whitespaces_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/remove_whitespaces_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/ripemd160_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/ripemd160_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/rot13_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/rot13_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/search_and_replace_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/search_and_replace_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/sha1_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/sha1_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/sha224_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/sha224_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/sha256_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/sha256_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/sha384_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/sha384_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/sha3_224_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/sha3_224_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/sha3_256_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/sha3_256_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/sha3_384_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/sha3_384_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/sha3_512_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/sha3_512_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/sha512_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/sha512_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/split_and_rejoin_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/split_and_rejoin_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/sun_md5_hasher_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/sun_md5_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/unescape_string_script_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/unescape_string_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/url_plus_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/url_plus_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/url_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/url_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/xpath_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/xpath_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/plugins/zlib_test.py` & `decoder-plus-plus-1.8.5/tests/plugins/zlib_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.8.0/tests/ui/classic_mode_test.py` & `decoder-plus-plus-1.8.5/tests/ui/classic_mode_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,23 @@
         plugin = load_plugin("Base45", PluginType.ENCODER)
         codec_frames.frame(0).setPlugin(plugin, block_signals=False)
         self.assertEqual(codec_frames.count(), 3)
         self.assertFrame(codec_frames.frame(0), "Hello, world!", "%69 VDK2EV4404ESVDX0", ("DEFAULT", None), False)
         self.assertFrame(codec_frames.frame(1), "%69 VDK2EV4404ESVDX0", "VV4:97Y+AZM9KY8:Q6A46HY8Y+AV6B", ("SUCCESS", None), True)
         self.assertFrame(codec_frames.frame(2), "VV4:97Y+AZM9KY8:Q6A46HY8Y+AV6B", "", ("SUCCESS", None), False)
 
+    def testTransformSelectedText(self):
+        # Selective Text Transformation #66
+        idx, codec_tab = self.dpp.newTab("Hello, world!")
+        codec_frames = codec_tab.frames()
+        codec_frames.frame(0).selectText(0, 5)
+        plugin = load_plugin("Base64", PluginType.ENCODER)
+        codec_frames.frame(0).setPlugin(plugin, block_signals=False)
+        self.assertFrame(codec_frames.frame(0), "Hello, world!", "SGVsbG8=, world!", ("DEFAULT", None), False)
+
     def testMoveCodecUp(self):
         """
         # Example:
         #
         #   1. "Hello, world" - Base64 - open
         #   2. "<base64> of hello world" - Sha256 - collapsed
         #   3. "<sha256> of base64 hello world" - <> - open
```

### Comparing `decoder-plus-plus-1.8.0/tests/utils.py` & `decoder-plus-plus-1.8.5/tests/utils.py`

 * *Files identical despite different names*

