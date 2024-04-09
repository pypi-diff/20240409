# Comparing `tmp/pyams_content_themes-1.99.0.tar.gz` & `tmp/pyams_content_themes-1.99.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_content_themes-1.99.0.tar", last modified: Tue Feb 27 10:57:27 2024, max compression
+gzip compressed data, was "dist/pyams_content_themes-1.99.1.tar", last modified: Tue Apr  9 21:12:00 2024, max compression
```

## Comparing `pyams_content_themes-1.99.0.tar` & `pyams_content_themes-1.99.1.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1685 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/docs/
--rwxrwxrwx   0 root         (0) root         (0)       64 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/docs/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/pkg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/pkg/assets/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/clock.png
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/email.png
--rw-rw-rw-   0 root         (0) root         (0)   187448 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/fa-brands-400.ttf
--rw-rw-rw-   0 root         (0) root         (0)   108000 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/fa-brands-400.woff2
--rw-rw-rw-   0 root         (0) root         (0)    63728 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/fa-regular-400.ttf
--rw-rw-rw-   0 root         (0) root         (0)    24840 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/fa-regular-400.woff2
--rw-rw-rw-   0 root         (0) root         (0)   394832 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/fa-solid-900.ttf
--rw-rw-rw-   0 root         (0) root         (0)   149908 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/fa-solid-900.woff2
--rw-rw-rw-   0 root         (0) root         (0)    10172 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/fa-v4compatibility.ttf
--rw-rw-rw-   0 root         (0) root         (0)     4536 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/fa-v4compatibility.woff2
--rw-rw-rw-   0 root         (0) root         (0)     7604 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/form.png
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/layers-2x.png
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/layers.png
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/list-item.png
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/map.png
--rw-rw-rw-   0 root         (0) root         (0)     1466 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/marker-icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/mobile-menu.png
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/phone.png
--rw-rw-rw-   0 root         (0) root         (0)     1849 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/select2-spinner.gif
--rw-rw-rw-   0 root         (0) root         (0)      613 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/select2.png
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/select2x2.png
--rw-rw-rw-   0 root         (0) root         (0)     7058 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/assets/social-icons.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/pkg/css/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/pkg/css/dev/
--rw-rw-rw-   0 root         (0) root         (0)   226317 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/dev/pyams-almond.css
--rw-rw-rw-   0 root         (0) root         (0)   226709 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/dev/pyams-darkgreen.css
--rw-rw-rw-   0 root         (0) root         (0)   226652 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/dev/pyams.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/pkg/css/dist/
--rw-rw-rw-   0 root         (0) root         (0)   204389 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/dist/pyams-almond.css
--rw-rw-rw-   0 root         (0) root         (0)   204439 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/dist/pyams-darkgreen.css
--rw-rw-rw-   0 root         (0) root         (0)   204319 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/dist/pyams.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/pkg/css/img/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/img/clock.png
--rw-rw-rw-   0 root         (0) root         (0)      880 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/img/download.svg
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/img/email.png
--rw-rw-rw-   0 root         (0) root         (0)     7604 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/img/form.png
--rw-rw-rw-   0 root         (0) root         (0)      339 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/img/link.svg
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/img/list-item.png
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/img/map.png
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/img/mobile-menu.png
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/img/phone.png
--rw-rw-rw-   0 root         (0) root         (0)      416 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/img/print.svg
--rw-rw-rw-   0 root         (0) root         (0)     4315 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/img/search.png
--rw-rw-rw-   0 root         (0) root         (0)     7058 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/css/img/social-icons.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/pkg/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/pkg/js/dev/
--rw-rw-rw-   0 root         (0) root         (0)     4615 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js
--rw-rw-rw-   0 root         (0) root         (0)     4633 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)    10687 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
--rw-rw-rw-   0 root         (0) root         (0)     6529 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)  2517657 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/pyams-almond.js
--rw-rw-rw-   0 root         (0) root         (0)  3071892 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/pyams-almond.js.map
--rw-rw-rw-   0 root         (0) root         (0)  2518611 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/pyams-darkgreen.js
--rw-rw-rw-   0 root         (0) root         (0)  3072711 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/pyams-darkgreen.js.map
--rw-rw-rw-   0 root         (0) root         (0)  2518257 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/pyams.js
--rw-rw-rw-   0 root         (0) root         (0)  3072453 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/pyams.js.map
--rw-rw-rw-   0 root         (0) root         (0)     8804 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/src_pyams_content_themes_resources_src_js__form_js.js
--rw-rw-rw-   0 root         (0) root         (0)    14704 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/src_pyams_content_themes_resources_src_js__form_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)    52125 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_jquery-validation_dist_jquery_validate_js.js
--rw-rw-rw-   0 root         (0) root         (0)    67260 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_jquery-validation_dist_jquery_validate_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)    18925 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js
--rw-rw-rw-   0 root         (0) root         (0)    20134 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   447964 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js
--rw-rw-rw-   0 root         (0) root         (0)   566807 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)    47821 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js
--rw-rw-rw-   0 root         (0) root         (0)    54546 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)   147853 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_select2_select2_js.js
--rw-rw-rw-   0 root         (0) root         (0)   174731 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_select2_select2_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   114226 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js
--rw-rw-rw-   0 root         (0) root         (0)   139878 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/pkg/js/dist/
--rw-rw-rw-   0 root         (0) root         (0)   148092 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/243.js
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/243.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     3187 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/284.js
--rw-rw-rw-   0 root         (0) root         (0)     3595 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/374.js
--rw-rw-rw-   0 root         (0) root         (0)    60371 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/553.js
--rw-rw-rw-   0 root         (0) root         (0)    24434 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/587.js
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/587.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    17191 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/623.js
--rw-rw-rw-   0 root         (0) root         (0)    61505 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/698.js
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/698.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    18227 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/830.js
--rw-rw-rw-   0 root         (0) root         (0)     1873 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/854.js
--rw-rw-rw-   0 root         (0) root         (0)   964741 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/pyams-almond.js
--rw-rw-rw-   0 root         (0) root         (0)     2028 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/pyams-almond.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)   965135 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/pyams-darkgreen.js
--rw-rw-rw-   0 root         (0) root         (0)     2028 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/pyams-darkgreen.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)   965069 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/pyams.js
--rw-rw-rw-   0 root         (0) root         (0)     2028 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/pkg/js/dist/pyams.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2763 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/
--rw-rw-rw-   0 root         (0) root         (0)     1885 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2645 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/include.py
--rw-rw-rw-   0 root         (0) root         (0)      789 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      522 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/locales/fr/LC_MESSAGES/pyams_content_themes.mo
--rw-rw-rw-   0 root         (0) root         (0)      820 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/locales/fr/LC_MESSAGES/pyams_content_themes.po
--rw-rw-rw-   0 root         (0) root         (0)      768 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/locales/pyams_content_themes.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/
--rw-rw-rw-   0 root         (0) root         (0)     5845 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/_form.js
--rw-rw-rw-   0 root         (0) root         (0)     5725 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/_gis.js
--rw-rw-rw-   0 root         (0) root         (0)     1460 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/_search.js
--rw-rw-rw-   0 root         (0) root         (0)     6202 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/_utils.js
--rw-rw-rw-   0 root         (0) root         (0)     4218 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/app.js
--rw-rw-rw-   0 root         (0) root         (0)      776 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/pyams-almond.js
--rw-rw-rw-   0 root         (0) root         (0)      779 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/pyams-darkgreen.js
--rw-rw-rw-   0 root         (0) root         (0)      769 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/pyams.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/
--rw-rw-rw-   0 root         (0) root         (0)      302 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_breadcrumbs.scss
--rw-rw-rw-   0 root         (0) root         (0)      320 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_carousel.scss
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_content.scss
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_footer.scss
--rw-rw-rw-   0 root         (0) root         (0)      490 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)     3046 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_layout.scss
--rw-rw-rw-   0 root         (0) root         (0)      275 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_list.scss
--rw-rw-rw-   0 root         (0) root         (0)     3959 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_misc.scss
--rw-rw-rw-   0 root         (0) root         (0)      960 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_mobile.scss
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_search.scss
--rw-rw-rw-   0 root         (0) root         (0)     1918 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_variables-almond.scss
--rw-rw-rw-   0 root         (0) root         (0)     2285 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_variables-darkgreen.scss
--rw-rw-rw-   0 root         (0) root         (0)     4281 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_variables.scss
--rw-rw-rw-   0 root         (0) root         (0)      840 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/pyams-almond.scss
--rw-rw-rw-   0 root         (0) root         (0)      843 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/pyams-darkgreen.scss
--rw-rw-rw-   0 root         (0) root         (0)      789 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/pyams.scss
--rw-rw-rw-   0 root         (0) root         (0)     2355 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/skin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/templates/
--rw-rw-rw-   0 root         (0) root         (0)      878 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/templates/checkbox-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     4177 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/templates/form-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     2109 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/templates/layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     1291 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/templates/object-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/templates/submit-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1195 2024-02-27 10:57:01.000000 pyams_content_themes-1.99.0/src/pyams_content_themes/templates/widget-layout.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1685 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5537 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 10:57:22.000000 pyams_content_themes-1.99.0/src/pyams_content_themes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      149 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-27 10:57:27.000000 pyams_content_themes-1.99.0/src/pyams_content_themes.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/docs/
+-rwxrwxrwx   0 root         (0) root         (0)      123 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/docs/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/pkg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/pkg/assets/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/clock.png
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/email.png
+-rw-rw-rw-   0 root         (0) root         (0)   187448 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/fa-brands-400.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   108000 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/fa-brands-400.woff2
+-rw-rw-rw-   0 root         (0) root         (0)    63728 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/fa-regular-400.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    24840 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/fa-regular-400.woff2
+-rw-rw-rw-   0 root         (0) root         (0)   394832 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/fa-solid-900.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   149908 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/fa-solid-900.woff2
+-rw-rw-rw-   0 root         (0) root         (0)    10172 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/fa-v4compatibility.ttf
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/fa-v4compatibility.woff2
+-rw-rw-rw-   0 root         (0) root         (0)     7604 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/form.png
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/layers-2x.png
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/layers.png
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/list-item.png
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/map.png
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/marker-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/mobile-menu.png
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/phone.png
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/select2-spinner.gif
+-rw-rw-rw-   0 root         (0) root         (0)      613 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/select2.png
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/select2x2.png
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/assets/social-icons.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/pkg/css/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/pkg/css/dev/
+-rw-rw-rw-   0 root         (0) root         (0)   226317 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/dev/pyams-almond.css
+-rw-rw-rw-   0 root         (0) root         (0)   226709 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/dev/pyams-darkgreen.css
+-rw-rw-rw-   0 root         (0) root         (0)   226652 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/dev/pyams.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/pkg/css/dist/
+-rw-rw-rw-   0 root         (0) root         (0)   204389 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/dist/pyams-almond.css
+-rw-rw-rw-   0 root         (0) root         (0)   204439 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/dist/pyams-darkgreen.css
+-rw-rw-rw-   0 root         (0) root         (0)   204319 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/dist/pyams.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/pkg/css/img/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/img/clock.png
+-rw-rw-rw-   0 root         (0) root         (0)      880 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/img/download.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/img/email.png
+-rw-rw-rw-   0 root         (0) root         (0)     7604 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/img/form.png
+-rw-rw-rw-   0 root         (0) root         (0)      339 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/img/link.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/img/list-item.png
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/img/map.png
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/img/mobile-menu.png
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/img/phone.png
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/img/print.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4315 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/img/search.png
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/css/img/social-icons.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/pkg/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/pkg/js/dev/
+-rw-rw-rw-   0 root         (0) root         (0)     4615 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js
+-rw-rw-rw-   0 root         (0) root         (0)     4633 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    10687 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
+-rw-rw-rw-   0 root         (0) root         (0)     6529 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)  2517657 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/pyams-almond.js
+-rw-rw-rw-   0 root         (0) root         (0)  3071892 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/pyams-almond.js.map
+-rw-rw-rw-   0 root         (0) root         (0)  2518611 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/pyams-darkgreen.js
+-rw-rw-rw-   0 root         (0) root         (0)  3072711 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/pyams-darkgreen.js.map
+-rw-rw-rw-   0 root         (0) root         (0)  2518257 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/pyams.js
+-rw-rw-rw-   0 root         (0) root         (0)  3072453 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/pyams.js.map
+-rw-rw-rw-   0 root         (0) root         (0)     8804 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/src_pyams_content_themes_resources_src_js__form_js.js
+-rw-rw-rw-   0 root         (0) root         (0)    14704 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/src_pyams_content_themes_resources_src_js__form_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    52125 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_jquery-validation_dist_jquery_validate_js.js
+-rw-rw-rw-   0 root         (0) root         (0)    67260 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_jquery-validation_dist_jquery_validate_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    18925 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js
+-rw-rw-rw-   0 root         (0) root         (0)    20134 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   447964 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   566807 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    47821 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js
+-rw-rw-rw-   0 root         (0) root         (0)    54546 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   147853 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_select2_select2_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   174731 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_select2_select2_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   114226 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   139878 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/pkg/js/dist/
+-rw-rw-rw-   0 root         (0) root         (0)   148092 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/243.js
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/243.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3187 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/284.js
+-rw-rw-rw-   0 root         (0) root         (0)     3595 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/374.js
+-rw-rw-rw-   0 root         (0) root         (0)    60371 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/553.js
+-rw-rw-rw-   0 root         (0) root         (0)    24434 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/587.js
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/587.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    17191 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/623.js
+-rw-rw-rw-   0 root         (0) root         (0)    61505 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/698.js
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/698.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    18227 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/830.js
+-rw-rw-rw-   0 root         (0) root         (0)     1873 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/854.js
+-rw-rw-rw-   0 root         (0) root         (0)   964741 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/pyams-almond.js
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/pyams-almond.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)   965135 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/pyams-darkgreen.js
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/pyams-darkgreen.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)   965069 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/pyams.js
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/pkg/js/dist/pyams.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2763 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/include.py
+-rw-rw-rw-   0 root         (0) root         (0)      789 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      522 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/locales/fr/LC_MESSAGES/pyams_content_themes.mo
+-rw-rw-rw-   0 root         (0) root         (0)      820 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/locales/fr/LC_MESSAGES/pyams_content_themes.po
+-rw-rw-rw-   0 root         (0) root         (0)      768 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/locales/pyams_content_themes.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/
+-rw-rw-rw-   0 root         (0) root         (0)     5845 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/_form.js
+-rw-rw-rw-   0 root         (0) root         (0)     5725 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/_gis.js
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/_search.js
+-rw-rw-rw-   0 root         (0) root         (0)     6202 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/_utils.js
+-rw-rw-rw-   0 root         (0) root         (0)     4218 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/app.js
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/pyams-almond.js
+-rw-rw-rw-   0 root         (0) root         (0)      779 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/pyams-darkgreen.js
+-rw-rw-rw-   0 root         (0) root         (0)      769 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/pyams.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_breadcrumbs.scss
+-rw-rw-rw-   0 root         (0) root         (0)      320 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_carousel.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_content.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_footer.scss
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_layout.scss
+-rw-rw-rw-   0 root         (0) root         (0)      275 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_list.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3959 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_misc.scss
+-rw-rw-rw-   0 root         (0) root         (0)      960 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_mobile.scss
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_search.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_variables-almond.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_variables-darkgreen.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4281 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_variables.scss
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/pyams-almond.scss
+-rw-rw-rw-   0 root         (0) root         (0)      843 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/pyams-darkgreen.scss
+-rw-rw-rw-   0 root         (0) root         (0)      789 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/pyams.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/skin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      878 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/templates/checkbox-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4187 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/templates/form-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/templates/layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/templates/object-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/templates/submit-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2024-04-09 21:11:36.000000 pyams_content_themes-1.99.1/src/pyams_content_themes/templates/widget-layout.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5537 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 21:11:55.000000 pyams_content_themes-1.99.1/src/pyams_content_themes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      149 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 21:12:00.000000 pyams_content_themes-1.99.1/src/pyams_content_themes.egg-info/top_level.txt
```

### Comparing `pyams_content_themes-1.99.0/LICENSE` & `pyams_content_themes-1.99.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/PKG-INFO` & `pyams_content_themes-1.99.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_content_themes
-Version: 1.99.0
+Version: 1.99.1
 Summary: PyAMS sample themes
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -46,10 +46,14 @@
 There are actually three packages ("PyAMS Bootstrap", "PyAMS Almond" and "PyAMS Dark Green"),
 which can be selected from PyAMS content management interface.
 
 
 Changelog
 =========
 
+1.99.1
+------
+ - added flex wrapper class to form buttons
+
 1.99.0
 ------
  - first preliminary release
```

### Comparing `pyams_content_themes-1.99.0/docs/README.rst` & `pyams_content_themes-1.99.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/clock.png` & `pyams_content_themes-1.99.1/pkg/assets/clock.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/email.png` & `pyams_content_themes-1.99.1/pkg/assets/email.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/fa-brands-400.ttf` & `pyams_content_themes-1.99.1/pkg/assets/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/fa-brands-400.woff2` & `pyams_content_themes-1.99.1/pkg/assets/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/fa-regular-400.ttf` & `pyams_content_themes-1.99.1/pkg/assets/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/fa-regular-400.woff2` & `pyams_content_themes-1.99.1/pkg/assets/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/fa-solid-900.ttf` & `pyams_content_themes-1.99.1/pkg/assets/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/fa-solid-900.woff2` & `pyams_content_themes-1.99.1/pkg/assets/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/fa-v4compatibility.ttf` & `pyams_content_themes-1.99.1/pkg/assets/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/fa-v4compatibility.woff2` & `pyams_content_themes-1.99.1/pkg/assets/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/form.png` & `pyams_content_themes-1.99.1/pkg/assets/form.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/layers-2x.png` & `pyams_content_themes-1.99.1/pkg/assets/layers-2x.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/layers.png` & `pyams_content_themes-1.99.1/pkg/assets/layers.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/list-item.png` & `pyams_content_themes-1.99.1/pkg/assets/list-item.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/map.png` & `pyams_content_themes-1.99.1/pkg/assets/map.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/marker-icon.png` & `pyams_content_themes-1.99.1/pkg/assets/marker-icon.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/mobile-menu.png` & `pyams_content_themes-1.99.1/pkg/assets/mobile-menu.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/phone.png` & `pyams_content_themes-1.99.1/pkg/assets/phone.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/select2-spinner.gif` & `pyams_content_themes-1.99.1/pkg/assets/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/select2.png` & `pyams_content_themes-1.99.1/pkg/assets/select2.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/select2x2.png` & `pyams_content_themes-1.99.1/pkg/assets/select2x2.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/assets/social-icons.png` & `pyams_content_themes-1.99.1/pkg/assets/social-icons.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/dev/pyams-almond.css` & `pyams_content_themes-1.99.1/pkg/css/dev/pyams-almond.css`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/dev/pyams-darkgreen.css` & `pyams_content_themes-1.99.1/pkg/css/dev/pyams-darkgreen.css`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/dev/pyams.css` & `pyams_content_themes-1.99.1/pkg/css/dev/pyams.css`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/dist/pyams-almond.css` & `pyams_content_themes-1.99.1/pkg/css/dist/pyams-almond.css`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/dist/pyams-darkgreen.css` & `pyams_content_themes-1.99.1/pkg/css/dist/pyams-darkgreen.css`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/dist/pyams.css` & `pyams_content_themes-1.99.1/pkg/css/dist/pyams.css`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/img/clock.png` & `pyams_content_themes-1.99.1/pkg/css/img/clock.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/img/download.svg` & `pyams_content_themes-1.99.1/pkg/css/img/download.svg`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/img/email.png` & `pyams_content_themes-1.99.1/pkg/css/img/email.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/img/form.png` & `pyams_content_themes-1.99.1/pkg/css/img/form.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/img/list-item.png` & `pyams_content_themes-1.99.1/pkg/css/img/list-item.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/img/map.png` & `pyams_content_themes-1.99.1/pkg/css/img/map.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/img/mobile-menu.png` & `pyams_content_themes-1.99.1/pkg/css/img/mobile-menu.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/img/phone.png` & `pyams_content_themes-1.99.1/pkg/css/img/phone.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/img/search.png` & `pyams_content_themes-1.99.1/pkg/css/img/search.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/css/img/social-icons.png` & `pyams_content_themes-1.99.1/pkg/css/img/social-icons.png`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js` & `pyams_content_themes-1.99.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map` & `pyams_content_themes-1.99.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js` & `pyams_content_themes-1.99.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map` & `pyams_content_themes-1.99.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/pyams-almond.js` & `pyams_content_themes-1.99.1/pkg/js/dev/pyams-almond.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/pyams-almond.js.map` & `pyams_content_themes-1.99.1/pkg/js/dev/pyams-almond.js.map`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/pyams-darkgreen.js` & `pyams_content_themes-1.99.1/pkg/js/dev/pyams-darkgreen.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/pyams-darkgreen.js.map` & `pyams_content_themes-1.99.1/pkg/js/dev/pyams-darkgreen.js.map`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/pyams.js` & `pyams_content_themes-1.99.1/pkg/js/dev/pyams.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/pyams.js.map` & `pyams_content_themes-1.99.1/pkg/js/dev/pyams.js.map`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/src_pyams_content_themes_resources_src_js__form_js.js` & `pyams_content_themes-1.99.1/pkg/js/dev/src_pyams_content_themes_resources_src_js__form_js.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/src_pyams_content_themes_resources_src_js__form_js.js.map` & `pyams_content_themes-1.99.1/pkg/js/dev/src_pyams_content_themes_resources_src_js__form_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_jquery-validation_dist_jquery_validate_js.js` & `pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_jquery-validation_dist_jquery_validate_js.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_jquery-validation_dist_jquery_validate_js.js.map` & `pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_jquery-validation_dist_jquery_validate_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js` & `pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map` & `pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js` & `pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map` & `pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js` & `pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map` & `pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_select2_select2_js.js` & `pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_select2_select2_js.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_select2_select2_js.js.map` & `pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_select2_select2_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js` & `pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map` & `pyams_content_themes-1.99.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dist/243.js` & `pyams_content_themes-1.99.1/pkg/js/dist/243.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dist/284.js` & `pyams_content_themes-1.99.1/pkg/js/dist/284.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dist/374.js` & `pyams_content_themes-1.99.1/pkg/js/dist/374.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dist/553.js` & `pyams_content_themes-1.99.1/pkg/js/dist/553.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dist/587.js` & `pyams_content_themes-1.99.1/pkg/js/dist/587.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dist/623.js` & `pyams_content_themes-1.99.1/pkg/js/dist/623.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dist/698.js` & `pyams_content_themes-1.99.1/pkg/js/dist/698.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dist/830.js` & `pyams_content_themes-1.99.1/pkg/js/dist/830.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dist/854.js` & `pyams_content_themes-1.99.1/pkg/js/dist/854.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dist/pyams-almond.js` & `pyams_content_themes-1.99.1/pkg/js/dist/pyams-almond.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dist/pyams-almond.js.LICENSE.txt` & `pyams_content_themes-1.99.1/pkg/js/dist/pyams-almond.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dist/pyams-darkgreen.js` & `pyams_content_themes-1.99.1/pkg/js/dist/pyams-darkgreen.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dist/pyams-darkgreen.js.LICENSE.txt` & `pyams_content_themes-1.99.1/pkg/js/dist/pyams-darkgreen.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dist/pyams.js` & `pyams_content_themes-1.99.1/pkg/js/dist/pyams.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/pkg/js/dist/pyams.js.LICENSE.txt` & `pyams_content_themes-1.99.1/pkg/js/dist/pyams.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/setup.py` & `pyams_content_themes-1.99.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.99.0'
+version = '1.99.1'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 data_dir = 'pkg'
 data_files = [(d, [os.path.join(d, f) for f in files])
               for d, folders, files in os.walk(data_dir)]
 
 tests_require = [
```

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/__init__.py` & `pyams_content_themes-1.99.1/src/pyams_content_themes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/include.py` & `pyams_content_themes-1.99.1/src/pyams_content_themes/include.py`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/interfaces.py` & `pyams_content_themes-1.99.1/src/pyams_content_themes/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/locales/fr/LC_MESSAGES/pyams_content_themes.mo` & `pyams_content_themes-1.99.1/src/pyams_content_themes/locales/fr/LC_MESSAGES/pyams_content_themes.mo`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/locales/fr/LC_MESSAGES/pyams_content_themes.po` & `pyams_content_themes-1.99.1/src/pyams_content_themes/locales/fr/LC_MESSAGES/pyams_content_themes.po`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/locales/pyams_content_themes.pot` & `pyams_content_themes-1.99.1/src/pyams_content_themes/locales/pyams_content_themes.pot`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/_form.js` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/_form.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/_gis.js` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/_gis.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/_search.js` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/_search.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/_utils.js` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/_utils.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/app.js` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/app.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/pyams-almond.js` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/pyams-almond.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/pyams-darkgreen.js` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/pyams-darkgreen.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/js/pyams.js` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/js/pyams.js`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_content.scss` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_content.scss`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_footer.scss` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_footer.scss`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_layout.scss` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_layout.scss`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_misc.scss` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_misc.scss`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_mobile.scss` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_mobile.scss`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_variables-almond.scss` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_variables-almond.scss`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_variables-darkgreen.scss` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_variables-darkgreen.scss`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/_variables.scss` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/_variables.scss`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/pyams-almond.scss` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/pyams-almond.scss`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/pyams-darkgreen.scss` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/pyams-darkgreen.scss`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/resources/src/sass/pyams.scss` & `pyams_content_themes-1.99.1/src/pyams_content_themes/resources/src/sass/pyams.scss`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/skin.py` & `pyams_content_themes-1.99.1/src/pyams_content_themes/skin.py`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/templates/checkbox-layout.pt` & `pyams_content_themes-1.99.1/src/pyams_content_themes/templates/checkbox-layout.pt`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/templates/form-layout.pt` & `pyams_content_themes-1.99.1/src/pyams_content_themes/templates/form-layout.pt`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                 <div tal:repeat="tabform view.tabforms"
                      id="tab_${tales:cache_key(tabform)}"
                      class="tab-pane fade show ${'active' if repeat['tabform'].start() else ''}">
                     <i tal:omit-tag="">${structure:tabform.render()}</i>
                 </div>
             </div>
         </div>
-        <footer class="d-flex justify-content-center m-3"
+        <footer class="d-flex flex-wrap justify-content-center m-3"
                 tal:condition="view.actions and (view.mode == 'input')">
             <tal:loop repeat="action view.actions.values()">
                 ${structure:action.render()}
             </tal:loop>
         </footer>
         <i tal:omit-tag="">${structure:provider:pyams.form_footer}</i>
     </form>
```

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/templates/layout.pt` & `pyams_content_themes-1.99.1/src/pyams_content_themes/templates/layout.pt`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/templates/object-input.pt` & `pyams_content_themes-1.99.1/src/pyams_content_themes/templates/object-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/templates/submit-input.pt` & `pyams_content_themes-1.99.1/src/pyams_content_themes/templates/submit-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes/templates/widget-layout.pt` & `pyams_content_themes-1.99.1/src/pyams_content_themes/templates/widget-layout.pt`

 * *Files identical despite different names*

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes.egg-info/PKG-INFO` & `pyams_content_themes-1.99.1/src/pyams_content_themes.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-content-themes
-Version: 1.99.0
+Version: 1.99.1
 Summary: PyAMS sample themes
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -46,10 +46,14 @@
 There are actually three packages ("PyAMS Bootstrap", "PyAMS Almond" and "PyAMS Dark Green"),
 which can be selected from PyAMS content management interface.
 
 
 Changelog
 =========
 
+1.99.1
+------
+ - added flex wrapper class to form buttons
+
 1.99.0
 ------
  - first preliminary release
```

### Comparing `pyams_content_themes-1.99.0/src/pyams_content_themes.egg-info/SOURCES.txt` & `pyams_content_themes-1.99.1/src/pyams_content_themes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

