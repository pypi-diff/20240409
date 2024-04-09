# Comparing `tmp/survey-5.2.4.tar.gz` & `tmp/survey-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survey-5.2.4.tar", last modified: Mon Feb 26 14:16:36 2024, max compression
+gzip compressed data, was "survey-5.3.0.tar", last modified: Tue Apr  9 16:05:34 2024, max compression
```

## Comparing `survey-5.2.4.tar` & `survey-5.3.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:16:36.699056 survey-5.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:16:36.683055 survey-5.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:16:36.683055 survey-5.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-26 14:16:25.000000 survey-5.2.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-02-26 14:16:25.000000 survey-5.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-26 14:16:25.000000 survey-5.2.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-26 14:16:25.000000 survey-5.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-26 14:16:36.699056 survey-5.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-26 14:16:25.000000 survey-5.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:16:36.683055 survey-5.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-26 14:16:25.000000 survey-5.2.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:16:36.683055 survey-5.2.4/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:16:36.691055 survey-5.2.4/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)   202490 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/graphics.lineprogress-1.gif
--rw-r--r--   0 runner    (1001) docker     (127)   823307 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/graphics.multilineprogress-1.gif
--rw-r--r--   0 runner    (1001) docker     (127)    39691 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/graphics.spinprogress-1.gif
--rw-r--r--   0 runner    (1001) docker     (127)     8033 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/printers.done-1.png
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/printers.fail-1.png
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/printers.info-1.png
--rw-r--r--   0 runner    (1001) docker     (127)    92650 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/routines.basket-1.gif
--rw-r--r--   0 runner    (1001) docker     (127)    64730 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/routines.basket-2.gif
--rw-r--r--   0 runner    (1001) docker     (127)    17906 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/routines.conceal-1.gif
--rw-r--r--   0 runner    (1001) docker     (127)    46839 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/routines.datetime-1.gif
--rw-r--r--   0 runner    (1001) docker     (127)    25618 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/routines.datetime-2.gif
--rw-r--r--   0 runner    (1001) docker     (127)    52677 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/routines.form-1.gif
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/routines.input-1.gif
--rw-r--r--   0 runner    (1001) docker     (127)    74363 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/routines.input-2.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/routines.inquire-1.gif
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/routines.numeric-1.gif
--rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/routines.numeric-2.gif
--rw-r--r--   0 runner    (1001) docker     (127)    27647 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/routines.select-1.gif
--rw-r--r--   0 runner    (1001) docker     (127)    39313 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/routines.select-2.gif
--rw-r--r--   0 runner    (1001) docker     (127)   472099 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/showcase-1.gif
--rw-r--r--   0 runner    (1001) docker     (127)   121555 2024-02-26 14:16:25.000000 survey-5.2.4/docs/_static/images/showcase-2.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-02-26 14:16:25.000000 survey-5.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-26 14:16:25.000000 survey-5.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-02-26 14:16:25.000000 survey-5.2.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-26 14:16:25.000000 survey-5.2.4/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 14:16:36.699056 survey-5.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-26 14:16:25.000000 survey-5.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:16:36.695056 survey-5.2.4/survey/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-26 14:16:25.000000 survey-5.2.4/survey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_controls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:16:36.699056 survey-5.2.4/survey/_core/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_core/_ansi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_core/_console.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_core/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7372 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_core/_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_core/_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_core/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_core/_intel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_core/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_core/_io_os.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_core/_io_os_nt.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_core/_io_os_posix.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_core/_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_core/_screen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_core/_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    31406 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_funnels.py
--rw-r--r--   0 runner    (1001) docker     (127)    23990 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18165 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_mutates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_printers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17015 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_routines.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_searches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10218 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_visuals.py
--rw-r--r--   0 runner    (1001) docker     (127)    60205 2024-02-26 14:16:25.000000 survey-5.2.4/survey/_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:16:36.699056 survey-5.2.4/survey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-26 14:16:36.000000 survey-5.2.4/survey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-02-26 14:16:36.000000 survey-5.2.4/survey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 14:16:36.000000 survey-5.2.4/survey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-26 14:16:36.000000 survey-5.2.4/survey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-26 14:16:36.000000 survey-5.2.4/survey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:05:34.351695 survey-5.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:05:34.335695 survey-5.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:05:34.335695 survey-5.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-09 16:05:17.000000 survey-5.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-09 16:05:17.000000 survey-5.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 16:05:17.000000 survey-5.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-09 16:05:17.000000 survey-5.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-09 16:05:34.351695 survey-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-09 16:05:17.000000 survey-5.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:05:34.335695 survey-5.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-09 16:05:17.000000 survey-5.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:05:34.335695 survey-5.3.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:05:34.343695 survey-5.3.0/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   202490 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/graphics.lineprogress-1.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   823307 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/graphics.multilineprogress-1.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    39691 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/graphics.spinprogress-1.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     8033 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/printers.done-1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/printers.fail-1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/printers.info-1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92650 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/routines.basket-1.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    64730 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/routines.basket-2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    17906 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/routines.conceal-1.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    46839 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/routines.datetime-1.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    25618 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/routines.datetime-2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    52677 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/routines.form-1.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/routines.input-1.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    74363 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/routines.input-2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/routines.inquire-1.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/routines.numeric-1.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/routines.numeric-2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    27647 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/routines.select-1.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    39313 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/routines.select-2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   472099 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/showcase-1.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   121555 2024-04-09 16:05:17.000000 survey-5.3.0/docs/_static/images/showcase-2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-09 16:05:17.000000 survey-5.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-09 16:05:17.000000 survey-5.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-09 16:05:17.000000 survey-5.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-09 16:05:17.000000 survey-5.3.0/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:05:34.351695 survey-5.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 16:05:17.000000 survey-5.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:05:34.347695 survey-5.3.0/survey/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-09 16:05:17.000000 survey-5.3.0/survey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_controls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:05:34.351695 survey-5.3.0/survey/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_core/_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_core/_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_core/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7372 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_core/_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_core/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_core/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_core/_intel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_core/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_core/_io_os.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_core/_io_os_nt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_core/_io_os_posix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_core/_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_core/_screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_core/_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31406 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_funnels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23990 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18165 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_mutates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_printers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17015 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_routines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_searches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10218 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_visuals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60205 2024-04-09 16:05:17.000000 survey-5.3.0/survey/_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:05:34.351695 survey-5.3.0/survey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-09 16:05:34.000000 survey-5.3.0/survey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-09 16:05:34.000000 survey-5.3.0/survey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:05:34.000000 survey-5.3.0/survey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 16:05:34.000000 survey-5.3.0/survey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 16:05:34.000000 survey-5.3.0/survey.egg-info/top_level.txt
```

### Comparing `survey-5.2.4/.github/workflows/publish.yml` & `survey-5.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/.gitignore` & `survey-5.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/LICENSE` & `survey-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/PKG-INFO` & `survey-5.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 5.2.4
+Version: 5.3.0
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
 Requires-Python: >=3.7
 License-File: LICENSE
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
```

### Comparing `survey-5.2.4/README.rst` & `survey-5.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/Makefile` & `survey-5.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/graphics.lineprogress-1.gif` & `survey-5.3.0/docs/_static/images/graphics.lineprogress-1.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/graphics.multilineprogress-1.gif` & `survey-5.3.0/docs/_static/images/graphics.multilineprogress-1.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/graphics.spinprogress-1.gif` & `survey-5.3.0/docs/_static/images/graphics.spinprogress-1.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/printers.done-1.png` & `survey-5.3.0/docs/_static/images/printers.done-1.png`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/printers.fail-1.png` & `survey-5.3.0/docs/_static/images/printers.fail-1.png`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/printers.info-1.png` & `survey-5.3.0/docs/_static/images/printers.info-1.png`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/routines.basket-1.gif` & `survey-5.3.0/docs/_static/images/routines.basket-1.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/routines.basket-2.gif` & `survey-5.3.0/docs/_static/images/routines.basket-2.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/routines.conceal-1.gif` & `survey-5.3.0/docs/_static/images/routines.conceal-1.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/routines.datetime-1.gif` & `survey-5.3.0/docs/_static/images/routines.datetime-1.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/routines.datetime-2.gif` & `survey-5.3.0/docs/_static/images/routines.datetime-2.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/routines.form-1.gif` & `survey-5.3.0/docs/_static/images/routines.form-1.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/routines.input-1.gif` & `survey-5.3.0/docs/_static/images/routines.input-1.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/routines.input-2.gif` & `survey-5.3.0/docs/_static/images/routines.input-2.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/routines.inquire-1.gif` & `survey-5.3.0/docs/_static/images/routines.inquire-1.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/routines.numeric-1.gif` & `survey-5.3.0/docs/_static/images/routines.numeric-1.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/routines.numeric-2.gif` & `survey-5.3.0/docs/_static/images/routines.numeric-2.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/routines.select-1.gif` & `survey-5.3.0/docs/_static/images/routines.select-1.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/routines.select-2.gif` & `survey-5.3.0/docs/_static/images/routines.select-2.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/showcase-1.gif` & `survey-5.3.0/docs/_static/images/showcase-1.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/_static/images/showcase-2.gif` & `survey-5.3.0/docs/_static/images/showcase-2.gif`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/conf.py` & `survey-5.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/index.rst` & `survey-5.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/make.bat` & `survey-5.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/docs/reference.rst` & `survey-5.3.0/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/setup.py` & `survey-5.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/__init__.py` & `survey-5.3.0/survey/__init__.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_colors.py` & `survey-5.3.0/survey/_colors.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_controls.py` & `survey-5.3.0/survey/_controls.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_core/__init__.py` & `survey-5.3.0/survey/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_core/_ansi.py` & `survey-5.3.0/survey/_core/_ansi.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_core/_console.py` & `survey-5.3.0/survey/_core/_console.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_core/_cursor.py` & `survey-5.3.0/survey/_core/_cursor.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_core/_handle.py` & `survey-5.3.0/survey/_core/_handle.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_core/_helpers.py` & `survey-5.3.0/survey/_core/_helpers.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_core/_intel.py` & `survey-5.3.0/survey/_core/_intel.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_core/_io.py` & `survey-5.3.0/survey/_core/_io.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_core/_io_os.py` & `survey-5.3.0/survey/_core/_io_os.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_core/_io_os_nt.py` & `survey-5.3.0/survey/_core/_io_os_nt.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_core/_io_os_posix.py` & `survey-5.3.0/survey/_core/_io_os_posix.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_core/_render.py` & `survey-5.3.0/survey/_core/_render.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_core/_screen.py` & `survey-5.3.0/survey/_core/_screen.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_core/_source.py` & `survey-5.3.0/survey/_core/_source.py`

 * *Files 11% similar despite different names*

```diff
@@ -85,15 +85,17 @@
         return self._intel
 
     _group = {
         EventType.control: {
             '\x7f': Event.delete_left,
             '\x08': Event.delete_right,
             '\x0d': Event.enter,
-            '\x09': Event.indent
+            '\x09': Event.indent,
+            '\x10': Event.arrow_up,
+            '\x0E': Event.arrow_down
         },
         EventType.escape: {
             '': Event.escape
         },
         EventType.sequence: {
             'A': Event.arrow_up,
             'B': Event.arrow_down,
```

### Comparing `survey-5.2.4/survey/_funnels.py` & `survey-5.3.0/survey/_funnels.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_graphics.py` & `survey-5.3.0/survey/_graphics.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_handle.py` & `survey-5.3.0/survey/_handle.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_helpers.py` & `survey-5.3.0/survey/_helpers.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_mutates.py` & `survey-5.3.0/survey/_mutates.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_printers.py` & `survey-5.3.0/survey/_printers.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_routines.py` & `survey-5.3.0/survey/_routines.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_searches.py` & `survey-5.3.0/survey/_searches.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_stage.py` & `survey-5.3.0/survey/_stage.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_system.py` & `survey-5.3.0/survey/_system.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_theme.py` & `survey-5.3.0/survey/_theme.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_utils.py` & `survey-5.3.0/survey/_utils.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_visuals.py` & `survey-5.3.0/survey/_visuals.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey/_widgets.py` & `survey-5.3.0/survey/_widgets.py`

 * *Files identical despite different names*

### Comparing `survey-5.2.4/survey.egg-info/PKG-INFO` & `survey-5.3.0/survey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 5.2.4
+Version: 5.3.0
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
 Requires-Python: >=3.7
 License-File: LICENSE
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
```

### Comparing `survey-5.2.4/survey.egg-info/SOURCES.txt` & `survey-5.3.0/survey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

