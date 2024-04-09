# Comparing `tmp/pyams_content-1.99.0.tar.gz` & `tmp/pyams_content-1.99.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_content-1.99.0.tar", last modified: Mon Feb 26 23:15:43 2024, max compression
+gzip compressed data, was "dist/pyams_content-1.99.1.tar", last modified: Tue Apr  9 20:48:29 2024, max compression
```

## Comparing `pyams_content-1.99.0.tar` & `pyams_content-1.99.1.tar`

### file list

```diff
@@ -1,634 +1,659 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-02-26 23:15:06.000000 pyams_content-1.99.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-26 23:15:06.000000 pyams_content-1.99.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1897 2024-02-26 23:15:43.000000 pyams_content-1.99.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/docs/
--rwxrwxrwx   0 root         (0) root         (0)       64 2024-02-26 23:15:06.000000 pyams_content-1.99.0/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-02-26 23:15:06.000000 pyams_content-1.99.0/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-26 23:15:43.000000 pyams_content-1.99.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3368 2024-02-26 23:15:06.000000 pyams_content-1.99.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/
--rw-rw-rw-   0 root         (0) root         (0)      865 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/association/
--rw-rw-rw-   0 root         (0) root         (0)     3402 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/association/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4072 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/association/container.py
--rw-rw-rw-   0 root         (0) root         (0)     3230 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/association/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2091 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/association/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/association/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2162 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/association/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1514 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/association/skin/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/association/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/association/skin/templates/association-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1960 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/association/skin/templates/association-viewlet.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/association/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     5882 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/association/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8776 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/association/zmi/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1238 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/association/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2039 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/association/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/calendar/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/calendar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/cards/
--rw-rw-rw-   0 root         (0) root         (0)     1679 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/cards/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/cards/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/cards/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2619 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/cards/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1148 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/cards/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/cards/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/cards/skin/templates/cards-masonry.pt
--rw-rw-rw-   0 root         (0) root         (0)     1773 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/cards/skin/templates/cards.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/cards/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2094 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/cards/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/contact/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/contact/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/extfile/
--rw-rw-rw-   0 root         (0) root         (0)     7387 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/extfile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4426 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/extfile/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/extfile/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     9775 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2159 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3254 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1213 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     2798 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/fields/
--rw-rw-rw-   0 root         (0) root         (0)      571 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/fields/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/fields/handler/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/fields/handler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3504 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/fields/handler/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     5218 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/fields/handler/mail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/fields/handler/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/fields/handler/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2497 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/fields/handler/zmi/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/fields/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1814 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/fields/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/fields/skin/
--rw-rw-rw-   0 root         (0) root         (0)      576 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/fields/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4340 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/fields/skin/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/fields/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      220 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/fields/skin/templates/form-submit.pt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/fields/skin/templates/paragraph-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/fields/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      575 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/fields/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2100 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/fields/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/file/
--rw-rw-rw-   0 root         (0) root         (0)     1583 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/file/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/frame/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/frame/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/frame/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/
--rw-rw-rw-   0 root         (0) root         (0)     6052 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4672 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/file.py
--rw-rw-rw-   0 root         (0) root         (0)     5094 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     1661 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     4655 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2175 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt
--rw-rw-rw-   0 root         (0) root         (0)     2954 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1242 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/zmi/templates/gallery-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/skin/
--rw-rw-rw-   0 root         (0) root         (0)     4053 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2120 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt
--rw-rw-rw-   0 root         (0) root         (0)     2891 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/skin/templates/gallery-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1185 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/skin/templates/gallery-random.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8399 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11894 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/file.py
--rw-rw-rw-   0 root         (0) root         (0)     1995 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1498 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt
--rw-rw-rw-   0 root         (0) root         (0)      961 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/
--rw-rw-rw-   0 root         (0) root         (0)     7780 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4725 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2005 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     1396 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1118 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6710 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2989 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1390 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     2530 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1328 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/zmi/templates/illustration-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/skin/
--rw-rw-rw-   0 root         (0) root         (0)     5098 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4472 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/skin/illustration.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/skin/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2087 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/skin/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      914 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/skin/templates/illustration-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     2388 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/skin/templates/illustration-side.pt
--rw-rw-rw-   0 root         (0) root         (0)      914 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1291 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4644 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5286 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/zmi/paragraph.py
--rw-rw-rw-   0 root         (0) root         (0)     1652 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/illustration/zmi/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/keynumber/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/keynumber/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/links/
--rw-rw-rw-   0 root         (0) root         (0)    10891 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/links/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4819 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/links/html.py
--rw-rw-rw-   0 root         (0) root         (0)     5037 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/links/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/links/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8653 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/links/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/links/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2658 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/links/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/map/
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/map/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/milestone/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/milestone/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/
--rw-rw-rw-   0 root         (0) root         (0)     6756 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5621 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/container.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     5077 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2114 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/interfaces/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     4693 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5340 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     7591 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1622 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt
--rw-rw-rw-   0 root         (0) root         (0)      532 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4105 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      606 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/zmi/templates/navigation-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     1794 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7323 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/skin/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/skin/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/skin/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2456 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/skin/interfaces/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      899 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/skin/templates/html.pt
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/skin/templates/raw-code.pt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/skin/templates/raw.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    17744 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17906 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/zmi/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/zmi/helper.py
--rw-rw-rw-   0 root         (0) root         (0)     4263 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/zmi/html.py
--rw-rw-rw-   0 root         (0) root         (0)     1494 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/paragraph/zmi/templates/title-toolbar.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/pictogram/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/pictogram/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/thesaurus/
--rw-rw-rw-   0 root         (0) root         (0)     7603 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/thesaurus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3500 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/thesaurus/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/thesaurus/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2699 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/thesaurus/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/thesaurus/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/thesaurus/skin/templates/tags.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/thesaurus/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    12144 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/thesaurus/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/thesaurus/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     5777 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/thesaurus/zmi/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/verbatim/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/verbatim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/video/
--rw-rw-rw-   0 root         (0) root         (0)     2307 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2937 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1971 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/video/provider/
--rw-rw-rw-   0 root         (0) root         (0)     2984 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/provider/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3286 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/provider/dailymotion.py
--rw-rw-rw-   0 root         (0) root         (0)     9322 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/provider/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2895 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/provider/vimeo.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/provider/youtube.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/video/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2151 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/video/skin/provider/
--rw-rw-rw-   0 root         (0) root         (0)     2159 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/skin/provider/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1737 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/skin/provider/dailymotion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/video/skin/provider/templates/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/skin/provider/templates/custom-render.pt
--rw-rw-rw-   0 root         (0) root         (0)      450 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/skin/provider/templates/dailymotion-render.pt
--rw-rw-rw-   0 root         (0) root         (0)      542 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt
--rw-rw-rw-   0 root         (0) root         (0)      387 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/skin/provider/templates/youtube-render.pt
--rw-rw-rw-   0 root         (0) root         (0)     1503 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/skin/provider/vimeo.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/skin/provider/youtube.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/video/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/skin/templates/video-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/component/video/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      574 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12014 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/component/video/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/doctests/
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/
--rw-rw-rw-   0 root         (0) root         (0)      567 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/alert/
--rw-rw-rw-   0 root         (0) root         (0)     3608 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/alert/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2151 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/alert/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/alert/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2127 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/alert/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/alert/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1882 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/alert/skin/templates/alerts.pt
--rw-rw-rw-   0 root         (0) root         (0)     1098 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/alert/skin/templates/context-alerts.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/alert/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1947 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/alert/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/audit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/audit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/
--rw-rw-rw-   0 root         (0) root         (0)     2343 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6737 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1803 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/sitemap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      406 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/templates/glossary-sitemap.pt
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/templates/glossary.pt
--rw-rw-rw-   0 root         (0) root         (0)     1731 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/templates/term-associations.pt
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/templates/term-body.pt
--rw-rw-rw-   0 root         (0) root         (0)      306 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/templates/term-footer.pt
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/templates/term-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      767 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/templates/term-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     3568 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/term.py
--rw-rw-rw-   0 root         (0) root         (0)     3180 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     3093 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/glossary/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/history/
--rw-rw-rw-   0 root         (0) root         (0)     3000 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/history/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2286 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/history/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/history/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      574 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/history/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/history/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/history/zmi/templates/history.pt
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/history/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/html/
--rw-rw-rw-   0 root         (0) root         (0)     3125 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/html/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/
--rw-rw-rw-   0 root         (0) root         (0)     6800 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4435 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     3392 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3551 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1441 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2154 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1339 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     3353 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1301 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      553 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     7353 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/zmi/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/navigation/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/preview/
--rw-rw-rw-   0 root         (0) root         (0)      570 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/preview/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/preview/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/preview/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2670 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/preview/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/preview/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      738 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/qrcode/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/qrcode/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/redirect/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/redirect/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/renderer/
--rw-rw-rw-   0 root         (0) root         (0)     5451 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/renderer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1662 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/renderer/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/review/
--rw-rw-rw-   0 root         (0) root         (0)     4326 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/review/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3253 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/review/chat.py
--rw-rw-rw-   0 root         (0) root         (0)     3206 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/review/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4664 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/review/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/review/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    11050 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/review/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/review/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/review/zmi/templates/comment.pt
--rw-rw-rw-   0 root         (0) root         (0)     2784 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/review/zmi/templates/comments.pt
--rw-rw-rw-   0 root         (0) root         (0)     1787 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/review/zmi/templates/mail-notification.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/search/
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7373 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/search/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3804 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/search/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4276 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/search/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/search/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/search/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3101 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/search/zmi/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/share/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/share/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/sitemap/
--rw-rw-rw-   0 root         (0) root         (0)     4558 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/sitemap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      796 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/sitemap/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/sitemap/templates/
--rw-rw-rw-   0 root         (0) root         (0)      299 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/sitemap/templates/humans.pt
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/sitemap/templates/robots.pt
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/sitemap/templates/root-sitemap.pt
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/sitemap/templates/tool-sitemap.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/feature/toolbox/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/feature/toolbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/generations/
--rw-rw-rw-   0 root         (0) root         (0)    10545 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8956 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/include.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     4405 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)   120378 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo
--rw-rw-rw-   0 root         (0) root         (0)   212198 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po
--rw-rw-rw-   0 root         (0) root         (0)   152300 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/locales/pyams_content.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/reference/
--rw-rw-rw-   0 root         (0) root         (0)     2851 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/
--rw-rw-rw-   0 root         (0) root         (0)     2577 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2797 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2917 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     6729 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3473 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/templates/pictogram-header.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/widget/
--rw-rw-rw-   0 root         (0) root         (0)     2896 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2831 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/widget/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/widget/templates/
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/widget/templates/selection-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     3174 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/reference/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1938 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4333 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/zmi/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/reference/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/reference/zmi/viewlet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/root/
--rw-rw-rw-   0 root         (0) root         (0)     4904 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/root/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6721 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/root/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     4841 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/root/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/root/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     3669 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/root/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25806 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/root/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)    13639 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/root/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     5338 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/root/zmi/sites.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/
--rw-rw-rw-   0 root         (0) root         (0)      561 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/alert/
--rw-rw-rw-   0 root         (0) root         (0)     2612 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/alert/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4195 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/alert/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2824 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/alert/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/alert/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2280 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/alert/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/blog/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/blog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/calendar/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/calendar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/common/
--rw-rw-rw-   0 root         (0) root         (0)    10980 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/common/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)    15315 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5998 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/interfaces/types.py
--rw-rw-rw-   0 root         (0) root         (0)     3368 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2786 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/
--rw-rw-rw-   0 root         (0) root         (0)      637 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2282 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/header.py
--rw-rw-rw-   0 root         (0) root         (0)     5197 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)      645 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1762 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/skin/header.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/skin/specificities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2618 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/skin/templates/specificities-default.pt
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/skin/templates/title-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/skin/title.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/specificities.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/title.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      658 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1386 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/zmi/header.py
--rw-rw-rw-   0 root         (0) root         (0)     1435 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/zmi/specificities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      644 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/zmi/templates/specificities-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/zmi/templates/title-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     1369 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/portlet/zmi/title.py
--rw-rw-rw-   0 root         (0) root         (0)     9807 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/restrictions.py
--rw-rw-rw-   0 root         (0) root         (0)     3878 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/security.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/common/skin/
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2333 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/skin/breadcrumb.py
--rw-rw-rw-   0 root         (0) root         (0)     5128 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/skin/oid.py
--rw-rw-rw-   0 root         (0) root         (0)     1765 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/skin/specificities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/common/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      201 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/skin/templates/breadcrumbs.pt
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/skin/templates/card-datatype.pt
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/skin/templates/publication-date.pt
--rw-rw-rw-   0 root         (0) root         (0)     1727 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/skin/title.py
--rw-rw-rw-   0 root         (0) root         (0)     2556 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/skin/types.py
--rw-rw-rw-   0 root         (0) root         (0)     4801 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/skin/url.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/skin/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)    12425 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    23132 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14617 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/content.py
--rw-rw-rw-   0 root         (0) root         (0)    36824 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)     3872 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/header.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4679 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)    18561 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/owner.py
--rw-rw-rw-   0 root         (0) root         (0)     3030 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/portal.py
--rw-rw-rw-   0 root         (0) root         (0)     2899 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/reference.py
--rw-rw-rw-   0 root         (0) root         (0)    18375 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/restrictions.py
--rw-rw-rw-   0 root         (0) root         (0)    17565 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     8992 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/templates/content-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/templates/content-workflow.pt
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/templates/owner-change.pt
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/templates/quick-search.pt
--rw-rw-rw-   0 root         (0) root         (0)      193 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/templates/sequence-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      608 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/types/
--rw-rw-rw-   0 root         (0) root         (0)     7223 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5005 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/types/container.py
--rw-rw-rw-   0 root         (0) root         (0)     2255 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/types/content.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/types/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)     3179 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/viewlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29957 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/common/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/file/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/file/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/form/
--rw-rw-rw-   0 root         (0) root         (0)     2560 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/form/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/form/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/form/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/form/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2046 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/form/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/form/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2195 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/form/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/hub/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/hub/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/logo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/logo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/logo/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1149 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/logo/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/news/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/news/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/resource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/resource/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/site/
--rw-rw-rw-   0 root         (0) root         (0)      610 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4564 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/container.py
--rw-rw-rw-   0 root         (0) root         (0)     5188 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     8784 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     7205 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/link.py
--rw-rw-rw-   0 root         (0) root         (0)     5429 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2845 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/topic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8526 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/folder.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    15922 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/link.py
--rw-rw-rw-   0 root         (0) root         (0)     8144 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     5391 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/rename.py
--rw-rw-rw-   0 root         (0) root         (0)     2689 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     5002 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/topic.py
--rw-rw-rw-   0 root         (0) root         (0)    21405 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/tree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)     1899 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/viewlet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/widget/
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1301 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/widget/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/widget/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/widget/templates/
--rw-rw-rw-   0 root         (0) root         (0)      924 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/topic/
--rw-rw-rw-   0 root         (0) root         (0)     2195 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/topic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1460 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/topic/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/topic/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/topic/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1737 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/topic/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/view/
--rw-rw-rw-   0 root         (0) root         (0)     8652 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/view/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     7639 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2760 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/interfaces/query.py
--rw-rw-rw-   0 root         (0) root         (0)     5853 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/interfaces/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     6223 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/merge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/view/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     4700 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5886 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/view/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6693 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6314 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/view/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1103 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt
--rw-rw-rw-   0 root         (0) root         (0)     3824 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt
--rw-rw-rw-   0 root         (0) root         (0)     2579 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/view/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1287 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/view/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     6586 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/query.py
--rw-rw-rw-   0 root         (0) root         (0)     6661 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/reference.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/view/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1398 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/view/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/skin/templates/preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     7845 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/shared/view/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4191 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/zmi/references.py
--rw-rw-rw-   0 root         (0) root         (0)     5706 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/shared/view/zmi/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/skin/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1873 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/tests/
--rw-rw-rw-   0 root         (0) root         (0)      802 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1864 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/workflow/
--rw-rw-rw-   0 root         (0) root         (0)    43555 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/workflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21211 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/workflow/basic.py
--rw-rw-rw-   0 root         (0) root         (0)     1227 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/workflow/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4984 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/workflow/notify.py
--rw-rw-rw-   0 root         (0) root         (0)     6272 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/workflow/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/workflow/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/workflow/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3222 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/workflow/zmi/publication.py
--rw-rw-rw-   0 root         (0) root         (0)     1139 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/workflow/zmi/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/workflow/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/workflow/zmi/templates/publication-header.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      777 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7680 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)     2383 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/html.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/properties.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/zmi/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)    19424 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/resources/js/content.js
--rw-rw-rw-   0 root         (0) root         (0)    10283 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/resources/js/content.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content/zmi/resources/js/tinymce/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/zmi/resources/js/tinymce/headers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/zmi/resources/js/tinymce/headers/langs/
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/resources/js/tinymce/headers/langs/fr.js
--rw-rw-rw-   0 root         (0) root         (0)     2115 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/zmi/resources/js/tinymce/internal-link/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/
--rw-rw-rw-   0 root         (0) root         (0)      607 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js
--rw-rw-rw-   0 root         (0) root         (0)     5919 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)      566 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/viewlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/viewlet/toplinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/zmi/widget/
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/widget/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2450 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/widget/seo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:43.000000 pyams_content-1.99.0/src/pyams_content/zmi/widget/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1260 2024-02-26 23:15:06.000000 pyams_content-1.99.0/src/pyams_content/zmi/widget/templates/seo-textline-input.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1897 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    23410 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 23:15:31.000000 pyams_content-1.99.0/src/pyams_content.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      625 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-02-26 23:15:42.000000 pyams_content-1.99.0/src/pyams_content.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-02-26 23:15:27.000000 pyams_content-1.99.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-26 23:15:27.000000 pyams_content-1.99.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2079 2024-04-09 20:48:29.000000 pyams_content-1.99.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/docs/
+-rwxrwxrwx   0 root         (0) root         (0)      246 2024-04-09 20:44:10.000000 pyams_content-1.99.1/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-02-26 23:15:27.000000 pyams_content-1.99.1/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 20:48:29.000000 pyams_content-1.99.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3377 2024-04-09 20:44:10.000000 pyams_content-1.99.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/
+-rw-rw-rw-   0 root         (0) root         (0)      865 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/association/
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4072 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     3230 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2091 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/association/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1514 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/skin/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/association/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/skin/templates/association-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1960 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/skin/templates/association-viewlet.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/association/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     5882 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8776 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/zmi/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2039 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/calendar/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/calendar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/cards/
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/cards/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/cards/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/cards/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2619 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/cards/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/cards/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/cards/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/cards/skin/templates/cards-masonry.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1773 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/cards/skin/templates/cards.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/cards/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/cards/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/contact/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/component/contact/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/
+-rw-rw-rw-   0 root         (0) root         (0)     7387 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4426 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     9775 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2467 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3254 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2798 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/fields/
+-rw-rw-rw-   0 root         (0) root         (0)      571 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/fields/handler/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/handler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3504 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/handler/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     5218 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/handler/mail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/fields/handler/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/handler/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/component/fields/handler/zmi/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/fields/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      576 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4340 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/skin/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/fields/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      220 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/skin/templates/form-submit.pt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/skin/templates/paragraph-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/fields/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/file/
+-rw-rw-rw-   0 root         (0) root         (0)     1583 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/file/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/frame/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/component/frame/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/frame/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/
+-rw-rw-rw-   0 root         (0) root         (0)     6052 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4672 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5094 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1661 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     4654 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2954 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/zmi/templates/gallery-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     4053 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2120 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2891 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/skin/templates/gallery-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/skin/templates/gallery-random.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8399 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11894 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1995 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1498 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/
+-rw-rw-rw-   0 root         (0) root         (0)     7780 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4725 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2005 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6710 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2989 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1390 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/zmi/templates/illustration-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     5098 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4472 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/illustration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2087 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/templates/illustration-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/templates/illustration-side.pt
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     5108 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5143 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/zmi/paragraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     1989 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/zmi/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/keynumber/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/keynumber/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/links/
+-rw-rw-rw-   0 root         (0) root         (0)    10891 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/links/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4819 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/links/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     5037 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/links/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/links/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8653 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/links/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/links/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2658 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/links/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/map/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/map/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/milestone/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/milestone/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/
+-rw-rw-rw-   0 root         (0) root         (0)     6756 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5621 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     5077 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/interfaces/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     4693 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5340 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     7591 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)      532 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     4105 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      606 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/zmi/templates/navigation-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7323 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2456 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/interfaces/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      899 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/templates/html.pt
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/templates/raw-code.pt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/templates/raw.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    17744 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17906 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     4263 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     1494 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/templates/title-toolbar.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/pictogram/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/component/pictogram/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/
+-rw-rw-rw-   0 root         (0) root         (0)     7603 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3500 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2699 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/skin/templates/tags.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    12144 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     6509 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/zmi/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/verbatim/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/component/verbatim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/video/
+-rw-rw-rw-   0 root         (0) root         (0)     2307 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1971 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/video/provider/
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/provider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3286 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/provider/dailymotion.py
+-rw-rw-rw-   0 root         (0) root         (0)     9322 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/provider/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2895 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/provider/vimeo.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/provider/youtube.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/
+-rw-rw-rw-   0 root         (0) root         (0)     2159 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/dailymotion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/templates/custom-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)      450 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/templates/dailymotion-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)      542 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)      387 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/templates/youtube-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/vimeo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/youtube.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/templates/video-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/video/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12014 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/
+-rw-rw-rw-   0 root         (0) root         (0)     3608 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2142 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/skin/templates/alerts.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/skin/templates/context-alerts.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2205 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/audit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/feature/audit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6737 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1803 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/sitemap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      406 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/glossary-sitemap.pt
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/glossary.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-associations.pt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-body.pt
+-rw-rw-rw-   0 root         (0) root         (0)      306 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-footer.pt
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3568 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/term.py
+-rw-rw-rw-   0 root         (0) root         (0)     3180 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/history/
+-rw-rw-rw-   0 root         (0) root         (0)     3000 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/history/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2286 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/history/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/history/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/history/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/history/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/history/zmi/templates/history.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/history/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/html/
+-rw-rw-rw-   0 root         (0) root         (0)     3125 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/html/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/
+-rw-rw-rw-   0 root         (0) root         (0)     6800 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4435 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     3392 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     3551 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2154 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3353 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      553 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     7353 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/zmi/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/preview/
+-rw-rw-rw-   0 root         (0) root         (0)      570 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/preview/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/preview/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/preview/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2670 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/preview/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/preview/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      738 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/qrcode/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/feature/qrcode/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/redirect/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/feature/redirect/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/renderer/
+-rw-rw-rw-   0 root         (0) root         (0)     5451 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/renderer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/renderer/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/review/
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3253 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/chat.py
+-rw-rw-rw-   0 root         (0) root         (0)     3206 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4664 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/review/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    11050 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/review/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/zmi/templates/comment.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2784 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/zmi/templates/comments.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1787 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/zmi/templates/mail-notification.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/search/
+-rw-rw-rw-   0 root         (0) root         (0)     3169 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7419 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3804 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/search/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     4825 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2527 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)    11035 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6230 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-card.pt
+-rw-rw-rw-   0 root         (0) root         (0)     5146 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt
+-rw-rw-rw-   0 root         (0) root         (0)     5176 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4985 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-panel.pt
+-rw-rw-rw-   0 root         (0) root         (0)     5184 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-result.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4002 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/zmi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      708 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4276 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/search/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/search/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     7625 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/search/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/zmi/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/zmi/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/share/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/feature/share/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/
+-rw-rw-rw-   0 root         (0) root         (0)     4558 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      796 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      299 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/templates/humans.pt
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/templates/robots.pt
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/templates/root-sitemap.pt
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/templates/tool-sitemap.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/toolbox/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/feature/toolbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/generations/
+-rw-rw-rw-   0 root         (0) root         (0)    10545 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8956 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/include.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     4405 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)   124539 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo
+-rw-rw-rw-   0 root         (0) root         (0)   223765 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po
+-rw-rw-rw-   0 root         (0) root         (0)   161700 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/locales/pyams_content.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/
+-rw-rw-rw-   0 root         (0) root         (0)     2851 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2917 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     6729 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3473 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/templates/pictogram-header.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/
+-rw-rw-rw-   0 root         (0) root         (0)     2896 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2831 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/templates/selection-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3174 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4333 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/zmi/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/zmi/viewlet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/root/
+-rw-rw-rw-   0 root         (0) root         (0)     4904 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/root/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6721 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/root/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4841 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/root/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/root/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3885 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/root/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25806 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/root/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)    13639 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/root/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     5338 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/root/zmi/sites.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/
+-rw-rw-rw-   0 root         (0) root         (0)      561 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5270 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2824 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4288 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3268 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     9134 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/zmi/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/blog/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/blog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/calendar/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/calendar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/
+-rw-rw-rw-   0 root         (0) root         (0)    11763 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)    15461 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/common/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5998 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/interfaces/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3368 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2282 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     5197 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1762 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/specificities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2618 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/templates/specificities-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/templates/title-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/title.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/specificities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1796 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/title.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      658 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1435 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/specificities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/templates/specificities-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/templates/title-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/title.py
+-rw-rw-rw-   0 root         (0) root         (0)     9807 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/restrictions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3878 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/security.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2333 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/breadcrumb.py
+-rw-rw-rw-   0 root         (0) root         (0)     5128 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/oid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/specificities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      201 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/templates/breadcrumbs.pt
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/templates/card-datatype.pt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/templates/publication-date.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/title.py
+-rw-rw-rw-   0 root         (0) root         (0)     2556 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     4801 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)    12425 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    23132 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14620 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/content.py
+-rw-rw-rw-   0 root         (0) root         (0)    36824 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3872 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4679 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    18561 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/owner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3030 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/portal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2899 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)    18640 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/restrictions.py
+-rw-rw-rw-   0 root         (0) root         (0)    17565 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     8992 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/content-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/content-workflow.pt
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/owner-change.pt
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/quick-search.pt
+-rw-rw-rw-   0 root         (0) root         (0)      193 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/sequence-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/
+-rw-rw-rw-   0 root         (0) root         (0)     7226 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5005 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     2605 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/content.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)     3179 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/viewlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29957 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/file/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/file/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/form/
+-rw-rw-rw-   0 root         (0) root         (0)     2560 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/form/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/form/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/form/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/form/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2046 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/form/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/form/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/form/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/hub/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/hub/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/logo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/shared/logo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/logo/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1149 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/logo/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/news/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/shared/news/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/shared/resource/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/site/
+-rw-rw-rw-   0 root         (0) root         (0)      610 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4564 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     5188 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8784 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     7205 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/link.py
+-rw-rw-rw-   0 root         (0) root         (0)     5429 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/topic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8526 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    15922 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/link.py
+-rw-rw-rw-   0 root         (0) root         (0)     8144 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5391 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/rename.py
+-rw-rw-rw-   0 root         (0) root         (0)     2689 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     5002 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/topic.py
+-rw-rw-rw-   0 root         (0) root         (0)    21405 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/tree.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/viewlet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      924 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/topic/
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/topic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/topic/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/topic/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/topic/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/topic/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/
+-rw-rw-rw-   0 root         (0) root         (0)     8677 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     7663 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/interfaces/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     5853 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/interfaces/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     6223 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/merge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     4700 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5886 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6787 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2449 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/zmi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     6586 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     6661 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/reference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/skin/templates/preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     7845 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     4191 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/zmi/references.py
+-rw-rw-rw-   0 root         (0) root         (0)     6188 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/zmi/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/workflow/
+-rw-rw-rw-   0 root         (0) root         (0)    43555 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21211 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/basic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4984 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/notify.py
+-rw-rw-rw-   0 root         (0) root         (0)     6272 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/workflow/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/zmi/publication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/zmi/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/workflow/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/zmi/templates/publication-header.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      777 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7680 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)     2383 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/properties.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)    19424 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/content.js
+-rw-rw-rw-   0 root         (0) root         (0)    10283 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/content.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/headers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/headers/langs/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/headers/langs/fr.js
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/internal-link/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)      566 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/viewlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/viewlet/toplinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/widget/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/widget/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/widget/seo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/widget/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/widget/templates/seo-textline-input.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2079 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24617 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:48:17.000000 pyams_content-1.99.1/src/pyams_content.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      632 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/top_level.txt
```

### Comparing `pyams_content-1.99.0/LICENSE` & `pyams_content-1.99.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/PKG-INFO` & `pyams_content-1.99.1/src/pyams_content.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams_content
-Version: 1.99.0
+Name: pyams-content
+Version: 1.99.1
 Summary: PyAMS content management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS CMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -48,10 +48,17 @@
 Please note that PyAMS_content only provide a basic Bootstrap based skin, so you will have to
 include other extension packages (like PyAMS_content_themes) to get more advanced graphical themes.
 
 
 Changelog
 =========
 
+1.99.1
+------
+ - added edit forms content getters
+ - added alerts types
+ - added vocabulary to handle shared contents which can be used by views and search folders
+ - minor updates
+
 1.99.0
 ------
  - first preliminary release
```

### Comparing `pyams_content-1.99.0/docs/README.rst` & `pyams_content-1.99.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/setup.py` & `pyams_content-1.99.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.99.0'
+version = '1.99.1'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_security_views',
     'pyams_zmi',
     'pyramid_zcml',
     'zope.exceptions'
@@ -65,15 +65,15 @@
           # -*- Extra requirements: -*-
           'fanstatic',
           'hypatia',
           'persistent',
           'pyams_catalog',
           'pyams_fields',
           'pyams_file',
-          'pyams_form',
+          'pyams_form >= 2.1.0',
           'pyams_i18n',
           'pyams_i18n_views',
           'pyams_layer',
           'pyams_mail',
           'pyams_pagelet',
           'pyams_portal',
           'pyams_scheduler',
```

### Comparing `pyams_content-1.99.0/src/pyams_content/__init__.py` & `pyams_content-1.99.1/src/pyams_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/association/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/association/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/association/container.py` & `pyams_content-1.99.1/src/pyams_content/component/association/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/association/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/association/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/association/paragraph.py` & `pyams_content-1.99.1/src/pyams_content/component/association/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/association/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/association/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/association/skin/paragraph.py` & `pyams_content-1.99.1/src/pyams_content/component/association/skin/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/association/skin/templates/association-viewlet.pt` & `pyams_content-1.99.1/src/pyams_content/component/association/skin/templates/association-viewlet.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/association/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/association/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/association/zmi/container.py` & `pyams_content-1.99.1/src/pyams_content/component/association/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/association/zmi/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/association/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/association/zmi/paragraph.py` & `pyams_content-1.99.1/src/pyams_content/component/association/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/calendar/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/cards/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/cards/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/cards/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/cards/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/cards/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/cards/skin/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/cards/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/cards/skin/templates/cards-masonry.pt` & `pyams_content-1.99.1/src/pyams_content/component/cards/skin/templates/cards-masonry.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/cards/skin/templates/cards.pt` & `pyams_content-1.99.1/src/pyams_content/component/cards/skin/templates/cards.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/cards/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/cards/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/extfile/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/extfile/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/extfile/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/extfile/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/extfile/manager.py` & `pyams_content-1.99.1/src/pyams_content/component/extfile/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/manager.py` & `pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 """
 
 from pyams_content.component.extfile import IExtFileManagerInfo
 from pyams_content.component.extfile.interfaces import IExtFileManagerTarget
 from pyams_content.interfaces import MANAGE_SITE_ROOT_PERMISSION
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
+from pyams_form.interfaces.form import IFormContent
 from pyams_layer.interfaces import IPyAMSLayer
+from pyams_utils.adapter import adapter_config
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.form import AdminEditForm
 from pyams_zmi.interfaces import IAdminLayer
 from pyams_zmi.interfaces.viewlet import IPropertiesMenu
 from pyams_zmi.zmi.viewlet.menu import NavigationMenuItem
 
 
@@ -51,10 +53,13 @@
     """External files manager properties edit form"""
 
     title = _("External files settings")
     legend = _("Default prefix")
 
     fields = Fields(IExtFileManagerInfo)
 
-    def get_content(self):
-        """Content getter"""
-        return IExtFileManagerInfo(self.context)
+
+@adapter_config(required=(IExtFileManagerTarget, IPyAMSLayer, ExtFileManagerPropertiesEditForm),
+                provides=IFormContent)
+def extfile_manager_properties_form_content(context, request, form):
+    """External file manager properties edit form content getter"""
+    return IExtFileManagerInfo(context)
```

### Comparing `pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/paragraph.py` & `pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt` & `pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt` & `pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/extfile/zmi/widget.py` & `pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/fields/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/fields/handler/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/fields/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/fields/handler/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/fields/handler/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/fields/handler/mail.py` & `pyams_content-1.99.1/src/pyams_content/component/fields/handler/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/fields/handler/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/fields/handler/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/fields/handler/zmi/mail.py` & `pyams_content-1.99.1/src/pyams_content/component/fields/handler/zmi/mail.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 """
 
 from pyams_content.component.fields.handler.interfaces import IMailtoHandlerInfo
 from pyams_content.shared.common.zmi import ISharedContentPropertiesMenu
 from pyams_fields.interfaces import IFormHandlersInfo, IFormHandlersTarget
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
+from pyams_form.interfaces.form import IFormContent
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
+from pyams_utils.adapter import adapter_config
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.form import AdminEditForm
 from pyams_zmi.interfaces import IAdminLayer
 from pyams_zmi.zmi.viewlet.menu import NavigationMenuItem
 
 
 __docformat__ = 'restructuredtext'
@@ -59,11 +61,14 @@
     """Mailto form handlers settings form"""
 
     title = _("Mailto notifications")
     legend = _("Mailto form handler settings")
 
     fields = Fields(IMailtoHandlerInfo)
 
-    def get_content(self):
-        """Form content getter"""
-        handlers = IFormHandlersInfo(self.context)
-        return IMailtoHandlerInfo(handlers, None)
+
+@adapter_config(required=(IFormHandlersTarget, IPyAMSLayer, MailtoFormHandlerSettingsEditForm),
+                provides=IFormContent)
+def form_handlers_settings_edit_form_content(context, request, form):
+    """Form handlers settings edit form content getter"""
+    handlers = IFormHandlersInfo(context)
+    return IMailtoHandlerInfo(handlers, None)
```

### Comparing `pyams_content-1.99.0/src/pyams_content/component/fields/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/fields/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/fields/paragraph.py` & `pyams_content-1.99.1/src/pyams_content/component/fields/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/fields/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/fields/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/fields/skin/paragraph.py` & `pyams_content-1.99.1/src/pyams_content/component/fields/skin/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/fields/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/fields/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/fields/zmi/paragraph.py` & `pyams_content-1.99.1/src/pyams_content/component/fields/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/file/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/file/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/frame/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/frame/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/file.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/file.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/paragraph.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from pyams_portal.interfaces import IPortalContext, IPortletRenderer
 from pyams_portal.skin import PortletRenderer
 from pyams_template.template import template_config
 from pyams_utils.adapter import adapter_config
 from pyams_utils.factory import factory_config
 from pyams_utils.list import random_iter
 
-
 __docformat__ = 'restructuredtext'
 
 from pyams_content import _
 
 
 class BaseGalleryPortletRenderer(PortletRenderer):
     """Base gallery portlet renderer"""
```

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/skin/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt` & `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt` & `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt` & `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/portlet/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/skin/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt` & `pyams_content-1.99.1/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/skin/templates/gallery-default.pt` & `pyams_content-1.99.1/src/pyams_content/component/gallery/skin/templates/gallery-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/skin/templates/gallery-random.pt` & `pyams_content-1.99.1/src/pyams_content/component/gallery/skin/templates/gallery-random.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/file.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/file.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/helpers.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/helpers.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/paragraph.py` & `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt` & `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt` & `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt` & `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/paragraph.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/skin/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt` & `pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt` & `pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/portlet/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/skin/illustration.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/skin/illustration.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/skin/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/skin/paragraph.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/skin/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/skin/templates/illustration-default.pt` & `pyams_content-1.99.1/src/pyams_content/component/illustration/skin/templates/illustration-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/skin/templates/illustration-side.pt` & `pyams_content-1.99.1/src/pyams_content/component/illustration/skin/templates/illustration-side.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt` & `pyams_content-1.99.1/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/thesaurus.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/zmi/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 """PyAMS_content.component.illustration.zmi module
 
 This module provides management interface components for illustrations.
 """
 
 from pyramid.events import subscriber
 
+from pyams_content.component.illustration import IIllustrationTargetBase, ILinkIllustration
 from pyams_content.component.illustration.interfaces import IBaseIllustration, \
     IBaseIllustrationTarget, IIllustration, IIllustrationTarget, ILinkIllustrationTarget
 from pyams_content.component.paragraph.interfaces import IBaseParagraph
 from pyams_zmi.interfaces.form import IPropertiesEditForm
 from pyams_form.field import Fields
-from pyams_form.interfaces.form import IAJAXFormRenderer, IFormUpdatedEvent, IInnerSubForm
+from pyams_form.interfaces.form import IAJAXFormRenderer, IFormContent, IFormUpdatedEvent, IInnerSubForm
 from pyams_portal.zmi.portlet import PortletRendererSettingsEditForm
 from pyams_portal.zmi.widget import RendererSelectFieldWidget
 from pyams_utils.adapter import ContextRequestViewAdapter, adapter_config
 from pyams_zmi.form import FormGroupSwitcher
 from pyams_zmi.helper.event import get_json_widget_refresh_callback
 from pyams_zmi.interfaces import IAdminLayer
 
@@ -44,29 +45,32 @@
 
     legend = _("Main illustration")
     weight = 10
 
     fields = Fields(IBaseIllustration)
     prefix = 'illustration.'
 
-    def get_content(self):
-        """Form content getter"""
-        return IIllustration(self.context)
-
     @property
     def mode(self):
         """Form mode getter"""
         return self.parent_form.mode
 
     @property
     def state(self):
         """Form state getter"""
         return 'open' if self.get_content().has_data() else 'closed'
 
 
+@adapter_config(required=(IIllustrationTargetBase, IAdminLayer, BasicIllustrationPropertiesEditForm),
+                provides=IFormContent)
+def base_illustration_edit_form_content(context, request, form):
+    """Base illustration properties edit form content getter"""
+    return IIllustration(context)
+
+
 @adapter_config(name='illustration',
                 required=(IIllustrationTarget, IAdminLayer, IPropertiesEditForm),
                 provides=IInnerSubForm, force_implements=False)
 class IllustrationPropertiesEditForm(BasicIllustrationPropertiesEditForm):
     """Illustration properties edit form"""
 
     fields = Fields(IIllustration)
@@ -85,17 +89,20 @@
     """Link illustration properties edit form"""
 
     legend = _("Navigation link illustration")
     weight = 15
 
     prefix = 'link_illustration.'
 
-    def get_content(self):
-        """Form content getter"""
-        return self.request.registry.getAdapter(self.context, IIllustration, name='link')
+
+@adapter_config(required=(ILinkIllustrationTarget, IAdminLayer, LinkIllustrationPropertiesEditForm),
+                provides=IFormContent)
+def link_illustration_edit_form_content(context, request, form):
+    """Link illustration properties edit form content getter"""
+    return ILinkIllustration(context)
 
 
 @adapter_config(required=(IBaseIllustrationTarget, IAdminLayer,
                           BasicIllustrationPropertiesEditForm),
                 provides=IAJAXFormRenderer)
 class BasicIllustrationPropertiesEditFormRenderer(ContextRequestViewAdapter):
     """Basic illustration properties AJAX form renderer"""
```

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/zmi/paragraph.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/zmi/paragraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,41 +15,35 @@
 This module provides management interface components for illustration paragraphs.
 """
 
 from pyams_content.component.illustration import IBaseIllustration, IIllustrationTarget, \
     IParagraphIllustration
 from pyams_content.component.illustration.interfaces import IIllustrationParagraph, \
     ILLUSTRATION_PARAGRAPH_ICON_CLASS, ILLUSTRATION_PARAGRAPH_NAME, ILLUSTRATION_PARAGRAPH_TYPE
-from pyams_content.component.paragraph import IBaseParagraph, IParagraphContainer, \
-    IParagraphContainerTarget
+from pyams_content.component.paragraph import IParagraphContainer, IParagraphContainerTarget
 from pyams_content.component.paragraph.zmi import BaseParagraphAddForm, BaseParagraphAddMenu, \
     BaseParagraphRendererSettingsEditForm, IParagraphContainerBaseTable, \
     IParagraphContainerFullTable
 from pyams_content.component.paragraph.zmi.container import ParagraphTitleToolbarItemMixin
 from pyams_content.component.paragraph.zmi.interfaces import IParagraphTitleToolbar
 from pyams_content.feature.renderer import IRendererSettings
-from pyams_zmi.interfaces.form import IPropertiesEditForm
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
 from pyams_form.interfaces.form import IFormContent, IFormFields
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_portal.zmi.widget import RendererSelectFieldWidget
 from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
 from pyams_utils.adapter import adapter_config
-from pyams_utils.traversing import get_parent
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.interfaces import IAdminLayer
+from pyams_zmi.interfaces.form import IPropertiesEditForm
 from pyams_zmi.interfaces.viewlet import IContextAddingsViewletManager
-from pyams_zmi.utils import get_object_label
-
 
 __docformat__ = 'restructuredtext'
 
-from pyams_content import _
-
 
 @viewlet_config(name='illustration',
                 context=IIllustrationTarget, layer=IAdminLayer,
                 view=IParagraphContainerFullTable, manager=IParagraphTitleToolbar,
                 weight=10)
 @viewlet_config(name='illustration',
                 context=IIllustrationParagraph, layer=IAdminLayer,
```

### Comparing `pyams_content-1.99.0/src/pyams_content/component/illustration/zmi/thesaurus.py` & `pyams_content-1.99.1/src/pyams_content/component/illustration/zmi/thesaurus.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 This module provides management components for thesaurus term
 illustration extension.
 """
 
 from pyams_content.component.illustration import IBaseIllustration, IIllustration
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
+from pyams_form.interfaces.form import IFormContent
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
 from pyams_thesaurus.interfaces.term import IThesaurusTerm
 from pyams_thesaurus.zmi.extension import ThesaurusTermExtensionEditForm
+from pyams_utils.adapter import adapter_config
 
 
 __docformat__ = 'restructuredtext'
 
 from pyams_content import _
 
 
@@ -38,9 +40,13 @@
 
     subtitle = _("Associated illustration")
     legend = _("Illustration properties")
     modal_class = 'modal-xl'
 
     fields = Fields(IBaseIllustration)
 
-    def get_content(self):
-        return IIllustration(self.context)
+
+@adapter_config(required=(IThesaurusTerm, IPyAMSLayer, ThesaurusTermIllustrationPropertiesEditForm),
+                provides=IFormContent)
+def thesaurus_term_illustration_form_content(context, request, form):
+    """Thesaurus term illustration edit form content getter"""
+    return IIllustration(context)
```

### Comparing `pyams_content-1.99.0/src/pyams_content/component/keynumber/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/keynumber/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/links/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/links/html.py` & `pyams_content-1.99.1/src/pyams_content/component/links/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/links/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/links/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/links/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/links/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/links/zmi/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/links/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/links/zmi/paragraph.py` & `pyams_content-1.99.1/src/pyams_content/component/links/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/map/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/map/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/milestone/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/milestone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/container.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/html.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/interfaces/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/interfaces/html.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/interfaces/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/skin/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/settings.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/settings.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/skin/html.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/skin/interfaces/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/skin/interfaces/html.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/interfaces/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/skin/templates/html.pt` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/templates/html.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/zmi/container.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/zmi/helper.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/helper.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/zmi/html.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/paragraph/zmi/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/thesaurus/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/thesaurus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/thesaurus/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/thesaurus/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/thesaurus/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/thesaurus/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/thesaurus/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/thesaurus/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/thesaurus/zmi/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/thesaurus/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/thesaurus/zmi/manager.py` & `pyams_content-1.99.1/src/pyams_content/component/thesaurus/zmi/manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,26 +19,25 @@
 
 from pyams_content.component.thesaurus import ICollectionsManager, ICollectionsManagerTarget, \
     ITagsManager, ITagsManagerTarget, IThemesManager, IThemesManagerTarget
 from pyams_content.interfaces import MANAGE_SITE_ROOT_PERMISSION
 from pyams_content.zmi import content_js
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
-from pyams_form.interfaces.form import IGroup
+from pyams_form.interfaces.form import IFormContent, IGroup
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_utils.adapter import adapter_config
 from pyams_utils.fanstatic import get_resource_path
 from pyams_utils.interfaces.data import IObjectData
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.form import AdminEditForm, FormGroupChecker
 from pyams_zmi.interfaces import IAdminLayer
 from pyams_zmi.interfaces.viewlet import IPropertiesMenu
 from pyams_zmi.zmi.viewlet.menu import NavigationMenuItem
 
-
 __docformat__ = 'restructuredtext'
 
 from pyams_content import _
 
 
 class BaseThesaurusManagerEditForm(AdminEditForm):
     """Base thesaurus manager edit form"""
@@ -87,32 +86,38 @@
     """Tags manager properties edit form"""
 
     title = _("Tags settings")
     legend = _("Selected tags thesaurus")
 
     fields = Fields(ITagsManager).select('thesaurus_name', 'extract_name')
 
-    def get_content(self):
-        """Content getter"""
-        return ITagsManager(self.context)
+
+@adapter_config(required=(ITagsManagerTarget, IAdminLayer, TagsManagerEditForm),
+                provides=IFormContent)
+def tags_manager_edit_form_content(context, request, form):
+    """Tags manager edit form content getter"""
+    return ITagsManager(context)
 
 
 @adapter_config(name='glossary',
                 required=(ITagsManagerTarget, IAdminLayer, TagsManagerEditForm),
                 provides=IGroup)
 class TagsManagerGlossaryGroup(FormGroupChecker):
     """Tags manager glossary group"""
 
     fields = Fields(ITagsManager).select('enable_glossary', 'glossary_thesaurus_name')
     checker_fieldname = 'enable_glossary'
     checker_mode = 'hide'
 
-    def get_content(self):
-        """Content getter"""
-        return ITagsManager(self.context)
+
+@adapter_config(required=(ITagsManagerTarget, IAdminLayer, TagsManagerGlossaryGroup),
+                provides=IFormContent)
+def tags_manager_glossary_group_content(context, request, group):
+    """Tags manager glossary edit form group content getter"""
+    return ITagsManager(context)
 
 
 #
 # Themes management
 #
 
 @viewlet_config(name='themes-manager.menu',
@@ -133,17 +138,20 @@
     """Themes manager properties edit form"""
 
     title = _("Themes settings")
     legend = _("Selected themes thesaurus")
 
     fields = Fields(IThemesManager)
 
-    def get_content(self):
-        """Content getter"""
-        return IThemesManager(self.context)
+
+@adapter_config(required=(IThemesManagerTarget, IAdminLayer, ThemesManagerEditForm),
+                provides=IFormContent)
+def themes_manager_edit_form_content(context, request, group):
+    """Themes manager edit form content getter"""
+    return IThemesManager(context)
 
 
 #
 # Collections management
 #
 
 @viewlet_config(name='collections-manager.menu',
@@ -164,10 +172,13 @@
     """Collections manager properties edit form"""
 
     title = _("Collections settings")
     legend = _("Selected collections thesaurus")
 
     fields = Fields(ICollectionsManager)
 
-    def get_content(self):
-        """Content getter"""
-        return ICollectionsManager(self.context)
+
+@adapter_config(required=(ICollectionsManagerTarget, IAdminLayer, CollectionsManagerEditForm),
+                provides=IFormContent)
+def collections_manager_edit_form_content(context, request, form):
+    """Collections manager edit form content getter"""
+    return ICollectionsManager(context)
```

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/video/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/video/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/paragraph.py` & `pyams_content-1.99.1/src/pyams_content/component/video/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/provider/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/video/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/provider/dailymotion.py` & `pyams_content-1.99.1/src/pyams_content/component/video/provider/dailymotion.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/provider/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/video/provider/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/provider/vimeo.py` & `pyams_content-1.99.1/src/pyams_content/component/video/provider/vimeo.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/provider/youtube.py` & `pyams_content-1.99.1/src/pyams_content/component/video/provider/youtube.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/video/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/skin/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/component/video/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/skin/provider/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/skin/provider/dailymotion.py` & `pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/dailymotion.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt` & `pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/skin/provider/vimeo.py` & `pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/vimeo.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/skin/provider/youtube.py` & `pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/youtube.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/skin/templates/video-default.pt` & `pyams_content-1.99.1/src/pyams_content/component/video/skin/templates/video-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/component/video/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/component/video/zmi/paragraph.py` & `pyams_content-1.99.1/src/pyams_content/component/video/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/doctests/README.rst` & `pyams_content-1.99.1/src/pyams_content/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/alert/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/alert/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/alert/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/feature/alert/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/alert/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/alert/skin/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 __docformat__ = 'restructuredtext'
 
 from zope.interface import Interface
 
 from pyams_content.feature.alert import IAlertManagerInfo
-from pyams_content.shared.alert.interfaces import ALERT_GRAVITY, ALERT_GRAVITY_NAMES
+from pyams_i18n.interfaces import II18n
 from pyams_layer.interfaces import IPyAMSUserLayer
 from pyams_template.template import template_config
 from pyams_viewlet.viewlet import ViewContentProvider, contentprovider_config
 
 
 @contentprovider_config(name='pyams_content.alerts',
                         layer=IPyAMSUserLayer, view=Interface)
@@ -36,15 +36,17 @@
         """Alerts getter"""
         alerts = IAlertManagerInfo(self.request.root, None)
         if alerts is not None:
             yield from alerts.get_visible_alerts(self.request)
 
     def get_gravity(self, alert):
         """Alert gravity getter"""
-        return self.request.localizer.translate(ALERT_GRAVITY_NAMES.get(ALERT_GRAVITY(alert.gravity)))
+        alert_type = alert.get_alert_type()
+        if alert_type is not None:
+            return II18n(alert_type).query_attribute('label', request=self.request)
 
 
 @contentprovider_config(name='pyams_content.context_alerts',
                         layer=IPyAMSUserLayer, view=Interface)
 @template_config(template='templates/context-alerts.pt',
                  layer=IPyAMSUserLayer)
 class ContextAlertsContentProvider(AlertsContentProvider):
```

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/alert/skin/templates/alerts.pt` & `pyams_content-1.99.1/src/pyams_content/feature/alert/skin/templates/alerts.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/alert/skin/templates/context-alerts.pt` & `pyams_content-1.99.1/src/pyams_content/feature/alert/skin/templates/context-alerts.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/alert/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/alert/zmi/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 
 """
 
 from pyams_content.feature.alert import IAlertManagerInfo
 from pyams_content.interfaces import MANAGE_SITE_ROOT_PERMISSION
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
+from pyams_form.interfaces.form import IFormContent
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_site.interfaces import ISiteRoot
+from pyams_utils.adapter import adapter_config
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.form import AdminEditForm
 from pyams_zmi.interfaces import IAdminLayer
 from pyams_zmi.interfaces.viewlet import IPropertiesMenu
 from pyams_zmi.zmi.viewlet.menu import NavigationMenuItem
 
 __docformat__ = 'restructuredtext'
@@ -49,10 +51,13 @@
     """Alerts manager edit form"""
 
     title = _("Alerts management")
     legend = _("Alerts management views")
 
     fields = Fields(IAlertManagerInfo)
 
-    def get_content(self):
-        """Form content getter"""
-        return IAlertManagerInfo(self.context)
+
+@adapter_config(required=(ISiteRoot, IPyAMSLayer, AlertsManagerEditForm),
+                provides=IFormContent)
+def site_root_alert_edit_form_content(context, request, form):
+    """Site root alerts edit form content getter"""
+    return IAlertManagerInfo(context)
```

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/glossary/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/glossary/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/glossary/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/feature/glossary/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/sitemap.py` & `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/sitemap.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt` & `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/templates/glossary.pt` & `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/glossary.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/templates/term-associations.pt` & `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-associations.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt` & `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/glossary/skin/term.py` & `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/term.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/glossary/task.py` & `pyams_content-1.99.1/src/pyams_content/feature/glossary/task.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/glossary/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/glossary/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/history/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/history/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/history/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/feature/history/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/history/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/history/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/history/zmi/viewlet.py` & `pyams_content-1.99.1/src/pyams_content/feature/history/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/html/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/html/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/navigation/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/navigation/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/feature/navigation/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/skin/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt` & `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt` & `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt` & `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt` & `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/navigation/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/navigation/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/navigation/zmi/container.py` & `pyams_content-1.99.1/src/pyams_content/feature/navigation/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/navigation/zmi/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/feature/navigation/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/preview/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/preview/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/preview/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/feature/preview/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/preview/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/preview/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt` & `pyams_content-1.99.1/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/renderer/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/renderer/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/feature/renderer/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/review/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/review/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/review/chat.py` & `pyams_content-1.99.1/src/pyams_content/feature/review/chat.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/review/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/feature/review/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/review/manager.py` & `pyams_content-1.99.1/src/pyams_content/feature/review/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/review/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/review/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/review/zmi/templates/comment.pt` & `pyams_content-1.99.1/src/pyams_content/feature/review/zmi/templates/comment.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/review/zmi/templates/comments.pt` & `pyams_content-1.99.1/src/pyams_content/feature/review/zmi/templates/comments.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/review/zmi/templates/mail-notification.pt` & `pyams_content-1.99.1/src/pyams_content/feature/review/zmi/templates/mail-notification.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/search/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,10 +6,13 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 
-"""PyAMS_*** module
+"""PyAMS_content.shared.common.portlet.zmi module
 
+This is the base module for management interface of shared contents portlets.
 """
+
+__docformat__ = 'restructuredtext'
```

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/search/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/feature/search/interfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 """
 
 from zope.interface import Attribute, Interface, Invalid, invariant
 from zope.schema import Bool, Choice, Set
 
 from pyams_content.interfaces import IBaseContent
-from pyams_content.shared.common import SHARED_CONTENT_TYPES_VOCABULARY
+from pyams_content.shared.common import VIEWS_SHARED_CONTENT_TYPES_VOCABULARY
 from pyams_content.shared.common.interfaces.types import ALL_DATA_TYPES_VOCABULARY
 from pyams_content.shared.site.interfaces import IBaseSiteItem, ISiteElement
-from pyams_content.shared.view import IViewQuery, IWfView
-from pyams_content.shared.view.interfaces import RELEVANCE_ORDER, USER_VIEW_ORDER_VOCABULARY
+from pyams_content.shared.view.interfaces import IWfView, RELEVANCE_ORDER, USER_VIEW_ORDER_VOCABULARY
+from pyams_content.shared.view.interfaces.query import IViewQuery
 from pyams_i18n.schema import I18nTextLineField
 from pyams_sequence.interfaces import IInternalReferencesList, ISequentialIdTarget
 from pyams_sequence.schema import InternalReferenceField
 
 __docformat__ = 'restructuredtext'
 
 from pyams_content import _
@@ -102,28 +102,28 @@
                                     "have been retired and re-published with a different "
                                     "publication date"),
                       vocabulary=USER_VIEW_ORDER_VOCABULARY,
                       required=False,
                       default=RELEVANCE_ORDER)
 
     visible_in_list = Bool(title=_("Visible in folders list"),
-                           description=_("If 'no', folder will not be displayed into folders "
-                                         "list"),
+                           description=_("If 'no', search folder will not be displayed into "
+                                         "parent's contents list"),
                            required=True,
                            default=True)
 
     navigation_title = I18nTextLineField(title=_("Navigation title"),
                                          description=_("Folder's title displayed in navigation "
                                                        "pages; original title will be used if "
                                                        "none is specified"),
                                          required=False)
 
     selected_content_types = Set(title=_("Selected content types"),
                                  description=_("Searched content types; leave empty for all"),
-                                 value_type=Choice(vocabulary=SHARED_CONTENT_TYPES_VOCABULARY),
+                                 value_type=Choice(vocabulary=VIEWS_SHARED_CONTENT_TYPES_VOCABULARY),
                                  required=False)
 
     selected_datatypes = Set(title=_("Selected data types"),
                              description=_("Searched data types; leave empty for all"),
                              value_type=Choice(vocabulary=ALL_DATA_TYPES_VOCABULARY),
                              required=False)
```

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/search/manager.py` & `pyams_content-1.99.1/src/pyams_content/feature/search/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/search/thesaurus.py` & `pyams_content-1.99.1/src/pyams_content/feature/search/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/search/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/blog/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/search/zmi/manager.py` & `pyams_content-1.99.1/src/pyams_content/feature/search/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/sitemap/__init__.py` & `pyams_content-1.99.1/src/pyams_content/feature/sitemap/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/feature/sitemap/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/feature/sitemap/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/generations/__init__.py` & `pyams_content-1.99.1/src/pyams_content/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/include.py` & `pyams_content-1.99.1/src/pyams_content/include.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/interfaces/__init__.py` & `pyams_content-1.99.1/src/pyams_content/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo` & `pyams_content-1.99.1/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,14 +9,17 @@
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 4.14\n"
 
 msgid "#{}"
 msgstr "N° {}"
 
+msgid "${count} result(s) found"
+msgstr "${count} résultat(s) trouvé(s)"
+
 msgid "${sender} added the following message to his request:"
 msgstr "${sender} a accompagné sa demande de relecture du message suivant :"
 
 msgid "'Off' state pictogram associated with this data type"
 msgstr ""
 "Pictogramme utilisé par certains modes de rendu pour illustrer le statut "
 "\"inactif\" de ce type de contenu"
@@ -55,14 +58,17 @@
 
 msgid "Accessibility title"
 msgstr "Alternative (accessibilité)"
 
 msgid "Action comment"
 msgstr "Commentaire associé"
 
+msgid "Add alert type"
+msgstr "Ajouter un type d'alerte"
+
 msgid "Add comment"
 msgstr "Ajouter ce commentaire"
 
 msgid "Add content type"
 msgstr "Ajouter un type de contenu"
 
 msgid "Add external link..."
@@ -79,14 +85,17 @@
 
 msgid "Add new: {}"
 msgstr "Ajouter un contenu : {}"
 
 msgid "Add pictogram"
 msgstr "Ajouter un pictogramme"
 
+msgid "Add search folder..."
+msgstr "Moteur de recherche"
+
 msgid "Add site folder..."
 msgstr "Rubrique"
 
 msgid "Add site manager"
 msgstr "Ajouter un site"
 
 msgid "Add site topic..."
@@ -125,28 +134,37 @@
 msgstr ""
 "Lorsque vous aurez pris connaissance du contenu, vous pourrez utiliser le "
 "menu « Commentaire » en colonne de gauche pour apporter vos commentaires."
 
 msgid "Alert"
 msgstr "Alerte"
 
-msgid "Alert gravity"
-msgstr "Niveau de gravité"
-
-msgid "Alert gravity can affect renderer alert style"
-msgstr ""
-"Le niveau de gravité peut éventuellement, en fonction du thème graphique, "
-"affecter le rendu de l'alerte"
-
 msgid "Alert management"
 msgstr "Cette alerte"
 
 msgid "Alert settings"
 msgstr "Paramètres de l'alerte"
 
+msgid "Alert type"
+msgstr "Type d'alerte"
+
+msgid "Alert type can affect renderer alert style"
+msgstr ""
+"Le type d'alerte peut éventuellement, en fonction du thème graphique, "
+"affecter le rendu de l'alerte"
+
+msgid "Alert type properties"
+msgstr "Propriétés du type d'alerte"
+
+msgid "Alert types"
+msgstr "Types d'alertes"
+
+msgid "Alert types list"
+msgstr "Liste des types d'alertes"
+
 msgid "Alerts management"
 msgstr "Paramétrage des alertes"
 
 msgid "Alerts management views"
 msgstr "Sélection des vues associées aux alertes"
 
 msgid "All interventions"
@@ -155,17 +173,26 @@
 msgid ""
 "All versions of this content which are not archived will be transferred to "
 "newly selected owner"
 msgstr ""
 "La propriété de toutes les versions de ce contenu qui ne sont pas archivées "
 "sera transférée au nouveau propriétaire sélectionné."
 
+msgid "Allow empty query?"
+msgstr "Recherche sans critère"
+
 msgid "Allow full screen?"
 msgstr "Accès au mode plein écran"
 
+msgid "Allow pagination?"
+msgstr "Autoriser la pagination"
+
+msgid "Allow results sorting?"
+msgstr "Autoriser le tri"
+
 msgid "Allow sharing?"
 msgstr "Autoriser le partage"
 
 msgid "Allow user params?"
 msgstr "Autoriser les paramètres utilisateur"
 
 msgid "Allowed paragraphs"
@@ -205,14 +232,18 @@
 "affiché ; il est également utilisé par les navigateurs des personnes "
 "soufrant de déficiences visuelles, et doit donc décrire le contenu de "
 "l'image pour se conformer aux normes d'accessibilité"
 
 msgid "Always include selected internal references"
 msgstr "Toujours inclure les références internes"
 
+msgid "An hidden alert type can't be assigned to new alerts"
+msgstr ""
+"Un type d'alerte inactif ne peut pas être affecté à de nouvelles alertes"
+
 msgid "An hidden data type can't be assigned to new contents"
 msgstr ""
 "Un type de contenu inactif ne peut pas être affecté à de nouveau contenus"
 
 msgid "Anchor?"
 msgstr "Ancre ?"
 
@@ -340,14 +371,17 @@
 msgstr "Libellé back-office"
 
 msgid "Base URL of the public site"
 msgstr ""
 "URL de base du site public ; cette adresse est notamment utilisée par les "
 "codes QR"
 
+msgid "Base color associated with this alert type"
+msgstr "Couleur de base associée à ce type d'alerte"
+
 msgid "Between all contents"
 msgstr "Parmi tous les contenus"
 
 msgid "Between all contents of « {} » content type"
 msgstr "Parmi les contenus du gabarit « {} »"
 
 msgid "Between all contents of « {} » site folder"
@@ -355,29 +389,38 @@
 
 msgid "Between all contents of « {} » site manager"
 msgstr "Parmi les contenus du site « {} »"
 
 msgid "Body"
 msgstr "Contenu HTML"
 
+msgid "Bootstrap Masonry cards search results"
+msgstr "Grille de résultats, sans facettes, style « Masonry »"
+
 msgid "Bootstrap cards"
 msgstr "Bootstrap: cartes"
 
 msgid "Bootstrap cards Masonry renderer"
 msgstr "Cartes Bootstrap avec rendu Masonry"
 
 msgid "Bootstrap cards renderer (default)"
 msgstr "Cartes Bootstrap (par défaut)"
 
+msgid "Bootstrap cards search results"
+msgstr "Grille de résultats, sans facettes, style « cartes Bootstrap »"
+
 msgid "Browser favourite icon"
 msgstr "Icône de favoris du site"
 
 msgid "Button label"
 msgstr "Libellé du lien"
 
+msgid "Button's title"
+msgstr "Libellé du bouton"
+
 msgid ""
 "By default, internal links use a \"relative\" URL, which tries to display "
 "link target in the current context; by using a canonical URL, you can "
 "display target in it's attachment context (if defined)"
 msgstr ""
 "Par défaut, les liens internes utilisent une URl \"relative\", qui tente "
 "d'afficher la cible du lien dans le contexte courant ; en utilisant une URL "
@@ -519,14 +562,17 @@
 
 msgid "Change item URL"
 msgstr "Modification de l'URL"
 
 msgid "Change owner"
 msgstr "Changer de propriétaire"
 
+msgid "Click icon to enable or disable alert type"
+msgstr "Cliquer pour activer ou désactiver ce type d'alerte"
+
 msgid "Click icon to enable or disable content type"
 msgstr "Cliquer pour activer ou désactiver ce type de contenu"
 
 msgid "Click to lock/unlock paragraph"
 msgstr "Cliquer pour (dé)verrouiller ce bloc"
 
 msgid "Click to open/close all folders"
@@ -612,14 +658,17 @@
 
 msgid "Content archived"
 msgstr "Archivage"
 
 msgid "Content archived after version publication"
 msgstr "Archivage automatique après publication"
 
+msgid "Content archiver task"
+msgstr "Archivage d'un contenu"
+
 msgid "Content archiving"
 msgstr "Archivage de contenu"
 
 msgid "Content blocks links and attachments"
 msgstr "Liens et pièces jointes par bloc de contenu"
 
 msgid "Content collections selection"
@@ -663,14 +712,17 @@
 
 msgid "Content publication start date is not passed yet"
 msgstr "La date de début de publication de ce contenu n'est pas encore passée"
 
 msgid "Content published"
 msgstr "Publication"
 
+msgid "Content publisher task"
+msgstr "Publication d'un contenu"
+
 msgid "Content removal"
 msgstr "Retrait de contenu"
 
 msgid "Content retired"
 msgstr "Retrait"
 
 msgid "Content retired after passed expiration date"
@@ -923,14 +975,17 @@
 
 msgid "Display full header"
 msgstr "Afficher le chapô en entier"
 
 msgid "Display header?"
 msgstr "Afficher le chapô"
 
+msgid "Display if empty?"
+msgstr "Afficher sans résultat"
+
 msgid "Display illustration?"
 msgstr "Afficher l'illustration"
 
 msgid "Display illustrations?"
 msgstr "Afficher l'illustration"
 
 msgid "Display image title"
@@ -947,14 +1002,17 @@
 
 msgid "Display pictogram properties"
 msgstr "Propriétés du pictogramme"
 
 msgid "Display publication date?"
 msgstr "Afficher la date de publication"
 
+msgid "Display results count?"
+msgstr "Afficher le nombre de résultats"
+
 msgid "Display specificities?"
 msgstr "Afficher les spécificités"
 
 msgid "Display tags?"
 msgstr "Afficher les tags"
 
 msgid "Display title?"
@@ -1011,17 +1069,14 @@
 
 msgid "Enable search by collection?"
 msgstr "Activer la recherche par collections"
 
 msgid "Enable search by tag?"
 msgstr "Activer la recherche par tags"
 
-msgid "End of alert"
-msgstr "Fin d'alerte"
-
 msgid "Entered text will be search in title only"
 msgstr "La requête s'applique au titre uniquement..."
 
 msgid "Exclude anchors"
 msgstr "Exclure les ancres"
 
 msgid "Exclude context?"
@@ -1094,25 +1149,31 @@
 
 msgid "File's content language"
 msgstr "Langue du fichier"
 
 msgid "First owner"
 msgstr "Premier propriétaire"
 
+msgid "First search results sample:"
+msgstr "Premiers résultats de la recherche :"
+
 msgid "Floating illustration to the left"
 msgstr "Illustration placée à gauche du texte"
 
 msgid "Floating illustration to the right"
 msgstr "Illustration placée à droite du texte"
 
 msgid "Folder behaviour when navigating to folder URL"
 msgstr ""
 "Comportement attendu lorsqu'un utilisateur navigue vers l'URL de cette "
 "rubrique"
 
+msgid "Folder search settings"
+msgstr "Paramètres de la recherche"
+
 msgid "Folder's parent"
 msgstr "Niveau de rattachement de cette rubrique"
 
 msgid ""
 "Folder's title displayed in navigation pages; original title will be used if "
 "none is specified"
 msgstr ""
@@ -1197,14 +1258,17 @@
 
 msgid "HTML source code (default)"
 msgstr "Code source HTML (par défaut)"
 
 msgid "Header"
 msgstr "Chapô"
 
+msgid "Header display"
+msgstr "Affichage du chapô"
+
 msgid "Header display mode"
 msgstr "Affichage du chapô"
 
 msgid "Heading displayed according to presentation template"
 msgstr ""
 "Le chapô peut être affiché ou non en fonction du paramétrage du modèle de "
 "présentation"
@@ -1256,14 +1320,20 @@
 "seront pas affichées dans l'en-tête de page"
 
 msgid "If 'no', all paragraphs will be used as navigation anchors"
 msgstr ""
 "Si 'non', tous les blocs de contenus seront utilisés comme liens de "
 "navigation même s'ils ne sont pas définis comme ancres de navigation"
 
+msgid ""
+"If 'no', and if no result is found, the portlet will not display anything"
+msgstr ""
+"Si cette option n'est pas sélectionnée et qu'aucun résultat n'est trouvé, le "
+"composant ne sera pas affiché"
+
 msgid "If 'no', folder will not be displayed into folders list"
 msgstr ""
 "Si 'non', la rubrique ne sera pas affichée dans la liste des rubriques du "
 "niveau parent"
 
 msgid "If 'no', link is not visible"
 msgstr "Si 'non', le lien ne sera pas visible"
@@ -1273,17 +1343,43 @@
 msgstr ""
 "Si 'non', les liens de navigation vers les contenus précédent et suivant "
 "positionnés dans la même rubrique ne seront pas affichés"
 
 msgid "If 'no', no header will be displayed"
 msgstr "Si 'non', le chapô ne sera pas affiché"
 
+msgid ""
+"If 'no', no result will be displayed if user didn't entered a search string"
+msgstr ""
+"Si cette option n'est pas sélectionnée, aucun résultat ne sera renvoyé si "
+"l'utilisateur ne saisit pas de critère de recherche"
+
+msgid "If 'no', results count will not be displayed"
+msgstr ""
+"Le nombre de résultats de la recherche ne sera affiché que si cette option "
+"est sélectionnée"
+
 msgid "If 'no', results pagination will be disabled"
 msgstr "Si 'non', la pagination des résultats sera désactivée"
 
+msgid "If 'no', results will not be paginated"
+msgstr ""
+"LA navigation entre les pages de résultats ne sera possible que si cette "
+"option est sélectionnée"
+
+msgid "If 'no', results will not be sortable"
+msgstr ""
+"Le tri des résultats ne sera possible que si cette option est sélectionnée"
+
+msgid ""
+"If 'no', search folder will not be displayed into parent's contents list"
+msgstr ""
+"Si 'non', le moteur de recherche ne sera pas affiché dans la liste des "
+"contenus du niveau parent"
+
 msgid "If 'no', specific content's information will not be displayed..."
 msgstr ""
 "Si 'non', les informations spécifiques au gabarit du contenu ne seront pas "
 "affichées"
 
 msgid "If 'no', this media won't be displayed in front office"
 msgstr "Si 'non', ce média ne sera pas affiché en front-office"
@@ -1688,23 +1784,17 @@
 
 msgid "Include selected internal references only if view is empty"
 msgstr "Inclure les références internes seulement lorsque la vue est vide"
 
 msgid "Info properties interface"
 msgstr "Interface des propriétés du lien"
 
-msgid "Information"
-msgstr "Information"
-
 msgid "Infos color"
 msgstr "Couleur des informations"
 
-msgid "Initial selection"
-msgstr "Utiliser les images d'origine"
-
 msgid ""
 "Initial video frame height; mandatory for old browsers but may be overridden "
 "by presentation skin"
 msgstr ""
 "Hauteur initiale de la vidéo ; cette information est obligatoire uniquement "
 "pour les navigateurs les plus anciens, et peut être redéfinie via le thème "
 "graphique et le modèle de présentation"
@@ -1996,14 +2086,17 @@
 
 msgid "Main tool properties"
 msgstr "Propriétés principales"
 
 msgid "Manage content properties"
 msgstr "Gérer les propriétés d'un contenu"
 
+msgid "Manage first level site tree elements"
+msgstr "Gérer les sites de premier niveau"
+
 msgid "Manage main site root properties"
 msgstr "Gérer les propriétés globales du site"
 
 msgid "Manage shared tool properties"
 msgstr "Gérer les propriétés d'un outil partagé"
 
 msgid "Manage site, blog or hub properties"
@@ -2226,14 +2319,20 @@
 
 msgid "Navigation properties"
 msgstr "Propriétés de navigation"
 
 msgid "Navigation title"
 msgstr "Libellé de navigation"
 
+msgid "New alert type"
+msgstr "Nouveau type d'alerte"
+
+msgid "New alert type properties"
+msgstr "Propriétés du nouveau type"
+
 msgid "New comment"
 msgstr "Nouveau commentaire"
 
 msgid "New content properties"
 msgstr "Propriétés du nouveau contenu"
 
 msgid "New content type"
@@ -2325,14 +2424,20 @@
 
 msgid "New pictogram"
 msgstr "Nouveau pictogramme"
 
 msgid "New pictogram properties"
 msgstr "Propriétés du nouveau pictogramme"
 
+msgid "New search folder"
+msgstr "Nouveau moteur de recherche"
+
+msgid "New search folder properties"
+msgstr "Propriétés du nouveau moteur de recherche"
+
 msgid "New site folder"
 msgstr "Nouvelle rubrique"
 
 msgid "New site folder properties"
 msgstr "Propriétés de la nouvelle rubrique"
 
 msgid "New site properties"
@@ -2352,14 +2457,20 @@
 
 msgid "No filter, all paragraphs are selected"
 msgstr "Aucun filtre, tous les blocs de contenu sont sélectionnés"
 
 msgid "No filter, all paragraphs types are selected"
 msgstr "Aucun filtre, tous les types de blocs de contenu sont sélectionnés"
 
+msgid "No result found!"
+msgstr "Aucun résultat trouvé !"
+
+msgid "No result found."
+msgstr "Aucun résultat trouvé"
+
 msgid "No selected pictogram"
 msgstr "Aucun pictogramme sélectionné"
 
 msgid "Not published"
 msgstr "Non publié"
 
 msgid "Not visible site"
@@ -2382,26 +2493,34 @@
 
 msgid "OFF pictogram"
 msgstr "Pictogramme 'inactif'"
 
 msgid "ON pictogram"
 msgstr "Pictogramme 'actif'"
 
+msgid "Object types"
+msgstr "Types de l'objet"
+
 msgid "Open preview in new tab"
 msgstr "Ouvrir l'aperçu dans un nouvel onglet"
 
 msgid "Operator (role)"
 msgstr "Opérateur (rôle)"
 
 msgid "Operators group"
 msgstr "Groupe des opérateurs"
 
 msgid "Optional label used in management pages instead of default label"
 msgstr "Libellé utilisé en back-office, à la place du libellé standard"
 
+msgid "Optional navigation button's title"
+msgstr ""
+"Un bouton de navigation associé à chaque résultat de recherche sera affiché "
+"si cette option est sélectionnée"
+
 msgid "Order by"
 msgstr "Ordre de tri"
 
 msgid "Other collections"
 msgstr "Autres collections"
 
 msgid "Other content types"
@@ -2427,25 +2546,31 @@
 
 msgid "Owner (role)"
 msgstr "Propriétaire (rôle)"
 
 msgid "Owner changed: {} -> {}"
 msgstr "Changement de propriétaire : {} -> {}"
 
+msgid "Page length:"
+msgstr "Longueur des pages :"
+
 msgid "Page size"
 msgstr "Taille des pages"
 
 msgid "Paginate?"
 msgstr "Pagination"
 
+msgid "Paginated search results (default)"
+msgstr "Liste de résultats, sans facettes (par défaut)"
+
 msgid "Pagination"
 msgstr "Pagination"
 
-msgid "Panoramic selection"
-msgstr "Utiliser la sélection panoramique"
+msgid "Paneled search results"
+msgstr "Grille de résultats, sans facettes, style « page carrefour »"
 
 msgid "Paragraph properties"
 msgstr "Propriétés du bloc de contenu"
 
 msgid "Paragraph renderer"
 msgstr "Mode de rendu"
 
@@ -2478,14 +2603,17 @@
 
 msgid "Parent"
 msgstr "Niveau parent"
 
 msgid "Pictogram"
 msgstr "Pictogramme"
 
+msgid "Pictogram associated with this alert type"
+msgstr "Nom du pictogramme associé à ce type d'alerte"
+
 msgid "Pictogram associated with this data type"
 msgstr "Nom du pictogramme associé à ce type de contenu"
 
 msgid "Pictogram content"
 msgstr "Image du pictogramme"
 
 msgid "Pictogram properties"
@@ -2528,17 +2656,14 @@
 msgstr ""
 "Vous pouvez faire un copier/coller du code d'intégration fourni par votre "
 "fournisseur de vidéos"
 
 msgid "Portlet main title"
 msgstr "Titre du composant"
 
-msgid "Portrait selection"
-msgstr "Utiliser la sélection en mode portrait"
-
 msgid ""
 "Position at which to start video, in 'seconds' or 'minutes:seconds' format"
 msgstr ""
 "Position à laquelle la vidéo doit démarrer, en secondes ou sous la forme "
 "'minutes:secondes'"
 
 msgid ""
@@ -2716,17 +2841,14 @@
 
 msgid "Recipient address"
 msgstr "Adresse du destinataire"
 
 msgid "Recipient name"
 msgstr "Nom du destinataire"
 
-msgid "Recommendation"
-msgstr "Recommandation"
-
 msgid "Redirect to first visible sub-folder or content"
 msgstr "Accéder à la première rubrique ou au premier contenu visible"
 
 msgid "Reference tables"
 msgstr "Références"
 
 msgid ""
@@ -2802,17 +2924,14 @@
 
 msgid "Reset refused publication to draft"
 msgstr "Publication refusée"
 
 msgid "Reset refused publication to retired"
 msgstr "Publication refusée"
 
-msgid "Responsive selection"
-msgstr "Utiliser les sélections responsives"
-
 msgid "Restricted"
 msgstr "Restrictions activées"
 
 msgid "Restricted contents"
 msgstr "Activer des restrictions d'accès"
 
 msgid "Results age limit"
@@ -2880,22 +2999,37 @@
 
 msgid "Save file as..."
 msgstr "Nom du fichier"
 
 msgid "Search engine name"
 msgstr "Nom du moteur de recherche"
 
+msgid "Search folder"
+msgstr "Moteur de recherche"
+
+msgid "Search folder collections settings"
+msgstr "Collections appliquées par le moteur de recherche"
+
 msgid ""
 "Search folder handling main site search. You can search a reference using "
 "'+' followed by internal number, or by entering text matching content title."
 msgstr ""
 "Moteur de recherche prenant en charge la recherche générale sur le site ; "
 "vous pouvez rechercher une référence en indiquant un '+' suivi du numéro "
 "interne de ce moteur de recherche, ou en entrant tout ou partie de son titre"
 
+msgid "Search folder management"
+msgstr "Ce moteur de recherche"
+
+msgid "Search folder tags settings"
+msgstr "Tags appliqués par le moteur de recherche"
+
+msgid "Search folder themes settings"
+msgstr "Thèmes appliqués par le moteur de recherche"
+
 msgid "Search results"
 msgstr "Résultats de la recherche"
 
 msgid "Search settings"
 msgstr "Paramétrage de la recherche"
 
 msgid "Search text"
@@ -3022,14 +3156,17 @@
 
 msgid "Selected views"
 msgstr "Vues sélectionnées"
 
 msgid "Selection of available pictograms"
 msgstr "Sélection des pictogrammes disponibles"
 
+msgid "Selection used to display illustrations thumbnails"
+msgstr "Sélections utilisées pour l'affichage des vignettes"
+
 msgid "Selection used to display images"
 msgstr "Sélections utilisées pour l'affichage des images"
 
 msgid "Selection used to display images thumbnails"
 msgstr "Sélections utilisées pour l'affichage des vignettes"
 
 msgid "Service name"
@@ -3209,14 +3346,23 @@
 
 msgid "Sort all results by first publication date"
 msgstr "Trier tous les résultats sur la date de première publication"
 
 msgid "Sort all results by last update date"
 msgstr "Trier tous les résultats sur la date de dernière mise à jour"
 
+msgid "Sort by last modification date"
+msgstr "Trier sur la date de dernière modification"
+
+msgid "Sort by publication date"
+msgstr "Trier sur la date de publication"
+
+msgid "Sort by relevance"
+msgstr "Trier par pertinence"
+
 msgid "Sought principals"
 msgstr "Relecteurs sollicités"
 
 msgid "Sound description"
 msgstr "Description"
 
 msgid "Sound file associated with the current media"
@@ -3249,17 +3395,14 @@
 msgstr "Termes spécifiques :"
 
 msgid "Specify how selected references are included into view results"
 msgstr ""
 "Indique comment les références internes définies au niveau du contexte "
 "d'application seront intégrées à la liste de résultats"
 
-msgid "Square selection"
-msgstr "Utiliser la sélection carrée"
-
 msgid "Standard file"
 msgstr "Fichier"
 
 msgid "Start at"
 msgstr "Position de départ"
 
 msgid "Start length"
@@ -3723,17 +3866,14 @@
 msgid ""
 "WARNING: this request was made by a contributor which is not the owner of "
 "this content"
 msgstr ""
 "ATTENTION : cette demande est formulée par un contributeur habilité qui "
 "n'est pas le propriétaire."
 
-msgid "Warning"
-msgstr "Avertissement"
-
 msgid "Webmaster (role)"
 msgstr "Webmestre (rôle)"
 
 msgid "Webmasters"
 msgstr "Webmestres"
 
 msgid "Webmasters can handle all contents, including published ones"
```

### Comparing `pyams_content-1.99.0/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po` & `pyams_content-1.99.1/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,85 +1,89 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2024-01-21 16:50+0100\n"
+"POT-Creation-Date: 2024-03-24 02:24+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 4.14\n"
 
 #: src/pyams_content/include.py:53
 msgid "Manage main site root properties"
 msgstr "Gérer les propriétés globales du site"
 
 #: src/pyams_content/include.py:57
+msgid "Manage first level site tree elements"
+msgstr "Gérer les sites de premier niveau"
+
+#: src/pyams_content/include.py:61
 msgid "Manage site, blog or hub properties"
 msgstr "Gérer les propriétés d'un site, d'un blog ou d'un hub"
 
-#: src/pyams_content/include.py:61
+#: src/pyams_content/include.py:65
 msgid "Manage shared tool properties"
 msgstr "Gérer les propriétés d'un outil partagé"
 
-#: src/pyams_content/include.py:65
+#: src/pyams_content/include.py:69
 msgid "Create new content"
 msgstr "Créer un nouveau contenu"
 
-#: src/pyams_content/include.py:69
+#: src/pyams_content/include.py:73
 msgid "Create new version of existing content"
 msgstr "Créer une nouvelle version d'un contenu"
 
-#: src/pyams_content/include.py:73
+#: src/pyams_content/include.py:77
 msgid "Manage content properties"
 msgstr "Gérer les propriétés d'un contenu"
 
-#: src/pyams_content/include.py:77
+#: src/pyams_content/include.py:81
 msgid "Comment existing content"
 msgstr "Commenter un contenu"
 
-#: src/pyams_content/include.py:81
+#: src/pyams_content/include.py:85
 msgid "Publish or retire existing content"
 msgstr "Publier ou retirer un contenu"
 
-#: src/pyams_content/include.py:96
+#: src/pyams_content/include.py:101
 msgid "Webmaster (role)"
 msgstr "Webmestre (rôle)"
 
-#: src/pyams_content/include.py:114
+#: src/pyams_content/include.py:120
 msgid "Pilot (role)"
 msgstr "Pilote (rôle)"
 
-#: src/pyams_content/include.py:130
+#: src/pyams_content/include.py:136
 msgid "Manager (role)"
 msgstr "Responsable (rôle)"
 
-#: src/pyams_content/include.py:146
+#: src/pyams_content/include.py:152
 msgid "Owner (role)"
 msgstr "Propriétaire (rôle)"
 
-#: src/pyams_content/include.py:156
+#: src/pyams_content/include.py:162
 msgid "Contributor (role)"
 msgstr "Contributeur (rôle)"
 
-#: src/pyams_content/include.py:173
+#: src/pyams_content/include.py:179
 msgid "Reader (role)"
 msgstr "Relecteur (rôle)"
 
-#: src/pyams_content/include.py:190
+#: src/pyams_content/include.py:196
 msgid "Operator (role)"
 msgstr "Opérateur (rôle)"
 
-#: src/pyams_content/include.py:201
+#: src/pyams_content/include.py:207
 msgid "Guest user (role)"
 msgstr "Invité (rôle)"
 
 #: src/pyams_content/zmi/dashboard.py:84
 msgid "Switch element visibility"
 msgstr "Cliquez pour rendre l'élément visible ou non"
 
@@ -89,15 +93,16 @@
 "Un élément peut ne pas être visible s'il n'a pas encore été publié ou si son "
 "niveau parent n'est pas publié"
 
 #: src/pyams_content/zmi/dashboard.py:112
 #: src/pyams_content/reference/zmi/table.py:99
 #: src/pyams_content/feature/navigation/portlet/interfaces.py:33
 #: src/pyams_content/feature/navigation/portlet/interfaces.py:47
-#: src/pyams_content/interfaces/__init__.py:113
+#: src/pyams_content/feature/search/portlet/interfaces.py:44
+#: src/pyams_content/interfaces/__init__.py:116
 #: src/pyams_content/component/paragraph/zmi/container.py:236
 #: src/pyams_content/component/paragraph/portlet/interfaces.py:33
 #: src/pyams_content/component/gallery/interfaces.py:118
 #: src/pyams_content/component/gallery/portlet/interfaces.py:33
 #: src/pyams_content/shared/site/zmi/folder.py:83
 #: src/pyams_content/shared/form/interfaces.py:49
 #: src/pyams_content/shared/view/portlet/interfaces.py:64
@@ -150,15 +155,15 @@
 msgstr "Dernière modification"
 
 #: src/pyams_content/zmi/viewlet/toplinks.py:37
 msgid "Shortcuts"
 msgstr "Contenus"
 
 #: src/pyams_content/reference/zmi/table.py:51
-#: src/pyams_content/shared/site/zmi/manager.py:166
+#: src/pyams_content/shared/site/zmi/manager.py:167
 #: src/pyams_content/shared/site/zmi/folder.py:180
 #: src/pyams_content/shared/common/zmi/manager.py:82
 #: src/pyams_content/shared/common/zmi/__init__.py:305
 #: src/pyams_content/root/zmi/__init__.py:63
 msgid "Properties"
 msgstr "Propriétés"
 
@@ -530,14 +535,22 @@
 msgstr "demande de publication annulée"
 
 #: src/pyams_content/workflow/basic.py:482
 #: src/pyams_content/workflow/__init__.py:894
 msgid "publication refused"
 msgstr "publication refusée"
 
+#: src/pyams_content/workflow/task.py:52
+msgid "Content publisher task"
+msgstr "Publication d'un contenu"
+
+#: src/pyams_content/workflow/task.py:88
+msgid "Content archiver task"
+msgstr "Archivage d'un contenu"
+
 #: src/pyams_content/workflow/__init__.py:84
 msgid "Proposed"
 msgstr "Proposé à la publication"
 
 #: src/pyams_content/workflow/__init__.py:85
 msgid "Canceled"
 msgstr "Annulé"
@@ -808,15 +821,15 @@
 msgstr "Commentaire"
 
 #: src/pyams_content/feature/review/interfaces.py:73
 msgid "Reviewer comment?"
 msgstr "Commentaire d'un relecteur"
 
 #: src/pyams_content/feature/review/interfaces.py:77
-#: src/pyams_content/interfaces/__init__.py:125
+#: src/pyams_content/interfaces/__init__.py:128
 #: src/pyams_content/shared/common/zmi/search.py:225
 #: src/pyams_content/root/zmi/search.py:160
 msgid "Creation date"
 msgstr "Date de création"
 
 #: src/pyams_content/feature/review/interfaces.py:89
 msgid "Reviewers list"
@@ -1025,14 +1038,15 @@
 msgstr "Menu de navigation"
 
 #: src/pyams_content/feature/navigation/interfaces.py:84
 #: src/pyams_content/component/paragraph/interfaces/__init__.py:49
 #: src/pyams_content/component/association/interfaces.py:42
 #: src/pyams_content/shared/site/interfaces.py:223
 #: src/pyams_content/shared/common/interfaces/types.py:52
+#: src/pyams_content/shared/alert/interfaces.py:46
 msgid "Visible?"
 msgstr "Visible ?"
 
 #: src/pyams_content/feature/navigation/interfaces.py:85
 #: src/pyams_content/component/association/interfaces.py:43
 msgid "Is this item visible in front-office?"
 msgstr "Cet élément est-il visible en front-office ?"
@@ -1042,15 +1056,15 @@
 msgstr "Titre"
 
 #: src/pyams_content/feature/navigation/interfaces.py:93
 msgid "Displayed menu label"
 msgstr "Libellé affiché pour ce menu"
 
 #: src/pyams_content/feature/navigation/interfaces.py:96
-#: src/pyams_content/shared/alert/interfaces.py:76
+#: src/pyams_content/shared/alert/interfaces.py:98
 msgid "Internal reference"
 msgstr "Référence interne"
 
 #: src/pyams_content/feature/navigation/interfaces.py:97
 msgid "Direct reference to menu target"
 msgstr ""
 "Référence directe vers la cible du lien, identifiée à partir de son numéro "
@@ -1080,14 +1094,15 @@
 "Si 'oui', les éléments de ce menu seront créés dynamiquement à partir du "
 "contenu de la référence interne ; s'il y a également des éléments définis "
 "manuellement au sein du menu, ceux-ci seront positionnés ensuite"
 
 #: src/pyams_content/feature/navigation/interfaces.py:113
 #: src/pyams_content/component/links/interfaces.py:49
 #: src/pyams_content/shared/common/interfaces/types.py:83
+#: src/pyams_content/shared/alert/interfaces.py:59
 msgid "Pictogram"
 msgstr "Pictogramme"
 
 #: src/pyams_content/feature/navigation/interfaces.py:114
 msgid ""
 "Name of the pictogram associated with this menu; pictogram display may "
 "depend on selected renderer and skin"
@@ -1116,14 +1131,15 @@
 
 #: src/pyams_content/feature/navigation/zmi/__init__.py:171
 msgid "Menu properties"
 msgstr "Propriétés du menu"
 
 #: src/pyams_content/feature/navigation/portlet/interfaces.py:34
 #: src/pyams_content/feature/navigation/portlet/interfaces.py:48
+#: src/pyams_content/feature/search/portlet/interfaces.py:45
 msgid "Portlet main title"
 msgstr "Titre du composant"
 
 #: src/pyams_content/feature/navigation/portlet/__init__.py:63
 msgid "Simple navigation menu"
 msgstr "Liens de navigation à un niveau"
 
@@ -1148,18 +1164,21 @@
 #: src/pyams_content/component/gallery/portlet/skin/interfaces.py:56
 #: src/pyams_content/component/gallery/skin/interfaces.py:44
 #: src/pyams_content/component/gallery/skin/interfaces.py:55
 msgid "Images selection"
 msgstr "Sélection des images"
 
 #: src/pyams_content/feature/navigation/portlet/skin/interfaces.py:31
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:100
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:117
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:134
 #: src/pyams_content/component/gallery/portlet/skin/interfaces.py:32
 #: src/pyams_content/component/gallery/skin/interfaces.py:31
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:83
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:130
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:74
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:121
 msgid "Selection used to display images thumbnails"
 msgstr "Sélections utilisées pour l'affichage des vignettes"
 
 #: src/pyams_content/feature/navigation/portlet/skin/__init__.py:65
 msgid "Horizontal grid links with illustrations (default)"
 msgstr "Grille de liens avec illustrations (par défaut)"
 
@@ -1192,20 +1211,20 @@
 "selected view"
 msgstr ""
 "Référence de la vue dont sont extraites les alertes associées à un contexte, "
 "qui peuvent être affichées dans leur en-tête de page ; veuillez noter que la "
 "sélection du gabarit est effectuée automatiquement quel que soit le "
 "paramétrage de la vue sélectionnée"
 
-#: src/pyams_content/feature/alert/zmi/__init__.py:41
-#: src/pyams_content/feature/alert/zmi/__init__.py:51
+#: src/pyams_content/feature/alert/zmi/__init__.py:43
+#: src/pyams_content/feature/alert/zmi/__init__.py:53
 msgid "Alerts management"
 msgstr "Paramétrage des alertes"
 
-#: src/pyams_content/feature/alert/zmi/__init__.py:52
+#: src/pyams_content/feature/alert/zmi/__init__.py:54
 msgid "Alerts management views"
 msgstr "Sélection des vues associées aux alertes"
 
 #: src/pyams_content/feature/alert/skin/templates/alerts.pt:17
 #: src/pyams_content/feature/alert/skin/templates/alerts.pt:22
 #: src/pyams_content/feature/alert/skin/templates/context-alerts.pt:19
 #: src/pyams_content/feature/alert/skin/templates/context-alerts.pt:24
@@ -1318,19 +1337,19 @@
 
 #: src/pyams_content/feature/search/interfaces.py:108
 #: src/pyams_content/shared/site/interfaces.py:127
 msgid "Visible in folders list"
 msgstr "Visible dans la liste des rubriques"
 
 #: src/pyams_content/feature/search/interfaces.py:109
-#: src/pyams_content/shared/site/interfaces.py:128
-msgid "If 'no', folder will not be displayed into folders list"
+msgid ""
+"If 'no', search folder will not be displayed into parent's contents list"
 msgstr ""
-"Si 'non', la rubrique ne sera pas affichée dans la liste des rubriques du "
-"niveau parent"
+"Si 'non', le moteur de recherche ne sera pas affiché dans la liste des "
+"contenus du niveau parent"
 
 #: src/pyams_content/feature/search/interfaces.py:114
 #: src/pyams_content/shared/site/interfaces.py:133
 #: src/pyams_content/shared/site/interfaces.py:206
 msgid "Navigation title"
 msgstr "Libellé de navigation"
 
@@ -1360,23 +1379,333 @@
 
 #: src/pyams_content/feature/search/interfaces.py:126
 msgid "Searched data types; leave empty for all"
 msgstr ""
 "Type de contenus à sélectionner ; laisser la sélection vide pour accepter "
 "tous les types de contenus"
 
+#: src/pyams_content/feature/search/__init__.py:42
+msgid "Search folder"
+msgstr "Moteur de recherche"
+
+#: src/pyams_content/feature/search/zmi/thesaurus.py:39
+#: src/pyams_content/component/thesaurus/zmi/manager.py:78
+#: src/pyams_content/component/thesaurus/zmi/manager.py:88
+#: src/pyams_content/shared/view/zmi/thesaurus.py:66
+msgid "Tags settings"
+msgstr "Paramétrage des tags"
+
+#: src/pyams_content/feature/search/zmi/thesaurus.py:40
+msgid "Search folder tags settings"
+msgstr "Tags appliqués par le moteur de recherche"
+
+#: src/pyams_content/feature/search/zmi/thesaurus.py:62
+#: src/pyams_content/component/thesaurus/zmi/manager.py:130
+#: src/pyams_content/component/thesaurus/zmi/manager.py:140
+#: src/pyams_content/shared/view/zmi/thesaurus.py:114
+msgid "Themes settings"
+msgstr "Paramétrage des thèmes"
+
+#: src/pyams_content/feature/search/zmi/thesaurus.py:63
+msgid "Search folder themes settings"
+msgstr "Thèmes appliqués par le moteur de recherche"
+
+#: src/pyams_content/feature/search/zmi/thesaurus.py:85
+#: src/pyams_content/component/thesaurus/zmi/manager.py:164
+#: src/pyams_content/component/thesaurus/zmi/manager.py:174
+#: src/pyams_content/shared/view/zmi/thesaurus.py:162
+msgid "Collections settings"
+msgstr "Paramétrage des collections"
+
+#: src/pyams_content/feature/search/zmi/thesaurus.py:86
+msgid "Search folder collections settings"
+msgstr "Collections appliquées par le moteur de recherche"
+
 #: src/pyams_content/feature/search/zmi/manager.py:50
 #: src/pyams_content/feature/search/zmi/manager.py:60
 msgid "Search settings"
 msgstr "Paramétrage de la recherche"
 
 #: src/pyams_content/feature/search/zmi/manager.py:61
 msgid "General search settings"
 msgstr "Propriétés du moteur de recherche général"
 
+#: src/pyams_content/feature/search/zmi/__init__.py:65
+msgid "Add search folder..."
+msgstr "Moteur de recherche"
+
+#: src/pyams_content/feature/search/zmi/__init__.py:82
+msgid "New search folder"
+msgstr "Nouveau moteur de recherche"
+
+#: src/pyams_content/feature/search/zmi/__init__.py:83
+msgid "New search folder properties"
+msgstr "Propriétés du nouveau moteur de recherche"
+
+#: src/pyams_content/feature/search/zmi/__init__.py:106
+msgid "Search folder management"
+msgstr "Ce moteur de recherche"
+
+#: src/pyams_content/feature/search/zmi/__init__.py:136
+msgid "Folder search settings"
+msgstr "Paramètres de la recherche"
+
+#: src/pyams_content/feature/search/zmi/__init__.py:156
+#: src/pyams_content/shared/site/zmi/folder.py:222
+msgid "Navigation properties"
+msgstr "Propriétés de navigation"
+
+#: src/pyams_content/feature/search/portlet/interfaces.py:48
+msgid "Allow empty query?"
+msgstr "Recherche sans critère"
+
+#: src/pyams_content/feature/search/portlet/interfaces.py:49
+msgid ""
+"If 'no', no result will be displayed if user didn't entered a search string"
+msgstr ""
+"Si cette option n'est pas sélectionnée, aucun résultat ne sera renvoyé si "
+"l'utilisateur ne saisit pas de critère de recherche"
+
+#: src/pyams_content/feature/search/portlet/interfaces.py:54
+#: src/pyams_content/component/links/interfaces.py:67
+#: src/pyams_content/shared/view/portlet/interfaces.py:111
+msgid "Force canonical URL?"
+msgstr "Imposer l'URL canonique"
+
+#: src/pyams_content/feature/search/portlet/interfaces.py:55
+#: src/pyams_content/component/links/interfaces.py:68
+#: src/pyams_content/shared/view/portlet/interfaces.py:112
+msgid ""
+"By default, internal links use a \"relative\" URL, which tries to display "
+"link target in the current context; by using a canonical URL, you can "
+"display target in it's attachment context (if defined)"
+msgstr ""
+"Par défaut, les liens internes utilisent une URl \"relative\", qui tente "
+"d'afficher la cible du lien dans le contexte courant ; en utilisant une URL "
+"canonique, vous pouvez imposer l'affichage de ce contenu dans son contexte "
+"d'origine, s'il est défini"
+
+#: src/pyams_content/feature/search/portlet/__init__.py:113
+#: src/pyams_content/shared/common/zmi/owner.py:362
+#: src/pyams_content/shared/common/zmi/search.py:430
+msgid "Search results"
+msgstr "Résultats de la recherche"
+
+#: src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt:5
+msgid "First search results sample:"
+msgstr "Premiers résultats de la recherche :"
+
+#: src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt:15
+msgid "No result found."
+msgstr "Aucun résultat trouvé"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:44
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:51
+msgid "Display full header"
+msgstr "Afficher le chapô en entier"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:45
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:52
+msgid "Display only header start"
+msgstr "Afficher seulement le début du chapô"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:46
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:53
+msgid "Hide header"
+msgstr "Masquer le chapô"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:59
+msgid "Display if empty?"
+msgstr "Afficher sans résultat"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:60
+msgid ""
+"If 'no', and if no result is found, the portlet will not display anything"
+msgstr ""
+"Si cette option n'est pas sélectionnée et qu'aucun résultat n'est trouvé, le "
+"composant ne sera pas affiché"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:65
+msgid "Display results count?"
+msgstr "Afficher le nombre de résultats"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:66
+msgid "If 'no', results count will not be displayed"
+msgstr ""
+"Le nombre de résultats de la recherche ne sera affiché que si cette option "
+"est sélectionnée"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:70
+msgid "Allow results sorting?"
+msgstr "Autoriser le tri"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:71
+msgid "If 'no', results will not be sortable"
+msgstr ""
+"Le tri des résultats ne sera possible que si cette option est sélectionnée"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:75
+msgid "Allow pagination?"
+msgstr "Autoriser la pagination"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:76
+msgid "If 'no', results will not be paginated"
+msgstr ""
+"LA navigation entre les pages de résultats ne sera possible que si cette "
+"option est sélectionnée"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:80
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:164
+msgid "Header display mode"
+msgstr "Affichage du chapô"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:81
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:165
+msgid "Defines how results headers will be rendered"
+msgstr "Mode d'affichage du chapô des résultats"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:86
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:170
+msgid "Start length"
+msgstr "Longueur du chapô"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:87
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:171
+msgid ""
+"If you choose to display only header start, you can specify maximum text "
+"length"
+msgstr ""
+"Si vous choisissez de n'afficher que le début du chapô, indiquer ici la "
+"longueur maximale du texte en nombre de caractères"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:92
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:66
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:135
+msgid "Display illustrations?"
+msgstr "Afficher l'illustration"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:93
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:67
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:136
+msgid "If 'no', view contents will not display illustrations"
+msgstr "Si 'non', l'illustration des résultats ne sera pas affichée"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:99
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:116
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:133
+#: src/pyams_content/component/gallery/portlet/skin/interfaces.py:31
+#: src/pyams_content/component/gallery/skin/interfaces.py:30
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:73
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:120
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:142
+msgid "Thumbnails selection"
+msgstr "Sélection des vignettes"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:124
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:141
+msgid "Button's title"
+msgstr "Libellé du bouton"
+
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:125
+#: src/pyams_content/feature/search/portlet/skin/interfaces.py:142
+msgid "Optional navigation button's title"
+msgstr ""
+"Un bouton de navigation associé à chaque résultat de recherche sera affiché "
+"si cette option est sélectionnée"
+
+#: src/pyams_content/feature/search/portlet/skin/zmi.py:83
+#: src/pyams_content/shared/view/portlet/skin/zmi.py:55
+msgid "Header display"
+msgstr "Affichage du chapô"
+
+#: src/pyams_content/feature/search/portlet/skin/__init__.py:107
+msgid "Paginated search results (default)"
+msgstr "Liste de résultats, sans facettes (par défaut)"
+
+#: src/pyams_content/feature/search/portlet/skin/__init__.py:133
+msgid "Paneled search results"
+msgstr "Grille de résultats, sans facettes, style « page carrefour »"
+
+#: src/pyams_content/feature/search/portlet/skin/__init__.py:159
+msgid "Bootstrap cards search results"
+msgstr "Grille de résultats, sans facettes, style « cartes Bootstrap »"
+
+#: src/pyams_content/feature/search/portlet/skin/__init__.py:182
+msgid "Bootstrap Masonry cards search results"
+msgstr "Grille de résultats, sans facettes, style « Masonry »"
+
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:27
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:27
+#: src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:27
+#: src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:27
+msgid "${count} result(s) found"
+msgstr "${count} résultat(s) trouvé(s)"
+
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:32
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:32
+#: src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:32
+#: src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:32
+msgid "No result found!"
+msgstr "Aucun résultat trouvé !"
+
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:41
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:41
+#: src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:41
+#: src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:41
+msgid "Sort by relevance"
+msgstr "Trier par pertinence"
+
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:44
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:44
+#: src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:44
+#: src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:44
+msgid "Sort by publication date"
+msgstr "Trier sur la date de publication"
+
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:47
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:47
+#: src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:47
+#: src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:47
+msgid "Sort by last modification date"
+msgstr "Trier sur la date de dernière modification"
+
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:53
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:53
+#: src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:53
+#: src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:53
+msgid "Page length:"
+msgstr "Longueur des pages :"
+
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:73
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:73
+#: src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:73
+#: src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:70
+#: src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt:60
+#: src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt:51
+msgid "Pagination"
+msgstr "Pagination"
+
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:82
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:82
+#: src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:82
+#: src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:79
+#: src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt:68
+#: src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt:59
+msgid "Previous page"
+msgstr "Page précédente"
+
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:120
+#: src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:120
+#: src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:120
+#: src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:117
+#: src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt:75
+#: src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt:66
+msgid "Next page"
+msgstr "Page suivante"
+
 #: src/pyams_content/feature/renderer/__init__.py:139
 msgid "Hidden content"
 msgstr "NON affiché"
 
 #: src/pyams_content/feature/renderer/__init__.py:153
 msgid "Default content renderer"
 msgstr "Mode de rendu par défaut"
@@ -1432,46 +1761,50 @@
 msgid "Preview"
 msgstr "Aperçu"
 
 #: src/pyams_content/feature/preview/zmi/__init__.py:75
 msgid "Open preview in new tab"
 msgstr "Ouvrir l'aperçu dans un nouvel onglet"
 
-#: src/pyams_content/interfaces/__init__.py:107
+#: src/pyams_content/interfaces/__init__.py:110
 msgid "Unique key"
 msgstr "Nom du contenu"
 
-#: src/pyams_content/interfaces/__init__.py:108
+#: src/pyams_content/interfaces/__init__.py:111
 msgid ""
 "WARNING: this key can't be modified after creation!!! Spaces, uppercase "
 "letters or accentuated characters will be replaced automatically."
 msgstr ""
 "ATTENTION : cette clé ne pourra pas être modifiée après sa création ! Les "
 "espaces, majuscules et caractères accentués seront remplacés "
 "automatiquement..."
 
-#: src/pyams_content/interfaces/__init__.py:114
+#: src/pyams_content/interfaces/__init__.py:117
 #: src/pyams_content/shared/site/zmi/folder.py:84
 msgid "Visible label used to display content"
 msgstr "Libellé principal du contenu"
 
-#: src/pyams_content/interfaces/__init__.py:117
+#: src/pyams_content/interfaces/__init__.py:120
 msgid "Short name"
 msgstr "Fil d'Ariane"
 
-#: src/pyams_content/interfaces/__init__.py:118
+#: src/pyams_content/interfaces/__init__.py:121
 msgid "Short name used in breadcrumbs"
 msgstr "Libellé court visible dans le fil d'Ariane"
 
-#: src/pyams_content/interfaces/__init__.py:129
+#: src/pyams_content/interfaces/__init__.py:132
 #: src/pyams_content/shared/common/zmi/search.py:228
 #: src/pyams_content/root/zmi/search.py:163
 msgid "Modification date"
 msgstr "Date de dernière modification"
 
+#: src/pyams_content/interfaces/__init__.py:144
+msgid "Object types"
+msgstr "Types de l'objet"
+
 #: src/pyams_content/component/illustration/interfaces.py:44
 #: src/pyams_content/component/illustration/interfaces.py:120
 #: src/pyams_content/component/gallery/interfaces.py:48
 msgid "Image or video data"
 msgstr "Contenu"
 
 #: src/pyams_content/component/illustration/interfaces.py:45
@@ -1535,31 +1868,31 @@
 msgid "Illustration"
 msgstr "Illustration"
 
 #: src/pyams_content/component/illustration/interfaces.py:129
 msgid "Presentation template used for illustration"
 msgstr "Mode de rendu utilisé pour ce bloc"
 
-#: src/pyams_content/component/illustration/zmi/thesaurus.py:39
+#: src/pyams_content/component/illustration/zmi/thesaurus.py:41
 msgid "Associated illustration"
 msgstr "Illustration associée"
 
-#: src/pyams_content/component/illustration/zmi/thesaurus.py:40
+#: src/pyams_content/component/illustration/zmi/thesaurus.py:42
 msgid "Illustration properties"
 msgstr "Propriétés de l'illustration"
 
-#: src/pyams_content/component/illustration/zmi/__init__.py:45
+#: src/pyams_content/component/illustration/zmi/__init__.py:46
 msgid "Main illustration"
 msgstr "Illustration principale"
 
-#: src/pyams_content/component/illustration/zmi/__init__.py:87
+#: src/pyams_content/component/illustration/zmi/__init__.py:91
 msgid "Navigation link illustration"
 msgstr "Illustration de navigation"
 
-#: src/pyams_content/component/illustration/zmi/__init__.py:126
+#: src/pyams_content/component/illustration/zmi/__init__.py:133
 msgid "Use responsive selection"
 msgstr "Utiliser les sélections responsives"
 
 #: src/pyams_content/component/illustration/portlet/skin/interfaces.py:33
 #: src/pyams_content/component/illustration/portlet/skin/interfaces.py:64
 #: src/pyams_content/component/illustration/skin/interfaces.py:49
 #: src/pyams_content/component/illustration/skin/interfaces.py:61
@@ -1611,24 +1944,24 @@
 msgid ""
 "If 'yes', a click on illustration thumbnail will open a modal window to "
 "display image"
 msgstr ""
 "Si 'oui', un clic sur l'illustration provoque l'ouverture d'une fenêtre "
 "modale pour afficher l'intégralité de l'image"
 
-#: src/pyams_content/component/illustration/portlet/skin/__init__.py:92
+#: src/pyams_content/component/illustration/portlet/skin/__init__.py:89
 msgid "Full width illustration (default)"
 msgstr "Illustration simple (par défaut)"
 
-#: src/pyams_content/component/illustration/portlet/skin/__init__.py:136
+#: src/pyams_content/component/illustration/portlet/skin/__init__.py:133
 #: src/pyams_content/component/illustration/skin/illustration.py:103
 msgid "Floating illustration to the left"
 msgstr "Illustration placée à gauche du texte"
 
-#: src/pyams_content/component/illustration/portlet/skin/__init__.py:157
+#: src/pyams_content/component/illustration/portlet/skin/__init__.py:154
 #: src/pyams_content/component/illustration/skin/illustration.py:115
 msgid "Floating illustration to the right"
 msgstr "Illustration placée à droite du texte"
 
 #: src/pyams_content/component/illustration/skin/illustration.py:81
 msgid "Centered image before text"
 msgstr "Illustration centrée avant le texte"
@@ -1760,20 +2093,20 @@
 msgid "Internal videos"
 msgstr "Vidéos téléchargeables"
 
 #: src/pyams_content/component/extfile/zmi/paragraph.py:84
 msgid "Internal audio files"
 msgstr "Bandes son téléchargeables"
 
-#: src/pyams_content/component/extfile/zmi/manager.py:43
-#: src/pyams_content/component/extfile/zmi/manager.py:53
+#: src/pyams_content/component/extfile/zmi/manager.py:45
+#: src/pyams_content/component/extfile/zmi/manager.py:55
 msgid "External files settings"
 msgstr "Paramétrage des pièces jointes"
 
-#: src/pyams_content/component/extfile/zmi/manager.py:54
+#: src/pyams_content/component/extfile/zmi/manager.py:56
 msgid "Default prefix"
 msgstr "Propriétés des pièces jointes"
 
 #: src/pyams_content/component/extfile/zmi/__init__.py:59
 msgid "New file properties"
 msgstr "Propriétés du nouveau fichier"
 
@@ -1825,19 +2158,19 @@
 msgid "Bootstrap cards"
 msgstr "Bootstrap: cartes"
 
 #: src/pyams_content/component/cards/interfaces.py:36
 msgid "Presentation template used for cards"
 msgstr "Mode de rendu utilisé pour ce bloc de contenu"
 
-#: src/pyams_content/component/cards/skin/__init__.py:47
+#: src/pyams_content/component/cards/skin/__init__.py:48
 msgid "Bootstrap cards renderer (default)"
 msgstr "Cartes Bootstrap (par défaut)"
 
-#: src/pyams_content/component/cards/skin/__init__.py:66
+#: src/pyams_content/component/cards/skin/__init__.py:67
 msgid "Bootstrap cards Masonry renderer"
 msgstr "Cartes Bootstrap avec rendu Masonry"
 
 #: src/pyams_content/component/paragraph/zmi/container.py:158
 msgid "Click to set/unset paragraph as navigation anchor"
 msgstr "Cliquer pour (dés)activer l'ancre de navigation sur ce bloc"
 
@@ -2169,31 +2502,31 @@
 msgid "Paragraphs navigation (default)"
 msgstr "Navigation au sein des blocs (par défaut)"
 
 #: src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt:28
 msgid "Previous and next topics"
 msgstr "Contenus précédent et suivant"
 
-#: src/pyams_content/component/paragraph/skin/html.py:55
+#: src/pyams_content/component/paragraph/skin/html.py:56
 msgid "HTML source code (default)"
 msgstr "Code source HTML (par défaut)"
 
-#: src/pyams_content/component/paragraph/skin/html.py:65
+#: src/pyams_content/component/paragraph/skin/html.py:66
 msgid "Formatted source code"
 msgstr "Code source formatté"
 
-#: src/pyams_content/component/paragraph/skin/html.py:107
+#: src/pyams_content/component/paragraph/skin/html.py:108
 msgid "ReStructured text"
 msgstr "Texte restructuré"
 
-#: src/pyams_content/component/paragraph/skin/html.py:132
+#: src/pyams_content/component/paragraph/skin/html.py:133
 msgid "Markdown text"
 msgstr "Markdown"
 
-#: src/pyams_content/component/paragraph/skin/html.py:189
+#: src/pyams_content/component/paragraph/skin/html.py:190
 msgid "Rich text (default)"
 msgstr "Texte enrichi (par défaut)"
 
 #: src/pyams_content/component/paragraph/skin/interfaces/html.py:31
 msgid "XS horizontal padding"
 msgstr "Marge sur smartphones"
 
@@ -2250,31 +2583,14 @@
 msgstr "Sélection du pictogramme associé à ce lien"
 
 #: src/pyams_content/component/links/interfaces.py:61
 #: src/pyams_content/shared/site/link.py:83
 msgid "Internal link"
 msgstr "Lien interne"
 
-#: src/pyams_content/component/links/interfaces.py:67
-#: src/pyams_content/shared/view/portlet/interfaces.py:111
-msgid "Force canonical URL?"
-msgstr "Imposer l'URL canonique"
-
-#: src/pyams_content/component/links/interfaces.py:68
-#: src/pyams_content/shared/view/portlet/interfaces.py:112
-msgid ""
-"By default, internal links use a \"relative\" URL, which tries to display "
-"link target in the current context; by using a canonical URL, you can "
-"display target in it's attachment context (if defined)"
-msgstr ""
-"Par défaut, les liens internes utilisent une URl \"relative\", qui tente "
-"d'afficher la cible du lien dans le contexte courant ; en utilisant une URL "
-"canonique, vous pouvez imposer l'affichage de ce contenu dans son contexte "
-"d'origine, s'il est défini"
-
 #: src/pyams_content/component/links/interfaces.py:89
 msgid ""
 "Marker interface provided by links directed to contents supporting this "
 "interface"
 msgstr ""
 "Interface de marquage fournie par les liens vers des contenus supportant "
 "cette interface"
@@ -2514,39 +2830,32 @@
 "médias de cette galerie seront intégrés automatiquement en plus de ceux "
 "ajoutés au niveau du composant"
 
 #: src/pyams_content/component/gallery/portlet/zmi/templates/gallery-preview.pt:3
 msgid "Medias list:"
 msgstr "Liste de médias :"
 
-#: src/pyams_content/component/gallery/portlet/skin/interfaces.py:31
-#: src/pyams_content/component/gallery/skin/interfaces.py:30
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:82
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:129
-msgid "Thumbnails selection"
-msgstr "Sélection des vignettes"
-
 #: src/pyams_content/component/gallery/portlet/skin/interfaces.py:46
 #: src/pyams_content/component/gallery/portlet/skin/interfaces.py:57
 #: src/pyams_content/component/gallery/skin/interfaces.py:45
 #: src/pyams_content/component/gallery/skin/interfaces.py:56
 msgid "Selection used to display images"
 msgstr "Sélections utilisées pour l'affichage des images"
 
-#: src/pyams_content/component/gallery/portlet/skin/__init__.py:77
+#: src/pyams_content/component/gallery/portlet/skin/__init__.py:76
 #: src/pyams_content/component/gallery/skin/__init__.py:68
 msgid "Grid gallery renderer (default)"
 msgstr "Grille de vignettes (par défaut)"
 
-#: src/pyams_content/component/gallery/portlet/skin/__init__.py:101
+#: src/pyams_content/component/gallery/portlet/skin/__init__.py:100
 #: src/pyams_content/component/gallery/skin/__init__.py:93
 msgid "Carousel gallery renderer"
 msgstr "Carousel horizontal"
 
-#: src/pyams_content/component/gallery/portlet/skin/__init__.py:125
+#: src/pyams_content/component/gallery/portlet/skin/__init__.py:124
 #: src/pyams_content/component/gallery/skin/__init__.py:118
 msgid "Random image renderer"
 msgstr "Sélection d'une image aléatoire"
 
 #: src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt:48
 #: src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt:62
 #: src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt:47
@@ -2590,15 +2899,15 @@
 msgid "Size"
 msgstr "Taille"
 
 #: src/pyams_content/component/association/zmi/container.py:234
 msgid "Links and external files list"
 msgstr "Liste des liens et pièces jointes"
 
-#: src/pyams_content/component/association/skin/paragraph.py:38
+#: src/pyams_content/component/association/skin/paragraph.py:39
 msgid "Associations list (default)"
 msgstr "Liens et pièces jointes (par défaut)"
 
 #: src/pyams_content/component/video/interfaces.py:52
 msgid "Name of video's author"
 msgstr "Nom de l'auteur de la vidéo, sous la forme \"Prénom Nom / Organisme\""
 
@@ -2632,15 +2941,15 @@
 msgstr "Vous devez sélectionner un fournisseur de contenu !"
 
 #: src/pyams_content/component/video/zmi/paragraph.py:136
 #: src/pyams_content/component/video/zmi/paragraph.py:226
 msgid "Provider settings"
 msgstr "Propriétés de la vidéo"
 
-#: src/pyams_content/component/video/skin/__init__.py:37
+#: src/pyams_content/component/video/skin/__init__.py:38
 msgid "External video renderer (default)"
 msgstr "Vidéo intégrée dans la page (par défaut)"
 
 #: src/pyams_content/component/video/provider/vimeo.py:70
 msgid "Vimeo"
 msgstr "Vimeo"
 
@@ -2982,23 +3291,23 @@
 msgstr ""
 "Si un champ de saisie d'une adresse de messagerie est présent dans le "
 "formulaire, ce message de confirmation sera envoyé à cette adresse ; vous "
 "pouvez inclure des champs du formulaire en indiquant leur nom entre "
 "{accolades}, la référence de la soumission pouvant être indiquée avec le nom "
 "{_reference}"
 
-#: src/pyams_content/component/fields/handler/zmi/mail.py:43
+#: src/pyams_content/component/fields/handler/zmi/mail.py:45
 msgid "Mailto handler settings"
 msgstr "Notifications par email"
 
-#: src/pyams_content/component/fields/handler/zmi/mail.py:61
+#: src/pyams_content/component/fields/handler/zmi/mail.py:63
 msgid "Mailto notifications"
 msgstr "Notifications par email"
 
-#: src/pyams_content/component/fields/handler/zmi/mail.py:62
+#: src/pyams_content/component/fields/handler/zmi/mail.py:64
 msgid "Mailto form handler settings"
 msgstr "Paramètres des notifications"
 
 #: src/pyams_content/component/fields/skin/paragraph.py:55
 msgid "Form fields list (default)"
 msgstr "Champs de saisie (par défaut)"
 
@@ -3016,67 +3325,49 @@
 "Vous devez spécifier le glossaire utilisé par le thésaurus pour pouvoir "
 "l'activer"
 
 #: src/pyams_content/component/thesaurus/interfaces.py:67
 #: src/pyams_content/component/thesaurus/zmi/__init__.py:101
 #: src/pyams_content/shared/common/zmi/search.py:231
 #: src/pyams_content/shared/common/zmi/search.py:294
-#: src/pyams_content/shared/view/zmi/thesaurus.py:52
+#: src/pyams_content/shared/view/zmi/thesaurus.py:56
 #: src/pyams_content/root/zmi/search.py:166
 #: src/pyams_content/root/zmi/search.py:224
 msgid "Tags"
 msgstr "Tags"
 
 #: src/pyams_content/component/thesaurus/interfaces.py:94
 #: src/pyams_content/component/thesaurus/zmi/__init__.py:186
 #: src/pyams_content/shared/common/zmi/search.py:234
 #: src/pyams_content/shared/common/zmi/search.py:308
-#: src/pyams_content/shared/view/zmi/thesaurus.py:94
+#: src/pyams_content/shared/view/zmi/thesaurus.py:104
 #: src/pyams_content/root/zmi/search.py:169
 #: src/pyams_content/root/zmi/search.py:238
 msgid "Themes"
 msgstr "Thèmes"
 
 #: src/pyams_content/component/thesaurus/interfaces.py:121
 #: src/pyams_content/component/thesaurus/zmi/__init__.py:314
 #: src/pyams_content/shared/common/zmi/search.py:237
 #: src/pyams_content/shared/common/zmi/search.py:322
-#: src/pyams_content/shared/view/zmi/thesaurus.py:137
+#: src/pyams_content/shared/view/zmi/thesaurus.py:152
 #: src/pyams_content/root/zmi/search.py:172
 #: src/pyams_content/root/zmi/search.py:252
 msgid "Collections"
 msgstr "Collections"
 
-#: src/pyams_content/component/thesaurus/zmi/manager.py:79
 #: src/pyams_content/component/thesaurus/zmi/manager.py:89
-#: src/pyams_content/shared/view/zmi/thesaurus.py:62
-msgid "Tags settings"
-msgstr "Paramétrage des tags"
-
-#: src/pyams_content/component/thesaurus/zmi/manager.py:90
 msgid "Selected tags thesaurus"
 msgstr "Thésaurus des tags"
 
-#: src/pyams_content/component/thesaurus/zmi/manager.py:125
-#: src/pyams_content/component/thesaurus/zmi/manager.py:135
-#: src/pyams_content/shared/view/zmi/thesaurus.py:104
-msgid "Themes settings"
-msgstr "Paramétrage des thèmes"
-
-#: src/pyams_content/component/thesaurus/zmi/manager.py:136
+#: src/pyams_content/component/thesaurus/zmi/manager.py:141
 msgid "Selected themes thesaurus"
 msgstr "Thésaurus des thèmes"
 
-#: src/pyams_content/component/thesaurus/zmi/manager.py:156
-#: src/pyams_content/component/thesaurus/zmi/manager.py:166
-#: src/pyams_content/shared/view/zmi/thesaurus.py:147
-msgid "Collections settings"
-msgstr "Paramétrage des collections"
-
-#: src/pyams_content/component/thesaurus/zmi/manager.py:167
+#: src/pyams_content/component/thesaurus/zmi/manager.py:175
 msgid "Selected collections thesaurus"
 msgstr "Thésaurus des collections"
 
 #: src/pyams_content/component/thesaurus/zmi/__init__.py:108
 msgid "Content tags selection"
 msgstr "Sélection des tags du contenu"
 
@@ -3180,14 +3471,20 @@
 #: src/pyams_content/shared/site/zmi/folder.py:92
 #: src/pyams_content/shared/common/interfaces/__init__.py:196
 msgid "Internal information to be known about this content"
 msgstr ""
 "Informations internes à l'attention des contributeurs et des gestionnaires "
 "du site"
 
+#: src/pyams_content/shared/site/interfaces.py:128
+msgid "If 'no', folder will not be displayed into folders list"
+msgstr ""
+"Si 'non', la rubrique ne sera pas affichée dans la liste des rubriques du "
+"niveau parent"
+
 #: src/pyams_content/shared/site/interfaces.py:140
 msgid "Folder behaviour when navigating to folder URL"
 msgstr ""
 "Comportement attendu lorsqu'un utilisateur navigue vers l'URL de cette "
 "rubrique"
 
 #: src/pyams_content/shared/site/interfaces.py:162
@@ -3375,40 +3672,40 @@
 msgstr "Parmi les contenus du site « {} »"
 
 #: src/pyams_content/shared/site/zmi/search.py:60
 #, python-format
 msgid "Between all contents of « {} » site folder"
 msgstr "Parmi les contenus de la rubrique « {} »"
 
-#: src/pyams_content/shared/site/zmi/manager.py:66
-#: src/pyams_content/shared/site/zmi/manager.py:79
+#: src/pyams_content/shared/site/zmi/manager.py:65
+#: src/pyams_content/shared/site/zmi/manager.py:78
 msgid "Add site manager"
 msgstr "Ajouter un site"
 
-#: src/pyams_content/shared/site/zmi/manager.py:80
+#: src/pyams_content/shared/site/zmi/manager.py:79
 msgid "New site properties"
 msgstr "Propriétés du nouveau site"
 
-#: src/pyams_content/shared/site/zmi/manager.py:98
+#: src/pyams_content/shared/site/zmi/manager.py:99
 msgid "Site name is required!"
 msgstr "Le nom du site est obligatoire !"
 
-#: src/pyams_content/shared/site/zmi/manager.py:102
+#: src/pyams_content/shared/site/zmi/manager.py:103
 msgid "A site manager is already registered with this name!"
 msgstr "Autre site a déjà été enregistré sous ce nom !"
 
-#: src/pyams_content/shared/site/zmi/manager.py:155
+#: src/pyams_content/shared/site/zmi/manager.py:156
 msgid "Site management"
 msgstr "Gérer ce site"
 
-#: src/pyams_content/shared/site/zmi/manager.py:177
+#: src/pyams_content/shared/site/zmi/manager.py:178
 msgid "Site manager properties"
 msgstr "Propriétés du site"
 
-#: src/pyams_content/shared/site/zmi/manager.py:178
+#: src/pyams_content/shared/site/zmi/manager.py:179
 #: src/pyams_content/root/zmi/__init__.py:74
 msgid "Main site properties"
 msgstr "Propriétés principales du site"
 
 #: src/pyams_content/shared/site/zmi/folder.py:73
 msgid "Add site folder..."
 msgstr "Rubrique"
@@ -3429,18 +3726,14 @@
 msgid "Site folder properties"
 msgstr "Propriétés de la rubrique"
 
 #: src/pyams_content/shared/site/zmi/folder.py:192
 msgid "Main folder properties"
 msgstr "Propriétés principales"
 
-#: src/pyams_content/shared/site/zmi/folder.py:222
-msgid "Navigation properties"
-msgstr "Propriétés de navigation"
-
 #: src/pyams_content/shared/site/zmi/viewlet/__init__.py:40
 msgid "Sites"
 msgstr "Sites"
 
 #: src/pyams_content/shared/form/interfaces.py:38
 msgid "Form"
 msgstr "Formulaire"
@@ -3474,16 +3767,16 @@
 msgstr "En-tête du formulaire"
 
 #: src/pyams_content/shared/common/types.py:234
 #, python-format
 msgid "-- missing value ({}) --"
 msgstr "-- valeur manquante ({}) --"
 
-#: src/pyams_content/shared/common/__init__.py:118
-#: src/pyams_content/shared/common/__init__.py:127
+#: src/pyams_content/shared/common/__init__.py:117
+#: src/pyams_content/shared/common/__init__.py:126
 #, python-format
 msgid "{date} by {principal}"
 msgstr "{date} par {principal}"
 
 #: src/pyams_content/shared/common/zmi/workflow.py:61
 msgid "Workflow action"
 msgstr "Action du workflow"
@@ -3918,19 +4211,14 @@
 #: src/pyams_content/shared/common/zmi/owner.py:343
 #, python-format
 msgid "{} contents selected, owner changed successfully for {} contents"
 msgstr ""
 "{} contenu(s) sélectionné(s), le propriétaire a été modifié pour {} "
 "contenu(s)"
 
-#: src/pyams_content/shared/common/zmi/owner.py:362
-#: src/pyams_content/shared/common/zmi/search.py:430
-msgid "Search results"
-msgstr "Résultats de la recherche"
-
 #: src/pyams_content/shared/common/zmi/owner.py:410
 msgid "The selected user will become the new content's owner"
 msgstr "Le mandataire sélectionné deviendra le nouveau propriétaire du contenu"
 
 #: src/pyams_content/shared/common/zmi/owner.py:413
 msgid "If 'yes', the previous owner will still be able to modify this content"
 msgstr ""
@@ -4333,14 +4621,16 @@
 
 #: src/pyams_content/shared/common/zmi/types/container.py:99
 msgid "Click icon to enable or disable content type"
 msgstr "Cliquer pour activer ou désactiver ce type de contenu"
 
 #: src/pyams_content/shared/common/zmi/types/container.py:116
 #: src/pyams_content/shared/common/interfaces/types.py:57
+#: src/pyams_content/shared/alert/interfaces.py:51
+#: src/pyams_content/shared/alert/zmi/types.py:129
 msgid "Label"
 msgstr "Libellé"
 
 #: src/pyams_content/shared/common/zmi/types/container.py:144
 msgid "Shared tool content types list"
 msgstr "Liste des types de contenus"
 
@@ -4423,22 +4713,25 @@
 msgstr "Libellé de navigation"
 
 #: src/pyams_content/shared/common/interfaces/types.py:71
 msgid "Label used for navigation entries"
 msgstr "Libellé utilisé pour les liens de navigation"
 
 #: src/pyams_content/shared/common/interfaces/types.py:74
+#: src/pyams_content/shared/alert/interfaces.py:54
 msgid "Back-office label"
 msgstr "Libellé back-office"
 
 #: src/pyams_content/shared/common/interfaces/types.py:75
+#: src/pyams_content/shared/alert/interfaces.py:55
 msgid "Optional label used in management pages instead of default label"
 msgstr "Libellé utilisé en back-office, à la place du libellé standard"
 
 #: src/pyams_content/shared/common/interfaces/types.py:79
+#: src/pyams_content/shared/alert/interfaces.py:64
 msgid "Color"
 msgstr "Couleur"
 
 #: src/pyams_content/shared/common/interfaces/types.py:80
 msgid "Color used to illustrate this data type"
 msgstr "Couleur utilisée pour représenter ce type de contenu"
 
@@ -4789,24 +5082,24 @@
 "If enabled, and if a header illustration is associated with the content, "
 "it's selected ratio may vary according to the selected renderer"
 msgstr ""
 "Si une illustration d'en-tête est associée au contenu, la sélection qui sera "
 "affichée peut dépendre du mode de rendu sélectionné"
 
 #: src/pyams_content/shared/common/portlet/interfaces.py:68
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:93
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:84
 msgid "Display breadcrumbs?"
 msgstr "Afficher le fil d'Ariane"
 
 #: src/pyams_content/shared/common/portlet/interfaces.py:72
 msgid "Display title?"
 msgstr "Afficher le titre"
 
 #: src/pyams_content/shared/common/portlet/interfaces.py:76
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:99
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:90
 msgid "Display tags?"
 msgstr "Afficher les tags"
 
 #: src/pyams_content/shared/common/portlet/interfaces.py:80
 msgid "Display header?"
 msgstr "Afficher le chapô"
 
@@ -4833,106 +5126,132 @@
 msgid "Shared content header (default)"
 msgstr "En-tête du contenu (par défaut)"
 
 #: src/pyams_content/shared/common/portlet/skin/specificities.py:38
 msgid "Shared content specificities (default)"
 msgstr "Spécificités du contenu (par défaut)"
 
-#: src/pyams_content/shared/alert/interfaces.py:37
-#: src/pyams_content/shared/alert/interfaces.py:50
-msgid "Alert"
-msgstr "Alerte"
+#: src/pyams_content/shared/alert/interfaces.py:47
+msgid "An hidden alert type can't be assigned to new alerts"
+msgstr ""
+"Un type d'alerte inactif ne peut pas être affecté à de nouvelles alertes"
 
-#: src/pyams_content/shared/alert/interfaces.py:51
-msgid "End of alert"
-msgstr "Fin d'alerte"
+#: src/pyams_content/shared/alert/interfaces.py:60
+msgid "Pictogram associated with this alert type"
+msgstr "Nom du pictogramme associé à ce type d'alerte"
 
-#: src/pyams_content/shared/alert/interfaces.py:52
-msgid "Information"
-msgstr "Information"
-
-#: src/pyams_content/shared/alert/interfaces.py:53
-msgid "Warning"
-msgstr "Avertissement"
+#: src/pyams_content/shared/alert/interfaces.py:65
+msgid "Base color associated with this alert type"
+msgstr "Couleur de base associée à ce type d'alerte"
 
-#: src/pyams_content/shared/alert/interfaces.py:54
-msgid "Recommendation"
-msgstr "Recommandation"
+#: src/pyams_content/shared/alert/interfaces.py:80
+msgid "Alert"
+msgstr "Alerte"
 
-#: src/pyams_content/shared/alert/interfaces.py:66
-msgid "Alert gravity"
-msgstr "Niveau de gravité"
+#: src/pyams_content/shared/alert/interfaces.py:86
+#: src/pyams_content/shared/alert/zmi/types.py:223
+msgid "Alert type"
+msgstr "Type d'alerte"
 
-#: src/pyams_content/shared/alert/interfaces.py:67
-msgid "Alert gravity can affect renderer alert style"
+#: src/pyams_content/shared/alert/interfaces.py:87
+msgid "Alert type can affect renderer alert style"
 msgstr ""
-"Le niveau de gravité peut éventuellement, en fonction du thème graphique, "
+"Le type d'alerte peut éventuellement, en fonction du thème graphique, "
 "affecter le rendu de l'alerte"
 
-#: src/pyams_content/shared/alert/interfaces.py:72
+#: src/pyams_content/shared/alert/interfaces.py:94
 msgid "Message content"
 msgstr "Contenu du message"
 
-#: src/pyams_content/shared/alert/interfaces.py:73
+#: src/pyams_content/shared/alert/interfaces.py:95
 msgid "Message body"
 msgstr ""
 "Le contenu du message n'est en général affiché que dans le corps de page, et "
 "non lorsque les alertes sont affichées en bas de page"
 
-#: src/pyams_content/shared/alert/interfaces.py:77
+#: src/pyams_content/shared/alert/interfaces.py:99
 msgid ""
 "Internal link target reference. You can search a reference using '+' "
 "followed by internal number, or by entering text matching content title"
 msgstr ""
 "Référence interne de l'alerte vers un contenu à consulter ; vous pouvez "
 "rechercher une référence en indiquant un '+' suivi du numéro interne de ce "
 "moteur de recherche, ou en entrant tout ou partie de son titre"
 
-#: src/pyams_content/shared/alert/interfaces.py:83
+#: src/pyams_content/shared/alert/interfaces.py:105
 msgid "External URL"
 msgstr "URL externe"
 
-#: src/pyams_content/shared/alert/interfaces.py:84
+#: src/pyams_content/shared/alert/interfaces.py:106
 msgid "Alternate external URL"
 msgstr "Adresse d'une page externe à consulter"
 
-#: src/pyams_content/shared/alert/interfaces.py:90
+#: src/pyams_content/shared/alert/interfaces.py:112
 msgid "You can't set internal reference and external URI simultaneously!"
 msgstr ""
 "Vous ne pouvez pas indiquer une référence interne et une URI externe "
 "simultanément !"
 
-#: src/pyams_content/shared/alert/interfaces.py:92
+#: src/pyams_content/shared/alert/interfaces.py:114
 msgid "Concerned contents"
 msgstr "Contenus concernés"
 
-#: src/pyams_content/shared/alert/interfaces.py:93
+#: src/pyams_content/shared/alert/interfaces.py:115
 msgid "If any, these contents will automatically display this alert"
 msgstr ""
 "Si vous sélectionnez des contenus ici, cette alerte leur sera directement "
 "associée et elle pourra être affichée dans leur en-tête de page"
 
-#: src/pyams_content/shared/alert/interfaces.py:97
+#: src/pyams_content/shared/alert/interfaces.py:119
 msgid "Maximum interval"
 msgstr "Intervale d'affichage"
 
-#: src/pyams_content/shared/alert/interfaces.py:98
+#: src/pyams_content/shared/alert/interfaces.py:120
 msgid ""
 "Maximum interval between alert displays on a given device, given in hours; "
 "set to 0 to always display the alert"
 msgstr ""
 "Délai maximum entre deux affichages de l'alerte sur un périphérique donné, "
 "exprimé en heures ; indiquer une valeur de 0 pour que l'alerte soit toujours "
 "affichée"
 
-#: src/pyams_content/shared/alert/zmi/__init__.py:41
+#: src/pyams_content/shared/alert/zmi/types.py:62
+#: src/pyams_content/shared/alert/zmi/types.py:154
+msgid "Alert types"
+msgstr "Types d'alertes"
+
+#: src/pyams_content/shared/alert/zmi/types.py:112
+msgid "Click icon to enable or disable alert type"
+msgstr "Cliquer pour activer ou désactiver ce type d'alerte"
+
+#: src/pyams_content/shared/alert/zmi/types.py:157
+msgid "Alert types list"
+msgstr "Liste des types d'alertes"
+
+#: src/pyams_content/shared/alert/zmi/types.py:171
+msgid "Add alert type"
+msgstr "Ajouter un type d'alerte"
+
+#: src/pyams_content/shared/alert/zmi/types.py:181
+msgid "New alert type"
+msgstr "Nouveau type d'alerte"
+
+#: src/pyams_content/shared/alert/zmi/types.py:182
+msgid "New alert type properties"
+msgstr "Propriétés du nouveau type"
+
+#: src/pyams_content/shared/alert/zmi/types.py:238
+msgid "Alert type properties"
+msgstr "Propriétés du type d'alerte"
+
+#: src/pyams_content/shared/alert/zmi/__init__.py:55
 msgid "Alert management"
 msgstr "Cette alerte"
 
-#: src/pyams_content/shared/alert/zmi/__init__.py:59
+#: src/pyams_content/shared/alert/zmi/__init__.py:82
 msgid "Alert settings"
 msgstr "Paramètres de l'alerte"
 
 #: src/pyams_content/shared/view/merge.py:62
 msgid "Concatenate views items in order"
 msgstr "Concaténer les résultats de chaque vue dans l'ordre sélectionné"
 
@@ -4970,23 +5289,23 @@
 msgid "References settings"
 msgstr "Paramétrage des références internes"
 
 #: src/pyams_content/shared/view/zmi/references.py:61
 msgid "View internal references settings"
 msgstr "Références internes de la vue"
 
-#: src/pyams_content/shared/view/zmi/thesaurus.py:63
+#: src/pyams_content/shared/view/zmi/thesaurus.py:67
 msgid "View tags settings"
 msgstr "Tags de la vue"
 
-#: src/pyams_content/shared/view/zmi/thesaurus.py:105
+#: src/pyams_content/shared/view/zmi/thesaurus.py:115
 msgid "View themes settings"
 msgstr "Thèmes de la vue"
 
-#: src/pyams_content/shared/view/zmi/thesaurus.py:148
+#: src/pyams_content/shared/view/zmi/thesaurus.py:163
 msgid "View collections settings"
 msgstr "Collections de la vue"
 
 #: src/pyams_content/shared/view/zmi/__init__.py:48
 msgid "View management"
 msgstr "Cette vue"
 
@@ -5390,151 +5709,78 @@
 msgid "Views list:"
 msgstr "Vues sélectionnées :"
 
 #: src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt:14
 msgid "(no selected view)"
 msgstr "(aucune vue sélectionnée)"
 
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:43
-msgid "Initial selection"
-msgstr "Utiliser les images d'origine"
-
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:44
-msgid "Responsive selection"
-msgstr "Utiliser les sélections responsives"
-
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:45
-msgid "Portrait selection"
-msgstr "Utiliser la sélection en mode portrait"
-
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:46
-msgid "Panoramic selection"
-msgstr "Utiliser la sélection panoramique"
-
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:47
-msgid "Square selection"
-msgstr "Utiliser la sélection carrée"
-
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:61
-msgid "Display full header"
-msgstr "Afficher le chapô en entier"
-
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:62
-msgid "Display only header start"
-msgstr "Afficher seulement le début du chapô"
-
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:63
-msgid "Hide header"
-msgstr "Masquer le chapô"
-
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:75
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:144
-msgid "Display illustrations?"
-msgstr "Afficher l'illustration"
-
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:76
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:145
-msgid "If 'no', view contents will not display illustrations"
-msgstr "Si 'non', l'illustration des résultats ne sera pas affichée"
-
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:94
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:85
 msgid "If 'no', view items breadcrumbs will not be displayed"
 msgstr "Si 'non', le fil d'Ariane des résultats ne sera pas affiché"
 
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:100
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:91
 msgid "If 'no', view items tags will not be displayed"
 msgstr "Si 'non', les tags des résultats ne seront pas affichés"
 
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:104
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:150
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:95
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:154
 msgid "Paginate?"
 msgstr "Pagination"
 
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:105
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:151
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:96
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:155
 msgid "If 'no', results pagination will be disabled"
 msgstr "Si 'non', la pagination des résultats sera désactivée"
 
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:109
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:155
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:100
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:159
 msgid "Page size"
 msgstr "Taille des pages"
 
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:110
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:156
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:101
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:160
 msgid "Number of items per page, if pagination is enabled"
 msgstr "Nombre de résultats par page, si la pagination est activée"
 
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:114
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:105
 msgid "'See all' link target"
 msgstr "Cible du lien 'Voir tous les résultats'"
 
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:115
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:106
 msgid ""
 "Internal reference to site or search folder displaying full list of view's "
 "contents"
 msgstr ""
 "Référence interne d'un site ou d'un moteur de recherche permettant d'accéder "
 "à la liste complète des résultats"
 
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:120
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:111
 msgid "Link label"
 msgstr "Libellé du lien"
 
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:121
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:112
 msgid "Label of the link to full list page"
 msgstr "Libellé du lien permettant d'accéder à la liste complète des résultats"
 
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:160
-msgid "Header display mode"
-msgstr "Affichage du chapô"
-
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:161
-msgid "Defines how results headers will be rendered"
-msgstr "Mode d'affichage du chapô des résultats"
-
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:166
-msgid "Start length"
-msgstr "Longueur du chapô"
-
-#: src/pyams_content/shared/view/portlet/skin/interfaces.py:167
-msgid ""
-"If you choose to display only header start, you can specify maximum text "
-"length"
-msgstr ""
-"Si vous choisissez de n'afficher que le début du chapô, indiquer ici la "
-"longueur maximale du texte en nombre de caractères"
+#: src/pyams_content/shared/view/portlet/skin/interfaces.py:143
+msgid "Selection used to display illustrations thumbnails"
+msgstr "Sélections utilisées pour l'affichage des vignettes"
 
 #: src/pyams_content/shared/view/portlet/skin/__init__.py:97
 msgid "Simple vertical list (default)"
 msgstr "Liste verticale simple (par défaut)"
 
 #: src/pyams_content/shared/view/portlet/skin/__init__.py:121
 msgid "Horizontal thumbnails list"
 msgstr "Liste horizontale de vignettes"
 
-#: src/pyams_content/shared/view/portlet/skin/__init__.py:149
+#: src/pyams_content/shared/view/portlet/skin/__init__.py:150
 msgid "Three vertical panels with panoramic illustrations"
 msgstr "Panneaux avec illustrations panoramiques"
 
-#: src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt:58
-#: src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt:54
-msgid "Pagination"
-msgstr "Pagination"
-
-#: src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt:66
-#: src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt:62
-msgid "Previous page"
-msgstr "Page précédente"
-
-#: src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt:73
-#: src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt:69
-msgid "Next page"
-msgstr "Page suivante"
-
 #: src/pyams_content/shared/view/skin/templates/preview.pt:2
 msgid "View result items"
 msgstr "Contenu de la vue"
 
 #: src/pyams_content/shared/view/skin/templates/preview.pt:3
 msgid "WARNING: items displayed in this preview are out of context!!"
 msgstr ""
@@ -5653,28 +5899,52 @@
 msgid "Main site management"
 msgstr "Gérer le portail"
 
 #: src/pyams_content/root/zmi/__init__.py:75
 msgid "Site information"
 msgstr "Informations générales"
 
+#~ msgid "End of alert"
+#~ msgstr "Fin d'alerte"
+
+#~ msgid "Information"
+#~ msgstr "Information"
+
+#~ msgid "Warning"
+#~ msgstr "Avertissement"
+
+#~ msgid "Recommendation"
+#~ msgstr "Recommandation"
+
+#~ msgid "Initial selection"
+#~ msgstr "Utiliser les images d'origine"
+
+#~ msgid "Responsive selection"
+#~ msgstr "Utiliser les sélections responsives"
+
+#~ msgid "Portrait selection"
+#~ msgstr "Utiliser la sélection en mode portrait"
+
+#~ msgid "Panoramic selection"
+#~ msgstr "Utiliser la sélection panoramique"
+
+#~ msgid "Square selection"
+#~ msgstr "Utiliser la sélection carrée"
+
 #~ msgid "No owner changed for empty selection!"
 #~ msgstr ""
 #~ "Pas de contenu sélectionné, aucun changement de propriétaire n'a été "
 #~ "effectué !"
 
-#, python-format
 #~ msgid "Manager restrictions: {}"
 #~ msgstr "Responsable : {}"
 
-#, python-format
 #~ msgid "Contributor restrictions: {}"
 #~ msgstr "Contributeur : {}"
 
-#, python-format
 #~ msgid "<small>Paragraph: {paragraph}</small><br />Renderer: {renderer}"
 #~ msgstr ""
 #~ "<small>Bloc de contenu : {paragraph}</small><br />Mode de rendu : "
 #~ "{renderer}"
 
 #~ msgid "Create new link"
 #~ msgstr "Ajouter un lien"
@@ -5684,32 +5954,26 @@
 
 #~ msgid "Add external link"
 #~ msgstr "Nouveau lien externe"
 
 #~ msgid "List of paragraphs allowed for this content type"
 #~ msgstr "Liste des types de blocs de contenu autorisés pour ce gabarit"
 
-#, python-format
 #~ msgid "Content type: {}"
 #~ msgstr "Type de contenu : {}"
 
 #~ msgid "Add external file"
 #~ msgstr "Nouveau fichier"
 
-#, python-format
 #~ msgid "<small>{}: {} (V {})</small><br />{}"
 #~ msgstr "<small>{} : {} (V {})</small><br />{}"
 
 #~ msgid "Alerts settings"
 #~ msgstr "Sélection des vues associées aux alertes"
 
-#~ msgid "Site alerts management"
-#~ msgstr "Paramétrage des alertes"
-
-#, fuzzy
 #~ msgid "Video provider settings"
 #~ msgstr "Notifications par email"
 
 #~ msgid "PyAMS default skin"
 #~ msgstr "PyAMS: thème par défaut"
 
 #~ msgid ""
```

### Comparing `pyams_content-1.99.0/src/pyams_content/locales/pyams_content.pot` & `pyams_content-1.99.1/src/pyams_content/locales/pyams_content.pot`

 * *Files 2% similar despite different names*

```diff
@@ -2,85 +2,89 @@
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2024-01-21 16:50+0100\n"
+"POT-Creation-Date: 2024-03-24 02:24+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 4.15.0\n"
 
 #: ./src/pyams_content/include.py:53
 msgid "Manage main site root properties"
 msgstr ""
 
 #: ./src/pyams_content/include.py:57
-msgid "Manage site, blog or hub properties"
+msgid "Manage first level site tree elements"
 msgstr ""
 
 #: ./src/pyams_content/include.py:61
-msgid "Manage shared tool properties"
+msgid "Manage site, blog or hub properties"
 msgstr ""
 
 #: ./src/pyams_content/include.py:65
-msgid "Create new content"
+msgid "Manage shared tool properties"
 msgstr ""
 
 #: ./src/pyams_content/include.py:69
-msgid "Create new version of existing content"
+msgid "Create new content"
 msgstr ""
 
 #: ./src/pyams_content/include.py:73
-msgid "Manage content properties"
+msgid "Create new version of existing content"
 msgstr ""
 
 #: ./src/pyams_content/include.py:77
-msgid "Comment existing content"
+msgid "Manage content properties"
 msgstr ""
 
 #: ./src/pyams_content/include.py:81
+msgid "Comment existing content"
+msgstr ""
+
+#: ./src/pyams_content/include.py:85
 msgid "Publish or retire existing content"
 msgstr ""
 
-#: ./src/pyams_content/include.py:96
+#: ./src/pyams_content/include.py:101
 msgid "Webmaster (role)"
 msgstr ""
 
-#: ./src/pyams_content/include.py:114
+#: ./src/pyams_content/include.py:120
 msgid "Pilot (role)"
 msgstr ""
 
-#: ./src/pyams_content/include.py:130
+#: ./src/pyams_content/include.py:136
 msgid "Manager (role)"
 msgstr ""
 
-#: ./src/pyams_content/include.py:146
+#: ./src/pyams_content/include.py:152
 msgid "Owner (role)"
 msgstr ""
 
-#: ./src/pyams_content/include.py:156
+#: ./src/pyams_content/include.py:162
 msgid "Contributor (role)"
 msgstr ""
 
-#: ./src/pyams_content/include.py:173
+#: ./src/pyams_content/include.py:179
 msgid "Reader (role)"
 msgstr ""
 
-#: ./src/pyams_content/include.py:190
+#: ./src/pyams_content/include.py:196
 msgid "Operator (role)"
 msgstr ""
 
-#: ./src/pyams_content/include.py:201
+#: ./src/pyams_content/include.py:207
 msgid "Guest user (role)"
 msgstr ""
 
 #: ./src/pyams_content/zmi/dashboard.py:84
 msgid "Switch element visibility"
 msgstr ""
 
@@ -88,15 +92,16 @@
 msgid "Visible element?"
 msgstr ""
 
 #: ./src/pyams_content/zmi/dashboard.py:112
 #: ./src/pyams_content/reference/zmi/table.py:99
 #: ./src/pyams_content/feature/navigation/portlet/interfaces.py:33
 #: ./src/pyams_content/feature/navigation/portlet/interfaces.py:47
-#: ./src/pyams_content/interfaces/__init__.py:113
+#: ./src/pyams_content/feature/search/portlet/interfaces.py:44
+#: ./src/pyams_content/interfaces/__init__.py:116
 #: ./src/pyams_content/component/paragraph/zmi/container.py:236
 #: ./src/pyams_content/component/paragraph/portlet/interfaces.py:33
 #: ./src/pyams_content/component/gallery/interfaces.py:118
 #: ./src/pyams_content/component/gallery/portlet/interfaces.py:33
 #: ./src/pyams_content/shared/site/zmi/folder.py:83
 #: ./src/pyams_content/shared/form/interfaces.py:49
 #: ./src/pyams_content/shared/view/portlet/interfaces.py:64
@@ -149,15 +154,15 @@
 msgstr ""
 
 #: ./src/pyams_content/zmi/viewlet/toplinks.py:37
 msgid "Shortcuts"
 msgstr ""
 
 #: ./src/pyams_content/reference/zmi/table.py:51
-#: ./src/pyams_content/shared/site/zmi/manager.py:166
+#: ./src/pyams_content/shared/site/zmi/manager.py:167
 #: ./src/pyams_content/shared/site/zmi/folder.py:180
 #: ./src/pyams_content/shared/common/zmi/manager.py:82
 #: ./src/pyams_content/shared/common/zmi/__init__.py:305
 #: ./src/pyams_content/root/zmi/__init__.py:63
 msgid "Properties"
 msgstr ""
 
@@ -514,14 +519,22 @@
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:482
 #: ./src/pyams_content/workflow/__init__.py:894
 msgid "publication refused"
 msgstr ""
 
+#: ./src/pyams_content/workflow/task.py:52
+msgid "Content publisher task"
+msgstr ""
+
+#: ./src/pyams_content/workflow/task.py:88
+msgid "Content archiver task"
+msgstr ""
+
 #: ./src/pyams_content/workflow/__init__.py:84
 msgid "Proposed"
 msgstr ""
 
 #: ./src/pyams_content/workflow/__init__.py:85
 msgid "Canceled"
 msgstr ""
@@ -789,15 +802,15 @@
 msgstr ""
 
 #: ./src/pyams_content/feature/review/interfaces.py:73
 msgid "Reviewer comment?"
 msgstr ""
 
 #: ./src/pyams_content/feature/review/interfaces.py:77
-#: ./src/pyams_content/interfaces/__init__.py:125
+#: ./src/pyams_content/interfaces/__init__.py:128
 #: ./src/pyams_content/shared/common/zmi/search.py:225
 #: ./src/pyams_content/root/zmi/search.py:160
 msgid "Creation date"
 msgstr ""
 
 #: ./src/pyams_content/feature/review/interfaces.py:89
 msgid "Reviewers list"
@@ -992,14 +1005,15 @@
 msgstr ""
 
 #: ./src/pyams_content/feature/navigation/interfaces.py:84
 #: ./src/pyams_content/component/paragraph/interfaces/__init__.py:49
 #: ./src/pyams_content/component/association/interfaces.py:42
 #: ./src/pyams_content/shared/site/interfaces.py:223
 #: ./src/pyams_content/shared/common/interfaces/types.py:52
+#: ./src/pyams_content/shared/alert/interfaces.py:46
 msgid "Visible?"
 msgstr ""
 
 #: ./src/pyams_content/feature/navigation/interfaces.py:85
 #: ./src/pyams_content/component/association/interfaces.py:43
 msgid "Is this item visible in front-office?"
 msgstr ""
@@ -1009,15 +1023,15 @@
 msgstr ""
 
 #: ./src/pyams_content/feature/navigation/interfaces.py:93
 msgid "Displayed menu label"
 msgstr ""
 
 #: ./src/pyams_content/feature/navigation/interfaces.py:96
-#: ./src/pyams_content/shared/alert/interfaces.py:76
+#: ./src/pyams_content/shared/alert/interfaces.py:98
 msgid "Internal reference"
 msgstr ""
 
 #: ./src/pyams_content/feature/navigation/interfaces.py:97
 msgid "Direct reference to menu target"
 msgstr ""
 
@@ -1040,14 +1054,15 @@
 "If 'yes', menu items will be built from internal reference navigation items; "
 "other static items will be placed after dynamic items"
 msgstr ""
 
 #: ./src/pyams_content/feature/navigation/interfaces.py:113
 #: ./src/pyams_content/component/links/interfaces.py:49
 #: ./src/pyams_content/shared/common/interfaces/types.py:83
+#: ./src/pyams_content/shared/alert/interfaces.py:59
 msgid "Pictogram"
 msgstr ""
 
 #: ./src/pyams_content/feature/navigation/interfaces.py:114
 msgid ""
 "Name of the pictogram associated with this menu; pictogram display may depend"
 " on selected renderer and skin"
@@ -1074,14 +1089,15 @@
 
 #: ./src/pyams_content/feature/navigation/zmi/__init__.py:171
 msgid "Menu properties"
 msgstr ""
 
 #: ./src/pyams_content/feature/navigation/portlet/interfaces.py:34
 #: ./src/pyams_content/feature/navigation/portlet/interfaces.py:48
+#: ./src/pyams_content/feature/search/portlet/interfaces.py:45
 msgid "Portlet main title"
 msgstr ""
 
 #: ./src/pyams_content/feature/navigation/portlet/__init__.py:63
 msgid "Simple navigation menu"
 msgstr ""
 
@@ -1106,18 +1122,21 @@
 #: ./src/pyams_content/component/gallery/portlet/skin/interfaces.py:56
 #: ./src/pyams_content/component/gallery/skin/interfaces.py:44
 #: ./src/pyams_content/component/gallery/skin/interfaces.py:55
 msgid "Images selection"
 msgstr ""
 
 #: ./src/pyams_content/feature/navigation/portlet/skin/interfaces.py:31
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:100
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:117
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:134
 #: ./src/pyams_content/component/gallery/portlet/skin/interfaces.py:32
 #: ./src/pyams_content/component/gallery/skin/interfaces.py:31
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:83
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:130
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:74
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:121
 msgid "Selection used to display images thumbnails"
 msgstr ""
 
 #: ./src/pyams_content/feature/navigation/portlet/skin/__init__.py:65
 msgid "Horizontal grid links with illustrations (default)"
 msgstr ""
 
@@ -1142,20 +1161,20 @@
 #: ./src/pyams_content/feature/alert/interfaces.py:41
 msgid ""
 "Reference to the view used to get context alerts; please note that alerts "
 "content type selection will be added automatically to settings of the "
 "selected view"
 msgstr ""
 
-#: ./src/pyams_content/feature/alert/zmi/__init__.py:41
-#: ./src/pyams_content/feature/alert/zmi/__init__.py:51
+#: ./src/pyams_content/feature/alert/zmi/__init__.py:43
+#: ./src/pyams_content/feature/alert/zmi/__init__.py:53
 msgid "Alerts management"
 msgstr ""
 
-#: ./src/pyams_content/feature/alert/zmi/__init__.py:52
+#: ./src/pyams_content/feature/alert/zmi/__init__.py:54
 msgid "Alerts management views"
 msgstr ""
 
 #: ./src/pyams_content/feature/alert/skin/templates/alerts.pt:17
 #: ./src/pyams_content/feature/alert/skin/templates/alerts.pt:22
 #: ./src/pyams_content/feature/alert/skin/templates/context-alerts.pt:19
 #: ./src/pyams_content/feature/alert/skin/templates/context-alerts.pt:24
@@ -1251,16 +1270,16 @@
 
 #: ./src/pyams_content/feature/search/interfaces.py:108
 #: ./src/pyams_content/shared/site/interfaces.py:127
 msgid "Visible in folders list"
 msgstr ""
 
 #: ./src/pyams_content/feature/search/interfaces.py:109
-#: ./src/pyams_content/shared/site/interfaces.py:128
-msgid "If 'no', folder will not be displayed into folders list"
+msgid ""
+"If 'no', search folder will not be displayed into parent's contents list"
 msgstr ""
 
 #: ./src/pyams_content/feature/search/interfaces.py:114
 #: ./src/pyams_content/shared/site/interfaces.py:133
 #: ./src/pyams_content/shared/site/interfaces.py:206
 msgid "Navigation title"
 msgstr ""
@@ -1284,23 +1303,316 @@
 msgid "Selected data types"
 msgstr ""
 
 #: ./src/pyams_content/feature/search/interfaces.py:126
 msgid "Searched data types; leave empty for all"
 msgstr ""
 
+#: ./src/pyams_content/feature/search/__init__.py:42
+msgid "Search folder"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/zmi/thesaurus.py:39
+#: ./src/pyams_content/component/thesaurus/zmi/manager.py:78
+#: ./src/pyams_content/component/thesaurus/zmi/manager.py:88
+#: ./src/pyams_content/shared/view/zmi/thesaurus.py:66
+msgid "Tags settings"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/zmi/thesaurus.py:40
+msgid "Search folder tags settings"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/zmi/thesaurus.py:62
+#: ./src/pyams_content/component/thesaurus/zmi/manager.py:130
+#: ./src/pyams_content/component/thesaurus/zmi/manager.py:140
+#: ./src/pyams_content/shared/view/zmi/thesaurus.py:114
+msgid "Themes settings"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/zmi/thesaurus.py:63
+msgid "Search folder themes settings"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/zmi/thesaurus.py:85
+#: ./src/pyams_content/component/thesaurus/zmi/manager.py:164
+#: ./src/pyams_content/component/thesaurus/zmi/manager.py:174
+#: ./src/pyams_content/shared/view/zmi/thesaurus.py:162
+msgid "Collections settings"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/zmi/thesaurus.py:86
+msgid "Search folder collections settings"
+msgstr ""
+
 #: ./src/pyams_content/feature/search/zmi/manager.py:50
 #: ./src/pyams_content/feature/search/zmi/manager.py:60
 msgid "Search settings"
 msgstr ""
 
 #: ./src/pyams_content/feature/search/zmi/manager.py:61
 msgid "General search settings"
 msgstr ""
 
+#: ./src/pyams_content/feature/search/zmi/__init__.py:65
+msgid "Add search folder..."
+msgstr ""
+
+#: ./src/pyams_content/feature/search/zmi/__init__.py:82
+msgid "New search folder"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/zmi/__init__.py:83
+msgid "New search folder properties"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/zmi/__init__.py:106
+msgid "Search folder management"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/zmi/__init__.py:136
+msgid "Folder search settings"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/zmi/__init__.py:156
+#: ./src/pyams_content/shared/site/zmi/folder.py:222
+msgid "Navigation properties"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/interfaces.py:48
+msgid "Allow empty query?"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/interfaces.py:49
+msgid ""
+"If 'no', no result will be displayed if user didn't entered a search string"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/interfaces.py:54
+#: ./src/pyams_content/component/links/interfaces.py:67
+#: ./src/pyams_content/shared/view/portlet/interfaces.py:111
+msgid "Force canonical URL?"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/interfaces.py:55
+#: ./src/pyams_content/component/links/interfaces.py:68
+#: ./src/pyams_content/shared/view/portlet/interfaces.py:112
+msgid ""
+"By default, internal links use a \"relative\" URL, which tries to display "
+"link target in the current context; by using a canonical URL, you can display"
+" target in it's attachment context (if defined)"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/__init__.py:113
+#: ./src/pyams_content/shared/common/zmi/owner.py:362
+#: ./src/pyams_content/shared/common/zmi/search.py:430
+msgid "Search results"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt:5
+msgid "First search results sample:"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt:15
+msgid "No result found."
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:44
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:51
+msgid "Display full header"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:45
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:52
+msgid "Display only header start"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:46
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:53
+msgid "Hide header"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:59
+msgid "Display if empty?"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:60
+msgid ""
+"If 'no', and if no result is found, the portlet will not display anything"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:65
+msgid "Display results count?"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:66
+msgid "If 'no', results count will not be displayed"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:70
+msgid "Allow results sorting?"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:71
+msgid "If 'no', results will not be sortable"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:75
+msgid "Allow pagination?"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:76
+msgid "If 'no', results will not be paginated"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:80
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:164
+msgid "Header display mode"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:81
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:165
+msgid "Defines how results headers will be rendered"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:86
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:170
+msgid "Start length"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:87
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:171
+msgid ""
+"If you choose to display only header start, you can specify maximum text "
+"length"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:92
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:66
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:135
+msgid "Display illustrations?"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:93
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:67
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:136
+msgid "If 'no', view contents will not display illustrations"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:99
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:116
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:133
+#: ./src/pyams_content/component/gallery/portlet/skin/interfaces.py:31
+#: ./src/pyams_content/component/gallery/skin/interfaces.py:30
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:73
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:120
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:142
+msgid "Thumbnails selection"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:124
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:141
+msgid "Button's title"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:125
+#: ./src/pyams_content/feature/search/portlet/skin/interfaces.py:142
+msgid "Optional navigation button's title"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/zmi.py:83
+#: ./src/pyams_content/shared/view/portlet/skin/zmi.py:55
+msgid "Header display"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/__init__.py:107
+msgid "Paginated search results (default)"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/__init__.py:133
+msgid "Paneled search results"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/__init__.py:159
+msgid "Bootstrap cards search results"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/__init__.py:182
+msgid "Bootstrap Masonry cards search results"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:27
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:27
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:27
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:27
+msgid "${count} result(s) found"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:32
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:32
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:32
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:32
+msgid "No result found!"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:41
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:41
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:41
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:41
+msgid "Sort by relevance"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:44
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:44
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:44
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:44
+msgid "Sort by publication date"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:47
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:47
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:47
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:47
+msgid "Sort by last modification date"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:53
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:53
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:53
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:53
+msgid "Page length:"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:73
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:73
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:73
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:70
+#: ./src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt:60
+#: ./src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt:51
+msgid "Pagination"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:82
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:82
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:82
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:79
+#: ./src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt:68
+#: ./src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt:59
+msgid "Previous page"
+msgstr ""
+
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt:120
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt:120
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt:120
+#: ./src/pyams_content/feature/search/portlet/skin/templates/search-default.pt:117
+#: ./src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt:75
+#: ./src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt:66
+msgid "Next page"
+msgstr ""
+
 #: ./src/pyams_content/feature/renderer/__init__.py:139
 msgid "Hidden content"
 msgstr ""
 
 #: ./src/pyams_content/feature/renderer/__init__.py:153
 msgid "Default content renderer"
 msgstr ""
@@ -1354,43 +1666,47 @@
 msgid "Preview"
 msgstr ""
 
 #: ./src/pyams_content/feature/preview/zmi/__init__.py:75
 msgid "Open preview in new tab"
 msgstr ""
 
-#: ./src/pyams_content/interfaces/__init__.py:107
+#: ./src/pyams_content/interfaces/__init__.py:110
 msgid "Unique key"
 msgstr ""
 
-#: ./src/pyams_content/interfaces/__init__.py:108
+#: ./src/pyams_content/interfaces/__init__.py:111
 msgid ""
 "WARNING: this key can't be modified after creation!!! Spaces, uppercase "
 "letters or accentuated characters will be replaced automatically."
 msgstr ""
 
-#: ./src/pyams_content/interfaces/__init__.py:114
+#: ./src/pyams_content/interfaces/__init__.py:117
 #: ./src/pyams_content/shared/site/zmi/folder.py:84
 msgid "Visible label used to display content"
 msgstr ""
 
-#: ./src/pyams_content/interfaces/__init__.py:117
+#: ./src/pyams_content/interfaces/__init__.py:120
 msgid "Short name"
 msgstr ""
 
-#: ./src/pyams_content/interfaces/__init__.py:118
+#: ./src/pyams_content/interfaces/__init__.py:121
 msgid "Short name used in breadcrumbs"
 msgstr ""
 
-#: ./src/pyams_content/interfaces/__init__.py:129
+#: ./src/pyams_content/interfaces/__init__.py:132
 #: ./src/pyams_content/shared/common/zmi/search.py:228
 #: ./src/pyams_content/root/zmi/search.py:163
 msgid "Modification date"
 msgstr ""
 
+#: ./src/pyams_content/interfaces/__init__.py:144
+msgid "Object types"
+msgstr ""
+
 #: ./src/pyams_content/component/illustration/interfaces.py:44
 #: ./src/pyams_content/component/illustration/interfaces.py:120
 #: ./src/pyams_content/component/gallery/interfaces.py:48
 msgid "Image or video data"
 msgstr ""
 
 #: ./src/pyams_content/component/illustration/interfaces.py:45
@@ -1447,31 +1763,31 @@
 msgid "Illustration"
 msgstr ""
 
 #: ./src/pyams_content/component/illustration/interfaces.py:129
 msgid "Presentation template used for illustration"
 msgstr ""
 
-#: ./src/pyams_content/component/illustration/zmi/thesaurus.py:39
+#: ./src/pyams_content/component/illustration/zmi/thesaurus.py:41
 msgid "Associated illustration"
 msgstr ""
 
-#: ./src/pyams_content/component/illustration/zmi/thesaurus.py:40
+#: ./src/pyams_content/component/illustration/zmi/thesaurus.py:42
 msgid "Illustration properties"
 msgstr ""
 
-#: ./src/pyams_content/component/illustration/zmi/__init__.py:45
+#: ./src/pyams_content/component/illustration/zmi/__init__.py:46
 msgid "Main illustration"
 msgstr ""
 
-#: ./src/pyams_content/component/illustration/zmi/__init__.py:87
+#: ./src/pyams_content/component/illustration/zmi/__init__.py:91
 msgid "Navigation link illustration"
 msgstr ""
 
-#: ./src/pyams_content/component/illustration/zmi/__init__.py:126
+#: ./src/pyams_content/component/illustration/zmi/__init__.py:133
 msgid "Use responsive selection"
 msgstr ""
 
 #: ./src/pyams_content/component/illustration/portlet/skin/interfaces.py:33
 #: ./src/pyams_content/component/illustration/portlet/skin/interfaces.py:64
 #: ./src/pyams_content/component/illustration/skin/interfaces.py:49
 #: ./src/pyams_content/component/illustration/skin/interfaces.py:61
@@ -1519,24 +1835,24 @@
 #: ./src/pyams_content/component/illustration/portlet/skin/interfaces.py:71
 #: ./src/pyams_content/component/illustration/skin/interfaces.py:68
 msgid ""
 "If 'yes', a click on illustration thumbnail will open a modal window to "
 "display image"
 msgstr ""
 
-#: ./src/pyams_content/component/illustration/portlet/skin/__init__.py:92
+#: ./src/pyams_content/component/illustration/portlet/skin/__init__.py:89
 msgid "Full width illustration (default)"
 msgstr ""
 
-#: ./src/pyams_content/component/illustration/portlet/skin/__init__.py:136
+#: ./src/pyams_content/component/illustration/portlet/skin/__init__.py:133
 #: ./src/pyams_content/component/illustration/skin/illustration.py:103
 msgid "Floating illustration to the left"
 msgstr ""
 
-#: ./src/pyams_content/component/illustration/portlet/skin/__init__.py:157
+#: ./src/pyams_content/component/illustration/portlet/skin/__init__.py:154
 #: ./src/pyams_content/component/illustration/skin/illustration.py:115
 msgid "Floating illustration to the right"
 msgstr ""
 
 #: ./src/pyams_content/component/illustration/skin/illustration.py:81
 msgid "Centered image before text"
 msgstr ""
@@ -1654,20 +1970,20 @@
 msgid "Internal videos"
 msgstr ""
 
 #: ./src/pyams_content/component/extfile/zmi/paragraph.py:84
 msgid "Internal audio files"
 msgstr ""
 
-#: ./src/pyams_content/component/extfile/zmi/manager.py:43
-#: ./src/pyams_content/component/extfile/zmi/manager.py:53
+#: ./src/pyams_content/component/extfile/zmi/manager.py:45
+#: ./src/pyams_content/component/extfile/zmi/manager.py:55
 msgid "External files settings"
 msgstr ""
 
-#: ./src/pyams_content/component/extfile/zmi/manager.py:54
+#: ./src/pyams_content/component/extfile/zmi/manager.py:56
 msgid "Default prefix"
 msgstr ""
 
 #: ./src/pyams_content/component/extfile/zmi/__init__.py:59
 msgid "New file properties"
 msgstr ""
 
@@ -1719,19 +2035,19 @@
 msgid "Bootstrap cards"
 msgstr ""
 
 #: ./src/pyams_content/component/cards/interfaces.py:36
 msgid "Presentation template used for cards"
 msgstr ""
 
-#: ./src/pyams_content/component/cards/skin/__init__.py:47
+#: ./src/pyams_content/component/cards/skin/__init__.py:48
 msgid "Bootstrap cards renderer (default)"
 msgstr ""
 
-#: ./src/pyams_content/component/cards/skin/__init__.py:66
+#: ./src/pyams_content/component/cards/skin/__init__.py:67
 msgid "Bootstrap cards Masonry renderer"
 msgstr ""
 
 #: ./src/pyams_content/component/paragraph/zmi/container.py:158
 msgid "Click to set/unset paragraph as navigation anchor"
 msgstr ""
 
@@ -2024,31 +2340,31 @@
 msgid "Paragraphs navigation (default)"
 msgstr ""
 
 #: ./src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt:28
 msgid "Previous and next topics"
 msgstr ""
 
-#: ./src/pyams_content/component/paragraph/skin/html.py:55
+#: ./src/pyams_content/component/paragraph/skin/html.py:56
 msgid "HTML source code (default)"
 msgstr ""
 
-#: ./src/pyams_content/component/paragraph/skin/html.py:65
+#: ./src/pyams_content/component/paragraph/skin/html.py:66
 msgid "Formatted source code"
 msgstr ""
 
-#: ./src/pyams_content/component/paragraph/skin/html.py:107
+#: ./src/pyams_content/component/paragraph/skin/html.py:108
 msgid "ReStructured text"
 msgstr ""
 
-#: ./src/pyams_content/component/paragraph/skin/html.py:132
+#: ./src/pyams_content/component/paragraph/skin/html.py:133
 msgid "Markdown text"
 msgstr ""
 
-#: ./src/pyams_content/component/paragraph/skin/html.py:189
+#: ./src/pyams_content/component/paragraph/skin/html.py:190
 msgid "Rich text (default)"
 msgstr ""
 
 #: ./src/pyams_content/component/paragraph/skin/interfaces/html.py:31
 msgid "XS horizontal padding"
 msgstr ""
 
@@ -2105,27 +2421,14 @@
 msgstr ""
 
 #: ./src/pyams_content/component/links/interfaces.py:61
 #: ./src/pyams_content/shared/site/link.py:83
 msgid "Internal link"
 msgstr ""
 
-#: ./src/pyams_content/component/links/interfaces.py:67
-#: ./src/pyams_content/shared/view/portlet/interfaces.py:111
-msgid "Force canonical URL?"
-msgstr ""
-
-#: ./src/pyams_content/component/links/interfaces.py:68
-#: ./src/pyams_content/shared/view/portlet/interfaces.py:112
-msgid ""
-"By default, internal links use a \"relative\" URL, which tries to display "
-"link target in the current context; by using a canonical URL, you can display"
-" target in it's attachment context (if defined)"
-msgstr ""
-
 #: ./src/pyams_content/component/links/interfaces.py:89
 msgid ""
 "Marker interface provided by links directed to contents supporting this "
 "interface"
 msgstr ""
 
 #: ./src/pyams_content/component/links/interfaces.py:101
@@ -2354,39 +2657,32 @@
 " will be used to get medias"
 msgstr ""
 
 #: ./src/pyams_content/component/gallery/portlet/zmi/templates/gallery-preview.pt:3
 msgid "Medias list:"
 msgstr ""
 
-#: ./src/pyams_content/component/gallery/portlet/skin/interfaces.py:31
-#: ./src/pyams_content/component/gallery/skin/interfaces.py:30
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:82
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:129
-msgid "Thumbnails selection"
-msgstr ""
-
 #: ./src/pyams_content/component/gallery/portlet/skin/interfaces.py:46
 #: ./src/pyams_content/component/gallery/portlet/skin/interfaces.py:57
 #: ./src/pyams_content/component/gallery/skin/interfaces.py:45
 #: ./src/pyams_content/component/gallery/skin/interfaces.py:56
 msgid "Selection used to display images"
 msgstr ""
 
-#: ./src/pyams_content/component/gallery/portlet/skin/__init__.py:77
+#: ./src/pyams_content/component/gallery/portlet/skin/__init__.py:76
 #: ./src/pyams_content/component/gallery/skin/__init__.py:68
 msgid "Grid gallery renderer (default)"
 msgstr ""
 
-#: ./src/pyams_content/component/gallery/portlet/skin/__init__.py:101
+#: ./src/pyams_content/component/gallery/portlet/skin/__init__.py:100
 #: ./src/pyams_content/component/gallery/skin/__init__.py:93
 msgid "Carousel gallery renderer"
 msgstr ""
 
-#: ./src/pyams_content/component/gallery/portlet/skin/__init__.py:125
+#: ./src/pyams_content/component/gallery/portlet/skin/__init__.py:124
 #: ./src/pyams_content/component/gallery/skin/__init__.py:118
 msgid "Random image renderer"
 msgstr ""
 
 #: ./src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt:48
 #: ./src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt:62
 #: ./src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt:47
@@ -2430,15 +2726,15 @@
 msgid "Size"
 msgstr ""
 
 #: ./src/pyams_content/component/association/zmi/container.py:234
 msgid "Links and external files list"
 msgstr ""
 
-#: ./src/pyams_content/component/association/skin/paragraph.py:38
+#: ./src/pyams_content/component/association/skin/paragraph.py:39
 msgid "Associations list (default)"
 msgstr ""
 
 #: ./src/pyams_content/component/video/interfaces.py:52
 msgid "Name of video's author"
 msgstr ""
 
@@ -2472,15 +2768,15 @@
 msgstr ""
 
 #: ./src/pyams_content/component/video/zmi/paragraph.py:136
 #: ./src/pyams_content/component/video/zmi/paragraph.py:226
 msgid "Provider settings"
 msgstr ""
 
-#: ./src/pyams_content/component/video/skin/__init__.py:37
+#: ./src/pyams_content/component/video/skin/__init__.py:38
 msgid "External video renderer (default)"
 msgstr ""
 
 #: ./src/pyams_content/component/video/provider/vimeo.py:70
 msgid "Vimeo"
 msgstr ""
 
@@ -2785,23 +3081,23 @@
 #, python-format
 msgid ""
 "If an email address is provided in the form, this message will be returned to"
 " the contact; you can include all form fields values by including their name,"
 " enclosed in {brackets}, or {_reference} to include submission ID"
 msgstr ""
 
-#: ./src/pyams_content/component/fields/handler/zmi/mail.py:43
+#: ./src/pyams_content/component/fields/handler/zmi/mail.py:45
 msgid "Mailto handler settings"
 msgstr ""
 
-#: ./src/pyams_content/component/fields/handler/zmi/mail.py:61
+#: ./src/pyams_content/component/fields/handler/zmi/mail.py:63
 msgid "Mailto notifications"
 msgstr ""
 
-#: ./src/pyams_content/component/fields/handler/zmi/mail.py:62
+#: ./src/pyams_content/component/fields/handler/zmi/mail.py:64
 msgid "Mailto form handler settings"
 msgstr ""
 
 #: ./src/pyams_content/component/fields/skin/paragraph.py:55
 msgid "Form fields list (default)"
 msgstr ""
 
@@ -2817,67 +3113,49 @@
 msgid "You must specify a glossary thesaurus to activate it!"
 msgstr ""
 
 #: ./src/pyams_content/component/thesaurus/interfaces.py:67
 #: ./src/pyams_content/component/thesaurus/zmi/__init__.py:101
 #: ./src/pyams_content/shared/common/zmi/search.py:231
 #: ./src/pyams_content/shared/common/zmi/search.py:294
-#: ./src/pyams_content/shared/view/zmi/thesaurus.py:52
+#: ./src/pyams_content/shared/view/zmi/thesaurus.py:56
 #: ./src/pyams_content/root/zmi/search.py:166
 #: ./src/pyams_content/root/zmi/search.py:224
 msgid "Tags"
 msgstr ""
 
 #: ./src/pyams_content/component/thesaurus/interfaces.py:94
 #: ./src/pyams_content/component/thesaurus/zmi/__init__.py:186
 #: ./src/pyams_content/shared/common/zmi/search.py:234
 #: ./src/pyams_content/shared/common/zmi/search.py:308
-#: ./src/pyams_content/shared/view/zmi/thesaurus.py:94
+#: ./src/pyams_content/shared/view/zmi/thesaurus.py:104
 #: ./src/pyams_content/root/zmi/search.py:169
 #: ./src/pyams_content/root/zmi/search.py:238
 msgid "Themes"
 msgstr ""
 
 #: ./src/pyams_content/component/thesaurus/interfaces.py:121
 #: ./src/pyams_content/component/thesaurus/zmi/__init__.py:314
 #: ./src/pyams_content/shared/common/zmi/search.py:237
 #: ./src/pyams_content/shared/common/zmi/search.py:322
-#: ./src/pyams_content/shared/view/zmi/thesaurus.py:137
+#: ./src/pyams_content/shared/view/zmi/thesaurus.py:152
 #: ./src/pyams_content/root/zmi/search.py:172
 #: ./src/pyams_content/root/zmi/search.py:252
 msgid "Collections"
 msgstr ""
 
-#: ./src/pyams_content/component/thesaurus/zmi/manager.py:79
 #: ./src/pyams_content/component/thesaurus/zmi/manager.py:89
-#: ./src/pyams_content/shared/view/zmi/thesaurus.py:62
-msgid "Tags settings"
-msgstr ""
-
-#: ./src/pyams_content/component/thesaurus/zmi/manager.py:90
 msgid "Selected tags thesaurus"
 msgstr ""
 
-#: ./src/pyams_content/component/thesaurus/zmi/manager.py:125
-#: ./src/pyams_content/component/thesaurus/zmi/manager.py:135
-#: ./src/pyams_content/shared/view/zmi/thesaurus.py:104
-msgid "Themes settings"
-msgstr ""
-
-#: ./src/pyams_content/component/thesaurus/zmi/manager.py:136
+#: ./src/pyams_content/component/thesaurus/zmi/manager.py:141
 msgid "Selected themes thesaurus"
 msgstr ""
 
-#: ./src/pyams_content/component/thesaurus/zmi/manager.py:156
-#: ./src/pyams_content/component/thesaurus/zmi/manager.py:166
-#: ./src/pyams_content/shared/view/zmi/thesaurus.py:147
-msgid "Collections settings"
-msgstr ""
-
-#: ./src/pyams_content/component/thesaurus/zmi/manager.py:167
+#: ./src/pyams_content/component/thesaurus/zmi/manager.py:175
 msgid "Selected collections thesaurus"
 msgstr ""
 
 #: ./src/pyams_content/component/thesaurus/zmi/__init__.py:108
 msgid "Content tags selection"
 msgstr ""
 
@@ -2972,14 +3250,18 @@
 #: ./src/pyams_content/shared/site/interfaces.py:124
 #: ./src/pyams_content/shared/site/interfaces.py:174
 #: ./src/pyams_content/shared/site/zmi/folder.py:92
 #: ./src/pyams_content/shared/common/interfaces/__init__.py:196
 msgid "Internal information to be known about this content"
 msgstr ""
 
+#: ./src/pyams_content/shared/site/interfaces.py:128
+msgid "If 'no', folder will not be displayed into folders list"
+msgstr ""
+
 #: ./src/pyams_content/shared/site/interfaces.py:140
 msgid "Folder behaviour when navigating to folder URL"
 msgstr ""
 
 #: ./src/pyams_content/shared/site/interfaces.py:162
 msgid "Site's header is generally displayed in page header"
 msgstr ""
@@ -3150,40 +3432,40 @@
 msgstr ""
 
 #: ./src/pyams_content/shared/site/zmi/search.py:60
 #, python-format
 msgid "Between all contents of « {} » site folder"
 msgstr ""
 
-#: ./src/pyams_content/shared/site/zmi/manager.py:66
-#: ./src/pyams_content/shared/site/zmi/manager.py:79
+#: ./src/pyams_content/shared/site/zmi/manager.py:65
+#: ./src/pyams_content/shared/site/zmi/manager.py:78
 msgid "Add site manager"
 msgstr ""
 
-#: ./src/pyams_content/shared/site/zmi/manager.py:80
+#: ./src/pyams_content/shared/site/zmi/manager.py:79
 msgid "New site properties"
 msgstr ""
 
-#: ./src/pyams_content/shared/site/zmi/manager.py:98
+#: ./src/pyams_content/shared/site/zmi/manager.py:99
 msgid "Site name is required!"
 msgstr ""
 
-#: ./src/pyams_content/shared/site/zmi/manager.py:102
+#: ./src/pyams_content/shared/site/zmi/manager.py:103
 msgid "A site manager is already registered with this name!"
 msgstr ""
 
-#: ./src/pyams_content/shared/site/zmi/manager.py:155
+#: ./src/pyams_content/shared/site/zmi/manager.py:156
 msgid "Site management"
 msgstr ""
 
-#: ./src/pyams_content/shared/site/zmi/manager.py:177
+#: ./src/pyams_content/shared/site/zmi/manager.py:178
 msgid "Site manager properties"
 msgstr ""
 
-#: ./src/pyams_content/shared/site/zmi/manager.py:178
+#: ./src/pyams_content/shared/site/zmi/manager.py:179
 #: ./src/pyams_content/root/zmi/__init__.py:74
 msgid "Main site properties"
 msgstr ""
 
 #: ./src/pyams_content/shared/site/zmi/folder.py:73
 msgid "Add site folder..."
 msgstr ""
@@ -3204,18 +3486,14 @@
 msgid "Site folder properties"
 msgstr ""
 
 #: ./src/pyams_content/shared/site/zmi/folder.py:192
 msgid "Main folder properties"
 msgstr ""
 
-#: ./src/pyams_content/shared/site/zmi/folder.py:222
-msgid "Navigation properties"
-msgstr ""
-
 #: ./src/pyams_content/shared/site/zmi/viewlet/__init__.py:40
 msgid "Sites"
 msgstr ""
 
 #: ./src/pyams_content/shared/form/interfaces.py:38
 msgid "Form"
 msgstr ""
@@ -3243,16 +3521,16 @@
 msgstr ""
 
 #: ./src/pyams_content/shared/common/types.py:234
 #, python-format
 msgid "-- missing value ({}) --"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/__init__.py:118
-#: ./src/pyams_content/shared/common/__init__.py:127
+#: ./src/pyams_content/shared/common/__init__.py:117
+#: ./src/pyams_content/shared/common/__init__.py:126
 #, python-format
 msgid "{date} by {principal}"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/zmi/workflow.py:61
 msgid "Workflow action"
 msgstr ""
@@ -3617,19 +3895,14 @@
 msgstr ""
 
 #: ./src/pyams_content/shared/common/zmi/owner.py:343
 #, python-format
 msgid "{} contents selected, owner changed successfully for {} contents"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/zmi/owner.py:362
-#: ./src/pyams_content/shared/common/zmi/search.py:430
-msgid "Search results"
-msgstr ""
-
 #: ./src/pyams_content/shared/common/zmi/owner.py:410
 msgid "The selected user will become the new content's owner"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/zmi/owner.py:413
 msgid "If 'yes', the previous owner will still be able to modify this content"
 msgstr ""
@@ -4018,14 +4291,16 @@
 
 #: ./src/pyams_content/shared/common/zmi/types/container.py:99
 msgid "Click icon to enable or disable content type"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/zmi/types/container.py:116
 #: ./src/pyams_content/shared/common/interfaces/types.py:57
+#: ./src/pyams_content/shared/alert/interfaces.py:51
+#: ./src/pyams_content/shared/alert/zmi/types.py:129
 msgid "Label"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/zmi/types/container.py:144
 msgid "Shared tool content types list"
 msgstr ""
 
@@ -4104,22 +4379,25 @@
 msgstr ""
 
 #: ./src/pyams_content/shared/common/interfaces/types.py:71
 msgid "Label used for navigation entries"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/interfaces/types.py:74
+#: ./src/pyams_content/shared/alert/interfaces.py:54
 msgid "Back-office label"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/interfaces/types.py:75
+#: ./src/pyams_content/shared/alert/interfaces.py:55
 msgid "Optional label used in management pages instead of default label"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/interfaces/types.py:79
+#: ./src/pyams_content/shared/alert/interfaces.py:64
 msgid "Color"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/interfaces/types.py:80
 msgid "Color used to illustrate this data type"
 msgstr ""
 
@@ -4420,24 +4698,24 @@
 #: ./src/pyams_content/shared/common/portlet/interfaces.py:62
 msgid ""
 "If enabled, and if a header illustration is associated with the content, it's"
 " selected ratio may vary according to the selected renderer"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/portlet/interfaces.py:68
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:93
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:84
 msgid "Display breadcrumbs?"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/portlet/interfaces.py:72
 msgid "Display title?"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/portlet/interfaces.py:76
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:99
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:90
 msgid "Display tags?"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/portlet/interfaces.py:80
 msgid "Display header?"
 msgstr ""
 
@@ -4462,92 +4740,117 @@
 msgid "Shared content header (default)"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/portlet/skin/specificities.py:38
 msgid "Shared content specificities (default)"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:37
-#: ./src/pyams_content/shared/alert/interfaces.py:50
-msgid "Alert"
-msgstr ""
-
-#: ./src/pyams_content/shared/alert/interfaces.py:51
-msgid "End of alert"
+#: ./src/pyams_content/shared/alert/interfaces.py:47
+msgid "An hidden alert type can't be assigned to new alerts"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:52
-msgid "Information"
+#: ./src/pyams_content/shared/alert/interfaces.py:60
+msgid "Pictogram associated with this alert type"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:53
-msgid "Warning"
+#: ./src/pyams_content/shared/alert/interfaces.py:65
+msgid "Base color associated with this alert type"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:54
-msgid "Recommendation"
+#: ./src/pyams_content/shared/alert/interfaces.py:80
+msgid "Alert"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:66
-msgid "Alert gravity"
+#: ./src/pyams_content/shared/alert/interfaces.py:86
+#: ./src/pyams_content/shared/alert/zmi/types.py:223
+msgid "Alert type"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:67
-msgid "Alert gravity can affect renderer alert style"
+#: ./src/pyams_content/shared/alert/interfaces.py:87
+msgid "Alert type can affect renderer alert style"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:72
+#: ./src/pyams_content/shared/alert/interfaces.py:94
 msgid "Message content"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:73
+#: ./src/pyams_content/shared/alert/interfaces.py:95
 msgid "Message body"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:77
+#: ./src/pyams_content/shared/alert/interfaces.py:99
 msgid ""
 "Internal link target reference. You can search a reference using '+' followed"
 " by internal number, or by entering text matching content title"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:83
+#: ./src/pyams_content/shared/alert/interfaces.py:105
 msgid "External URL"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:84
+#: ./src/pyams_content/shared/alert/interfaces.py:106
 msgid "Alternate external URL"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:90
+#: ./src/pyams_content/shared/alert/interfaces.py:112
 msgid "You can't set internal reference and external URI simultaneously!"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:92
+#: ./src/pyams_content/shared/alert/interfaces.py:114
 msgid "Concerned contents"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:93
+#: ./src/pyams_content/shared/alert/interfaces.py:115
 msgid "If any, these contents will automatically display this alert"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:97
+#: ./src/pyams_content/shared/alert/interfaces.py:119
 msgid "Maximum interval"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/interfaces.py:98
+#: ./src/pyams_content/shared/alert/interfaces.py:120
 msgid ""
 "Maximum interval between alert displays on a given device, given in hours; "
 "set to 0 to always display the alert"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/zmi/__init__.py:41
+#: ./src/pyams_content/shared/alert/zmi/types.py:62
+#: ./src/pyams_content/shared/alert/zmi/types.py:154
+msgid "Alert types"
+msgstr ""
+
+#: ./src/pyams_content/shared/alert/zmi/types.py:112
+msgid "Click icon to enable or disable alert type"
+msgstr ""
+
+#: ./src/pyams_content/shared/alert/zmi/types.py:157
+msgid "Alert types list"
+msgstr ""
+
+#: ./src/pyams_content/shared/alert/zmi/types.py:171
+msgid "Add alert type"
+msgstr ""
+
+#: ./src/pyams_content/shared/alert/zmi/types.py:181
+msgid "New alert type"
+msgstr ""
+
+#: ./src/pyams_content/shared/alert/zmi/types.py:182
+msgid "New alert type properties"
+msgstr ""
+
+#: ./src/pyams_content/shared/alert/zmi/types.py:238
+msgid "Alert type properties"
+msgstr ""
+
+#: ./src/pyams_content/shared/alert/zmi/__init__.py:55
 msgid "Alert management"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/zmi/__init__.py:59
+#: ./src/pyams_content/shared/alert/zmi/__init__.py:82
 msgid "Alert settings"
 msgstr ""
 
 #: ./src/pyams_content/shared/view/merge.py:62
 msgid "Concatenate views items in order"
 msgstr ""
 
@@ -4583,23 +4886,23 @@
 msgid "References settings"
 msgstr ""
 
 #: ./src/pyams_content/shared/view/zmi/references.py:61
 msgid "View internal references settings"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/zmi/thesaurus.py:63
+#: ./src/pyams_content/shared/view/zmi/thesaurus.py:67
 msgid "View tags settings"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/zmi/thesaurus.py:105
+#: ./src/pyams_content/shared/view/zmi/thesaurus.py:115
 msgid "View themes settings"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/zmi/thesaurus.py:148
+#: ./src/pyams_content/shared/view/zmi/thesaurus.py:163
 msgid "View collections settings"
 msgstr ""
 
 #: ./src/pyams_content/shared/view/zmi/__init__.py:48
 msgid "View management"
 msgstr ""
 
@@ -4926,147 +5229,76 @@
 msgid "Views list:"
 msgstr ""
 
 #: ./src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt:14
 msgid "(no selected view)"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:43
-msgid "Initial selection"
-msgstr ""
-
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:44
-msgid "Responsive selection"
-msgstr ""
-
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:45
-msgid "Portrait selection"
-msgstr ""
-
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:46
-msgid "Panoramic selection"
-msgstr ""
-
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:47
-msgid "Square selection"
-msgstr ""
-
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:61
-msgid "Display full header"
-msgstr ""
-
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:62
-msgid "Display only header start"
-msgstr ""
-
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:63
-msgid "Hide header"
-msgstr ""
-
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:75
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:144
-msgid "Display illustrations?"
-msgstr ""
-
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:76
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:145
-msgid "If 'no', view contents will not display illustrations"
-msgstr ""
-
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:94
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:85
 msgid "If 'no', view items breadcrumbs will not be displayed"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:100
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:91
 msgid "If 'no', view items tags will not be displayed"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:104
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:150
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:95
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:154
 msgid "Paginate?"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:105
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:151
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:96
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:155
 msgid "If 'no', results pagination will be disabled"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:109
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:155
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:100
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:159
 msgid "Page size"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:110
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:156
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:101
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:160
 msgid "Number of items per page, if pagination is enabled"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:114
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:105
 msgid "'See all' link target"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:115
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:106
 msgid ""
 "Internal reference to site or search folder displaying full list of view's "
 "contents"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:120
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:111
 msgid "Link label"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:121
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:112
 msgid "Label of the link to full list page"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:160
-msgid "Header display mode"
-msgstr ""
-
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:161
-msgid "Defines how results headers will be rendered"
-msgstr ""
-
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:166
-msgid "Start length"
-msgstr ""
-
-#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:167
-msgid ""
-"If you choose to display only header start, you can specify maximum text "
-"length"
+#: ./src/pyams_content/shared/view/portlet/skin/interfaces.py:143
+msgid "Selection used to display illustrations thumbnails"
 msgstr ""
 
 #: ./src/pyams_content/shared/view/portlet/skin/__init__.py:97
 msgid "Simple vertical list (default)"
 msgstr ""
 
 #: ./src/pyams_content/shared/view/portlet/skin/__init__.py:121
 msgid "Horizontal thumbnails list"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/portlet/skin/__init__.py:149
+#: ./src/pyams_content/shared/view/portlet/skin/__init__.py:150
 msgid "Three vertical panels with panoramic illustrations"
 msgstr ""
 
-#: ./src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt:58
-#: ./src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt:54
-msgid "Pagination"
-msgstr ""
-
-#: ./src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt:66
-#: ./src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt:62
-msgid "Previous page"
-msgstr ""
-
-#: ./src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt:73
-#: ./src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt:69
-msgid "Next page"
-msgstr ""
-
 #: ./src/pyams_content/shared/view/skin/templates/preview.pt:2
 msgid "View result items"
 msgstr ""
 
 #: ./src/pyams_content/shared/view/skin/templates/preview.pt:3
 msgid "WARNING: items displayed in this preview are out of context!!"
 msgstr ""
```

### Comparing `pyams_content-1.99.0/src/pyams_content/reference/__init__.py` & `pyams_content-1.99.1/src/pyams_content/reference/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/reference/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/reference/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/reference/pictogram/__init__.py` & `pyams_content-1.99.1/src/pyams_content/reference/pictogram/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/reference/pictogram/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/reference/pictogram/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/reference/pictogram/manager.py` & `pyams_content-1.99.1/src/pyams_content/reference/pictogram/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/manager.py` & `pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/table.py` & `pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/table.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/widget/__init__.py` & `pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/widget/manager.py` & `pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt` & `pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/reference/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/reference/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/reference/zmi/table.py` & `pyams_content-1.99.1/src/pyams_content/reference/zmi/table.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/reference/zmi/viewlet/__init__.py` & `pyams_content-1.99.1/src/pyams_content/reference/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/root/__init__.py` & `pyams_content-1.99.1/src/pyams_content/root/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/root/configuration.py` & `pyams_content-1.99.1/src/pyams_content/root/configuration.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/root/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/root/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/root/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/root/zmi/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from zope.interface import Interface
 
 from pyams_content.root import ISiteRootInfos
 from pyams_content.zmi.properties import PropertiesEditForm
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
-from pyams_form.interfaces.form import IAJAXFormRenderer
+from pyams_form.interfaces.form import IAJAXFormRenderer, IFormContent
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
 from pyams_site.interfaces import ISiteRoot
 from pyams_utils.adapter import ContextRequestViewAdapter, adapter_config
 from pyams_viewlet.manager import viewletmanager_config
 from pyams_zmi.interfaces import IAdminLayer, IObjectLabel
 from pyams_zmi.interfaces.configuration import IZMIConfiguration
@@ -72,24 +72,28 @@
     """Site root properties edit form"""
 
     title = _("Main site properties")
     legend = _("Site information")
 
     fields = Fields(ISiteRootInfos)
 
-    def get_content(self):
-        return ISiteRootInfos(self.context)
-
     def update_widgets(self, prefix=None):
         super().update_widgets(prefix)
         description = self.widgets.get('description')
         if description is not None:
             description.set_widgets_attr('rows', 5)
 
 
+@adapter_config(required=(ISiteRoot, IPyAMSLayer, SiteRootPropertiesEditForm),
+                provides=IFormContent)
+def site_root_properties_form_content(context, request, form):
+    """Site root properties edit form content getter"""
+    return ISiteRootInfos(context)
+
+
 @adapter_config(required=(ISiteRoot, IAdminLayer, SiteRootPropertiesEditForm),
                 provides=IAJAXFormRenderer)
 class SiteRootPropertiesEditFormRenderer(ContextRequestViewAdapter):
     """Site root properties edit form renderer"""
 
     def render(self, changes):
         """Form renderer"""
```

### Comparing `pyams_content-1.99.0/src/pyams_content/root/zmi/dashboard.py` & `pyams_content-1.99.1/src/pyams_content/root/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/root/zmi/search.py` & `pyams_content-1.99.1/src/pyams_content/root/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/root/zmi/sites.py` & `pyams_content-1.99.1/src/pyams_content/root/zmi/sites.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/alert/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/alert/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 """
 
 from zope.interface import implementer
 from zope.schema.fieldproperty import FieldProperty
 
 from pyams_content.component.thesaurus import ITagsTarget, IThemesTarget
 from pyams_content.feature.review import IReviewTarget
-from pyams_content.shared.alert.interfaces import ALERT_CONTENT_NAME, ALERT_CONTENT_TYPE, IAlert, IWfAlert
+from pyams_content.shared.alert.interfaces import ALERT_CONTENT_NAME, ALERT_CONTENT_TYPE, IAlert, IAlertManager, \
+    IAlertTypesManager, IWfAlert
 from pyams_content.shared.common import ISharedContent, IWfSharedContent, SharedContent, WfSharedContent
 from pyams_sequence.reference import InternalReferenceMixin, get_reference_target
 from pyams_utils.factory import factory_config
 from pyams_utils.request import check_request
+from pyams_utils.traversing import get_parent
 
 __docformat__ = 'restructuredtext'
 
 
 @factory_config(IWfAlert)
 @factory_config(IWfSharedContent, name=ALERT_CONTENT_TYPE)
 @implementer(ITagsTarget, IThemesTarget, IReviewTarget)
@@ -40,21 +42,28 @@
     content_intf = IWfAlert
     content_view = False
 
     handle_content_url = False
     handle_header = False
     handle_description = False
 
-    gravity = FieldProperty(IWfAlert['gravity'])
+    alert_type = FieldProperty(IWfAlert['alert_type'])
     body = FieldProperty(IWfAlert['body'])
     _reference = FieldProperty(IWfAlert['reference'])
     external_url = FieldProperty(IWfAlert['external_url'])
     references = FieldProperty(IWfAlert['references'])
     maximum_interval = FieldProperty(IWfAlert['maximum_interval'])
 
+    def get_alert_type(self):
+        """Alert type getter"""
+        manager = get_parent(self, IAlertManager)
+        types = IAlertTypesManager(manager, None)
+        if types is not None:
+            return types.get(self.alert_type)
+
     @property
     def reference(self):
         return self._reference
 
     @reference.setter
     def reference(self, value):
         self._reference = value
@@ -71,7 +80,8 @@
 @factory_config(IAlert)
 @factory_config(ISharedContent, name=ALERT_CONTENT_TYPE)
 class Alert(SharedContent):
     """Workflow managed alert class"""
 
     content_type = ALERT_CONTENT_TYPE
     content_name = ALERT_CONTENT_NAME
+    content_view = False
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/alert/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/shared/alert/interfaces.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,64 +14,86 @@
 
 This module defines interfaces of alerts tool and contents.
 """
 
 from collections import OrderedDict
 from enum import Enum
 
+from zope.container.constraints import contains
+from zope.container.interfaces import IContainer
 from zope.interface import Invalid, invariant
-from zope.schema import Choice, Int, URI
-from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary
+from zope.location.interfaces import ILocation
+from zope.schema import Bool, Choice, Int, TextLine, URI
 
+from pyams_content.reference.pictogram import PICTOGRAM_VOCABULARY
 from pyams_content.shared.common import ISharedContent, IWfSharedContent
 from pyams_content.shared.common.interfaces import ISharedTool
-from pyams_i18n.schema import I18nTextField
+from pyams_i18n.schema import I18nTextField, I18nTextLineField
 from pyams_sequence.interfaces import IInternalReferencesList
 from pyams_sequence.schema import InternalReferenceField, InternalReferencesListField
+from pyams_utils.schema import ColorField
 
 __docformat__ = 'restructuredtext'
 
 from pyams_content import _
 
+ALERT_TYPES_MANAGER_ANNOTATION_KEY = 'pyams_content.alerts.types'
+ALERT_TYPES_VOCABULARY = 'pyams_content.alerts.types'
 
-ALERT_CONTENT_TYPE = 'alert'
-ALERT_CONTENT_NAME = _("Alert")
+
+class IAlertType(ILocation):
+    """Alert type interface"""
+
+    visible = Bool(title=_("Visible?"),
+                   description=_("An hidden alert type can't be assigned to new alerts"),
+                   required=True,
+                   default=True)
+
+    label = I18nTextLineField(title=_("Label"),
+                              required=True)
+
+    backoffice_label = I18nTextLineField(title=_("Back-office label"),
+                                         description=_("Optional label used in management pages "
+                                                       "instead of default label"),
+                                         required=False)
+
+    pictogram = Choice(title=_("Pictogram"),
+                       description=_("Pictogram associated with this alert type"),
+                       vocabulary=PICTOGRAM_VOCABULARY,
+                       required=False)
+
+    color = ColorField(title=_("Color"),
+                       description=_("Base color associated with this alert type"),
+                       required=False,
+                       default='dc3545')
 
 
-class ALERT_GRAVITY(Enum):
-    """Alert gravity enumeration"""
-    alert = 'alert'
-    alert_end = 'alert_end'
-    info = 'info'
-    warning = 'warning'
-    recommend = 'recommend'
-
-
-ALERT_GRAVITY_NAMES = OrderedDict((
-    (ALERT_GRAVITY.alert, _("Alert")),
-    (ALERT_GRAVITY.alert_end, _("End of alert")),
-    (ALERT_GRAVITY.info, _("Information")),
-    (ALERT_GRAVITY.warning, _("Warning")),
-    (ALERT_GRAVITY.recommend, _("Recommendation"))
-))
-
-ALERT_GRAVITY_VOCABULARY = SimpleVocabulary([
-    SimpleTerm(v.value, title=t)
-    for v, t in ALERT_GRAVITY_NAMES.items()
-])
+class IAlertTypesManager(IContainer):
+    """Alert types manager interface"""
+
+    contains(IAlertType)
+
+    def get_visible_items(self):
+        """Visible alert types iterator"""
+
+
+ALERT_CONTENT_TYPE = 'alert'
+ALERT_CONTENT_NAME = _("Alert")
 
 
 class IWfAlert(IWfSharedContent, IInternalReferencesList):
     """Alert interface"""
 
-    gravity = Choice(title=_("Alert gravity"),
-                     description=_("Alert gravity can affect renderer alert style"),
-                     required=True,
-                     vocabulary=ALERT_GRAVITY_VOCABULARY,
-                     default='info')
+    alert_type = Choice(title=_("Alert type"),
+                        description=_("Alert type can affect renderer alert style"),
+                        required=True,
+                        vocabulary=ALERT_TYPES_VOCABULARY)
+
+    def get_alert_type(self):
+        """Alert type getter"""
 
     body = I18nTextField(title=_("Message content"),
                          description=_("Message body"),
                          required=False)
 
     reference = InternalReferenceField(title=_("Internal reference"),
                                        description=_("Internal link target reference. You can "
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/alert/manager.py` & `pyams_content-1.99.1/src/pyams_content/shared/alert/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/alert/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/alert/zmi/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,38 +13,61 @@
 """PyAMS_content.shared.alert.zmi module
 
 This module defines components used for alerts management interface.
 """
 
 from zope.interface import Interface
 
-from pyams_content.shared.alert import IWfAlert
-from pyams_content.shared.common.zmi import SharedContentPropertiesEditForm
+from pyams_content.interfaces import CREATE_CONTENT_PERMISSION
+from pyams_content.shared.alert import IAlertManager, IWfAlert
+from pyams_content.shared.common.zmi import SharedContentAddForm, SharedContentPropertiesEditForm
+from pyams_content.zmi.interfaces import IDashboardColumn, IDashboardContentType
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
 from pyams_form.interfaces.form import IGroup
-from pyams_layer.interfaces import IPyAMSLayer
+from pyams_i18n.interfaces import II18n
+from pyams_layer.interfaces import IFormLayer, IPyAMSLayer
 from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
 from pyams_utils.adapter import adapter_config
 from pyams_zmi.form import FormGroupSwitcher
 from pyams_zmi.interfaces import IAdminLayer
 from pyams_zmi.interfaces.viewlet import IContentManagementMenu, IMenuHeader
 
 __docformat__ = 'restructuredtext'
 
 from pyams_content import _
 
 
+@adapter_config(required=(IWfAlert, IAdminLayer, IDashboardColumn),
+                provides=IDashboardContentType)
+def wf_alert_content_type(context, request, column):
+    """Alert content type"""
+    alert_type = context.get_alert_type()
+    if alert_type is not None:
+        i18n = II18n(alert_type)
+        return i18n.query_attributes_in_order(('backoffice_label', 'label'),
+                                              request=request)
+
+
 @adapter_config(required=(IWfAlert, IAdminLayer, Interface, IContentManagementMenu),
                 provides=IMenuHeader)
 def alert_management_menu_header(context, request, view, manager):
     """Alert management menu header"""
     return request.localizer.translate(_("Alert management"))
 
 
+@ajax_form_config(name='add-shared-content.html',
+                  context=IAlertManager, layer=IFormLayer,
+                  permission=CREATE_CONTENT_PERMISSION)
+class AlertAddForm(SharedContentAddForm):
+    """Alert add form"""
+
+    fields = Fields(IWfAlert).select('title', 'alert_type', 'notepad')
+
+
 @ajax_form_config(name='properties.html',
                   context=IWfAlert, layer=IPyAMSLayer,
                   permission=VIEW_SYSTEM_PERMISSION)
 class AlertPropertiesEditForm(SharedContentPropertiesEditForm):
     """Alert properties edit form"""
 
     interface = IWfAlert
@@ -54,9 +77,9 @@
                 required=(IWfAlert, IAdminLayer, AlertPropertiesEditForm),
                 provides=IGroup)
 class AlertPropertiesGroup(FormGroupSwitcher):
     """Alert properties group"""
 
     legend = _("Alert settings")
 
-    fields = Fields(IWfAlert).select('gravity', 'body', 'reference', 'external_url',
+    fields = Fields(IWfAlert).select('alert_type', 'body', 'reference', 'external_url',
                                      'references', 'maximum_interval')
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/blog/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/calendar/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/file/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 from zope.intid import IIntIds
 from zope.lifecycleevent import IObjectModifiedEvent
 from zope.schema.fieldproperty import FieldProperty
 from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary
 
 from pyams_content.interfaces import IBaseContentInfo, IObjectType
 from pyams_content.shared.common.interfaces import CONTENT_TYPES_VOCABULARY, IBaseSharedTool, \
-    ISharedContent, IWfSharedContent, IWfSharedContentRoles, SHARED_CONTENT_TYPES_VOCABULARY
+    ISharedContent, IWfSharedContent, IWfSharedContentRoles, SHARED_CONTENT_TYPES_VOCABULARY, \
+    VIEWS_SHARED_CONTENT_TYPES_VOCABULARY
 from pyams_i18n.content import I18nManagerMixin
 from pyams_i18n.interfaces import II18n
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_security.interfaces import IDefaultProtectionPolicy
 from pyams_security.interfaces.base import VIEW_PERMISSION
 from pyams_security.security import ProtectedObjectMixin
 from pyams_security.utility import get_principal
@@ -69,14 +70,31 @@
             SimpleTerm(factory.content_type, title=translate(factory.content_name))
             for _name, factory in get_all_factories(ISharedContent)
             if asbool(settings.get(f'pyams_content.register.{factory.content_type}', True))
         ], key=lambda x: x.title)
         super().__init__(terms)
 
 
+@vocabulary_config(name=VIEWS_SHARED_CONTENT_TYPES_VOCABULARY)
+class ViewsContentTypesVocabulary(SimpleVocabulary):
+    """Views and search folders content types vocabulary"""
+
+    def __init__(self, context):
+        request = check_request()
+        settings = request.registry.settings
+        translate = request.localizer.translate
+        terms = sorted([
+            SimpleTerm(factory.content_type, title=translate(factory.content_name))
+            for _name, factory in get_all_factories(ISharedContent)
+            if factory.content_view and
+               asbool(settings.get(f'pyams_content.register.{factory.content_type}', True))
+        ], key=lambda x: x.title)
+        super().__init__(terms)
+
+
 #
 # Workflow shared content class and adapters
 #
 
 @implementer(IDefaultProtectionPolicy, IWfSharedContent, IWorkflowPublicationSupport)
 class WfSharedContent(ProtectedObjectMixin, I18nManagerMixin, Persistent, Contained):
     """Shared data content class"""
@@ -229,14 +247,15 @@
     view_permission = VIEW_PERMISSION
 
     sequence_name = ''  # use default sequence generator
     sequence_prefix = ''
 
     content_type = None
     content_name = None
+    content_view = True
 
     @classproperty
     def content_factory(cls):
         """Content class getter"""
         return get_object_factory(IWfSharedContent, name=cls.content_type)
 
     @property
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/interfaces/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/interfaces/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,22 +261,25 @@
 
 class ISharedContent(IWorkflowManagedContent):
     """Workflow managed shared content interface"""
 
     content_type = Attribute("Content type interface")
     content_name = Attribute("Content name")
     content_factory = Attribute("Content factory attribute")
+    content_view = Attribute("Available for views searching")
 
     visible_version = Attribute("Link to actually visible version")
 
 
 CONTENT_TYPES_VOCABULARY = 'pyams_content.content.types'
 
 SHARED_CONTENT_TYPES_VOCABULARY = 'pyams_content.shared_content.types'
 
+VIEWS_SHARED_CONTENT_TYPES_VOCABULARY = 'pyams_content.shared_content.types.views'
+
 
 #
 # Generic restrictions interfaces
 #
 
 class ISharedToolRestrictions(Interface):
     """Base shared tool restrictions interface"""
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/interfaces/types.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/interfaces/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/manager.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portal.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/portal.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portlet/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portlet/header.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portlet/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portlet/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portlet/skin/header.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portlet/skin/specificities.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt` & `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portlet/skin/title.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portlet/specificities.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portlet/title.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portlet/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #
-# Copyright (c) 2015-2023 Thierry Florac <tflorac AT ulthar.net>
+# Copyright (c) 2015-2021 Thierry Florac <tflorac AT ulthar.net>
 # All Rights Reserved.
 #
 # This software is subject to the provisions of the Zope Public License,
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 
-"""PyAMS_content.shared.common.portlet.zmi module
+"""PyAMS_content.shared.site module
 
-This is the base module for management interface of shared contents portlets.
 """
 
 __docformat__ = 'restructuredtext'
+
+
+from .topic import SiteTopic, WfSiteTopic
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portlet/zmi/header.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portlet/zmi/specificities.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt` & `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/portlet/zmi/title.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/restrictions.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/restrictions.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/security.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/security.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/skin/breadcrumb.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/skin/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/skin/oid.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/skin/oid.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/skin/specificities.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/skin/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/skin/title.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/skin/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/skin/types.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/skin/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/skin/url.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/skin/url.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/skin/workflow.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/skin/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/types.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/content.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/content.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,16 +84,16 @@
                 provides=IDashboardContentType)
 def wf_shared_content_type(context, request, column):
     """Workflow-managed shared content type"""
     if IWfTypedSharedContent.providedBy(context):
         data_type = context.get_data_type()
         if data_type is not None:
             i18n = II18n(data_type)
-            return i18n.query_attribute('backoffice_label', request=request) or \
-                i18n.query_attribute('label', request=request)
+            return i18n.query_attributes_in_order(('backoffice_label', 'label'),
+                                                  request=request)
     return None
 
 
 @adapter_config(required=(ISharedContent, IAdminLayer, Interface),
                 provides=IDashboardContentType)
 def shared_content_type(context, request, view):
     """Shared content label"""
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/dashboard.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/header.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/manager.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/owner.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/owner.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/portal.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/portal.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/reference.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/restrictions.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/restrictions.py`

 * *Files 1% similar despite different names*

```diff
@@ -502,9 +502,13 @@
                 provides=IGroup)
 class ContributorRestrictionsWorkflowGroup(Group):
     """Contributor_restrictions workflow group"""
 
     legend = _("Principal restrictions")
     fields = Fields(IContributorWorkflowRestrictions)
 
-    def get_content(self):
-        return IContributorWorkflowRestrictions(self.parent_form.get_content())
+
+@adapter_config(required=(IBaseSharedTool, IAdminLayer, ContributorRestrictionsWorkflowGroup),
+                provides=IFormContent)
+def base_shared_tool_contributor_restrictions_form_content(context, request, form):
+    """Base shared tool contributor restrictions edit form content getter"""
+    return IContributorWorkflowRestrictions(form.parent_form.get_content())
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/search.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/summary.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/summary.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/templates/quick-search.pt` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/quick-search.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/types/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,16 +107,16 @@
 
 
 @adapter_config(required=(IDataType, IAdminLayer, Interface),
                 provides=IObjectLabel)
 def data_type_label(context, request, view):
     """Data type label"""
     i18n = II18n(context)
-    return i18n.query_attribute('backoffice_label', request=request) or \
-        i18n.query_attribute('label', request=request)
+    return i18n.query_attributes_in_order(('backoffice_label', 'label'),
+                                          request=request)
 
 
 @adapter_config(required=(IDataType, IAdminLayer, Interface),
                 provides=IObjectHint)
 def data_type_hint(context, request, view):  # pylint: disable=unused-argument
     """Data type hint"""
     return request.localizer.translate(_("Data type"))
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/types/container.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/types/content.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/content.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,16 +21,19 @@
 from pyramid.decorator import reify
 from zope.interface import Interface
 
 from pyams_content.shared.common.interfaces import ISharedTool
 from pyams_content.shared.common.interfaces.types import IWfTypedSharedContent
 from pyams_content.shared.common.zmi import SharedContentPropertiesEditForm
 from pyams_form.field import Fields
+from pyams_form.interfaces.form import IFormContent
+from pyams_utils.adapter import adapter_config
 from pyams_utils.registry import get_utility
 from pyams_zmi.form import AdminEditForm
+from pyams_zmi.interfaces import IAdminLayer
 
 
 class TypedSharedContentPropertiesEditForm(SharedContentPropertiesEditForm):
     """Typed shared content properties edit form"""
 
     interface = IWfTypedSharedContent
     fieldnames = ('title', 'short_name', 'content_url', 'data_type',
@@ -44,20 +47,23 @@
     def datatype(self):
         """Form context datatype getter"""
         context = self.context
         if IWfTypedSharedContent.providedBy(context):
             return context.get_data_type()
         return None
 
-    def get_content(self):
-        """Form content getter"""
-        manager = get_utility(ISharedTool, name=self.context.content_type)
-        return manager.shared_content_info_factory(self.context)
-
     @property
     def fields(self):
         """Form fields getter"""
         datatype = self.datatype
         if datatype is None:
             return Fields(Interface)
         manager = get_utility(ISharedTool, name=self.context.content_type)
         return Fields(manager.shared_content_info_factory).select(*datatype.field_names)
+
+
+@adapter_config(required=(IWfTypedSharedContent, IAdminLayer, TypedSharedContentCustomInfoEditForm),
+                provides=IFormContent)
+def typed_shared_content_custom_info_edit_form_content(context, request, layer):
+    """Typed shared content custom info edit content getter"""
+    manager = get_utility(ISharedTool, name=context.content_type)
+    return manager.shared_content_info_factory(context)
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/types/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/viewlet/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/common/zmi/workflow.py` & `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/file/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/form/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/form/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/form/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/shared/form/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/form/manager.py` & `pyams_content-1.99.1/src/pyams_content/shared/form/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/form/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/form/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/form/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/form/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/hub/__init__.py` & `pyams_content-1.99.1/src/pyams_content/skin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2015-2023 Thierry Florac <tflorac AT ulthar.net>
+# Copyright (c) 2015-2022 Thierry Florac <tflorac AT ulthar.net>
 # All Rights Reserved.
 #
 # This software is subject to the provisions of the Zope Public License,
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/logo/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/logo/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/__init__.py` & `pyams_content-1.99.1/src/pyams_content/zmi/widget/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,12 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 
-"""PyAMS_content.shared.site module
+"""PyAMS_content.zmi.widget module
 
 """
 
 __docformat__ = 'restructuredtext'
-
-
-from .topic import SiteTopic, WfSiteTopic
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/container.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/folder.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/link.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/link.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/manager.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/topic.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/topic.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/zmi/folder.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/zmi/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/zmi/link.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/link.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/zmi/manager.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/zmi/rename.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/rename.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/zmi/search.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/zmi/topic.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/topic.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/zmi/tree.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/tree.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/zmi/viewlet/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/zmi/widget/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/zmi/widget/folder.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/zmi/widget/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt` & `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/topic/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/topic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/topic/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/shared/topic/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/topic/manager.py` & `pyams_content-1.99.1/src/pyams_content/shared/topic/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/topic/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/topic/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,7 +198,8 @@
 @factory_config(IView)
 @factory_config(ISharedContent, name=VIEW_CONTENT_TYPE)
 class View(SharedContent):
     """Workflow managed view class"""
 
     content_type = VIEW_CONTENT_TYPE
     content_name = VIEW_CONTENT_NAME
+    content_view = False
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/interfaces/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/interfaces/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from collections import OrderedDict
 
 from zope.interface import Attribute
 from zope.schema import Bool, Choice, Int, Set
 from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary
 
 from pyams_content.shared.common.interfaces import ISharedContent, ISharedTool, IWfSharedContent, \
-    SHARED_CONTENT_TYPES_VOCABULARY
+    VIEWS_SHARED_CONTENT_TYPES_VOCABULARY
 from pyams_content.shared.common.interfaces.types import ALL_DATA_TYPES_VOCABULARY
 
 __docformat__ = 'restructuredtext'
 
 from pyams_content import _
 
 
@@ -68,15 +68,15 @@
     (FIRST_PUBLICATION_DATE_ORDER, _("Current version first publication date")),
     (CONTENT_PUBLICATION_DATE_ORDER, _("Content first publication date")),
     (VISIBLE_PUBLICATION_DATE_ORDER, _("Visible publication date")),
     (EXPIRATION_DATE_ORDER, _("Expiration date"))
 ))
 
 USER_VIEW_ORDER_VOCABULARY = SimpleVocabulary([
-    SimpleTerm(v, t)
+    SimpleTerm(v, title=t)
     for v, t in USER_VIEW_ORDERS.items()
 ])
 
 
 class IWfView(IWfSharedContent):
     """View interface"""
 
@@ -93,15 +93,15 @@
                                description=_("If 'yes', content type will be extracted from "
                                              "context"),
                                required=True,
                                default=False)
 
     selected_content_types = Set(title=_("Other content types"),
                                  description=_("Selected content types; leave empty for all"),
-                                 value_type=Choice(vocabulary=SHARED_CONTENT_TYPES_VOCABULARY),
+                                 value_type=Choice(vocabulary=VIEWS_SHARED_CONTENT_TYPES_VOCABULARY),
                                  required=False)
 
     def get_ignored_types(self):
         """Get content typed which are excluded from views (except if specified explicitly at runtime)"""
 
     def get_content_types(self, context):
         """Get content types for given context"""
@@ -118,15 +118,15 @@
                              required=False)
 
     def get_data_types(self, context):
         """Get data types for given context"""
 
     excluded_content_types = Set(title=_("Excluded content types"),
                                  description=_("Excluded content types; leave empty for all"),
-                                 value_type=Choice(vocabulary=SHARED_CONTENT_TYPES_VOCABULARY),
+                                 value_type=Choice(vocabulary=VIEWS_SHARED_CONTENT_TYPES_VOCABULARY),
                                  required=False)
 
     def get_excluded_content_types(self, context):
         """Get excluded content types for given context"""
 
     excluded_datatypes = Set(title=_("Excluded data types"),
                              description=_("Excluded data types; leave empty for all"),
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/interfaces/query.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/interfaces/query.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/interfaces/settings.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/interfaces/settings.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/manager.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,28 +13,25 @@
 """PyAMS_content.shared.view.manager module
 
 This module defines views manager shared tool.
 """
 
 from pyramid.events import subscriber
 from zope.component.interfaces import ISite
-from zope.interface import implementer
 from zope.lifecycleevent.interfaces import IObjectAddedEvent
 
-from pyams_content.component.thesaurus import ICollectionsManagerTarget, IThemesManagerTarget
 from pyams_content.shared.common.manager import SharedTool
 from pyams_content.shared.view.interfaces import IViewManager, VIEW_CONTENT_TYPE
 from pyams_utils.factory import factory_config
 from pyams_utils.traversing import get_parent
 
 __docformat__ = 'restructuredtext'
 
 
 @factory_config(IViewManager)
-@implementer(IThemesManagerTarget, ICollectionsManagerTarget)
 class ViewManager(SharedTool):
     """View manager class"""
 
     shared_content_type = VIEW_CONTENT_TYPE
     shared_content_menu = False
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/merge.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/merge.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/portlet/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/portlet/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/portlet/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 from persistent import Persistent
 from zope.container.contained import Contained
 from zope.interface import Interface
 from zope.schema.fieldproperty import FieldProperty
 
 from pyams_content.component.links import IInternalLink
 from pyams_content.shared.view.portlet import IViewItemsPortletSettings
-from pyams_content.shared.view.portlet.skin.interfaces import HIDDEN_HEADER_DISPLAY, IViewItemTargetURL, \
+from pyams_content.shared.view.portlet.skin.interfaces import HEADER_DISPLAY_MODE, IViewItemTargetURL, \
     IViewItemsPortletHorizontalRendererSettings, IViewItemsPortletPanelsRendererSettings, \
-    IViewItemsPortletVerticalRendererSettings, START_HEADER_DISPLAY
+    IViewItemsPortletVerticalRendererSettings
 from pyams_i18n.interfaces import II18n
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_portal.interfaces import IPortalContext, IPortletRenderer
 from pyams_portal.skin import PortletRenderer
 from pyams_sequence.reference import InternalReferenceMixin
 from pyams_template.template import template_config
 from pyams_utils.adapter import adapter_config
@@ -129,14 +129,15 @@
 #
 
 @factory_config(IViewItemsPortletPanelsRendererSettings)
 class ViewItemsPortletPanelsRendererSettings(Persistent, Contained):
     """View items portlet panels renderer settings"""
 
     display_illustrations = FieldProperty(IViewItemsPortletPanelsRendererSettings['display_illustrations'])
+    thumb_selection = FieldProperty(IViewItemsPortletPanelsRendererSettings['thumb_selection'])
     paginate = FieldProperty(IViewItemsPortletPanelsRendererSettings['paginate'])
     page_size = FieldProperty(IViewItemsPortletPanelsRendererSettings['page_size'])
     header_display_mode = FieldProperty(IViewItemsPortletPanelsRendererSettings['header_display_mode'])
     start_length = FieldProperty(IViewItemsPortletPanelsRendererSettings['start_length'])
 
 
 @adapter_config(name='panels',
@@ -150,13 +151,13 @@
     weight = 30
 
     settings_interface = IViewItemsPortletPanelsRendererSettings
 
     def get_header(self, item):
         settings = self.renderer_settings
         display_mode = settings.header_display_mode
-        if display_mode == HIDDEN_HEADER_DISPLAY:
+        if display_mode == HEADER_DISPLAY_MODE.HIDDEN.value:
             return ''
         header = II18n(item).query_attribute('header', request=self.request)
-        if display_mode == START_HEADER_DISPLAY:
+        if display_mode == HEADER_DISPLAY_MODE.START.value:
             header = get_text_start(header, settings.start_length)
         return header
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/portlet/skin/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/interfaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 """PyAMS_content.shared.view.portlet.skin.interfaces module
 
 This module defines interfaces of view items portlet renderers settings.
 """
 
 from collections import OrderedDict
+from enum import Enum
 
 from zope.interface import Attribute, Interface
 from zope.schema import Bool, Choice, Int
 from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary
 
 from pyams_i18n.schema import I18nTextLineField
 from pyams_sequence.interfaces import IInternalReference
@@ -35,41 +36,31 @@
     """View item target URL"""
 
     target = Attribute("Reference target")
 
     url = Attribute("Reference URL")
 
 
-VIEW_ITEMS_THUMBNAILS = OrderedDict((
-    ('', _("Initial selection")),
-    ('responsive', _("Responsive selection")),
-    ('portrait', _("Portrait selection")),
-    ('pano', _("Panoramic selection")),
-    ('square', _("Square selection"))
-))
-
-VIEW_ITEMS_THUMBNAILS_VOCABULARY = SimpleVocabulary([
-    SimpleTerm(v, title=t)
-    for v, t in VIEW_ITEMS_THUMBNAILS.items()
-])
+class HEADER_DISPLAY_MODE(Enum):
+    """Header display modes"""
+    FULL = 'full'
+    START = 'start'
+    HIDDEN = 'none'
 
 
-FULL_HEADER_DISPLAY = 'full'
-START_HEADER_DISPLAY = 'start'
-HIDDEN_HEADER_DISPLAY = 'none'
-
-PANELS_HEADER_DISPLAY_MODES = OrderedDict((
-    (FULL_HEADER_DISPLAY, _("Display full header")),
-    (START_HEADER_DISPLAY, _("Display only header start")),
-    (HIDDEN_HEADER_DISPLAY, _("Hide header"))
+HEADER_DISPLAY_MODES_NAMES = OrderedDict((
+    (HEADER_DISPLAY_MODE.FULL, _("Display full header")),
+    (HEADER_DISPLAY_MODE.START, _("Display only header start")),
+    (HEADER_DISPLAY_MODE.HIDDEN, _("Hide header"))
 ), )
 
-PANELS_HEADER_DISPLAY_MODES_VOCABULARY = SimpleVocabulary([
-    SimpleTerm(k, title=v)
-    for k, v in PANELS_HEADER_DISPLAY_MODES.items()
+
+HEADER_DISPLAY_MODES_VOCABULARY = SimpleVocabulary([
+    SimpleTerm(v.value, title=t)
+    for v, t in HEADER_DISPLAY_MODES_NAMES.items()
 ])
 
 
 class IViewItemsPortletVerticalRendererSettings(IInternalReference):
     """View items portlet vertical renderer settings interface"""
 
     display_illustrations = Bool(title=_("Display illustrations?"),
@@ -143,28 +134,41 @@
 
     display_illustrations = Bool(title=_("Display illustrations?"),
                                  description=_("If 'no', view contents will not display "
                                                "illustrations"),
                                  required=True,
                                  default=True)
 
+    thumb_selection = BootstrapThumbnailsSelectionField(
+        title=_("Thumbnails selection"),
+        description=_("Selection used to display illustrations thumbnails"),
+        default_selection='pano',
+        default_width={
+            'xs': 6,
+            'sm': 6,
+            'md': 4,
+            'lg': 3,
+            'xl': 2
+        },
+        required=True)
+
     paginate = Bool(title=_("Paginate?"),
                     description=_("If 'no', results pagination will be disabled"),
                     required=True,
                     default=True)
 
     page_size = Int(title=_("Page size"),
                     description=_("Number of items per page, if pagination is enabled"),
                     required=False,
                     default=9)
 
     header_display_mode = Choice(title=_("Header display mode"),
                                  description=_("Defines how results headers will be rendered"),
                                  required=True,
-                                 vocabulary=PANELS_HEADER_DISPLAY_MODES_VOCABULARY,
-                                 default=FULL_HEADER_DISPLAY)
+                                 vocabulary=HEADER_DISPLAY_MODES_VOCABULARY,
+                                 default=HEADER_DISPLAY_MODE.FULL.value)
 
     start_length = Int(title=_("Start length"),
                        description=_("If you choose to display only header start, you can specify "
                                      "maximum text length"),
                        required=True,
                        default=120)
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt` & `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 				 tal:define="illustration tales:pyams_illustration(item);
 							 target view.get_url(item);"
 				 tal:condition="illustration">
 				<a href="${target}">
 					<tal:if define="image i18n:illustration.data;
 									alt_title i18n:illustration.alt_title;"
 							condition="image">
-						${structure:tales:picture(image, selections=selections,
-												  alt=alt_title, css_class='w-100')}
+						${structure:tales:picture(image,
+												  selections=selections,
+												  alt=alt_title,
+												  css_class='w-100')}
 					</tal:if>
 				</a>
 			</div>
 		</tal:loop>
 	</div>
 </div>
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt` & `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt`

 * *Files 19% similar despite different names*

```diff
@@ -9,33 +9,30 @@
 	<h3 tal:define="title i18n:settings.title"
 		tal:condition="title"
 		class="position-relative border-bottom pb-2 mt-4">
 		${title}
 		<span class="position-absolute underline"></span>
 	</h3>
 	<div class="row row-cols-1 row-cols-sm-2 row-cols-md-3"
-		 tal:define="global count 0;">
+		 tal:define="global count 0;
+					 selections renderer_settings.thumb_selection;">
 		<div class="col my-3 d-flex flex-column"
 			 tal:repeat="item results">
 			<tal:var define="global count count + 1;
 							 target view.get_url(item);
 							 illustration tales:pyams_illustration(item);">
 				<div tal:define="illustration tales:pyams_illustration(item)"
 					 tal:condition="illustration"
 					 class="d-none d-sm-block">
 					<a href="${target}">
 						<tal:if define="image i18n:illustration.data;
 										alt_title i18n:illustration.alt_title;"
 								condition="image">
 							${structure:tales:picture(image,
-													  xl_thumb='pano', lg_width=4,
-													  lg_thumb='pano', lg_width=4,
-													  md_thumb='pano', md_width=4,
-													  sm_thumb='pano', sm_width=6,
-													  xs_thumb='pano', xs_width=6,
+													  selections=selections,
 													  alt=alt_title)}
 						</tal:if>
 					</a>
 				</div>
 				<div>
 					<a href="${target}">
 						<h4 class="mt-2">${i18n:item.title}</h4>
```

#### html2text {}

```diff
@@ -1,8 +1,6 @@
 ******** $${{ttiittllee}} ********
-_$_{_s_t_r_u_c_t_u_r_e_:_t_a_l_e_s_:_p_i_c_t_u_r_e_(_i_m_a_g_e_,_ _x_l___t_h_u_m_b_=_'_p_a_n_o_'_,_ _l_g___w_i_d_t_h_=_4_,_ _l_g___t_h_u_m_b_=_'_p_a_n_o_'_,
-_l_g___w_i_d_t_h_=_4_,_ _m_d___t_h_u_m_b_=_'_p_a_n_o_'_,_ _m_d___w_i_d_t_h_=_4_,_ _s_m___t_h_u_m_b_=_'_p_a_n_o_'_,_ _s_m___w_i_d_t_h_=_6_,
-_x_s___t_h_u_m_b_=_'_p_a_n_o_'_,_ _x_s___w_i_d_t_h_=_6_,_ _a_l_t_=_a_l_t___t_i_t_l_e_)_}
+_$_{_s_t_r_u_c_t_u_r_e_:_t_a_l_e_s_:_p_i_c_t_u_r_e_(_i_m_a_g_e_,_ _s_e_l_e_c_t_i_o_n_s_=_s_e_l_e_c_t_i_o_n_s_,_ _a_l_t_=_a_l_t___t_i_t_l_e_)_}
 _**_**_**_ _$$_{{_ii_11_88_nn_::_ii_tt_ee_mm_.._tt_ii_tt_ll_ee_}}_ _**_**_**
 _$_{_s_t_r_u_c_t_u_r_e_:_h_e_a_d_e_r_}
     * _←_ _P_r_e_v_i_o_u_s_ _p_a_g_e
     * _N_e_x_t_ _p_a_g_e_ _→
```

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/portlet/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt` & `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/query.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/query.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/reference.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/thesaurus.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/zmi/references.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/zmi/references.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/shared/view/zmi/thesaurus.py` & `pyams_content-1.99.1/src/pyams_content/shared/view/zmi/thesaurus.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,29 +8,27 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 
 """PyAMS_content.shared.view.zmi.thesaurus module
 
-This module defines management interface components used to to handle
+This module defines management interface components used to handle
 thesaurus-based views settings.
 """
 
 from pyams_content.component.thesaurus import ICollectionsManager, ITagsManager, IThemesManager
 from pyams_content.shared.view import IWfView
-from pyams_content.shared.view.interfaces import IViewManager
 from pyams_content.shared.view.interfaces.settings import IViewCollectionsSettings, IViewTagsSettings, \
     IViewThemesSettings
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
 from pyams_thesaurus.zmi.widget import ThesaurusTermsTreeFieldWidget
-from pyams_utils.registry import get_utility
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.form import AdminEditForm
 from pyams_zmi.interfaces import IAdminLayer
 from pyams_zmi.interfaces.viewlet import IPropertiesMenu
 from pyams_zmi.zmi.viewlet.menu import NavigationMenuItem
 
 __docformat__ = 'restructuredtext'
@@ -45,14 +43,20 @@
 @viewlet_config(name='tags.menu',
                 context=IWfView, layer=IAdminLayer,
                 manager=IPropertiesMenu, weight=350,
                 permission=VIEW_SYSTEM_PERMISSION)
 class ViewTagsMenu(NavigationMenuItem):
     """View tags menu"""
 
+    def __new__(cls, context, request, view, manager):
+        manager = ITagsManager(request.root, None)
+        if not manager.thesaurus_name:
+            return None
+        return NavigationMenuItem.__new__(cls)
+
     label = _("Tags")
     href = '#tags.html'
 
 
 @ajax_form_config(name='tags.html',
                   context=IWfView, layer=IPyAMSLayer,
                   permission=VIEW_SYSTEM_PERMISSION)
@@ -87,14 +91,20 @@
 @viewlet_config(name='themes.menu',
                 context=IWfView, layer=IAdminLayer,
                 manager=IPropertiesMenu, weight=360,
                 permission=VIEW_SYSTEM_PERMISSION)
 class ViewThemesMenu(NavigationMenuItem):
     """View themes menu"""
 
+    def __new__(cls, context, request, view, manager):
+        manager = IThemesManager(request.root, None)
+        if not manager.thesaurus_name:
+            return None
+        return NavigationMenuItem.__new__(cls)
+
     label = _("Themes")
     href = '#themes.html'
 
 
 @ajax_form_config(name='themes.html',
                   context=IWfView, layer=IPyAMSLayer,
                   permission=VIEW_SYSTEM_PERMISSION)
@@ -110,16 +120,15 @@
     fields = Fields(IViewThemesSettings)
     fields['themes'].widget_factory = ThesaurusTermsTreeFieldWidget
 
     def update_widgets(self, prefix=None):
         super().update_widgets(prefix)
         widget = self.widgets.get('themes')
         if widget is not None:
-            views = get_utility(IViewManager)
-            manager = IThemesManager(views, None)
+            manager = IThemesManager(self.request.root, None)
             if manager is not None:
                 widget.label_css_class = 'control-label col-md-2'
                 widget.input_css_class = 'col-md-12'
                 widget.thesaurus_name = manager.thesaurus_name
                 widget.extract_name = manager.extract_name
 
 
@@ -130,14 +139,20 @@
 @viewlet_config(name='collections.menu',
                 context=IWfView, layer=IAdminLayer,
                 manager=IPropertiesMenu, weight=370,
                 permission=VIEW_SYSTEM_PERMISSION)
 class ViewCollectionsMenu(NavigationMenuItem):
     """View collections menu"""
 
+    def __new__(cls, context, request, view, manager):
+        manager = ICollectionsManager(request.root, None)
+        if not manager.thesaurus_name:
+            return None
+        return NavigationMenuItem.__new__(cls)
+
     label = _("Collections")
     href = '#collections.html'
 
 
 @ajax_form_config(name='collections.html',
                   context=IWfView, layer=IPyAMSLayer,
                   permission=VIEW_SYSTEM_PERMISSION)
@@ -153,14 +168,13 @@
     fields = Fields(IViewCollectionsSettings)
     fields['collections'].widget_factory = ThesaurusTermsTreeFieldWidget
 
     def update_widgets(self, prefix=None):
         super().update_widgets(prefix)
         widget = self.widgets.get('collections')
         if widget is not None:
-            views = get_utility(IViewManager)
-            manager = ICollectionsManager(views, None)
+            manager = ICollectionsManager(self.request.root, None)
             if manager is not None:
                 widget.label_css_class = 'control-label col-md-2'
                 widget.input_css_class = 'col-md-12'
                 widget.thesaurus_name = manager.thesaurus_name
                 widget.extract_name = manager.extract_name
```

### Comparing `pyams_content-1.99.0/src/pyams_content/skin/__init__.py` & `pyams_content-1.99.1/src/pyams_content/workflow/zmi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2015-2022 Thierry Florac <tflorac AT ulthar.net>
+# Copyright (c) 2015-2021 Thierry Florac <tflorac AT ulthar.net>
 # All Rights Reserved.
 #
 # This software is subject to the provisions of the Zope Public License,
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
```

### Comparing `pyams_content-1.99.0/src/pyams_content/skin/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/skin/interfaces.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,17 +58,26 @@
     """Content header getter interface"""
 
 
 class IContentSummaryInfo(Interface):
     """Content summary info getter interface"""
 
     context = Attribute("Link to adapted context")
-
     title = Attribute("Content title")
-
     header = Attribute("Content header")
-
     button_title = Attribute("Button title")
 
 
 class IPublicURL(Interface):
     """Public URL target getter interface"""
+
+
+class ISearchResultsView(Interface):
+    """Search results view marker interface"""
+
+
+class ISearchResultsPanelsView(ISearchResultsView):
+    """Search results panels view marker interface"""
+
+
+class ISearchResultsCardsView(ISearchResultsView):
+    """Search results cards view marker interface"""
```

### Comparing `pyams_content-1.99.0/src/pyams_content/tests/__init__.py` & `pyams_content-1.99.1/src/pyams_content/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/tests/test_utilsdocs.py` & `pyams_content-1.99.1/src/pyams_content/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/tests/test_utilsdocstrings.py` & `pyams_content-1.99.1/src/pyams_content/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/utils/__init__.py` & `pyams_content-1.99.1/src/pyams_content/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/workflow/__init__.py` & `pyams_content-1.99.1/src/pyams_content/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/workflow/basic.py` & `pyams_content-1.99.1/src/pyams_content/workflow/basic.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/workflow/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/workflow/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/workflow/notify.py` & `pyams_content-1.99.1/src/pyams_content/workflow/notify.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/workflow/task.py` & `pyams_content-1.99.1/src/pyams_content/workflow/task.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/workflow/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/shared/alert/zmi/interfaces.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 #
-# Copyright (c) 2015-2021 Thierry Florac <tflorac AT ulthar.net>
+# Copyright (c) 2015-2024 Thierry Florac <tflorac AT ulthar.net>
 # All Rights Reserved.
 #
 # This software is subject to the provisions of the Zope Public License,
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 
 """PyAMS_*** module
 
 """
 
+from zope.interface import Interface
+
+
 __docformat__ = 'restructuredtext'
+
+
+class IAlertTypesTable(Interface):
+    """Alert types table interface"""
```

### Comparing `pyams_content-1.99.0/src/pyams_content/workflow/zmi/publication.py` & `pyams_content-1.99.1/src/pyams_content/workflow/zmi/publication.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/workflow/zmi/task.py` & `pyams_content-1.99.1/src/pyams_content/workflow/zmi/task.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/zmi/__init__.py` & `pyams_content-1.99.1/src/pyams_content/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/zmi/dashboard.py` & `pyams_content-1.99.1/src/pyams_content/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/zmi/html.py` & `pyams_content-1.99.1/src/pyams_content/zmi/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/zmi/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/zmi/properties.py` & `pyams_content-1.99.1/src/pyams_content/zmi/properties.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/zmi/resources/js/content.js` & `pyams_content-1.99.1/src/pyams_content/zmi/resources/js/content.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/zmi/resources/js/content.min.js` & `pyams_content-1.99.1/src/pyams_content/zmi/resources/js/content.min.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js` & `pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js` & `pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js` & `pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/zmi/viewlet/__init__.py` & `pyams_content-1.99.1/src/pyams_content/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/zmi/viewlet/toplinks.py` & `pyams_content-1.99.1/src/pyams_content/zmi/viewlet/toplinks.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/zmi/widget/interfaces.py` & `pyams_content-1.99.1/src/pyams_content/zmi/widget/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/zmi/widget/seo.py` & `pyams_content-1.99.1/src/pyams_content/zmi/widget/seo.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content/zmi/widget/templates/seo-textline-input.pt` & `pyams_content-1.99.1/src/pyams_content/zmi/widget/templates/seo-textline-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.0/src/pyams_content.egg-info/PKG-INFO` & `pyams_content-1.99.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams-content
-Version: 1.99.0
+Name: pyams_content
+Version: 1.99.1
 Summary: PyAMS content management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS CMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -48,10 +48,17 @@
 Please note that PyAMS_content only provide a basic Bootstrap based skin, so you will have to
 include other extension packages (like PyAMS_content_themes) to get more advanced graphical themes.
 
 
 Changelog
 =========
 
+1.99.1
+------
+ - added edit forms content getters
+ - added alerts types
+ - added vocabulary to handle shared contents which can be used by views and search folders
+ - minor updates
+
 1.99.0
 ------
  - first preliminary release
```

### Comparing `pyams_content-1.99.0/src/pyams_content.egg-info/SOURCES.txt` & `pyams_content-1.99.1/src/pyams_content.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -239,16 +239,32 @@
 src/pyams_content/feature/review/zmi/templates/comment.pt
 src/pyams_content/feature/review/zmi/templates/comments.pt
 src/pyams_content/feature/review/zmi/templates/mail-notification.pt
 src/pyams_content/feature/search/__init__.py
 src/pyams_content/feature/search/interfaces.py
 src/pyams_content/feature/search/manager.py
 src/pyams_content/feature/search/thesaurus.py
+src/pyams_content/feature/search/portlet/__init__.py
+src/pyams_content/feature/search/portlet/interfaces.py
+src/pyams_content/feature/search/portlet/skin/__init__.py
+src/pyams_content/feature/search/portlet/skin/interfaces.py
+src/pyams_content/feature/search/portlet/skin/zmi.py
+src/pyams_content/feature/search/portlet/skin/templates/search-card.pt
+src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt
+src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt
+src/pyams_content/feature/search/portlet/skin/templates/search-default.pt
+src/pyams_content/feature/search/portlet/skin/templates/search-panel.pt
+src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt
+src/pyams_content/feature/search/portlet/skin/templates/search-result.pt
+src/pyams_content/feature/search/portlet/zmi/__init__.py
+src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt
 src/pyams_content/feature/search/zmi/__init__.py
 src/pyams_content/feature/search/zmi/manager.py
+src/pyams_content/feature/search/zmi/reference.py
+src/pyams_content/feature/search/zmi/thesaurus.py
 src/pyams_content/feature/share/__init__.py
 src/pyams_content/feature/sitemap/__init__.py
 src/pyams_content/feature/sitemap/interfaces.py
 src/pyams_content/feature/sitemap/templates/humans.pt
 src/pyams_content/feature/sitemap/templates/robots.pt
 src/pyams_content/feature/sitemap/templates/root-sitemap.pt
 src/pyams_content/feature/sitemap/templates/tool-sitemap.pt
@@ -281,15 +297,18 @@
 src/pyams_content/root/zmi/dashboard.py
 src/pyams_content/root/zmi/search.py
 src/pyams_content/root/zmi/sites.py
 src/pyams_content/shared/__init__.py
 src/pyams_content/shared/alert/__init__.py
 src/pyams_content/shared/alert/interfaces.py
 src/pyams_content/shared/alert/manager.py
+src/pyams_content/shared/alert/types.py
 src/pyams_content/shared/alert/zmi/__init__.py
+src/pyams_content/shared/alert/zmi/interfaces.py
+src/pyams_content/shared/alert/zmi/types.py
 src/pyams_content/shared/blog/__init__.py
 src/pyams_content/shared/calendar/__init__.py
 src/pyams_content/shared/common/__init__.py
 src/pyams_content/shared/common/manager.py
 src/pyams_content/shared/common/portal.py
 src/pyams_content/shared/common/restrictions.py
 src/pyams_content/shared/common/security.py
@@ -395,14 +414,15 @@
 src/pyams_content/shared/view/interfaces/__init__.py
 src/pyams_content/shared/view/interfaces/query.py
 src/pyams_content/shared/view/interfaces/settings.py
 src/pyams_content/shared/view/portlet/__init__.py
 src/pyams_content/shared/view/portlet/interfaces.py
 src/pyams_content/shared/view/portlet/skin/__init__.py
 src/pyams_content/shared/view/portlet/skin/interfaces.py
+src/pyams_content/shared/view/portlet/skin/zmi.py
 src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt
 src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt
 src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt
 src/pyams_content/shared/view/portlet/zmi/__init__.py
 src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt
 src/pyams_content/shared/view/skin/__init__.py
 src/pyams_content/shared/view/skin/templates/preview.pt
```

### Comparing `pyams_content-1.99.0/src/pyams_content.egg-info/requires.txt` & `pyams_content-1.99.1/src/pyams_content.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 setuptools
 fanstatic
 hypatia
 persistent
 pyams_catalog
 pyams_fields
 pyams_file
-pyams_form
+pyams_form>=2.1.0
 pyams_i18n
 pyams_i18n_views
 pyams_layer
 pyams_mail
 pyams_pagelet
 pyams_portal
 pyams_scheduler
```

