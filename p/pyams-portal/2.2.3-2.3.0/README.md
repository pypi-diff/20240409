# Comparing `tmp/pyams_portal-2.2.3.tar.gz` & `tmp/pyams_portal-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_portal-2.2.3.tar", last modified: Wed Feb 14 17:27:08 2024, max compression
+gzip compressed data, was "dist/pyams_portal-2.3.0.tar", last modified: Tue Apr  9 20:29:40 2024, max compression
```

## Comparing `pyams_portal-2.2.3.tar` & `pyams_portal-2.3.0.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6171 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/docs/
--rwxrwxrwx   0 root         (0) root         (0)     4102 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1540 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2948 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/
--rw-rw-rw-   0 root         (0) root         (0)      863 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    36160 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/generations/
--rw-rw-rw-   0 root         (0) root         (0)     1735 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1926 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/generations/evolve1.py
--rw-rw-rw-   0 root         (0) root         (0)     1591 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/generations/evolve2.py
--rw-rw-rw-   0 root         (0) root         (0)     1805 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/generations/evolve3.py
--rw-rw-rw-   0 root         (0) root         (0)     1874 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/generations/evolve4.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/include.py
--rw-rw-rw-   0 root         (0) root         (0)    21042 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    25441 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.mo
--rw-rw-rw-   0 root         (0) root         (0)    42359 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.po
--rw-rw-rw-   0 root         (0) root         (0)    28892 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/locales/pyams_portal.pot
--rw-rw-rw-   0 root         (0) root         (0)    11053 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/page.py
--rw-rw-rw-   0 root         (0) root         (0)    14705 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/
--rw-rw-rw-   0 root         (0) root         (0)      567 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/cards/
--rw-rw-rw-   0 root         (0) root         (0)     3941 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/cards/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3618 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/cards/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/cards/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3002 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/cards/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2377 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/cards/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/cards/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1946 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/cards/skin/templates/cards-masonry.pt
--rw-rw-rw-   0 root         (0) root         (0)     2015 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/cards/skin/templates/cards.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/cards/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    10037 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/cards/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/cards/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/cards/zmi/templates/cards-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/
--rw-rw-rw-   0 root         (0) root         (0)     3902 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2376 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2670 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3108 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2542 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/skin/templates/carousel.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     9782 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      455 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/zmi/templates/carousel-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/html/
--rw-rw-rw-   0 root         (0) root         (0)     2061 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/html/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1678 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/html/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/html/skin/
--rw-rw-rw-   0 root         (0) root         (0)     5034 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/html/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/html/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/html/skin/templates/html.pt
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/html/skin/templates/raw-code.pt
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/html/skin/templates/raw.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/html/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2827 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/html/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/html/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/html/zmi/templates/html-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      615 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/html/zmi/templates/raw-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/image/
--rw-rw-rw-   0 root         (0) root         (0)     1819 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/image/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      989 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/image/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/image/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1426 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/image/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/image/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/image/skin/templates/image.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/image/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/image/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/image/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2931 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/image/zmi/templates/image-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/jumbotron/
--rw-rw-rw-   0 root         (0) root         (0)     1999 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/jumbotron/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2895 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/jumbotron/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/jumbotron/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1382 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/jumbotron/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/jumbotron/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      807 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/jumbotron/skin/templates/jumbotron.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/jumbotron/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1234 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/jumbotron/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/jumbotron/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      509 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/jumbotron/zmi/templates/jumbotron-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/
--rw-rw-rw-   0 root         (0) root         (0)     1293 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1925 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2996 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/skin/templates/spacer-double.pt
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/skin/templates/spacer-thin.pt
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/skin/templates/spacer.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1213 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/zmi/templates/spacer-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/skin/
--rw-rw-rw-   0 root         (0) root         (0)     9743 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8759 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/skin/page.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1197 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/skin/templates/layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     1185 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/skin/templates/pagelet.pt
--rw-rw-rw-   0 root         (0) root         (0)     4159 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/slot.py
--rw-rw-rw-   0 root         (0) root         (0)    15789 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/tests/
--rw-rw-rw-   0 root         (0) root         (0)      801 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20212 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/tests/test_image.png
--rw-rw-rw-   0 root         (0) root         (0)     1827 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1861 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     4869 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/thumbnails.py
--rw-rw-rw-   0 root         (0) root         (0)     1443 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     7142 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8464 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    15952 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/layout.py
--rw-rw-rw-   0 root         (0) root         (0)    22951 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/portlet.py
--rw-rw-rw-   0 root         (0) root         (0)    13637 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/presentation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/resources/css/
--rw-rw-rw-   0 root         (0) root         (0)    24268 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/resources/css/layout.css
--rw-rw-rw-   0 root         (0) root         (0)    20882 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/resources/css/layout.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/resources/img/
--rw-rw-rw-   0 root         (0) root         (0)     6515 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/resources/img/hidden.png
--rw-rw-rw-   0 root         (0) root         (0)     1534 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/resources/img/unknown.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/resources/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/resources/js/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      345 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/resources/js/i18n/layout-fr.js
--rw-rw-rw-   0 root         (0) root         (0)    33614 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/resources/js/layout.js
--rw-rw-rw-   0 root         (0) root         (0)    15539 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/resources/js/layout.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/resources/sass/
--rw-rw-rw-   0 root         (0) root         (0)    14582 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/resources/sass/layout.scss
--rw-rw-rw-   0 root         (0) root         (0)    13798 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/slot.py
--rw-rw-rw-   0 root         (0) root         (0)     8022 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/templates/empty.pt
--rw-rw-rw-   0 root         (0) root         (0)     7548 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/templates/layout.pt
--rw-rw-rw-   0 root         (0) root         (0)      181 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/templates/portlet-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)     1089 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/templates/portlet-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     2649 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/templates/presentation-template.pt
--rw-rw-rw-   0 root         (0) root         (0)     2110 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/templates/renderer-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/templates/setting-bool-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/templates/setting-none-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/templates/setting-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/templates/thumbnails-widget.pt
--rw-rw-rw-   0 root         (0) root         (0)     8030 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/thumbnails.py
--rw-rw-rw-   0 root         (0) root         (0)     2275 2024-02-14 17:26:32.000000 pyams_portal-2.2.3/src/pyams_portal/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6171 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4951 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 17:27:00.000000 pyams_portal-2.2.3/src/pyams_portal.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      413 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-02-14 17:27:08.000000 pyams_portal-2.2.3/src/pyams_portal.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6345 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     4276 2024-04-09 20:22:38.000000 pyams_portal-2.3.0/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2947 2024-04-09 20:22:38.000000 pyams_portal-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/
+-rw-rw-rw-   0 root         (0) root         (0)      863 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    36160 2024-02-14 17:21:12.000000 pyams_portal-2.3.0/src/pyams_portal/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     1735 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/generations/evolve1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/generations/evolve2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1805 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/generations/evolve3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1874 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/generations/evolve4.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/include.py
+-rw-rw-rw-   0 root         (0) root         (0)    21042 2024-02-01 22:15:37.000000 pyams_portal-2.3.0/src/pyams_portal/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    25441 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.mo
+-rw-rw-rw-   0 root         (0) root         (0)    42240 2024-04-09 20:22:38.000000 pyams_portal-2.3.0/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.po
+-rw-rw-rw-   0 root         (0) root         (0)    28892 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/locales/pyams_portal.pot
+-rw-rw-rw-   0 root         (0) root         (0)    11053 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/page.py
+-rw-rw-rw-   0 root         (0) root         (0)    14705 2024-02-14 17:08:58.000000 pyams_portal-2.3.0/src/pyams_portal/portlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/cards/
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/cards/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3618 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/cards/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/cards/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2024-04-09 20:22:38.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/cards/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2218 2024-04-09 20:22:38.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/cards/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/cards/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1537 2024-04-09 20:22:38.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/cards/skin/templates/cards-masonry.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1597 2024-04-09 20:22:38.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/cards/skin/templates/cards.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/cards/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    10037 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/cards/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/cards/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/cards/zmi/templates/cards-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/
+-rw-rw-rw-   0 root         (0) root         (0)     3902 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2376 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2670 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3108 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/skin/templates/carousel.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     9782 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      455 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/zmi/templates/carousel-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/html/
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/html/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1678 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/html/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/html/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     5034 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/html/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/html/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/html/skin/templates/html.pt
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/html/skin/templates/raw-code.pt
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/html/skin/templates/raw.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/html/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2827 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/html/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/html/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/html/zmi/templates/html-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/html/zmi/templates/raw-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/image/
+-rw-rw-rw-   0 root         (0) root         (0)     1819 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/image/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      989 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/image/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/image/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/image/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/image/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/image/skin/templates/image.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/image/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/image/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/image/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/image/zmi/templates/image-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/
+-rw-rw-rw-   0 root         (0) root         (0)     1999 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2920 2024-04-09 20:22:38.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1382 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/skin/templates/jumbotron.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      509 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/zmi/templates/jumbotron-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2996 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/skin/templates/spacer-double.pt
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/skin/templates/spacer-thin.pt
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/skin/templates/spacer.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/zmi/templates/spacer-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     9743 2024-02-14 17:08:58.000000 pyams_portal-2.3.0/src/pyams_portal/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8759 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/skin/page.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/skin/templates/layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/skin/templates/pagelet.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4159 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/slot.py
+-rw-rw-rw-   0 root         (0) root         (0)    15789 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20212 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/tests/test_image.png
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     4869 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/thumbnails.py
+-rw-rw-rw-   0 root         (0) root         (0)     1443 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     7142 2023-12-18 13:04:21.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8464 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2024-04-09 20:22:38.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    15952 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/layout.py
+-rw-rw-rw-   0 root         (0) root         (0)    23640 2024-04-09 20:22:38.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/portlet.py
+-rw-rw-rw-   0 root         (0) root         (0)    14099 2024-04-09 20:22:38.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/presentation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/resources/css/
+-rw-rw-rw-   0 root         (0) root         (0)    24268 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/resources/css/layout.css
+-rw-rw-rw-   0 root         (0) root         (0)    20882 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/resources/css/layout.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/resources/img/
+-rw-rw-rw-   0 root         (0) root         (0)     6823 2024-04-09 20:22:38.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/resources/img/hidden.png
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2024-04-09 20:22:38.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/resources/img/unknown.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/resources/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/resources/js/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/resources/js/i18n/layout-fr.js
+-rw-rw-rw-   0 root         (0) root         (0)    33614 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/resources/js/layout.js
+-rw-rw-rw-   0 root         (0) root         (0)    15539 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/resources/js/layout.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/resources/sass/
+-rw-rw-rw-   0 root         (0) root         (0)    14582 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/resources/sass/layout.scss
+-rw-rw-rw-   0 root         (0) root         (0)    14154 2024-04-09 20:22:38.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/slot.py
+-rw-rw-rw-   0 root         (0) root         (0)     8022 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:28:53.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/templates/empty.pt
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/templates/layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/templates/portlet-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/templates/portlet-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2649 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/templates/presentation-template.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2110 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/templates/renderer-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/templates/setting-bool-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/templates/setting-none-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-12-13 08:45:27.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/templates/setting-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/templates/thumbnails-widget.pt
+-rw-rw-rw-   0 root         (0) root         (0)     8030 2024-02-01 22:15:37.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/thumbnails.py
+-rw-rw-rw-   0 root         (0) root         (0)     2275 2024-02-01 22:00:51.000000 pyams_portal-2.3.0/src/pyams_portal/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6345 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4951 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:29:30.000000 pyams_portal-2.3.0/src/pyams_portal.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      412 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-09 20:29:40.000000 pyams_portal-2.3.0/src/pyams_portal.egg-info/top_level.txt
```

### Comparing `pyams_portal-2.2.3/LICENSE` & `pyams_portal-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/PKG-INFO` & `pyams_portal-2.3.0/src/pyams_portal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams_portal
-Version: 2.2.3
+Name: pyams-portal
+Version: 2.3.0
 Summary: PyAMS portlets management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -52,14 +52,20 @@
 content management packages like PyAMS_content, while other extension packages can be used to
 provide custom portlets renderers.
 
 
 Changelog
 =========
 
+2.3.0
+-----
+ - updated cards portlet thumbnails selection field
+ - updated portlet renderer settings edit form fields and groups getters
+ - added edit forms content getters
+
 2.2.3
 -----
  - corrected doctest
 
 2.2.2
 -----
  - updated portlets cache key to include page name (which may be required when
```

### Comparing `pyams_portal-2.2.3/docs/HISTORY.rst` & `pyams_portal-2.3.0/docs/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+2.3.0
+-----
+ - updated cards portlet thumbnails selection field
+ - updated portlet renderer settings edit form fields and groups getters
+ - added edit forms content getters
+
 2.2.3
 -----
  - corrected doctest
 
 2.2.2
 -----
  - updated portlets cache key to include page name (which may be required when
```

### Comparing `pyams_portal-2.2.3/docs/README.rst` & `pyams_portal-2.3.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/setup.py` & `pyams_portal-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '2.2.3'
+version = '2.3.0'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_catalog',
     'pyams_form',
     'pyams_zmi',
     'pyramid_zcml',
@@ -68,15 +68,15 @@
           'pyams_file',
           'pyams_i18n',
           'pyams_layer',
           'pyams_pagelet',
           'pyams_security',
           'pyams_sequence',
           'pyams_site',
-          'pyams_skin >= 1.8.0',
+          'pyams_skin > 2.1.0',
           'pyams_template',
           'pyams_utils >= 2.2.0',
           'pyams_workflow',
           'pyramid >= 2.0.0',
           'venusian',
           'zope.annotation',
           'zope.container',
```

### Comparing `pyams_portal-2.2.3/src/pyams_portal/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/doctests/README.rst` & `pyams_portal-2.3.0/src/pyams_portal/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/generations/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/generations/evolve1.py` & `pyams_portal-2.3.0/src/pyams_portal/generations/evolve1.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/generations/evolve2.py` & `pyams_portal-2.3.0/src/pyams_portal/generations/evolve2.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/generations/evolve3.py` & `pyams_portal-2.3.0/src/pyams_portal/generations/evolve3.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/generations/evolve4.py` & `pyams_portal-2.3.0/src/pyams_portal/generations/evolve4.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/include.py` & `pyams_portal-2.3.0/src/pyams_portal/include.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/interfaces.py` & `pyams_portal-2.3.0/src/pyams_portal/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.mo` & `pyams_portal-2.3.0/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.mo`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.po` & `pyams_portal-2.3.0/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.po`

 * *Files 1% similar despite different names*

```diff
@@ -1228,49 +1228,42 @@
 msgid "Bootstrap Jumbotron renderer (default)"
 msgstr "Jumbotron Bootstrap (par défaut)"
 
 #: src/pyams_portal/skin/__init__.py:221
 msgid "Hidden portlet"
 msgstr "NON affiché"
 
-#, python-format
 #~ msgid "Portlet configuration: « {} »"
 #~ msgstr "Configuration du composant : {}"
 
-#, python-format
 #~ msgid "Portlet: {portlet}"
 #~ msgstr "Composant « {portlet} »"
 
-#, python-format
 #~ msgid "<small>Portlet: {portlet}</small><br />« {renderer} » renderer"
 #~ msgstr ""
 #~ "<small>Composant « {portlet} »</small><br />Mode de rendu « {renderer} »"
 
 #~ msgid "Edit renderer settings"
 #~ msgstr "Propriétés du mode de rendu"
 
-#, python-format
 #~ msgid "« {} »  portal template"
 #~ msgstr "Modèle de présentation « {} »"
 
 #~ msgid "Portlet configuration"
 #~ msgstr "Configuration du composant"
 
-#, python-format
 #~ msgid "« {} » shared template"
 #~ msgstr "Modèle de présentation « {} »"
 
-#, python-format
 #~ msgid "« {} » portlet"
 #~ msgstr "Composant « {} »"
 
 #~ msgid "Add slot"
 #~ msgstr "Ajouter un bloc"
 
-#, python-format
 #~ msgid "« {} » slot properties"
 #~ msgstr "Propriétés du bloc « {} »"
 
 #~ msgid "Add row..."
 #~ msgstr "Ajouter une ligne"
 
 #~ msgid "Add portlet..."
```

### Comparing `pyams_portal-2.2.3/src/pyams_portal/locales/pyams_portal.pot` & `pyams_portal-2.3.0/src/pyams_portal/locales/pyams_portal.pot`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/page.py` & `pyams_portal-2.3.0/src/pyams_portal/page.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlet.py` & `pyams_portal-2.3.0/src/pyams_portal/portlet.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/cards/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/cards/interfaces.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/cards/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/cards/skin/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/cards/skin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 from persistent import Persistent
 from zope.container.contained import Contained
 from zope.interface import Interface
 from zope.schema.fieldproperty import FieldProperty
 
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_portal.interfaces import IPortalContext, IPortletRenderer
-from pyams_portal.portlets.cards import ICardsPortletSettings
-from pyams_portal.portlets.cards.skin.interfaces import CARDS_RENDERER_SETTINGS_KEY, \
-    ICardsPortletMasonryRendererSettings, ICardsPortletRendererSettings
+from pyams_portal.portlets.cards.interfaces import ICardsPortletSettings
+from pyams_portal.portlets.cards.skin.interfaces import ICardsPortletMasonryRendererSettings, \
+    ICardsPortletRendererSettings
 from pyams_portal.skin import PortletRenderer
 from pyams_template.template import template_config
 from pyams_utils.adapter import adapter_config
 from pyams_utils.factory import factory_config
 
 __docformat__ = 'restructuredtext'
```

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/cards/skin/interfaces.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/skin/interfaces.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,56 +6,70 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 
-"""PyAMS_portal.portlets.cards.skin.interfaces module
+"""PyAMS_portal.portlets.carousel.skin.interfaces module
 
 """
 
 from zope.interface import Interface
-from zope.schema import Choice, TextLine
+from zope.schema import Bool, Choice, TextLine
 
 from pyams_file.interfaces.thumbnail import THUMBNAILERS_VOCABULARY_NAME
 
 
 __docformat__ = 'restructuredtext'
 
 from pyams_portal import _  # pylint: disable=ungrouped-imports
 
 
-CARDS_RENDERER_SETTINGS_KEY = 'pyams_portal.renderer::cards'
+CAROUSEL_RENDERER_SETTINGS_KEY = 'pyams_portal.renderer::carousel'
 
 
-class ICardsPortletRendererSettings(Interface):
-    """Cards portlet renderer settings interface"""
+class ICarouselPortletRendererSettings(Interface):
+    """Carousel portlet renderer settings interface"""
 
     css_class = TextLine(title=_("CSS class"),
-                         description=_("Cards container CSS class"),
-                         default='row row-cols-2 row-cols-md-3 row-cols-lg-4')
+                         description=_("Carousel container CSS class"),
+                         required=False,
+                         default='carousel')
 
     thumb_selection = Choice(title=_("Images selection"),
-                             description=_("Cards will use responsive selections by default, "
-                                           "but you can also force selection of another "
-                                           "specific selection"),
+                             description=_("Carousel can use responsive selections, but you can "
+                                           "also force selection of another specific selection"),
                              vocabulary=THUMBNAILERS_VOCABULARY_NAME,
                              required=False)
 
-
-MASONRY_CARDS_RENDERER_SETTINGS_KEY = 'pyams_portal.renderer::cards::masonry'
-
-
-class ICardsPortletMasonryRendererSettings(Interface):
-    """Cards portlet Masonry renderer settings interface"""
-
-    css_class = TextLine(title=_("CSS class"),
-                         description=_("Cards container CSS class"),
-                         default='card-columns')
-
-    thumb_selection = Choice(title=_("Images selection"),
-                             description=_("Cards will use responsive selections by default, "
-                                           "but you can also force selection of another "
-                                           "specific selection"),
-                             vocabulary=THUMBNAILERS_VOCABULARY_NAME,
-                             required=False)
+    automatic_slide = Bool(title=_("Automatic sliding"),
+                           description=_("If 'no', sliding will only be activated manually"),
+                           required=True,
+                           default=True)
+
+    fade_effect = Bool(title=_("Fade effect"),
+                       description=_("If 'yes', slide to slide animation will use a fade effect "
+                                     "instead of lateral sliding"),
+                       required=True,
+                       default=False)
+
+    display_controls = Bool(title=_("Display controls"),
+                            description=_("If 'yes', display arrows to navigate between slides"),
+                            required=True,
+                            default=False)
+
+    display_indicators = Bool(title=_("Display indicators"),
+                              description=_("If 'yes', display indicators to show position of "
+                                            "current slide"),
+                              required=True,
+                              default=False)
+
+    display_captions = Bool(title=_("Display captions"),
+                            description=_("If 'no', slides titles and leads are not displayed"),
+                            required=True,
+                            default=True)
+
+    enable_touch = Bool(title=_("Enable swiping"),
+                        description=_("If 'no', touch events will be disabled on touchscreens"),
+                        required=True,
+                        default=True)
```

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/cards/skin/templates/cards-masonry.pt` & `pyams_portal-2.3.0/src/pyams_portal/portlets/cards/skin/templates/cards-masonry.pt`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 <div tal:define="settings view.settings;
 				 renderer_settings view.renderer_settings;
-				 slot_config view.slot_configuration;">
+				 slot_config view.slot_configuration;
+				 selections renderer_settings.thumb_selection;">
 	<h2 tal:define="title i18n:settings.title"
 		tal:condition="title">
 		${title}
 	</h2>
 	<p class="lead" tal:define="lead i18n:settings.lead"
 	   tal:condition="lead">${lead}</p>
 	<div class="${renderer_settings.css_class}">
 		<div tal:repeat="card settings.get_visible_items()"
 			 class="card ${card.css_class} px-0">
 			<tal:if define="illustration card.illustration"
 					condition="illustration">
 				${structure:tales:picture(illustration,
-										  xs_thumb=renderer_settings.thumb_selection,
-										  xs_width=slot_config.xs_width,
-										  sm_thumb=renderer_settings.thumb_selection,
-										  sm_width=slot_config.sm_width,
-										  md_thumb=renderer_settings.thumb_selection,
-										  md_width=slot_config.md_width,
-										  lg_thumb=renderer_settings.thumb_selection,
-										  lg_width=slot_config.lg_width,
-										  xl_thumb=renderer_settings.thumb_selection,
-										  xl_width=slot_config.xl_width,
+										  selections=selections,
 										  css_class='card-img-top w-100')}
 			</tal:if>
 			<div class="card-body"
 				 tal:define="title i18n:card.title;
 							 body i18n:card.body;"
 				 tal:condition="title or body">
 				<h3 class="card-title"
```

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/cards/skin/templates/cards.pt` & `pyams_portal-2.3.0/src/pyams_portal/portlets/cards/skin/templates/cards.pt`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,25 @@
 <div tal:define="settings view.settings;
 				 renderer_settings view.renderer_settings;
-				 slot_config view.slot_configuration;">
+				 slot_config view.slot_configuration;
+				 selections renderer_settings.thumb_selection;">
 	<h2 tal:define="title i18n:settings.title"
 		tal:condition="title">
 		${title}
 	</h2>
 	<p class="lead" tal:define="lead i18n:settings.lead"
 	   tal:condition="lead">${lead}</p>
 	<div class="${renderer_settings.css_class}">
 		<div tal:repeat="card settings.get_visible_items()"
 			 class="${card.css_class}">
 			<div class="card h-100">
 				<tal:if define="illustration card.illustration"
 						condition="illustration">
 					${structure:tales:picture(illustration,
-											  xs_thumb=renderer_settings.thumb_selection,
-											  xs_width=slot_config.xs_width,
-											  sm_thumb=renderer_settings.thumb_selection,
-											  sm_width=slot_config.sm_width,
-											  md_thumb=renderer_settings.thumb_selection,
-											  md_width=slot_config.md_width,
-											  lg_thumb=renderer_settings.thumb_selection,
-											  lg_width=slot_config.lg_width,
-											  xl_thumb=renderer_settings.thumb_selection,
-											  xl_width=slot_config.xl_width,
+											  selections=selections,
 											  css_class='card-img-top w-100')}
 				</tal:if>
 				<div class="card-body"
 					 tal:define="title i18n:card.title;
 								 body i18n:card.body;"
 					 tal:condition="title or body">
 					<h3 class="card-title"
```

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/cards/zmi/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/cards/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/interfaces.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/skin/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/skin/interfaces.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/interfaces.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,70 +6,68 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 
-"""PyAMS_portal.portlets.carousel.skin.interfaces module
+"""PyAMS_portal.portlets.jumbotron.interfaces module
 
-"""
 
-from zope.interface import Interface
-from zope.schema import Bool, Choice, TextLine
+"""
 
-from pyams_file.interfaces.thumbnail import THUMBNAILERS_VOCABULARY_NAME
+from zope.interface import Invalid, invariant
+from zope.schema import Bool, Choice, URI
 
+from pyams_i18n.schema import I18nTextField, I18nTextLineField
+from pyams_portal.interfaces import IPortletSettings
+from pyams_sequence.schema import InternalReferenceField
+from pyams_skin.interfaces import BOOTSTRAP_STATUS_VOCABULARY
 
 __docformat__ = 'restructuredtext'
 
 from pyams_portal import _  # pylint: disable=ungrouped-imports
 
 
-CAROUSEL_RENDERER_SETTINGS_KEY = 'pyams_portal.renderer::carousel'
-
-
-class ICarouselPortletRendererSettings(Interface):
-    """Carousel portlet renderer settings interface"""
+class IJumbotronPortletSettings(IPortletSettings):
+    """Jumbotron portlet settings interface"""
 
-    css_class = TextLine(title=_("CSS class"),
-                         description=_("Carousel container CSS class"),
-                         required=False,
-                         default='carousel')
+    title = I18nTextLineField(title=_("Title"),
+                              description=_("Main component title"),
+                              required=True)
 
-    thumb_selection = Choice(title=_("Images selection"),
-                             description=_("Carousel can use responsive selections, but you can "
-                                           "also force selection of another specific selection"),
-                             vocabulary=THUMBNAILERS_VOCABULARY_NAME,
+    lead = I18nTextLineField(title=_("Leading text"),
+                             description=_("Short text to be displayed below title"),
                              required=False)
 
-    automatic_slide = Bool(title=_("Automatic sliding"),
-                           description=_("If 'no', sliding will only be activated manually"),
-                           required=True,
-                           default=True)
-
-    fade_effect = Bool(title=_("Fade effect"),
-                       description=_("If 'yes', slide to slide animation will use a fade effect "
-                                     "instead of lateral sliding"),
-                       required=True,
-                       default=False)
-
-    display_controls = Bool(title=_("Display controls"),
-                            description=_("If 'yes', display arrows to navigate between slides"),
-                            required=True,
-                            default=False)
-
-    display_indicators = Bool(title=_("Display indicators"),
-                              description=_("If 'yes', display indicators to show position of "
-                                            "current slide"),
-                              required=True,
-                              default=False)
-
-    display_captions = Bool(title=_("Display captions"),
-                            description=_("If 'no', slides titles and leads are not displayed"),
-                            required=True,
-                            default=True)
-
-    enable_touch = Bool(title=_("Enable swiping"),
-                        description=_("If 'no', touch events will be disabled on touchscreens"),
-                        required=True,
-                        default=True)
+    display_ruler = Bool(title=_("Display ruler"),
+                         description=_("If 'yes', an horizontal line will be displayed "
+                                       "between leading text and body"),
+                         required=True,
+                         default=True)
+
+    body = I18nTextField(title=_("Body"),
+                         description=_("Main text"),
+                         required=False)
+
+    reference = InternalReferenceField(title=_("Button internal target"),
+                                       description=_("Optional button reference target"),
+                                       required=False)
+
+    target_url = URI(title=_("Button external URI"),
+                     description=_("Alternate URI target used for optional button"),
+                     required=False)
+
+    @invariant
+    def check_target(self):
+        """Check for internal reference or external URL"""
+        if self.reference and self.target_url:
+            raise Invalid(_("You can only set an internal target OR an external URL..."))
+
+    button_label = I18nTextLineField(title=_("Button label"),
+                                     description=_("Optional button label"),
+                                     required=False)
+
+    button_status = Choice(title=_("Button status"),
+                           description=_("Status of optional button"),
+                           vocabulary=BOOTSTRAP_STATUS_VOCABULARY,
+                           default='primary')
```

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/skin/templates/carousel.pt` & `pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/skin/templates/carousel.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/carousel/zmi/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/carousel/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/html/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/html/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/html/interfaces.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/html/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/html/skin/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/html/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/html/zmi/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/html/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/html/zmi/templates/raw-preview.pt` & `pyams_portal-2.3.0/src/pyams_portal/portlets/html/zmi/templates/raw-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/image/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/image/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/image/interfaces.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/image/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/image/skin/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/image/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/image/zmi/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/image/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/image/zmi/templates/image-preview.pt` & `pyams_portal-2.3.0/src/pyams_portal/portlets/image/zmi/templates/image-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/jumbotron/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/jumbotron/skin/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/jumbotron/skin/templates/jumbotron.pt` & `pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/skin/templates/jumbotron.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/jumbotron/zmi/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/jumbotron/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/interfaces.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/skin/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/portlets/spacer/zmi/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/portlets/spacer/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/skin/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/skin/page.py` & `pyams_portal-2.3.0/src/pyams_portal/skin/page.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/skin/templates/layout.pt` & `pyams_portal-2.3.0/src/pyams_portal/skin/templates/layout.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/skin/templates/pagelet.pt` & `pyams_portal-2.3.0/src/pyams_portal/skin/templates/pagelet.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/slot.py` & `pyams_portal-2.3.0/src/pyams_portal/slot.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/template.py` & `pyams_portal-2.3.0/src/pyams_portal/template.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/tests/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/tests/test_image.png` & `pyams_portal-2.3.0/src/pyams_portal/tests/test_image.png`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/tests/test_utilsdocs.py` & `pyams_portal-2.3.0/src/pyams_portal/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/tests/test_utilsdocstrings.py` & `pyams_portal-2.3.0/src/pyams_portal/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/thumbnails.py` & `pyams_portal-2.3.0/src/pyams_portal/thumbnails.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/utils.py` & `pyams_portal-2.3.0/src/pyams_portal/utils.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/__init__.py` & `pyams_portal-2.3.0/src/pyams_portal/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/container.py` & `pyams_portal-2.3.0/src/pyams_portal/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/interfaces.py` & `pyams_portal-2.3.0/src/pyams_portal/zmi/interfaces.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 __docformat__ = 'restructuredtext'
 
 
 from zope.interface import Attribute, Interface
 
-from pyams_form.interfaces.form import IForm
+from pyams_form.interfaces.form import IEditForm, IForm
 
 
 class IPortletConfigurationEditor(Interface):
     """Portlet configuration editor interface"""
 
     settings_factory = Attribute("Editor settings factory interface")
 
@@ -41,7 +41,11 @@
     """Portal context footer presentation menu marker interface"""
 
 
 class IPortalContextPresentationForm(IForm):
     """Portal context presentation form marker interface"""
 
     page_name = Attribute("Portal page name getter")
+
+
+class IPortletRendererSettingsEditForm(IEditForm):
+    """Portlet renderer settings edit form marker interface"""
```

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/layout.py` & `pyams_portal-2.3.0/src/pyams_portal/zmi/layout.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/portlet.py` & `pyams_portal-2.3.0/src/pyams_portal/zmi/portlet.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,27 @@
 from pyramid.renderers import render
 from pyramid.view import view_config
 from zope.component import ComponentLookupError
 from zope.interface import Interface, alsoProvides, implementer
 
 from pyams_form.ajax import AJAXFormRenderer, ajax_form_config
 from pyams_form.field import Fields
+from pyams_form.form import get_form_weight
 from pyams_form.interfaces import HIDDEN_MODE
-from pyams_form.interfaces.form import IAJAXFormRenderer, IFormContent, IGroup, IInnerSubForm
+from pyams_form.interfaces.form import IAJAXFormRenderer, IFormContent, IFormFields, IGroup, IInnerSubForm
 from pyams_form.subform import InnerEditForm
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_portal.interfaces import HIDDEN_RENDERER_NAME, IPortalContext, IPortalPage, IPortalPortletsConfiguration, \
     IPortalTemplate, IPortalTemplateConfiguration, IPortalTemplateContainer, IPortletAddingInfo, IPortletConfiguration, \
     IPortletPreviewer, IPortletRenderer, IPortletRendererSettings, IPortletSettings, IPortletsRenderersThumbnails, \
     MANAGE_TEMPLATE_PERMISSION
 from pyams_portal.page import check_local_template, portal_context_portlets_configuration
 from pyams_portal.portlet import LOGGER
 from pyams_portal.skin import PORTLETS_CACHE_NAME, PORTLETS_CACHE_NAMESPACE, PORTLETS_CACHE_REGION
-from pyams_portal.zmi.interfaces import IPortletConfigurationEditor
+from pyams_portal.zmi.interfaces import IPortletConfigurationEditor, IPortletRendererSettingsEditForm
 from pyams_portal.zmi.widget import RendererSelectFieldWidget
 from pyams_skin.interfaces.view import IModalPage
 from pyams_skin.interfaces.viewlet import IHeaderViewletManager
 from pyams_skin.viewlet.help import AlertMessage
 from pyams_utils.adapter import ContextRequestViewAdapter, adapter_config, get_adapter_weight
 from pyams_utils.cache import get_cache
 from pyams_utils.dict import merge_dict
@@ -471,14 +472,15 @@
 #
 # Portlet renderer settings edit form
 #
 
 @ajax_form_config(name='renderer-settings.html',
                   context=IPortletSettings, layer=IPyAMSLayer,
                   permission=MANAGE_TEMPLATE_PERMISSION)
+@implementer(IPortletRendererSettingsEditForm)
 class PortletRendererSettingsEditForm(AdminModalEditForm):
     """Portlet renderer settings edit form"""
 
     def __init__(self, context, request):
         super().__init__(context, request)
         self.renderer = self.context.get_renderer(request)
 
@@ -490,15 +492,27 @@
 
     legend = _("Renderer settings")
     modal_class = 'modal-xl'
 
     @property
     def fields(self):
         """Form fields getter"""
-        return Fields(self.renderer.settings_interface or Interface)
+        settings = self.get_content()
+        fields = self.request.registry.queryMultiAdapter((settings, self.request, self),
+                                                         IFormFields)
+        if fields is None:
+            fields = Fields(self.renderer.settings_interface or Interface)
+        return fields
+
+    def get_groups(self):
+        settings = self.get_content()
+        registry = self.request.registry
+        yield from sorted((adapter for name, adapter in
+                           registry.getAdapters((settings, self.request, self), IGroup)),
+                          key=get_form_weight)
 
 
 @adapter_config(required=(IPortletSettings, IAdminLayer, PortletRendererSettingsEditForm),
                 provides=IFormContent)
 def get_portlet_renderer_settings_edit_form_content(context, request, form):
     """Portlet renderer settings edit form content getter"""
     return IPortletRendererSettings(context)
```

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/presentation.py` & `pyams_portal-2.3.0/src/pyams_portal/zmi/presentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 from pyramid.events import subscriber
 from zope.interface import Invalid, alsoProvides, implementer
 
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
-from pyams_form.interfaces.form import IDataExtractedEvent, IGroup, IInnerSubForm
+from pyams_form.interfaces.form import IDataExtractedEvent, IFormContent, IGroup, IInnerSubForm
 from pyams_form.subform import InnerEditForm
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_pagelet.pagelet import pagelet_config
 from pyams_portal.interfaces import IPortalContext, IPortalFooterContext, IPortalHeaderContext, \
     IPortalPage, MANAGE_TEMPLATE_PERMISSION
 from pyams_portal.utils import get_portal_page
 from pyams_portal.zmi.interfaces import IPortalContextPresentationForm, \
@@ -83,18 +83,14 @@
 
     def __init__(self, context, request):
         super().__init__(context, request)
         page = self.get_content()
         if not page.can_inherit:
             alsoProvides(self, IPortalContextPresentationForm)
 
-    def get_content(self):
-        """Form content getter"""
-        return get_portal_page(self.context, page_name=self.page_name)
-
     def apply_changes(self, data):
         page = self.get_content()
         params = self.request.params
         override = True
         if page.can_inherit:
             override = params.get(
                 '{}{}override_parent'.format(self.prefix, self.widgets.prefix))
@@ -113,14 +109,21 @@
                     template.css_class = params.get(
                         '{}{}css_class'.format(self.prefix, self.widgets.prefix))
         return {
             IPortalPage: ('inherit_parent', 'use_local_template', 'shared_template')
         }
 
 
+@adapter_config(required=(IPortalContext, IPyAMSLayer, PortalContextPresentationEditForm),
+                provides=IFormContent)
+def portal_context_presentation_form_content(context, request, form):
+    """Portal context presentation edit form content getter"""
+    return get_portal_page(context, page_name=form.page_name)
+
+
 #
 # Header presentation
 #
 
 @viewletmanager_config(name='header-presentation.menu',
                        context=IPortalHeaderContext, layer=IAdminLayer,
                        manager=IPortalContextPresentationMenu, weight=20,
@@ -228,17 +231,14 @@
                 provides=IInnerSubForm)
 @template_config(template='templates/presentation-template.pt', layer=IAdminLayer)
 class PortalContextPresentationTemplateEditForm(InnerEditForm):
     """Portal context presentation template edit form"""
 
     fields = Fields(IPortalPage).select('shared_template')
 
-    def get_content(self):
-        return self.parent_form.get_content()
-
     @property
     def template_css_class(self):
         """Template CSS class getter"""
         result = None
         page = self.get_content()
         template = page.local_template
         if template is not None:
@@ -254,14 +254,21 @@
             template.placeholder = _("Please select template...")
             template.object_data = {
                 'ams-change-handler': 'MyAMS.portal.presentation.setSharedTemplate'
             }
             alsoProvides(template, IObjectData)
 
 
+@adapter_config(required=(IPortalContext, IPyAMSLayer, PortalContextPresentationTemplateEditForm),
+                provides=IFormContent)
+def portal_context_presentation_template_form_content(context, request, form):
+    """Portal context presentation template form content getter"""
+    return form.parent_form.get_content()
+
+
 @viewlet_config(name='presentation-template.help',
                 context=IPortalContext, layer=IAdminLayer,
                 view=PortalContextPresentationEditForm, manager=IHelpViewletManager, weight=10)
 class PortalContextPresentationEditFormHelp(AlertMessage):
     """Portal context presentation edit form help"""
 
     status = 'info'
```

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/resources/css/layout.css` & `pyams_portal-2.3.0/src/pyams_portal/zmi/resources/css/layout.css`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/resources/css/layout.min.css` & `pyams_portal-2.3.0/src/pyams_portal/zmi/resources/css/layout.min.css`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/resources/js/layout.js` & `pyams_portal-2.3.0/src/pyams_portal/zmi/resources/js/layout.js`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/resources/js/layout.min.js` & `pyams_portal-2.3.0/src/pyams_portal/zmi/resources/js/layout.min.js`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/resources/sass/layout.scss` & `pyams_portal-2.3.0/src/pyams_portal/zmi/resources/sass/layout.scss`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/slot.py` & `pyams_portal-2.3.0/src/pyams_portal/zmi/slot.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pyramid.events import subscriber
 from pyramid.view import view_config
 from zope.interface import Interface, Invalid, alsoProvides
 
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
 from pyams_form.interfaces import HIDDEN_MODE
-from pyams_form.interfaces.form import IAJAXFormRenderer, IDataExtractedEvent, IGroup
+from pyams_form.interfaces.form import IAJAXFormRenderer, IDataExtractedEvent, IFormContent, IGroup
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_portal.interfaces import IPortalPage, IPortalTemplate, \
     IPortalTemplateConfiguration, IPortalTemplateContainer, ISlot, ISlotConfiguration, \
     MANAGE_TEMPLATE_PERMISSION
 from pyams_portal.page import check_local_template
 from pyams_utils.adapter import ContextRequestViewAdapter, adapter_config
 from pyams_utils.interfaces.data import IObjectData
@@ -187,30 +187,35 @@
     fields = Fields(ISlotConfiguration).omit('visible', 'portlet_ids', 'prefix', 'suffix')
 
     def __init__(self, context, request):
         check_local_template(context)
         super().__init__(context, request)
         self.config = IPortalTemplateConfiguration(self.context)
 
-    def get_content(self):
-        """Content getter"""
-        slot_name = self.request.params.get('{0}widgets.slot_name'.format(self.prefix))
-        return self.config.slot_config[slot_name]
-
     def update_widgets(self, prefix=None):
         super().update_widgets(prefix)
         slot_name = self.widgets.get('slot_name')
         if slot_name is not None:
             slot_name.mode = HIDDEN_MODE
         for name in ('container_css_class', 'css_class', 'portlets_css_class'):
             widget = self.widgets.get(name)
             if widget is not None:
                 widget.input_css_class = 'col-sm-6'
 
 
+@adapter_config(required=(IPortalTemplate, IAdminLayer, PortalTemplateSlotPropertiesEditForm),
+                provides=IFormContent)
+@adapter_config(required=(IPortalPage, IAdminLayer, PortalTemplateSlotPropertiesEditForm),
+                provides=IFormContent)
+def portal_template_slot_properties_edit_form_content(context, request, form):
+    """Portal template slot properties edit form content getter"""
+    slot_name = request.params.get('{0}widgets.slot_name'.format(form.prefix))
+    return form.config.slot_config[slot_name]
+
+
 @adapter_config(name='html-codes',
                 required=(Interface, IAdminLayer, PortalTemplateSlotPropertiesEditForm),
                 provides=IGroup)
 class PortalTemplateSlotPropertiesHTMLCodes(FormGroupSwitcher):
     """Portal template slot properties HTML codes"""
 
     legend = _("HTML codes")
```

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/template.py` & `pyams_portal-2.3.0/src/pyams_portal/zmi/template.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/templates/layout.pt` & `pyams_portal-2.3.0/src/pyams_portal/zmi/templates/layout.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/templates/portlet-preview.pt` & `pyams_portal-2.3.0/src/pyams_portal/zmi/templates/portlet-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/templates/presentation-template.pt` & `pyams_portal-2.3.0/src/pyams_portal/zmi/templates/presentation-template.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/templates/renderer-input.pt` & `pyams_portal-2.3.0/src/pyams_portal/zmi/templates/renderer-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/templates/thumbnails-widget.pt` & `pyams_portal-2.3.0/src/pyams_portal/zmi/templates/thumbnails-widget.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/thumbnails.py` & `pyams_portal-2.3.0/src/pyams_portal/zmi/thumbnails.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal/zmi/widget.py` & `pyams_portal-2.3.0/src/pyams_portal/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-2.2.3/src/pyams_portal.egg-info/PKG-INFO` & `pyams_portal-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams-portal
-Version: 2.2.3
+Name: pyams_portal
+Version: 2.3.0
 Summary: PyAMS portlets management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -52,14 +52,20 @@
 content management packages like PyAMS_content, while other extension packages can be used to
 provide custom portlets renderers.
 
 
 Changelog
 =========
 
+2.3.0
+-----
+ - updated cards portlet thumbnails selection field
+ - updated portlet renderer settings edit form fields and groups getters
+ - added edit forms content getters
+
 2.2.3
 -----
  - corrected doctest
 
 2.2.2
 -----
  - updated portlets cache key to include page name (which may be required when
```

### Comparing `pyams_portal-2.2.3/src/pyams_portal.egg-info/SOURCES.txt` & `pyams_portal-2.3.0/src/pyams_portal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

