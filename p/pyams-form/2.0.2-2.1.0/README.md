# Comparing `tmp/pyams_form-2.0.2.tar.gz` & `tmp/pyams_form-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_form-2.0.2.tar", last modified: Mon Dec 11 13:34:34 2023, max compression
+gzip compressed data, was "dist/pyams_form-2.1.0.tar", last modified: Tue Apr  9 19:56:28 2024, max compression
```

## Comparing `pyams_form-2.0.2.tar` & `pyams_form-2.1.0.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-12-11 13:33:54.000000 pyams_form-2.0.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-12-11 13:33:54.000000 pyams_form-2.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4781 2023-12-11 13:34:34.000000 pyams_form-2.0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/docs/
--rwxrwxrwx   0 root         (0) root         (0)     3019 2023-12-11 13:33:54.000000 pyams_form-2.0.2/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1215 2023-12-11 13:33:54.000000 pyams_form-2.0.2/docs/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-12-11 13:33:54.000000 pyams_form-2.0.2/docs/form-graph.dot
--rw-rw-rw-   0 root         (0) root         (0)    11877 2023-12-11 13:33:54.000000 pyams_form-2.0.2/docs/form-graph.png
--rw-rw-rw-   0 root         (0) root         (0)     1510 2023-12-11 13:33:54.000000 pyams_form-2.0.2/docs/widget-graph.dot
--rw-rw-rw-   0 root         (0) root         (0)    13789 2023-12-11 13:33:54.000000 pyams_form-2.0.2/docs/widget-graph.png
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-11 13:34:34.000000 pyams_form-2.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2877 2023-12-11 13:33:54.000000 pyams_form-2.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form/
--rw-rw-rw-   0 root         (0) root         (0)      854 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/action.py
--rw-rw-rw-   0 root         (0) root         (0)    16892 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/ajax.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form/browser/
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1656 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/button.py
--rw-rw-rw-   0 root         (0) root         (0)     3500 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/checkbox.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/file.py
--rw-rw-rw-   0 root         (0) root         (0)     2256 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/image.py
--rw-rw-rw-   0 root         (0) root         (0)    13085 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3801 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/multi.py
--rw-rw-rw-   0 root         (0) root         (0)     1421 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/object.py
--rw-rw-rw-   0 root         (0) root         (0)     3729 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/orderedselect.py
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/password.py
--rw-rw-rw-   0 root         (0) root         (0)     3745 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/radio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form/browser/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form/browser/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)     3364 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/resources/js/orderedselect-input.js
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/resources/js/orderedselect-input.min.js
--rw-rw-rw-   0 root         (0) root         (0)     5163 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/select.py
--rw-rw-rw-   0 root         (0) root         (0)     1518 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/submit.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/text.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/textarea.py
--rw-rw-rw-   0 root         (0) root         (0)     1641 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/textlines.py
--rw-rw-rw-   0 root         (0) root         (0)     8027 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/browser/widget.py
--rw-rw-rw-   0 root         (0) root         (0)    11593 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/button.py
--rw-rw-rw-   0 root         (0) root         (0)     5383 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/contentprovider.py
--rw-rw-rw-   0 root         (0) root         (0)    16755 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/converter.py
--rw-rw-rw-   0 root         (0) root         (0)     5480 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/datamanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form/doctests/
--rw-rw-rw-   0 root         (0) root         (0)     3471 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     9810 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/action.rst
--rw-rw-rw-   0 root         (0) root         (0)    19164 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/ajax.rst
--rw-rw-rw-   0 root         (0) root         (0)   113044 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/browser.rst
--rw-rw-rw-   0 root         (0) root         (0)    19674 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/button.rst
--rw-rw-rw-   0 root         (0) root         (0)    10584 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/contentprovider.rst
--rw-rw-rw-   0 root         (0) root         (0)    32750 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/converter.rst
--rw-rw-rw-   0 root         (0) root         (0)    10500 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/datamanager.rst
--rw-rw-rw-   0 root         (0) root         (0)     8281 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/error.rst
--rw-rw-rw-   0 root         (0) root         (0)    30830 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/field.rst
--rw-rw-rw-   0 root         (0) root         (0)    65455 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/form.rst
--rw-rw-rw-   0 root         (0) root         (0)    33058 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/group.rst
--rw-rw-rw-   0 root         (0) root         (0)    26338 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/hint.rst
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/index-browser.rst
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2589 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/object-caveat.rst
--rw-rw-rw-   0 root         (0) root         (0)     5942 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/security.rst
--rw-rw-rw-   0 root         (0) root         (0)    38934 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/subform.rst
--rw-rw-rw-   0 root         (0) root         (0)    20978 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/term.rst
--rw-rw-rw-   0 root         (0) root         (0)     1466 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/testing.rst
--rw-rw-rw-   0 root         (0) root         (0)    15386 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/util.rst
--rw-rw-rw-   0 root         (0) root         (0)    20915 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/validator.rst
--rw-rw-rw-   0 root         (0) root         (0)     8357 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/value.rst
--rw-rw-rw-   0 root         (0) root         (0)     2257 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-button.rst
--rw-rw-rw-   0 root         (0) root         (0)    12744 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-checkbox.rst
--rw-rw-rw-   0 root         (0) root         (0)     4496 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-file-testing.rst
--rw-rw-rw-   0 root         (0) root         (0)     3221 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-file.rst
--rw-rw-rw-   0 root         (0) root         (0)     2669 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-image.rst
--rw-rw-rw-   0 root         (0) root         (0)    21423 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-multi-dict-integration.rst
--rw-rw-rw-   0 root         (0) root         (0)    14042 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-multi-list-integration.rst
--rw-rw-rw-   0 root         (0) root         (0)    52089 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-multi.rst
--rw-rw-rw-   0 root         (0) root         (0)    20939 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-object-multi-dict-integration.rst
--rw-rw-rw-   0 root         (0) root         (0)    17704 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-object-multi-list-integration.rst
--rw-rw-rw-   0 root         (0) root         (0)     7548 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-object-single-integration.rst
--rw-rw-rw-   0 root         (0) root         (0)    39953 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-object.rst
--rw-rw-rw-   0 root         (0) root         (0)    63193 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-objectmulti.rst
--rw-rw-rw-   0 root         (0) root         (0)     8679 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-orderedselect.rst
--rw-rw-rw-   0 root         (0) root         (0)     2669 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-password.rst
--rw-rw-rw-   0 root         (0) root         (0)     9424 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-radio.rst
--rw-rw-rw-   0 root         (0) root         (0)     8172 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-select-missing-terms.rst
--rw-rw-rw-   0 root         (0) root         (0)     2997 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-select-source.rst
--rw-rw-rw-   0 root         (0) root         (0)    12593 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-select.rst
--rw-rw-rw-   0 root         (0) root         (0)     2482 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-submit.rst
--rw-rw-rw-   0 root         (0) root         (0)     2345 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-text.rst
--rw-rw-rw-   0 root         (0) root         (0)     2299 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-textarea.rst
--rw-rw-rw-   0 root         (0) root         (0)     2787 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget-textlines.rst
--rw-rw-rw-   0 root         (0) root         (0)    31086 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/doctests/widget.rst
--rw-rw-rw-   0 root         (0) root         (0)     4433 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/error.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/events.py
--rw-rw-rw-   0 root         (0) root         (0)    13295 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/field.py
--rw-rw-rw-   0 root         (0) root         (0)    20194 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/form.py
--rw-rw-rw-   0 root         (0) root         (0)     4473 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/group.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/hint.py
--rw-rw-rw-   0 root         (0) root         (0)     1028 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/include.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     9914 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4651 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/button.py
--rw-rw-rw-   0 root         (0) root         (0)     1620 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/error.py
--rw-rw-rw-   0 root         (0) root         (0)    13723 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/form.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/button-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      868 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/button-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      680 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/checkbox-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1183 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/checkbox-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)     2725 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/checkbox-input.pt
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/error.pt
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/file-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      931 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/file-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/image-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/image-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1701 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/multi-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/multi-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)     1849 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/multi-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      371 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/object-display.pt
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/object-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/object-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      678 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/orderedselect-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     3266 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/orderedselect-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/password-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      975 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/password-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/radio-display-single.pt
--rw-rw-rw-   0 root         (0) root         (0)      680 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/radio-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/radio-hidden-single.pt
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/radio-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/radio-input-single.pt
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/radio-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      680 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/select-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/select-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/select-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/submit-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      868 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/submit-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/text-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/text-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)     1008 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/text-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/textarea-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/textarea-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/textarea-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/textlines-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/textlines-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/textlines-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/widget-layout-display.pt
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/widget-layout-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/templates/widget-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)    19108 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/interfaces/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    14287 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.mo
--rw-rw-rw-   0 root         (0) root         (0)    20915 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.po
--rw-rw-rw-   0 root         (0) root         (0)    15253 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/locales/pyams_form.pot
--rw-rw-rw-   0 root         (0) root         (0)    14307 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/object.py
--rw-rw-rw-   0 root         (0) root         (0)     4226 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/outputchecker.py
--rw-rw-rw-   0 root         (0) root         (0)     2969 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/subform.py
--rw-rw-rw-   0 root         (0) root         (0)     6833 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/template.py
--rw-rw-rw-   0 root         (0) root         (0)    11899 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/term.py
--rw-rw-rw-   0 root         (0) root         (0)    20278 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form/tests/
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form/tests/templates/
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/templates/custom-error.pt
--rw-rw-rw-   0 root         (0) root         (0)     1100 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/templates/file-testing-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/templates/integration-edit.pt
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/templates/simple-caredit-subforms.pt
--rw-rw-rw-   0 root         (0) root         (0)      709 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/templates/simple-caredit.pt
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/templates/simple-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1243 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/templates/simple-edit-with-providers.pt
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/templates/simple-edit-with-subforms.pt
--rw-rw-rw-   0 root         (0) root         (0)      628 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/templates/simple-edit.pt
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/templates/simple-groupedit.pt
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/templates/simple-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/templates/simple-nested-groupedit.pt
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/templates/simple-owneredit.pt
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/templates/simple-subedit.pt
--rw-rw-rw-   0 root         (0) root         (0)     1836 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1855 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     8555 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/util.py
--rw-rw-rw-   0 root         (0) root         (0)     8061 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/validator.py
--rw-rw-rw-   0 root         (0) root         (0)     3006 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/value.py
--rw-rw-rw-   0 root         (0) root         (0)    24867 2023-12-11 13:33:54.000000 pyams_form-2.0.2/src/pyams_form/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4781 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7239 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-11 13:34:13.000000 pyams_form-2.0.2/src/pyams_form.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      351 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-12-11 13:34:34.000000 pyams_form-2.0.2/src/pyams_form.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-09 19:55:47.000000 pyams_form-2.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-04-09 19:55:47.000000 pyams_form-2.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4899 2024-04-09 19:56:28.000000 pyams_form-2.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     3137 2024-04-09 19:55:47.000000 pyams_form-2.1.0/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-04-09 19:55:47.000000 pyams_form-2.1.0/docs/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-04-09 19:55:47.000000 pyams_form-2.1.0/docs/form-graph.dot
+-rw-rw-rw-   0 root         (0) root         (0)    11877 2024-04-09 19:55:47.000000 pyams_form-2.1.0/docs/form-graph.png
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2024-04-09 19:55:47.000000 pyams_form-2.1.0/docs/widget-graph.dot
+-rw-rw-rw-   0 root         (0) root         (0)    13789 2024-04-09 19:55:47.000000 pyams_form-2.1.0/docs/widget-graph.png
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 19:56:28.000000 pyams_form-2.1.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2877 2024-04-09 19:55:47.000000 pyams_form-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form/
+-rw-rw-rw-   0 root         (0) root         (0)      854 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/action.py
+-rw-rw-rw-   0 root         (0) root         (0)    16892 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/ajax.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form/browser/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1656 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/button.py
+-rw-rw-rw-   0 root         (0) root         (0)     3500 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/checkbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/image.py
+-rw-rw-rw-   0 root         (0) root         (0)    13085 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3801 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/multi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1421 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/object.py
+-rw-rw-rw-   0 root         (0) root         (0)     3729 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/orderedselect.py
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/password.py
+-rw-rw-rw-   0 root         (0) root         (0)     3745 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/radio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form/browser/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form/browser/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)     3364 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/resources/js/orderedselect-input.js
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/resources/js/orderedselect-input.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     5163 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/select.py
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/submit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/text.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/textarea.py
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/textlines.py
+-rw-rw-rw-   0 root         (0) root         (0)     8027 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/browser/widget.py
+-rw-rw-rw-   0 root         (0) root         (0)    11593 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/button.py
+-rw-rw-rw-   0 root         (0) root         (0)     5383 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/contentprovider.py
+-rw-rw-rw-   0 root         (0) root         (0)    16755 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     5480 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/datamanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)     3471 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9810 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/action.rst
+-rw-rw-rw-   0 root         (0) root         (0)    19164 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/ajax.rst
+-rw-rw-rw-   0 root         (0) root         (0)   113044 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/browser.rst
+-rw-rw-rw-   0 root         (0) root         (0)    19674 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/button.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10584 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/contentprovider.rst
+-rw-rw-rw-   0 root         (0) root         (0)    32750 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/converter.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10500 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/datamanager.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8281 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/error.rst
+-rw-rw-rw-   0 root         (0) root         (0)    30830 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/field.rst
+-rw-rw-rw-   0 root         (0) root         (0)    65455 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/form.rst
+-rw-rw-rw-   0 root         (0) root         (0)    33058 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/group.rst
+-rw-rw-rw-   0 root         (0) root         (0)    26338 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/hint.rst
+-rw-rw-rw-   0 root         (0) root         (0)      522 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/index-browser.rst
+-rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2589 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/object-caveat.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5942 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/security.rst
+-rw-rw-rw-   0 root         (0) root         (0)    38934 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/subform.rst
+-rw-rw-rw-   0 root         (0) root         (0)    20978 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/term.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/testing.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15386 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/util.rst
+-rw-rw-rw-   0 root         (0) root         (0)    20915 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/validator.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8357 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/value.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2257 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-button.rst
+-rw-rw-rw-   0 root         (0) root         (0)    12744 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-checkbox.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4496 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-file-testing.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-file.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-image.rst
+-rw-rw-rw-   0 root         (0) root         (0)    21423 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-multi-dict-integration.rst
+-rw-rw-rw-   0 root         (0) root         (0)    14042 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-multi-list-integration.rst
+-rw-rw-rw-   0 root         (0) root         (0)    52089 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-multi.rst
+-rw-rw-rw-   0 root         (0) root         (0)    20939 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-object-multi-dict-integration.rst
+-rw-rw-rw-   0 root         (0) root         (0)    17704 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-object-multi-list-integration.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-object-single-integration.rst
+-rw-rw-rw-   0 root         (0) root         (0)    39953 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-object.rst
+-rw-rw-rw-   0 root         (0) root         (0)    63193 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-objectmulti.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8679 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-orderedselect.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-password.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9424 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-radio.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8172 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-select-missing-terms.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-select-source.rst
+-rw-rw-rw-   0 root         (0) root         (0)    12593 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-select.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2482 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-submit.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-text.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-textarea.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget-textlines.rst
+-rw-rw-rw-   0 root         (0) root         (0)    31086 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/doctests/widget.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/error.py
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/events.py
+-rw-rw-rw-   0 root         (0) root         (0)    13295 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/field.py
+-rw-rw-rw-   0 root         (0) root         (0)    20493 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/form.py
+-rw-rw-rw-   0 root         (0) root         (0)     4579 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/group.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/hint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1028 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/include.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     9914 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4651 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/button.py
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/error.py
+-rw-rw-rw-   0 root         (0) root         (0)    13796 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/form.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/button-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      868 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/button-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      680 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/checkbox-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/checkbox-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2725 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/checkbox-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/error.pt
+-rw-rw-rw-   0 root         (0) root         (0)      563 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/file-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      931 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/file-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      205 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/image-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/image-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1701 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/multi-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      301 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/multi-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/multi-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/object-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/object-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)      516 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/object-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      678 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/orderedselect-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3266 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/orderedselect-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      563 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/password-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/password-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/radio-display-single.pt
+-rw-rw-rw-   0 root         (0) root         (0)      680 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/radio-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/radio-hidden-single.pt
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/radio-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)      952 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/radio-input-single.pt
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/radio-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      680 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/select-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      283 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/select-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/select-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/submit-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      868 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/submit-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      480 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/text-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/text-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/text-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      480 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/textarea-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/textarea-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/textarea-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      563 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/textlines-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/textlines-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/textlines-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/widget-layout-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/widget-layout-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)      408 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/templates/widget-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)    19108 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/interfaces/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    14287 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.mo
+-rw-rw-rw-   0 root         (0) root         (0)    20915 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.po
+-rw-rw-rw-   0 root         (0) root         (0)    15253 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/locales/pyams_form.pot
+-rw-rw-rw-   0 root         (0) root         (0)    14307 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/object.py
+-rw-rw-rw-   0 root         (0) root         (0)     4226 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/outputchecker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/subform.py
+-rw-rw-rw-   0 root         (0) root         (0)     6833 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/template.py
+-rw-rw-rw-   0 root         (0) root         (0)    11899 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/term.py
+-rw-rw-rw-   0 root         (0) root         (0)    20278 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      799 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form/tests/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/templates/custom-error.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1100 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/templates/file-testing-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      651 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/templates/integration-edit.pt
+-rw-rw-rw-   0 root         (0) root         (0)      744 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/templates/simple-caredit-subforms.pt
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/templates/simple-caredit.pt
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/templates/simple-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1243 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/templates/simple-edit-with-providers.pt
+-rw-rw-rw-   0 root         (0) root         (0)      744 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/templates/simple-edit-with-subforms.pt
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/templates/simple-edit.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/templates/simple-groupedit.pt
+-rw-rw-rw-   0 root         (0) root         (0)      268 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/templates/simple-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/templates/simple-nested-groupedit.pt
+-rw-rw-rw-   0 root         (0) root         (0)      584 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/templates/simple-owneredit.pt
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/templates/simple-subedit.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1855 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     8555 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     8061 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3006 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/value.py
+-rw-rw-rw-   0 root         (0) root         (0)    24867 2024-04-09 19:55:47.000000 pyams_form-2.1.0/src/pyams_form/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4899 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7239 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 19:56:06.000000 pyams_form-2.1.0/src/pyams_form.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      351 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-09 19:56:28.000000 pyams_form-2.1.0/src/pyams_form.egg-info/top_level.txt
```

### Comparing `pyams_form-2.0.2/LICENSE` & `pyams_form-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/PKG-INFO` & `pyams_form-2.1.0/src/pyams_form.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams_form
-Version: 2.0.2
+Name: pyams-form
+Version: 2.1.0
 Summary: PyAMS forms management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -50,14 +50,19 @@
 ** Package API is also converted to common Python standards, using snake_case for variables and
 methods.
 
 
 Changelog
 =========
 
+2.1.0
+-----
+ - added final decorator to form content getter (using only adapters)
+ - added form groups getter method
+
 2.0.2
 -----
  - added mising interfaces attributes
 
 2.0.1
 -----
  - updated Buildout configuration
```

### Comparing `pyams_form-2.0.2/docs/HISTORY.rst` & `pyams_form-2.1.0/docs/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+2.1.0
+-----
+ - added final decorator to form content getter (using only adapters)
+ - added form groups getter method
+
 2.0.2
 -----
  - added mising interfaces attributes
 
 2.0.1
 -----
  - updated Buildout configuration
```

### Comparing `pyams_form-2.0.2/docs/README.rst` & `pyams_form-2.1.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/docs/form-graph.dot` & `pyams_form-2.1.0/docs/form-graph.dot`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/docs/form-graph.png` & `pyams_form-2.1.0/docs/form-graph.png`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/docs/widget-graph.dot` & `pyams_form-2.1.0/docs/widget-graph.dot`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/docs/widget-graph.png` & `pyams_form-2.1.0/docs/widget-graph.png`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/setup.py` & `pyams_form-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '2.0.2'
+version = '2.1.0'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_i18n',
     'zc.sourcefactory',
     'zope.testing'
 ]
```

### Comparing `pyams_form-2.0.2/src/pyams_form/__init__.py` & `pyams_form-2.1.0/src/pyams_form/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/action.py` & `pyams_form-2.1.0/src/pyams_form/action.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/ajax.py` & `pyams_form-2.1.0/src/pyams_form/ajax.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/__init__.py` & `pyams_form-2.1.0/src/pyams_form/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/button.py` & `pyams_form-2.1.0/src/pyams_form/browser/button.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/checkbox.py` & `pyams_form-2.1.0/src/pyams_form/browser/checkbox.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/file.py` & `pyams_form-2.1.0/src/pyams_form/browser/file.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/image.py` & `pyams_form-2.1.0/src/pyams_form/browser/image.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/interfaces.py` & `pyams_form-2.1.0/src/pyams_form/browser/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/multi.py` & `pyams_form-2.1.0/src/pyams_form/browser/multi.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/object.py` & `pyams_form-2.1.0/src/pyams_form/browser/object.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/orderedselect.py` & `pyams_form-2.1.0/src/pyams_form/browser/orderedselect.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/password.py` & `pyams_form-2.1.0/src/pyams_form/browser/password.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/radio.py` & `pyams_form-2.1.0/src/pyams_form/browser/radio.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/resources/js/orderedselect-input.js` & `pyams_form-2.1.0/src/pyams_form/browser/resources/js/orderedselect-input.js`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/resources/js/orderedselect-input.min.js` & `pyams_form-2.1.0/src/pyams_form/browser/resources/js/orderedselect-input.min.js`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/select.py` & `pyams_form-2.1.0/src/pyams_form/browser/select.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/submit.py` & `pyams_form-2.1.0/src/pyams_form/browser/submit.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/text.py` & `pyams_form-2.1.0/src/pyams_form/browser/text.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/textarea.py` & `pyams_form-2.1.0/src/pyams_form/browser/textarea.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/textlines.py` & `pyams_form-2.1.0/src/pyams_form/browser/textlines.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/browser/widget.py` & `pyams_form-2.1.0/src/pyams_form/browser/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/button.py` & `pyams_form-2.1.0/src/pyams_form/button.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/contentprovider.py` & `pyams_form-2.1.0/src/pyams_form/contentprovider.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/converter.py` & `pyams_form-2.1.0/src/pyams_form/converter.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/datamanager.py` & `pyams_form-2.1.0/src/pyams_form/datamanager.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/README.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/action.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/action.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/ajax.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/ajax.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/browser.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/browser.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/button.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/button.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/contentprovider.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/contentprovider.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/converter.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/converter.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/datamanager.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/datamanager.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/error.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/error.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/field.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/field.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/form.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/form.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/group.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/group.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/hint.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/hint.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/index-browser.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/index-browser.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/object-caveat.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/object-caveat.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/security.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/security.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/subform.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/subform.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/term.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/term.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/testing.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/testing.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/util.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/util.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/validator.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/validator.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/value.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/value.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-button.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-button.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-checkbox.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-checkbox.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-file-testing.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-file-testing.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-file.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-file.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-image.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-image.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-multi-dict-integration.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-multi-dict-integration.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-multi-list-integration.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-multi-list-integration.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-multi.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-multi.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-object-multi-dict-integration.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-object-multi-dict-integration.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-object-multi-list-integration.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-object-multi-list-integration.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-object-single-integration.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-object-single-integration.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-object.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-object.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-objectmulti.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-objectmulti.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-orderedselect.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-orderedselect.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-password.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-password.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-radio.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-radio.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-select-missing-terms.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-select-missing-terms.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-select-source.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-select-source.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-select.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-select.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-submit.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-submit.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-text.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-text.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-textarea.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-textarea.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget-textlines.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget-textlines.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/doctests/widget.rst` & `pyams_form-2.1.0/src/pyams_form/doctests/widget.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/error.py` & `pyams_form-2.1.0/src/pyams_form/error.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/events.py` & `pyams_form-2.1.0/src/pyams_form/events.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/field.py` & `pyams_form-2.1.0/src/pyams_form/field.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/form.py` & `pyams_form-2.1.0/src/pyams_form/form.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 """PyAMS_form.form module
 
 This module defines all main forms management classes.
 """
 
 import json
 import sys
+try:
+    from typing import final
+except ImportError:
+    def final(func):
+        return func
 
 from persistent import IPersistent
 from pyramid.decorator import reify
 from pyramid.events import subscriber
 from pyramid.response import Response
 from zope.interface import implementer
 from zope.lifecycleevent import Attributes, ObjectCreatedEvent, ObjectModifiedEvent
@@ -213,16 +218,22 @@
         """Form content getter"""
         content = self.request.registry.queryMultiAdapter((self.context, self.request, self),
                                                           IFormContent)
         if content is None:
             content = self.context
         return content
 
+    @final
     def get_content(self):
-        """See interfaces.form.IForm"""
+        """See interfaces.form.IForm
+
+        You should not override this method!
+        If you need custom content getter in your form, just add
+        a custom IFormContent adapter (see "form_content" getter above).
+        """
         return self.form_content
 
     @property
     def required_info(self):
         """Form required information label"""
         if (self.required_label is not None and self.widgets is not None and
                 self.widgets.has_required_fields):
```

### Comparing `pyams_form-2.0.2/src/pyams_form/group.py` & `pyams_form-2.1.0/src/pyams_form/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,32 +29,36 @@
 
 @implementer(IGroupManager)
 class GroupManager:  # pylint: disable=no-member
     """Base groups manager mixin class"""
 
     groups = ()
 
+    def get_groups(self):
+        """Internal groups iterator getter"""
+        registry = self.request.registry
+        yield from sorted((adapter for name, adapter in
+                           registry.getAdapters((self.context, self.request, self), IGroup)),
+                          key=get_form_weight)
+
     def update(self):
         """See interfaces.IForm"""
         self.update_widgets()
         groups = []
         # static groups list
         for group_class in self.groups:
             # only instantiate the group_class if it hasn't already
             # been instantiated
             if IGroup.providedBy(group_class):
                 group = group_class
             else:
                 group = group_class(self.context, self.request, self)
             groups.append(group)
         # groups can also be added dynamically using adapters
-        registry = self.request.registry
-        for group in sorted((adapter for name, adapter in
-                             registry.getAdapters((self.context, self.request, self), IGroup)),
-                            key=get_form_weight):
+        for group in self.get_groups():
             groups.append(group)
         # update all groups
         [group.update() for group in groups]  # pylint: disable=expression-not-assigned
         self.groups = tuple(groups)
         [subform.update() for subform in self.subforms]  # pylint: disable=expression-not-assigned
         [tabform.update() for tabform in self.tabforms]  # pylint: disable=expression-not-assigned
         self.request.registry.notify(FormUpdatedEvent(self))
```

### Comparing `pyams_form-2.0.2/src/pyams_form/hint.py` & `pyams_form-2.1.0/src/pyams_form/hint.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/include.py` & `pyams_form-2.1.0/src/pyams_form/include.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/__init__.py` & `pyams_form-2.1.0/src/pyams_form/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/button.py` & `pyams_form-2.1.0/src/pyams_form/interfaces/button.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/error.py` & `pyams_form-2.1.0/src/pyams_form/interfaces/error.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/form.py` & `pyams_form-2.1.0/src/pyams_form/interfaces/form.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,14 +363,17 @@
     """Groups manager interface"""
 
     groups = Tuple(title='Groups',
                    description=('Initially a collection of group classes, which are '
                                 'converted to group instances when the form is '
                                 'updated.'))
 
+    def get_groups(self):
+        """Internal groups iterator getter"""
+
 
 class IGroup(IGroupManager):
     """A group of fields/widgets within a form."""
 
     parent_form = Attribute("Parent form")
```

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/button-input.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/button-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/checkbox-display.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/checkbox-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/checkbox-hidden.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/checkbox-hidden.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/checkbox-input.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/checkbox-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/file-display.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/file-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/file-input.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/file-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/image-input.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/image-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/multi-display.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/multi-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/multi-input.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/multi-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/object-input.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/object-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/orderedselect-display.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/orderedselect-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/orderedselect-input.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/orderedselect-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/password-display.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/password-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/password-input.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/password-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/radio-display-single.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/radio-display-single.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/radio-display.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/radio-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/radio-input-single.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/radio-input-single.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/select-display.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/select-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/select-input.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/select-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/submit-input.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/submit-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/text-input.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/text-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/textarea-input.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/textarea-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/textlines-display.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/textlines-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/templates/textlines-input.pt` & `pyams_form-2.1.0/src/pyams_form/interfaces/templates/textlines-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/interfaces/widget.py` & `pyams_form-2.1.0/src/pyams_form/interfaces/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.mo` & `pyams_form-2.1.0/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.mo`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.po` & `pyams_form-2.1.0/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.po`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/locales/pyams_form.pot` & `pyams_form-2.1.0/src/pyams_form/locales/pyams_form.pot`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/object.py` & `pyams_form-2.1.0/src/pyams_form/object.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/outputchecker.py` & `pyams_form-2.1.0/src/pyams_form/outputchecker.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/subform.py` & `pyams_form-2.1.0/src/pyams_form/subform.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/template.py` & `pyams_form-2.1.0/src/pyams_form/template.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/term.py` & `pyams_form-2.1.0/src/pyams_form/term.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/testing.py` & `pyams_form-2.1.0/src/pyams_form/testing.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/tests/__init__.py` & `pyams_form-2.1.0/src/pyams_form/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/tests/templates/file-testing-input.pt` & `pyams_form-2.1.0/src/pyams_form/tests/templates/file-testing-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/tests/templates/integration-edit.pt` & `pyams_form-2.1.0/src/pyams_form/tests/templates/integration-edit.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/tests/templates/simple-caredit-subforms.pt` & `pyams_form-2.1.0/src/pyams_form/tests/templates/simple-caredit-subforms.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/tests/templates/simple-caredit.pt` & `pyams_form-2.1.0/src/pyams_form/tests/templates/simple-caredit.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/tests/templates/simple-edit-with-providers.pt` & `pyams_form-2.1.0/src/pyams_form/tests/templates/simple-edit-with-providers.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/tests/templates/simple-edit-with-subforms.pt` & `pyams_form-2.1.0/src/pyams_form/tests/templates/simple-edit-with-subforms.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/tests/templates/simple-edit.pt` & `pyams_form-2.1.0/src/pyams_form/tests/templates/simple-edit.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/tests/templates/simple-groupedit.pt` & `pyams_form-2.1.0/src/pyams_form/tests/templates/simple-groupedit.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/tests/templates/simple-nested-groupedit.pt` & `pyams_form-2.1.0/src/pyams_form/tests/templates/simple-nested-groupedit.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/tests/templates/simple-owneredit.pt` & `pyams_form-2.1.0/src/pyams_form/tests/templates/simple-owneredit.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/tests/test_utilsdocs.py` & `pyams_form-2.1.0/src/pyams_form/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/tests/test_utilsdocstrings.py` & `pyams_form-2.1.0/src/pyams_form/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/util.py` & `pyams_form-2.1.0/src/pyams_form/util.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/validator.py` & `pyams_form-2.1.0/src/pyams_form/validator.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/value.py` & `pyams_form-2.1.0/src/pyams_form/value.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form/widget.py` & `pyams_form-2.1.0/src/pyams_form/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_form-2.0.2/src/pyams_form.egg-info/PKG-INFO` & `pyams_form-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams-form
-Version: 2.0.2
+Name: pyams_form
+Version: 2.1.0
 Summary: PyAMS forms management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -50,14 +50,19 @@
 ** Package API is also converted to common Python standards, using snake_case for variables and
 methods.
 
 
 Changelog
 =========
 
+2.1.0
+-----
+ - added final decorator to form content getter (using only adapters)
+ - added form groups getter method
+
 2.0.2
 -----
  - added mising interfaces attributes
 
 2.0.1
 -----
  - updated Buildout configuration
```

### Comparing `pyams_form-2.0.2/src/pyams_form.egg-info/SOURCES.txt` & `pyams_form-2.1.0/src/pyams_form.egg-info/SOURCES.txt`

 * *Files identical despite different names*

