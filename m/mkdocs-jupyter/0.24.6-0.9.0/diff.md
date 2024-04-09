# Comparing `tmp/mkdocs_jupyter-0.24.6.tar.gz` & `tmp/mkdocs-jupyter-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "dist/mkdocs-jupyter-0.9.0.tar", last modified: Wed Dec 18 02:23:16 2019, max compression
```

## Comparing `mkdocs_jupyter-0.24.6.tar` & `mkdocs-jupyter-0.9.0.tar`

### file list

```diff
@@ -1,105 +1,27 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/.DS_Store
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/.firebaserc
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/.prettierignore
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/.prettierrc
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/CHANGELOG.md
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/CONTRIBUTING.md
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/RELEASE.md
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/Taskfile.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/codecov.yml
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/firebase.json
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/requirements-dev.lock
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/requirements.lock
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/setup.cfg
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/demo/mkdocs.yml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/demo/extras/README.md
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/demo/extras/default.css
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/demo/extras/material.css
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/demo/extras/styles.css
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/demo/extras/styles.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/demo/overrides/main.html
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/js/.gitignore
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/js/package.json
--rw-r--r--   0        0        0    13414 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/js/pnpm-lock.yaml
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/js/vite.config.js
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/js/src/index.js
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/js/src/theme-dark.js
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/js/src/theme-light.js
--rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/js/src/styles/index.scss
--rw-r--r--   0        0        0   591157 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/js/src/styles/jupyter-lab-index.scss
--rw-r--r--   0        0        0    16744 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/js/src/styles/jupyter-lab-theme-dark.scss
--rw-r--r--   0        0        0    16499 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/js/src/styles/jupyter-lab-theme-light.scss
--rw-r--r--   0        0        0    31035 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/js/src/styles/theme-switcher.scss
--rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/js/src/styles/variables.scss
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/__about__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/config.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/convert.py
--rw-r--r--   0        0        0    10206 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/nbconvert2.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/plugin.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/preprocessors.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/utils.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/templates/mkdocs_html/conf.json
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/templates/mkdocs_html/notebook.html.j2
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/templates/mkdocs_html/assets/.gitignore
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/templates/mkdocs_html/assets/clipboard.umd.js
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/templates/mkdocs_html/assets/dark.js
--rw-r--r--   0        0        0   575110 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/templates/mkdocs_html/assets/index.css
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/templates/mkdocs_html/assets/index.js
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/templates/mkdocs_html/assets/light.js
--rw-r--r--   0        0        0    10296 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/templates/mkdocs_html/assets/theme-dark.css
--rw-r--r--   0        0        0     9813 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/templates/mkdocs_html/assets/theme-light.css
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/templates/mkdocs_md/conf.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/templates/mkdocs_md/md-no-codecell.md.j2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/__init__.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/test_base_usage.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/test_pkg.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/base-with-nbs-failure.yml
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/base-with-nbs-pys.yml
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/base-with-nbs.yml
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/base-with-pys.yml
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/base-without-nbs.yml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/material-execute-ignore.yml
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/material-with-nbs-pys.yml
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/material-with-nbs.yml
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/material-with-pys.yml
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/docs/demo-script.py
--rw-r--r--   0        0        0  3714417 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/docs/demo.ipynb
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/docs/fail.ipynb
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/docs/index.md
--rw-r--r--   0        0        0   488224 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/docs/ruby.ipynb
--rw-r--r--   0        0        0    25658 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/docs/variational-inference-script.py
--rw-r--r--   0        0        0   116450 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/docs/variational-inference.ipynb
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/docs/extras/README.md
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/docs/extras/default.css
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/docs/extras/material.css
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/docs/extras/styles.css
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/docs/extras/styles.py
--rw-r--r--   0        0        0    38960 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/docs/img/jupyter.png
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/overrides/main.html
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/404.html
--rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/index.html
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/sitemap.xml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/sitemap.xml.gz
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/css/base.css
--rw-r--r--   0        0        0   163091 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/css/bootstrap.min.css
--rw-r--r--   0        0        0    31000 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/css/font-awesome.min.css
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/extras/default.css
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/extras/material.css
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/extras/styles.css
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/img/favicon.ico
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/img/grid.png
--rw-r--r--   0        0        0    38960 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/img/jupyter.png
--rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/js/base.js
--rw-r--r--   0        0        0    58073 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/js/bootstrap.min.js
--rw-r--r--   0        0        0    93107 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/src/mkdocs_jupyter/tests/mkdocs/site/js/jquery-1.10.2.min.js
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/LICENSE.txt
--rw-r--r--   0        0        0     8252 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/README.md
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/pyproject.toml
--rw-r--r--   0        0        0     9390 2020-02-02 00:00:00.000000 mkdocs_jupyter-0.24.6/PKG-INFO
+drwxr-xr-x   0 danielfrg   (501) staff       (20)        0 2019-12-18 02:23:16.977059 mkdocs-jupyter-0.9.0/
+-rw-r--r--   0 danielfrg   (501) staff       (20)    11346 2019-12-18 01:58:08.000000 mkdocs-jupyter-0.9.0/LICENSE.txt
+-rw-r--r--   0 danielfrg   (501) staff       (20)      153 2019-12-18 02:16:48.000000 mkdocs-jupyter-0.9.0/MANIFEST.in
+-rw-r--r--   0 danielfrg   (501) staff       (20)      816 2019-12-18 02:23:16.977221 mkdocs-jupyter-0.9.0/PKG-INFO
+-rw-r--r--   0 danielfrg   (501) staff       (20)      290 2019-12-18 02:21:51.000000 mkdocs-jupyter-0.9.0/README.md
+drwxr-xr-x   0 danielfrg   (501) staff       (20)        0 2019-12-18 02:23:16.978059 mkdocs-jupyter-0.9.0/mkdocs_jupyter/
+-rw-r--r--   0 danielfrg   (501) staff       (20)       93 2019-12-18 01:58:25.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter/__init__.py
+-rw-r--r--   0 danielfrg   (501) staff       (20)      497 2019-12-18 02:23:16.978141 mkdocs-jupyter-0.9.0/mkdocs_jupyter/_version.py
+drwxr-xr-x   0 danielfrg   (501) staff       (20)        0 2019-12-18 02:23:16.976797 mkdocs-jupyter-0.9.0/mkdocs_jupyter/assets/
+-rw-r--r--   0 danielfrg   (501) staff       (20)     2150 2019-12-18 00:11:59.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter/assets/jupyter-fixes.css
+-rw-r--r--   0 danielfrg   (501) staff       (20)     1169 2019-12-18 00:11:45.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter/assets/jupyter-fixes.min.css
+-rw-r--r--   0 danielfrg   (501) staff       (20)      232 2019-12-18 00:12:53.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter/assets/notebook.tpl
+-rw-r--r--   0 danielfrg   (501) staff       (20)     5990 2019-12-18 00:14:07.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter/convert.py
+-rw-r--r--   0 danielfrg   (501) staff       (20)     1249 2019-12-18 00:09:13.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter/plugin.py
+-rw-r--r--   0 danielfrg   (501) staff       (20)     1607 2019-12-18 00:33:20.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter/templates.py
+drwxr-xr-x   0 danielfrg   (501) staff       (20)        0 2019-12-18 02:23:16.975762 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/
+-rw-r--r--   0 danielfrg   (501) staff       (20)      816 2019-12-18 02:23:16.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 danielfrg   (501) staff       (20)      602 2019-12-18 02:23:16.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 danielfrg   (501) staff       (20)        1 2019-12-18 02:23:16.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 danielfrg   (501) staff       (20)       64 2019-12-18 02:23:16.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/entry_points.txt
+-rw-r--r--   0 danielfrg   (501) staff       (20)        1 2019-12-18 02:04:07.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/not-zip-safe
+-rw-r--r--   0 danielfrg   (501) staff       (20)       25 2019-12-18 02:23:16.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/requires.txt
+-rw-r--r--   0 danielfrg   (501) staff       (20)       15 2019-12-18 02:23:16.000000 mkdocs-jupyter-0.9.0/mkdocs_jupyter.egg-info/top_level.txt
+-rw-r--r--   0 danielfrg   (501) staff       (20)       25 2019-12-18 01:50:35.000000 mkdocs-jupyter-0.9.0/requirements.txt
+-rw-r--r--   0 danielfrg   (501) staff       (20)      221 2019-12-18 02:23:16.977749 mkdocs-jupyter-0.9.0/setup.cfg
+-rw-r--r--   0 danielfrg   (501) staff       (20)     1036 2019-12-18 02:05:34.000000 mkdocs-jupyter-0.9.0/setup.py
+-rw-r--r--   0 danielfrg   (501) staff       (20)    68611 2019-12-18 01:58:25.000000 mkdocs-jupyter-0.9.0/versioneer.py
```

### Comparing `mkdocs_jupyter-0.24.6/LICENSE.txt` & `mkdocs-jupyter-0.9.0/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
@@ -183,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2019 Daniel Rodriguez
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

